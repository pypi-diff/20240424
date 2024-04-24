# Comparing `tmp/pyvserv-1.0.3.tar.gz` & `tmp/pyvserv-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyvserv-1.0.3.tar", last modified: Thu Apr  4 07:48:56 2024, max compression
+gzip compressed data, was "pyvserv-1.0.4.tar", last modified: Wed Apr 24 16:22:50 2024, max compression
```

## Comparing `pyvserv-1.0.3.tar` & `pyvserv-1.0.4.tar`

### file list

```diff
@@ -1,86 +1,144 @@
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.664012 pyvserv-1.0.3/
--rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.3/LICENSE
--rw-r--r--   0 peterglen  (1000) users      (100)    14003 2024-04-04 07:48:56.660012 pyvserv-1.0.3/PKG-INFO
--rw-rw-r--   0 peterglen  (1000) users      (100)    13441 2024-04-04 07:48:11.000000 pyvserv-1.0.3/README.md
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.520001 pyvserv-1.0.3/pyvclient/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:10.000000 pyvserv-1.0.3/pyvclient/__init__.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.3/pyvclient/loadtest.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3979 2024-03-02 11:01:52.000000 pyvserv-1.0.3/pyvclient/pyvcli_akey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4767 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_bigget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5698 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_cd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     9981 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_cli.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3595 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_fdel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3689 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_fget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3916 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_file.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3745 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_fput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4087 2024-04-02 09:10:12.000000 pyvserv-1.0.3/pyvclient/pyvcli_gethelp.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2328 2024-04-02 08:13:29.000000 pyvserv-1.0.3/pyvclient/pyvcli_hello.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2097 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_id.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6005 2024-03-11 12:10:04.000000 pyvserv-1.0.3/pyvclient/pyvcli_ihost.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4119 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_login.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5016 2024-03-17 10:20:16.000000 pyvserv-1.0.3/pyvclient/pyvcli_ls.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4891 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_lsd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3958 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_mkdir.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3907 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_pass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_ping.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3599 2024-04-02 15:41:33.000000 pyvserv-1.0.3/pyvclient/pyvcli_qr.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     9414 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_replic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     5940 2024-04-02 09:10:50.000000 pyvserv-1.0.3/pyvclient/pyvcli_rget.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4814 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_rlist.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6511 2024-04-02 08:59:15.000000 pyvserv-1.0.3/pyvclient/pyvcli_rput.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     6401 2024-03-02 15:00:25.000000 pyvserv-1.0.3/pyvclient/pyvcli_sess.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     7033 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_sess_tout.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2680 2024-02-25 16:08:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_tout.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3348 2024-03-17 00:44:33.000000 pyvserv-1.0.3/pyvclient/pyvcli_uadd.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4215 2024-03-17 07:30:55.000000 pyvserv-1.0.3/pyvclient/pyvcli_uchpass.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3187 2024-03-17 06:46:46.000000 pyvserv-1.0.3/pyvclient/pyvcli_udel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3566 2024-04-02 16:12:24.000000 pyvserv-1.0.3/pyvclient/pyvcli_uena.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3432 2024-04-02 09:29:19.000000 pyvserv-1.0.3/pyvclient/pyvcli_uini.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4869 2024-04-02 10:38:36.000000 pyvserv-1.0.3/pyvclient/pyvcli_uman.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2725 2024-04-02 16:14:25.000000 pyvserv-1.0.3/pyvclient/pyvcli_ver.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.608008 pyvserv-1.0.3/pyvcommon/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:18.000000 pyvserv-1.0.3/pyvcommon/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10832 2024-03-03 15:44:52.000000 pyvserv-1.0.3/pyvcommon/comline.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.3/pyvcommon/crysupp.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.3/pyvcommon/genstrerr.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14953 2024-04-02 10:45:49.000000 pyvserv-1.0.3/pyvcommon/pyclisup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.3/pyvcommon/pycrypt.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     6671 2024-03-11 08:42:22.000000 pyvserv-1.0.3/pyvcommon/pydata.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    23396 2024-04-04 02:24:00.000000 pyvserv-1.0.3/pyvcommon/pyservsup.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.3/pyvcommon/pysyslog.py
--rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.3/pyvcommon/pyv2fa.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    10237 2024-04-04 06:05:08.000000 pyvserv-1.0.3/pyvcommon/pyvhash.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.3/pyvcommon/pywrap.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9527 2024-04-01 14:21:20.000000 pyvserv-1.0.3/pyvcommon/support.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.616008 pyvserv-1.0.3/pyvgui/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:37:55.000000 pyvserv-1.0.3/pyvgui/__init__.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.628009 pyvserv-1.0.3/pyvgui/guilib/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:42:21.000000 pyvserv-1.0.3/pyvgui/guilib/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14657 2024-03-16 15:57:54.000000 pyvserv-1.0.3/pyvgui/guilib/mainwin.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     5928 2024-04-03 06:14:02.000000 pyvserv-1.0.3/pyvgui/guilib/mainwinserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     9305 2024-03-16 16:07:42.000000 pyvserv-1.0.3/pyvgui/guilib/mainwintally.py
--rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.3/pyvgui/guilib/pgui.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.3/pyvgui/guilib/pymenu.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3104 2024-04-03 07:29:15.000000 pyvserv-1.0.3/pyvgui/pyvcpanel.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2682 2024-04-03 07:32:33.000000 pyvserv-1.0.3/pyvgui/pyvservui.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     3089 2024-04-03 07:47:23.000000 pyvserv-1.0.3/pyvgui/pyvtally.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.660012 pyvserv-1.0.3/pyvserv.egg-info/
--rw-r--r--   0 peterglen  (1000) users      (100)    14003 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/PKG-INFO
--rw-r--r--   0 peterglen  (1000) users      (100)     1801 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/SOURCES.txt
--rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/dependency_links.txt
--rw-r--r--   0 peterglen  (1000) users      (100)      598 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/entry_points.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       48 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/requires.txt
--rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-04-04 07:48:56.000000 pyvserv-1.0.3/pyvserv.egg-info/top_level.txt
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.648011 pyvserv-1.0.3/pyvserver/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-02-24 15:10:04.000000 pyvserv-1.0.3/pyvserver/__init__.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    56484 2024-04-04 03:20:07.000000 pyvserv-1.0.3/pyvserver/pyvfunc.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    10855 2024-04-03 07:15:57.000000 pyvserv-1.0.3/pyvserver/pyvpuller.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    10940 2024-04-03 07:59:18.000000 pyvserv-1.0.3/pyvserver/pyvreplic.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)    20718 2024-04-04 05:56:40.000000 pyvserv-1.0.3/pyvserver/pyvserv.py
--rw-rw-r--   0 peterglen  (1000) users      (100)    14047 2024-04-04 03:19:43.000000 pyvserv-1.0.3/pyvserver/pyvstate.py
-drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-04 07:48:56.656012 pyvserv-1.0.3/pyvtools/
--rw-r--r--   0 peterglen  (1000) users      (100)        0 2024-03-11 04:46:04.000000 pyvserv-1.0.3/pyvtools/__init__.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     4542 2024-04-04 05:48:31.000000 pyvserv-1.0.3/pyvtools/pyvgenkey.py
--rwxrwxr-x   0 peterglen  (1000) users      (100)     2507 2024-03-11 08:52:17.000000 pyvserv-1.0.3/pyvtools/pyvgenkeys.py
--rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-04 07:48:56.664012 pyvserv-1.0.3/setup.cfg
--rw-rw-r--   0 peterglen  (1000) users      (100)     4076 2024-04-04 05:10:28.000000 pyvserv-1.0.3/setup.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/
+-rw-rw-r--   0 peterglen  (1000) users      (100)     1097 2024-03-15 11:18:08.000000 pyvserv-1.0.4/LICENSE
+-rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-04-24 16:22:50.264470 pyvserv-1.0.4/PKG-INFO
+-rw-rw-r--   0 peterglen  (1000) users      (100)    17156 2024-04-10 00:53:07.000000 pyvserv-1.0.4/README.md
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.208470 pyvserv-1.0.4/pyvclient/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       14 2024-04-15 07:22:33.000000 pyvserv-1.0.4/pyvclient/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.232470 pyvserv-1.0.4/pyvclient/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    13937 2024-04-15 06:50:03.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_acc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12079 2024-04-15 06:49:27.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_akey.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13072 2024-04-15 06:49:28.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_bigget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14945 2024-04-15 06:49:29.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_cd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24511 2024-04-15 06:49:30.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_cli.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11941 2024-04-15 06:49:31.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fdel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11688 2024-04-15 06:49:31.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12082 2024-04-15 06:49:32.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_file.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    18815 2024-04-15 06:49:33.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11794 2024-04-15 06:49:34.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_fput.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12743 2024-04-15 06:49:35.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_gethelp.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13095 2024-04-15 06:49:36.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_hello.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10536 2024-04-10 00:54:07.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_id.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14864 2024-04-15 06:49:38.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ihost.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12497 2024-04-15 06:49:39.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_login.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    13464 2024-04-15 06:49:41.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ls.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12238 2024-04-15 06:49:40.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_lsd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:42.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_mkdir.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12205 2024-04-15 06:49:42.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_pass.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10253 2024-04-15 06:49:43.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ping.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14879 2024-04-15 06:49:44.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_qr.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16745 2024-04-15 06:49:45.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rabs.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16354 2024-04-15 06:49:46.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rcheck.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14273 2024-04-15 06:49:47.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rcount.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    32879 2024-04-15 06:57:46.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_replic.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    17860 2024-04-15 06:49:49.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rget.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16101 2024-04-15 06:49:50.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rlist.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    24463 2024-04-15 06:49:51.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11544 2024-04-15 06:49:52.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rmdir.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    18495 2024-04-15 06:49:53.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_rput.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14769 2024-04-15 06:49:54.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_sess.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16015 2024-04-15 06:50:05.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_sess_tout.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11681 2024-04-15 06:49:55.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_throt.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10607 2024-04-15 06:50:04.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_tout.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11574 2024-04-15 06:49:56.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uadd.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    14358 2024-04-15 06:49:57.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uchpass.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    11365 2024-04-15 06:49:58.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_udel.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12115 2024-04-15 06:49:59.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uena.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    16680 2024-04-15 06:50:00.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uini.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    20642 2024-04-15 06:50:01.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_uman.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    12963 2024-04-15 06:50:02.000000 pyvserv-1.0.4/pyvclient/docs/pyvcli_ver.html
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     1208 2024-02-05 14:55:18.000000 pyvserv-1.0.4/pyvclient/loadtest.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3848 2024-04-06 08:48:29.000000 pyvserv-1.0.4/pyvclient/pyvcli_akey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4743 2024-04-09 14:23:35.000000 pyvserv-1.0.4/pyvclient/pyvcli_bigget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5567 2024-04-06 08:47:43.000000 pyvserv-1.0.4/pyvclient/pyvcli_cd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     9985 2024-04-11 22:53:59.000000 pyvserv-1.0.4/pyvclient/pyvcli_cli.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3784 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_fdel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3503 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_fget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3976 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_file.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6078 2024-04-10 01:59:10.000000 pyvserv-1.0.4/pyvclient/pyvcli_fman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3639 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_fput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3156 2024-04-09 05:49:52.000000 pyvserv-1.0.4/pyvclient/pyvcli_gethelp.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3409 2024-04-09 05:40:35.000000 pyvserv-1.0.4/pyvclient/pyvcli_hello.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2432 2024-04-05 22:02:34.000000 pyvserv-1.0.4/pyvclient/pyvcli_id.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6166 2024-04-12 22:44:34.000000 pyvserv-1.0.4/pyvclient/pyvcli_ihost.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3988 2024-04-06 08:49:18.000000 pyvserv-1.0.4/pyvclient/pyvcli_login.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4960 2024-04-06 08:50:29.000000 pyvserv-1.0.4/pyvclient/pyvcli_ls.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4076 2024-04-06 08:50:00.000000 pyvserv-1.0.4/pyvclient/pyvcli_lsd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_mkdir.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3776 2024-04-06 08:50:51.000000 pyvserv-1.0.4/pyvclient/pyvcli_pass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2351 2024-02-25 16:08:36.000000 pyvserv-1.0.4/pyvclient/pyvcli_ping.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4099 2024-04-09 05:32:53.000000 pyvserv-1.0.4/pyvclient/pyvcli_qr.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4992 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rabs.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4816 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rcheck.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3850 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rcount.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    13786 2024-04-15 11:47:19.000000 pyvserv-1.0.4/pyvclient/pyvcli_replic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5462 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rget.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4659 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rlist.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     8530 2024-04-10 01:58:55.000000 pyvserv-1.0.4/pyvclient/pyvcli_rman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3394 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_rmdir.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5788 2024-04-12 12:45:56.000000 pyvserv-1.0.4/pyvclient/pyvcli_rput.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6137 2024-04-05 13:27:04.000000 pyvserv-1.0.4/pyvclient/pyvcli_sess.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3548 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_throt.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3353 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_uadd.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     5689 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_uchpass.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3192 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_udel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3867 2024-04-09 05:45:08.000000 pyvserv-1.0.4/pyvclient/pyvcli_uena.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4818 2024-04-14 07:07:11.000000 pyvserv-1.0.4/pyvclient/pyvcli_uini.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     6972 2024-04-10 01:56:40.000000 pyvserv-1.0.4/pyvclient/pyvcli_uman.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3171 2024-04-09 05:24:42.000000 pyvserv-1.0.4/pyvclient/pyvcli_ver.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.244470 pyvserv-1.0.4/pyvcommon/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:55.000000 pyvserv-1.0.4/pyvcommon/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    12254 2024-04-15 07:57:44.000000 pyvserv-1.0.4/pyvcommon/comline.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4270 2021-02-05 17:39:14.000000 pyvserv-1.0.4/pyvcommon/crysupp.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      608 2024-03-09 10:44:12.000000 pyvserv-1.0.4/pyvcommon/genstrerr.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    17642 2024-04-08 08:14:28.000000 pyvserv-1.0.4/pyvcommon/pyclisup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5322 2021-02-05 17:39:14.000000 pyvserv-1.0.4/pyvcommon/pycrypt.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     6778 2024-04-11 23:55:27.000000 pyvserv-1.0.4/pyvcommon/pydata.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    29729 2024-04-13 16:24:30.000000 pyvserv-1.0.4/pyvcommon/pyservsup.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3479 2024-03-10 14:51:33.000000 pyvserv-1.0.4/pyvcommon/pysyslog.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)      571 2024-03-01 12:52:57.000000 pyvserv-1.0.4/pyvcommon/pyv2fa.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10878 2024-04-22 16:13:09.000000 pyvserv-1.0.4/pyvcommon/pyvhash.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4762 2024-03-03 14:03:00.000000 pyvserv-1.0.4/pyvcommon/pywrap.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     9529 2024-04-15 10:48:15.000000 pyvserv-1.0.4/pyvcommon/support.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.248470 pyvserv-1.0.4/pyvgui/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:37.000000 pyvserv-1.0.4/pyvgui/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.248470 pyvserv-1.0.4/pyvgui/guilib/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:46.000000 pyvserv-1.0.4/pyvgui/guilib/__init__.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14679 2024-04-15 14:58:07.000000 pyvserv-1.0.4/pyvgui/guilib/mainwin.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     5928 2024-04-03 06:14:02.000000 pyvserv-1.0.4/pyvgui/guilib/mainwinserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13042 2024-04-16 02:33:20.000000 pyvserv-1.0.4/pyvgui/guilib/mainwintally.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    25146 2024-04-24 15:14:24.000000 pyvserv-1.0.4/pyvgui/guilib/mainwinvote.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    10767 2024-04-21 14:12:22.000000 pyvserv-1.0.4/pyvgui/guilib/pgcal.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)     3214 2024-03-11 03:29:27.000000 pyvserv-1.0.4/pyvgui/guilib/pgui.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    11922 2021-02-03 22:50:23.000000 pyvserv-1.0.4/pyvgui/guilib/pymenu.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    13331 2024-04-24 16:00:43.000000 pyvserv-1.0.4/pyvgui/guilib/recsel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3104 2024-04-03 07:29:15.000000 pyvserv-1.0.4/pyvgui/pyvcpanel.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2682 2024-04-03 07:32:33.000000 pyvserv-1.0.4/pyvgui/pyvservui.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     3089 2024-04-03 07:47:23.000000 pyvserv-1.0.4/pyvgui/pyvtally.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2893 2024-04-24 13:07:58.000000 pyvserv-1.0.4/pyvgui/pyvvote.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/pyvserv.egg-info/
+-rw-r--r--   0 peterglen  (1000) users      (100)    17718 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/PKG-INFO
+-rw-r--r--   0 peterglen  (1000) users      (100)     3498 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/SOURCES.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)        1 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/dependency_links.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)      640 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/entry_points.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       48 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/requires.txt
+-rw-r--r--   0 peterglen  (1000) users      (100)       46 2024-04-24 16:22:50.000000 pyvserv-1.0.4/pyvserv.egg-info/top_level.txt
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.256470 pyvserv-1.0.4/pyvserver/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:48:41.000000 pyvserv-1.0.4/pyvserver/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.260470 pyvserv-1.0.4/pyvserver/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)   171300 2024-04-15 06:32:07.000000 pyvserv-1.0.4/pyvserver/docs/pyvfunc.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    76482 2024-04-15 06:32:05.000000 pyvserv-1.0.4/pyvserver/docs/pyvreplic.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    68036 2024-04-15 06:32:04.000000 pyvserv-1.0.4/pyvserver/docs/pyvserv.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    35380 2024-04-15 06:32:06.000000 pyvserv-1.0.4/pyvserver/docs/pyvstate.html
+-rw-rw-r--   0 peterglen  (1000) users      (100)    67566 2024-04-15 10:22:32.000000 pyvserv-1.0.4/pyvserver/pyvfunc.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    23259 2024-04-15 06:31:36.000000 pyvserv-1.0.4/pyvserver/pyvreplic.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)    22417 2024-04-15 05:56:51.000000 pyvserv-1.0.4/pyvserver/pyvserv.py
+-rw-rw-r--   0 peterglen  (1000) users      (100)    14128 2024-04-15 10:48:53.000000 pyvserv-1.0.4/pyvserver/pyvstate.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/pyvtools/
+-rw-rw-r--   0 peterglen  (1000) users      (100)       13 2024-04-06 09:49:20.000000 pyvserv-1.0.4/pyvtools/__init__.py
+drwxr-xr-x   0 peterglen  (1000) users      (100)        0 2024-04-24 16:22:50.264470 pyvserv-1.0.4/pyvtools/docs/
+-rw-r--r--   0 peterglen  (1000) users      (100)    16315 2024-04-23 13:55:15.000000 pyvserv-1.0.4/pyvtools/docs/pyvgenkey.html
+-rw-r--r--   0 peterglen  (1000) users      (100)    10283 2024-04-23 13:55:14.000000 pyvserv-1.0.4/pyvtools/docs/pyvgenkeys.html
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     4542 2024-04-04 05:48:31.000000 pyvserv-1.0.4/pyvtools/pyvgenkey.py
+-rwxrwxr-x   0 peterglen  (1000) users      (100)     2508 2024-04-09 08:30:16.000000 pyvserv-1.0.4/pyvtools/pyvgenkeys.py
+-rw-r--r--   0 peterglen  (1000) users      (100)       38 2024-04-24 16:22:50.264470 pyvserv-1.0.4/setup.cfg
+-rw-rw-r--   0 peterglen  (1000) users      (100)     4908 2024-04-24 16:22:17.000000 pyvserv-1.0.4/setup.py
```

### Comparing `pyvserv-1.0.3/LICENSE` & `pyvserv-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/PKG-INFO` & `pyvserv-1.0.4/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -1,26 +1,7 @@
-Metadata-Version: 2.1
-Name: pyvserv
-Version: 1.0.3
-Summary: High power secure server with blockchain backend.
-Home-page: https://github.com/pglen/pyvserv
-Author: Peter Glen
-Author-email: peterglen99@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pyvpacker
-Requires-Dist: pydbase
-Requires-Dist: pycryptodome
-Requires-Dist: pyvecc
-Requires-Dist: pyvguicom
-
 #  PyvServer
 
 ## 	Fully encrypted TCP/IP server.
 
  &nbsp; &nbsp; PyvServ is an encrypting TCP/IP server written in Python. The
 encryption algorithm is AES. (Advanced Encryption Standard) The key exchange
 uses ECC. (Elliptic curve) The server can be fully administered from the
@@ -115,53 +96,82 @@
 #### Start server
 
  The python server can be added to the system servers with the Makefile targets
 'make genservice' and 'make instservice'
  The scripts will generate the service file to run under current user's
  credentials, and install it onto the running system. (requires sudo)
 
-#### Platform:
+#### Platforms:
 
  This project was developed on Ubuntu 22.x. Most linux distributions should work.
 It is ported to Windows MSYS2, with all major functions operating as expected.
 
  On Fedora, the service files need to be re-written to accomodate the
 quirk that the Fedora systectl does not allow user executables. Install
 the 'pip pyvserv' as root, and adjust the service file accordingly. If you want
 to use pyvserv with  particular data directory, use the -r option.
 
+ On Debian and newer (23+) Ubuntu the system needs the --break-system-packages
+ on pip. (unless one creates a venv for it) This is a cutionary arrangement
+ for the OS, pyvserv does not break anything.
+
+    pip install pyvserv --break-system-packages
+
+Also the scripts are installed in ~/.local/bin, so add the following line
+  to the end of ~/.bashrc:
+
+    PATH=$PATH:~/.local/bin
+
+This workaround is not needed if one installs pyvserv in a virtual environment.
+
+    python3 -m venv pip_pyvserv
+    cd pip_pyvserv
+    source ./bin/avtivate
+    pip install pyvserv
+    ... continue as needed.
+
+The makefile target 'make installvirt' will install pyvserv in a virtual
+environment.
+
+ Running pyvserv as a system daemon from virtual environment needs extra
+configuration steps. You may use the make target: 'make genservice_virt'
+and activate with 'make instservice'
+Please see the relevant systemctl manuals.
+
 #### Quick map:
 
     Server.     subdir: pyvserver       -- Server has most all the commands done
     Client.     subdir: pyvclient       -- Exercise server commands / demo code
     Test Suite. subdir: pyvclient/tests -- official pytest tests
     Tool Suite. subdir: pyvtools        -- Key generation etc ...
     GUI base    subdir: pyvgui          -- Monitoring / administering the server
     Studies.    subdir: study           -- testing/learning subsystems (ignore it)
 
 #### Quick start:
 
  One can mimic global connectivity on a single machine. This would allow the study
 of the client / server interaction before live deployment. This chapter assumes
-installation from github, replicating directory structure on the local drive.
+installation / clone from github, replicating directory structure on the
+local drive.
 
     open terminal window
     navigate to the server's pyvserver subdir
     type: ./pyvserv.py
 
     open another terminal window
     navigate to the pyvclient subdir
     type: ./pyvcli_hello.py
 
 The following (and more) should be printed on the command line:
 
     ./pyvcli_hello.py
-    Server initial: ['OK', 'pyvserv 1.0 ready']
-    resp ['OK', 'Hello', '6ccdaaf1-a22d-4140-9608-8fb93a8845af', '11812']
-    Server quit response: ['OK', 'Bye', '11812']
+
+    Server initial: ['OK', 'pyvserv 1.0.4 ready']
+    resp ['OK', 'Hello', '4814b46a-9489-4720-af7d-aa14ba19f2be', '11367']
+    Server quit response: ['OK', 'Bye', '11367']
 
 Quick rundown of the above test:
 
     1.) Server responds to connection with signin message
     2.) Delivers OK status, hello message, server serial number, and a unique id
     3.) Server signs off. Repeats unique id / session number.
 
@@ -184,15 +194,22 @@
  (two factor authentication)
 
  The command line client can be started as:
 
     pyvcli_cli
 
   In the command line client most of the server functions can be exercised.
-See the pyvcli_* utils for more examples of driving the server.
+See the pyvcli_* utils for more examples of driving the server. On a
+fresh install, one may need to execute the pyvcli_uini.py to create an initial
+admin user, with password 1234. The uini command will prompt if this is
+what was intended.
+
+ The cli utility command 'help' will deliver information on the available commands.
+
+!!! IMPORTANT !!! Make sure you change this when testing / learning is over.
 
 ## Command line help
 
     Usage: pyvserv.py [options]
 
     Options:
             -n   --host                 -  Set server hostname / interface.
@@ -209,36 +226,72 @@
             -h   --help                 -  Show Help
 
 ## Client command line help example:
 
  While most command line clients have their own help screen, here as a typical
 client utility's help screen:
 
-    Usage: pyvcli_uman.py [options]
+    Usage: pyvcli_uman.py [options] [hostname]
 
     Options:    -d level  - Debug level 0-10
                 -p        - Port to use (default: 6666)
                 -l login  - Login Name; default: 'user'
                 -s lpass  - Login Pass; default: '1234'
                 -u user   - User Name; default: 'user'
-                -a        - Add user. Must be unique.
-                -r        - Remove user (one of add or remove needed.
+                -t        - prompt for login pass
+                -a        - Add user. Must be a unique user name.
+                -r        - Remove user
                 -u user   - User Name; default: 'user'
-                -p pass   - User pssword; default: '1234' (!!! for tests only)
+                -p pass   - User password; default: '1234' (!!for tests only!!)
+                -T        - prompt for new pass
                 -m        - Add admin instead of regular user
+                -e enflag - Enable / Disable user.
+                -i kind   - List users (user or admin
                 -v        - Verbose
                 -q        - Quiet
                 -h        - Help
 
+     One of Add / Remove / Enable / List option is needed.
+
+## pyvser clients
+
+ Some client programs are supplied to administer / drive / monitor pyvserv.
+ The -h option on the client programs give a brief help of usage / purpose.
+
+ | Client name  | Description               |        Purpose                |
+ | -----------  |  -----------              |  ------------------------     |
+ | pyvcli_cli   | Command line interface    | All aspects of pyvserv        |
+ | pyvcli_uini  | Create initial user       | Create initial admin user     |
+ | pyvcli_fman  | File manager              | Upload / Download files       |
+ | pyvcli_uman  | User manager              | Add remove users / admins     |
+ | pyvcli_rman  | Record manager            | Get / Put Blockchain Records  |
+ | pyvcli_hello | Get hello message         | Connectivity test             |
+ | pyvcli_ver   | Get Version number        | Check for server version      |
+
+ The utilities can also be executed from the 'pyvclient' sub directory by
+ post fixing with script extension. (add the .py extension like: ./pyvcli_cli.py)
+
+ The date formats for specifying record date filter dates are:
+
+   'Y-m-d+H:M' 'Y-m-d' 'm-d' 'm-d+H-M'
+
+Where Y=year m=month d=day H=hour M=minutes, just like in strftime.
+The hour is in 24 hour notation.
+
+The following are all valid dates specs, specifying the same date
+(in 2024 apr 15 at 00:00):
+
+    2024-04-15 2024-04-15+0:0 04-15 04-15+00:00
+
 ## Testing:
 
- All pytest cases pass. Note that the for the pytest client tests one needs to
- start the 'pyvserv.py' server.
- The server --port and --dataroot option can ba used to start the server in an alternate
- universe. Please make sure it does not interfere with production.
+ All pytest cases pass successfully. Note that for the pytest client
+ tests one needs to start the server. ('./pyvserv.py' or pyvserv if installed)
+ The server --port and --dataroot option can be used to start the server in
+ an alternate 'universe', so it does not interfere with production.
 
     ============================ test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
     rootdir: /home/<homedir>/pgpygtk/pyvserv
     collected 15 items
 
     test_afirst.py .                                                         [  6%]
@@ -253,45 +306,56 @@
     test_rput.py .                                                           [ 73%]
     test_sess.py ..                                                          [ 86%]
     test_user.py .                                                           [ 93%]
     test_ver.py .                                                            [100%]
 
     ============================== 15 passed in 9.47s ==============================
 
-Additional tests can be found in the tests/ directory. The pyvcli_* files may also
-serve as test cases.
+Additional tests can be found in the tests/ directory. The pyvcli_* files in the
+'pyvclient' directory may also serve as test cases.
+
+## Production:
 
-More test coming soon ....
+Once the testing phase is complete, deploying it for production needs a
+complete wipe of the data. There are Makefile targets that do that
+(make cleanall). Restarting the server will create the new environment without
+any users. To allow operation one may create the initial user with the uini
+functions and / or scripts.
+The uini command can only operate successfully if there are no users present in the
+pyvserv system, and it is executed from the loopback interface. For example,
+the command line utility ./pyvcli_uini.py can be used;
+For production, it can executed with the -t option to prompt for a password.
 
 ## Screen shots:
 
 Screen shot of the Monitoring tool:
 
 ![Screen Shot](montool.png)
 
  This screen shot depicts the monitoring (control panel) application 'pyvcpanel'.
 The top left area contains a live view of the pyvserver syslog. The top right
 contains a live view of the replicator log.
 
  The bottom area of the window contains a live view of the incoming data, as it is
 originally formatted, without the blockchain and hash details.
 
-  All views monitor the live files, on the default setup, without interfering
-with any of the operations.
+  All views monitor the live log files, on the default setup. The montor functions
+operate, without interfering with any of the operations.
 
 ## Windows compatibility
 
- Pyvserv now functions in the Windows MSYS2 subsystem. All the major
+  Pyvserv now functions in the Windows MSYS2 subsystem. All the major
 functionalities are ported. The file locking mechanism works, and all the
 pytests pass. Naturally, logging and readline etc ... works with the usual
 windows caveat.
 
-  For the GUI functions install the PyGobject subsystem. Instructions can
-be found very easily for that. Below, a screenshot of the pyvserv control panel
-in MSYS2.
+  For the GUI functions ona my need to install the PyGobject subsystem.
+Instructions can be found very easily for that.
+
+Below, a screenshot of the pyvserv control panel in MSYS2.
 
 ![Screen Shot](winscreen.png)
 
 The project is functional in MSYS2, but for real deployment we recommend Linux.
 
 ## History:
 
@@ -299,31 +363,34 @@
 
     1.0.0   Sun 03.Mar.2024    Beta ready
     1.0.0   Mon 11.Mar.2024    PIP installation with utils
     1.0.0   Wed 13.Mar.2024    rget rput and family (rget=BC record get)
     1.0.0   Thu 14.Mar.2024    Started GUI tools
     1.0.1   Fri 15.Mar.2024    Added LIC, verification, doc, tally
     1.0.3   Wed 03.Apr.2024    Ported to MSYS2, throttle, for multiprocess
+    1.0.4   Tue 09.Apr.2024    Cleanup, uman fman rman completed
 
 ## Statistics
 
     Project name
         pyvserv
+    Generated
+        2024-04-09 20:45:56
     Report Period
-        2018-12-31 20:50:04 to 2024-03-15 04:47:25
+        2018-12-31 20:50:04 to 2024-04-09 20:41:24
     Age
-        1901 days, 101 active days (5.31%)
+        1927 days, 111 active days (5.76%)
     Total Files
-        287
+        211
     Total Lines of Code
-        70286 (235368 added, 165082 removed)
+        44443 (258657 added, 214214 removed)
     Total Commits
-        216 (average 2.1 commits per active day, 0.1 per all days)
+        257 (average 2.3 commits per active day, 0.1 per all days)
     Authors
-        6 (average 36.0 commits per author)
+        6 (average 42.8 commits per author)
 
 ![Screen Shot](commits_by_year_month.png)
 
 ## Security review:
 
  &nbsp;  As of today, (Fri 15.Mar.2024) the 256 bit AES is considered unbreakable by
 available state of the art means. The key exchange algorithm ECC 384 bit is
@@ -331,15 +398,15 @@
 key is used in every session. The session is also able to dynamically change keys
 mid flight, on command.
 
  &nbsp; The checksum verification and link verification both use SHA256 (256 bit)
 hashes. This is generated every time a transaction is created.
 
  &nbsp; The proof of work is a modest 3 generations deep. This can be calculated
-with an everyday desktop in one - to - three seconds. Even though this looks like
+with an everyday desktop in one ... to ... three seconds. Even though this looks like
 a small amount, it adds up if one wants to re-generate (fake) a whole chain.
 Additionally, the check sum, the link sum, and proof of work interact, changing one
 will effect the other. This way a sum verification and link verification and the
 proof of work verification together create an ironclad safety solution.
 
 Written by Peter Glen, 2022, 2023, 2024
 Released under MIT License (MIT)
```

### Comparing `pyvserv-1.0.3/README.md` & `pyvserv-1.0.4/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,26 @@
+Metadata-Version: 2.1
+Name: pyvserv
+Version: 1.0.4
+Summary: High power secure server with blockchain backend.
+Home-page: https://github.com/pglen/pyvserv
+Author: Peter Glen
+Author-email: peterglen99@gmail.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pyvpacker
+Requires-Dist: pydbase
+Requires-Dist: pycryptodome
+Requires-Dist: pyvecc
+Requires-Dist: pyvguicom
+
 #  PyvServer
 
 ## 	Fully encrypted TCP/IP server.
 
  &nbsp; &nbsp; PyvServ is an encrypting TCP/IP server written in Python. The
 encryption algorithm is AES. (Advanced Encryption Standard) The key exchange
 uses ECC. (Elliptic curve) The server can be fully administered from the
@@ -96,53 +115,82 @@
 #### Start server
 
  The python server can be added to the system servers with the Makefile targets
 'make genservice' and 'make instservice'
  The scripts will generate the service file to run under current user's
  credentials, and install it onto the running system. (requires sudo)
 
-#### Platform:
+#### Platforms:
 
  This project was developed on Ubuntu 22.x. Most linux distributions should work.
 It is ported to Windows MSYS2, with all major functions operating as expected.
 
  On Fedora, the service files need to be re-written to accomodate the
 quirk that the Fedora systectl does not allow user executables. Install
 the 'pip pyvserv' as root, and adjust the service file accordingly. If you want
 to use pyvserv with  particular data directory, use the -r option.
 
+ On Debian and newer (23+) Ubuntu the system needs the --break-system-packages
+ on pip. (unless one creates a venv for it) This is a cutionary arrangement
+ for the OS, pyvserv does not break anything.
+
+    pip install pyvserv --break-system-packages
+
+Also the scripts are installed in ~/.local/bin, so add the following line
+  to the end of ~/.bashrc:
+
+    PATH=$PATH:~/.local/bin
+
+This workaround is not needed if one installs pyvserv in a virtual environment.
+
+    python3 -m venv pip_pyvserv
+    cd pip_pyvserv
+    source ./bin/avtivate
+    pip install pyvserv
+    ... continue as needed.
+
+The makefile target 'make installvirt' will install pyvserv in a virtual
+environment.
+
+ Running pyvserv as a system daemon from virtual environment needs extra
+configuration steps. You may use the make target: 'make genservice_virt'
+and activate with 'make instservice'
+Please see the relevant systemctl manuals.
+
 #### Quick map:
 
     Server.     subdir: pyvserver       -- Server has most all the commands done
     Client.     subdir: pyvclient       -- Exercise server commands / demo code
     Test Suite. subdir: pyvclient/tests -- official pytest tests
     Tool Suite. subdir: pyvtools        -- Key generation etc ...
     GUI base    subdir: pyvgui          -- Monitoring / administering the server
     Studies.    subdir: study           -- testing/learning subsystems (ignore it)
 
 #### Quick start:
 
  One can mimic global connectivity on a single machine. This would allow the study
 of the client / server interaction before live deployment. This chapter assumes
-installation from github, replicating directory structure on the local drive.
+installation / clone from github, replicating directory structure on the
+local drive.
 
     open terminal window
     navigate to the server's pyvserver subdir
     type: ./pyvserv.py
 
     open another terminal window
     navigate to the pyvclient subdir
     type: ./pyvcli_hello.py
 
 The following (and more) should be printed on the command line:
 
     ./pyvcli_hello.py
-    Server initial: ['OK', 'pyvserv 1.0 ready']
-    resp ['OK', 'Hello', '6ccdaaf1-a22d-4140-9608-8fb93a8845af', '11812']
-    Server quit response: ['OK', 'Bye', '11812']
+
+    Server initial: ['OK', 'pyvserv 1.0.4 ready']
+    resp ['OK', 'Hello', '4814b46a-9489-4720-af7d-aa14ba19f2be', '11367']
+    Server quit response: ['OK', 'Bye', '11367']
 
 Quick rundown of the above test:
 
     1.) Server responds to connection with signin message
     2.) Delivers OK status, hello message, server serial number, and a unique id
     3.) Server signs off. Repeats unique id / session number.
 
@@ -165,15 +213,22 @@
  (two factor authentication)
 
  The command line client can be started as:
 
     pyvcli_cli
 
   In the command line client most of the server functions can be exercised.
-See the pyvcli_* utils for more examples of driving the server.
+See the pyvcli_* utils for more examples of driving the server. On a
+fresh install, one may need to execute the pyvcli_uini.py to create an initial
+admin user, with password 1234. The uini command will prompt if this is
+what was intended.
+
+ The cli utility command 'help' will deliver information on the available commands.
+
+!!! IMPORTANT !!! Make sure you change this when testing / learning is over.
 
 ## Command line help
 
     Usage: pyvserv.py [options]
 
     Options:
             -n   --host                 -  Set server hostname / interface.
@@ -190,36 +245,72 @@
             -h   --help                 -  Show Help
 
 ## Client command line help example:
 
  While most command line clients have their own help screen, here as a typical
 client utility's help screen:
 
-    Usage: pyvcli_uman.py [options]
+    Usage: pyvcli_uman.py [options] [hostname]
 
     Options:    -d level  - Debug level 0-10
                 -p        - Port to use (default: 6666)
                 -l login  - Login Name; default: 'user'
                 -s lpass  - Login Pass; default: '1234'
                 -u user   - User Name; default: 'user'
-                -a        - Add user. Must be unique.
-                -r        - Remove user (one of add or remove needed.
+                -t        - prompt for login pass
+                -a        - Add user. Must be a unique user name.
+                -r        - Remove user
                 -u user   - User Name; default: 'user'
-                -p pass   - User pssword; default: '1234' (!!! for tests only)
+                -p pass   - User password; default: '1234' (!!for tests only!!)
+                -T        - prompt for new pass
                 -m        - Add admin instead of regular user
+                -e enflag - Enable / Disable user.
+                -i kind   - List users (user or admin
                 -v        - Verbose
                 -q        - Quiet
                 -h        - Help
 
+     One of Add / Remove / Enable / List option is needed.
+
+## pyvser clients
+
+ Some client programs are supplied to administer / drive / monitor pyvserv.
+ The -h option on the client programs give a brief help of usage / purpose.
+
+ | Client name  | Description               |        Purpose                |
+ | -----------  |  -----------              |  ------------------------     |
+ | pyvcli_cli   | Command line interface    | All aspects of pyvserv        |
+ | pyvcli_uini  | Create initial user       | Create initial admin user     |
+ | pyvcli_fman  | File manager              | Upload / Download files       |
+ | pyvcli_uman  | User manager              | Add remove users / admins     |
+ | pyvcli_rman  | Record manager            | Get / Put Blockchain Records  |
+ | pyvcli_hello | Get hello message         | Connectivity test             |
+ | pyvcli_ver   | Get Version number        | Check for server version      |
+
+ The utilities can also be executed from the 'pyvclient' sub directory by
+ post fixing with script extension. (add the .py extension like: ./pyvcli_cli.py)
+
+ The date formats for specifying record date filter dates are:
+
+   'Y-m-d+H:M' 'Y-m-d' 'm-d' 'm-d+H-M'
+
+Where Y=year m=month d=day H=hour M=minutes, just like in strftime.
+The hour is in 24 hour notation.
+
+The following are all valid dates specs, specifying the same date
+(in 2024 apr 15 at 00:00):
+
+    2024-04-15 2024-04-15+0:0 04-15 04-15+00:00
+
 ## Testing:
 
- All pytest cases pass. Note that the for the pytest client tests one needs to
- start the 'pyvserv.py' server.
- The server --port and --dataroot option can ba used to start the server in an alternate
- universe. Please make sure it does not interfere with production.
+ All pytest cases pass successfully. Note that for the pytest client
+ tests one needs to start the server. ('./pyvserv.py' or pyvserv if installed)
+ The server --port and --dataroot option can be used to start the server in
+ an alternate 'universe', so it does not interfere with production.
 
     ============================ test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
     rootdir: /home/<homedir>/pgpygtk/pyvserv
     collected 15 items
 
     test_afirst.py .                                                         [  6%]
@@ -234,45 +325,56 @@
     test_rput.py .                                                           [ 73%]
     test_sess.py ..                                                          [ 86%]
     test_user.py .                                                           [ 93%]
     test_ver.py .                                                            [100%]
 
     ============================== 15 passed in 9.47s ==============================
 
-Additional tests can be found in the tests/ directory. The pyvcli_* files may also
-serve as test cases.
+Additional tests can be found in the tests/ directory. The pyvcli_* files in the
+'pyvclient' directory may also serve as test cases.
+
+## Production:
 
-More test coming soon ....
+Once the testing phase is complete, deploying it for production needs a
+complete wipe of the data. There are Makefile targets that do that
+(make cleanall). Restarting the server will create the new environment without
+any users. To allow operation one may create the initial user with the uini
+functions and / or scripts.
+The uini command can only operate successfully if there are no users present in the
+pyvserv system, and it is executed from the loopback interface. For example,
+the command line utility ./pyvcli_uini.py can be used;
+For production, it can executed with the -t option to prompt for a password.
 
 ## Screen shots:
 
 Screen shot of the Monitoring tool:
 
 ![Screen Shot](montool.png)
 
  This screen shot depicts the monitoring (control panel) application 'pyvcpanel'.
 The top left area contains a live view of the pyvserver syslog. The top right
 contains a live view of the replicator log.
 
  The bottom area of the window contains a live view of the incoming data, as it is
 originally formatted, without the blockchain and hash details.
 
-  All views monitor the live files, on the default setup, without interfering
-with any of the operations.
+  All views monitor the live log files, on the default setup. The montor functions
+operate, without interfering with any of the operations.
 
 ## Windows compatibility
 
- Pyvserv now functions in the Windows MSYS2 subsystem. All the major
+  Pyvserv now functions in the Windows MSYS2 subsystem. All the major
 functionalities are ported. The file locking mechanism works, and all the
 pytests pass. Naturally, logging and readline etc ... works with the usual
 windows caveat.
 
-  For the GUI functions install the PyGobject subsystem. Instructions can
-be found very easily for that. Below, a screenshot of the pyvserv control panel
-in MSYS2.
+  For the GUI functions ona my need to install the PyGobject subsystem.
+Instructions can be found very easily for that.
+
+Below, a screenshot of the pyvserv control panel in MSYS2.
 
 ![Screen Shot](winscreen.png)
 
 The project is functional in MSYS2, but for real deployment we recommend Linux.
 
 ## History:
 
@@ -280,31 +382,34 @@
 
     1.0.0   Sun 03.Mar.2024    Beta ready
     1.0.0   Mon 11.Mar.2024    PIP installation with utils
     1.0.0   Wed 13.Mar.2024    rget rput and family (rget=BC record get)
     1.0.0   Thu 14.Mar.2024    Started GUI tools
     1.0.1   Fri 15.Mar.2024    Added LIC, verification, doc, tally
     1.0.3   Wed 03.Apr.2024    Ported to MSYS2, throttle, for multiprocess
+    1.0.4   Tue 09.Apr.2024    Cleanup, uman fman rman completed
 
 ## Statistics
 
     Project name
         pyvserv
+    Generated
+        2024-04-09 20:45:56
     Report Period
-        2018-12-31 20:50:04 to 2024-03-15 04:47:25
+        2018-12-31 20:50:04 to 2024-04-09 20:41:24
     Age
-        1901 days, 101 active days (5.31%)
+        1927 days, 111 active days (5.76%)
     Total Files
-        287
+        211
     Total Lines of Code
-        70286 (235368 added, 165082 removed)
+        44443 (258657 added, 214214 removed)
     Total Commits
-        216 (average 2.1 commits per active day, 0.1 per all days)
+        257 (average 2.3 commits per active day, 0.1 per all days)
     Authors
-        6 (average 36.0 commits per author)
+        6 (average 42.8 commits per author)
 
 ![Screen Shot](commits_by_year_month.png)
 
 ## Security review:
 
  &nbsp;  As of today, (Fri 15.Mar.2024) the 256 bit AES is considered unbreakable by
 available state of the art means. The key exchange algorithm ECC 384 bit is
@@ -312,15 +417,15 @@
 key is used in every session. The session is also able to dynamically change keys
 mid flight, on command.
 
  &nbsp; The checksum verification and link verification both use SHA256 (256 bit)
 hashes. This is generated every time a transaction is created.
 
  &nbsp; The proof of work is a modest 3 generations deep. This can be calculated
-with an everyday desktop in one - to - three seconds. Even though this looks like
+with an everyday desktop in one ... to ... three seconds. Even though this looks like
 a small amount, it adds up if one wants to re-generate (fake) a whole chain.
 Additionally, the check sum, the link sum, and proof of work interact, changing one
 will effect the other. This way a sum verification and link verification and the
 proof of work verification together create an ironclad safety solution.
 
 Written by Peter Glen, 2022, 2023, 2024
 Released under MIT License (MIT)
```

### Comparing `pyvserv-1.0.3/pyvclient/loadtest.py` & `pyvserv-1.0.4/pyvclient/loadtest.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_akey.py` & `pyvserv-1.0.4/pyvclient/pyvcli_akey.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,18 +8,14 @@
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat
 
 from pyvecc.Key import Key
 
 from Crypto.Hash import SHA512
 from Crypto.Hash import SHA256
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
 from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_bigget.py` & `pyvserv-1.0.4/pyvclient/pyvcli_bigget.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
@@ -45,32 +45,25 @@
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
     ["f:",  "file",     6666,   None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
-    ["n",   "plain",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
-    #print(dir(conf))
-
-    #if conf.comm:
-    #    print("Save to filename", conf.comm)
-
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
@@ -97,54 +90,60 @@
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
     #print("Sess Key ACCEPTED:",  resp3[1])
 
-    if conf.sess_key:
-        if not conf.quiet:
-            print("Post session, session key:", conf.sess_key[:12], "...")
-
-    resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    if not conf.quiet:
-        print("Hello Response:", resp3)
+    #if conf.sess_key:
+    #    if not conf.quiet:
+    #        print("Post session, session key:", conf.sess_key[:12], "...")
+
+    #resp3 = hand.client(["hello", ],  conf.sess_key, False)
+    #if not conf.quiet:
+    #    print("Hello Response:", resp3)
 
     # Session estabilished, try a simple command
     #resp4 = hand.client(["hello",], conf.sess_key)
     #print("Hello Response:", resp4[1])
 
     cresp = hand.login("admin", "1234", conf)
+    if not cresp[0] == "OK":
+        print("Cannot login", cresp)
+        sys.exit()
+
     if not conf.quiet:
         print ("Server login response:", cresp)
 
     bigfname = "bigfile"    # Use this name for cleaning it
-    bigbuff = b"a" * 1024
+    bigbuff = b"abcdef" * 1024
     # Create bigfile
     fp = open(bigfname, "wb")
-    for aa in range(1024 * 20):
+    for aa in range(1024 * 10):
         fp.write(bigbuff)
     fp.close()
 
     # Put big file up
-    print("Started file UP ...", )
+    if not conf.quiet:
+        print("Started file UP ...", )
     ttt = time.time()
     resp = hand.putfile(bigfname, "", conf.sess_key)
     filesize = support.fsize(bigfname)
     rate = filesize / (time.time() - ttt)
     if not conf.quiet:
         print("filesize", filesize)
     if resp[0] != "OK":
         print ("fput resp:", resp)
         cresp = hand.client(["quit", ], conf.sess_key)
         print ("Server quit response:", cresp)
         sys.exit()
     print ("fput response:", resp, "time %.2f kbytes/sec" % (rate/1024))
 
-    print("Started bigfile DOWN")
+    if not conf.quiet:
+        print("Started bigfile DOWN")
     ttt = time.time()
     ret = hand.getfile(bigfname, bigfname + "_local", conf.sess_key)
     filesize = support.fsize(bigfname + "_local")
     if not conf.quiet:
         print("filesize", filesize)
     rate = filesize / (time.time() - ttt)
     print ("fget response:", ret, "time %.2f kbytes/sec" % (rate/1024))
@@ -154,13 +153,13 @@
 
     ret = os.system("diff " + bigfname + " " + bigfname + "_local")
     if ret:
         print("Error: Files Differ", ret)
     else:
         print("Files Compare OK")
 
-    os.remove(bigfname)
-    os.remove(bigfname + "_local")
+    #os.remove(bigfname)
+    #os.remove(bigfname + "_local")
 
     sys.exit(0)
 
  # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_cd.py` & `pyvserv-1.0.4/pyvclient/pyvcli_cd.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 from Crypto.Hash import SHA512
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, datetime
 
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
 from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_cli.py` & `pyvserv-1.0.4/pyvclient/pyvcli_cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -35,19 +35,21 @@
 ''' Test unit for pyvserv. Command line interpreter. This interface is similar
     to the FTP client interface. Some functions are sent through directly,
     and some functions are interpreted via client helpers.
     All encryption functionality is exercised as the real client would.
     The command that starts with the exclamation point is executed
     in the local shell.
 
-## The following commands (and more) may be issued.
+    ## The following commands (and more) may be issued.
 
-        user logon_name                 -- Name of user to log in with
+    ### Type 'help' for a complete list
+
+        user login_name                 -- Name of user to log in with
         akey                            -- Get asymmetric key
-        pass logon_pass                 -- Password
+        pass login_pass                 -- Password
         chpass newpass                  -- Change pass (not tested)
         file fname                      -- Specify name for upload
         fget fname                      -- Download (get) file
         fput fname                      -- Upload (put) file
         del  fname                      -- Delete file
         uadd user_name user_pass        -- Create new user
         kadd key_name key_val           -- Add new encryption key
@@ -79,71 +81,90 @@
         ihave                           -- The 'i have you have' protocol entry point
         ihost                           -- Add / delete replicator host
 
 '''
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
-
+version = "1.0.0"
+progn = os.path.basename(sys.argv[0])
 # ------------------------------------------------------------------------
 
-def phelp():
+__doc__ = '''\
+The pyvserv command line client.
+Usage: %s [options] [hostname]
+  hostname: host to connect to. (default: 127.0.0.1)
+  options:  -d level  - Debug level 0-10
+            -p        - Port to use (default: 6666)
+            -l login  - Login Name; default: 'user'
+            -s lpass  - Login Pass; default: '1234' !!For tests Only!!
+            -t        - Prompt for pass
+            -x comm   - Execute command and quit
+            -q        - Quiet
+            -v        - Verbose
+            -V        - Print version number
+            -h        - Help
+Prefix local commands with '!' (exclamation mark) ''' \
+ % (progn)
 
+def phelp():
     ''' Provide local help '''
-
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 6666)")
-    print( "            -l login  - Login Name; default: 'user'")
-    print( "            -s lpass  - Login Pass; default: '1234'")
-    print( "            -v        - Verbose")
-    print( "            -q        - Quiet")
-    print( "            -x comm   - Execute command and quit")
-    print( "            -n        - No encryption (plain)")
-    print( "            -h        - Help")
-    print()
+    print(__doc__)
     sys.exit(0)
 
 def pversion():
 
     ''' Print version string '''
 
-    print( os.path.basename(sys.argv[0]), "Version", version)
+    print(progn, "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
+
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
     ["l:",  "login",    "admin",    None],      \
-    ["s:",  "lpass",    "1234",    None],      \
-    ["x:",  "comm",     "",     None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["s:",  "lpass",    "1234",     None],      \
+    ["t",   "prompt",   0,          None],      \
+    ["x:",  "comm",     "",         None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 def mainfunct():
 
     ''' Command line interpreter '''
 
-    args = conf.comline(sys.argv[1:])
-
-    #print(vars(conf))
+    try:
+        args = conf.comline(sys.argv[1:])
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
+    if conf.prompt:
+        import getpass
+        strx = getpass.getpass("Enter Pass: ")
+        if not strx:
+            print("Aborting ...")
+            sys.exit(0)
+        conf.lpass  = strx
+
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
@@ -153,70 +174,56 @@
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     atexit.register(pyclisup.atexit_func, hand, conf)
 
-    resp3 = hand.client(["id",] , "", False)
-    if not conf.quiet:
-        print("ID Response:", resp3[1])
+    resp3 = hand.client(["ver",] , "", False)
+    if conf.verbose:
+        print("Ver  Resp: ", resp3)
 
     conf.sess_key = ""
-    #ret = ["OK",];  conf.sess_key = ""
     resp3 = hand.start_session(conf)
     if resp3[0] != "OK":
         print("Error on setting session:", resp3[1])
         sys.exit(0)
 
-    # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
-
-    if conf.sess_key:
-        if not conf.quiet:
-            print(" ------ Post session, session key:", conf.sess_key[:12], "...")
-
-    resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    if not conf.quiet:
+    if conf.verbose:
+        resp3 = hand.client(["hello", ],  conf.sess_key, False)
         print("Hello Resp:", resp3)
 
     cresp = hand.login(conf.login, conf.lpass, conf)
-    if not conf.quiet:
-        print ("Login resp:", cresp)
     if cresp[0] != "OK":
-        print("Error on logging in, exiting.")
+        print("Error on login, exiting.", cresp)
         sys.exit(1)
 
+    if conf.verbose:
+        print ("Login resp:", cresp)
+
     # Start a new session for the rest of the work
     resp3 = hand.start_session(conf)
     if resp3[0] != "OK":
         print("Error on setting session:", resp3[1])
         sys.exit(0)
 
-    if conf.sess_key:
-        if not conf.quiet:
-            print(" ------ Post session, session key:", conf.sess_key[:12], "...")
-
-    resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    if not conf.quiet:
-        print("Hello2 Resp:", resp3)
-
     # Interactive, need more time
-    hand.client(["tout", "30",], conf.sess_key)
+    hand.client(["tout", "10",], conf.sess_key)
 
     if conf.comm:
         import shlex
         #print("exec:", conf.comm)
         commx = shlex.split(conf.comm)
         if not conf.quiet:
-            print("Issue:", commx)
+            print("Issued:", commx)
         resp = hand.client([*commx], conf.sess_key)
-        print("resp:", resp)
+        print("resp:  ", resp)
     else:
-        print ("Enter commands, Ctrl-C or 'done' to quit. Prefix local commands with '!'")
+        if not conf.quiet:
+            print ("Enter commands, Ctrl-C or Ctrl-D or 'quit' to exit.")
         mainloop(conf, hand)
 
     sys.exit(0)
 
 
 def mainloop(conf, hand):
 
@@ -241,23 +248,23 @@
                         print("Post session, session key:", conf.sess_key[:12], "...")
 
                 elif ss[0] == "fget":
                     if len(ss) < 2:
                         print("Use: fget fname")
                         continue
                     ret2 = hand.getfile(ss[1], ss[1] + "_local", conf.sess_key)
-                    print ("Server fget response:", ret2)
+                    print ("fget response:", ret2)
                     continue
 
                 elif ss[0] == "fput":
                     if len(ss) < 2:
                         print("Use: fput fname")
                         continue
                     ret2 = hand.putfile(ss[1], "", conf.sess_key)
-                    print ("Server fput response:", ret2)
+                    print ("fput response:", ret2)
                     continue
 
                 elif ss[0] == "file":
                     if not os.path.isfile(ss[1]):
                         print("File must exist.")
                         continue
                     cresp = hand.start_session(conf)
@@ -269,15 +276,15 @@
                     #print ("local command")
                     os.system(ss[0][1:] + " " + " ".join(ss[1:]))
                     continue
                 else:
                     # No wrapper needed
                     cresp = hand.client(ss, conf.sess_key)
                     # post process
-                    print ("Server response:", cresp)
+                    print ("resp:", cresp)
         except:
             print(sys.exc_info())
             break
 
 if __name__ == '__main__':
     mainfunct()
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_fdel.py` & `pyvserv-1.0.4/pyvclient/pyvcli_fdel.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,53 +2,60 @@
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -f fname  - Send file")
     print( "            -p        - Port to use (default: 6666)")
+    print( "            -f fname  - Delete file")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["f:",  "fname",    "test.txt", None],      \
     ["d:",  "pgdebug",  0,          None],      \
     ["p:",  "port",     6666,       None],      \
+    ["f:",  "fname",    "test.txt", None],      \
     ["v",   "verbose",  0,          None],      \
     ["q",   "quiet",    0,          None],      \
-    ["t",   "test",     "x",        None],      \
     ["V",   None,       None,       pversion],  \
     ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
@@ -83,45 +90,43 @@
 
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
-    # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
-    #print("Post session, all is encrypted")
-
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
     if conf.verbose:
         print("Hello (plain) Response:", resp4)
         #print("Hello (encrypted) Response:", resp4[1])
 
     cresp = hand.client(["user", "admin"], conf.sess_key)
-    #print ("Server user response:", cresp[1])
+    #if not conf.quiet:
+    #    print ("Server user response:", cresp[1])
 
     cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print ("Server pass response:", cresp[1])
+    if not conf.quiet:
+        print ("Server pass response:", cresp[1])
 
     if conf.verbose:
         cresp = hand.client(["ls", ], conf.sess_key)
         print ("Server  ls response:", cresp)
 
     cresp = hand.client(["del", conf.fname], conf.sess_key)
     print ("Server del response:", cresp)
 
     if cresp[0] != "OK":
         #print("Err: ", cresp)
         cresp = hand.client(["quit", ], conf.sess_key)
-        print ("Server quit response:", cresp)
+        #print ("Server quit response:", cresp)
         sys.exit(0)
 
     cresp = hand.client(["quit", ], conf.sess_key)
-    print ("Server quit response:", cresp)
+    #print ("Server quit response:", cresp)
 
     sys.exit(0)
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_fget.py` & `pyvserv-1.0.4/pyvclient/pyvcli_fget.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
@@ -97,33 +97,28 @@
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
     #print("Sess Key ACCEPTED:",  resp3[1])
 
-    if conf.sess_key:
-        print("Post session, session key:", conf.sess_key[:12], "...")
+    if not conf.quiet:
+        print("Session key:", conf.sess_key[:12], "...")
 
     resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    print("Hello Response:", resp3)
-
-    # Session estabilished, try a simple command
-    #resp4 = hand.client(["hello",], conf.sess_key)
-    #print("Hello Response:", resp4[1])
+    if not conf.quiet:
+        print("Hello Response:", resp3)
 
     cresp = hand.login("admin", "1234", conf)
-    print ("Server login response:", cresp)
+    if not conf.quiet:
+        print ("Server login response:", cresp)
 
-    #cresp = hand.client(["ls", ], conf.sess_key)
-    #print ("Server  ls response:", cresp)
+    cresp = hand.client(["throt", "off"], conf.sess_key)
+    print ("Server throttle:", cresp)
 
     ret2 = hand.getfile(conf.fname, conf.fname + "_local", conf.sess_key)
     print ("Server fget response:", ret2)
 
-    cresp = hand.client(["ls", ], conf.sess_key)
-    print ("Server  ls response:", cresp)
-
     cresp = hand.client(["quit", ], conf.sess_key)
-    print ("Server quit response:", cresp)
+    #print ("Server quit response:", cresp)
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_file.py` & `pyvserv-1.0.4/pyvclient/pyvcli_login.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,143 +1,134 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+from __future__ import print_function
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Download file.
+# Test client for the pyserv project. Encrypt test.
+
+from Crypto.Hash import SHA512
+import  os, sys, getopt, signal, select, socket, time, struct
+import  random, stat
 
-import os, sys, getopt, signal, select, socket, time, struct
-import random, stat
+from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
-# Globals
-
-version = 1.0
-
-# ------------------------------------------------------------------------
+# Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 6666)")
+    print( "            -p port   - Port to use (default: 6666)")
+    print( "            -l level  - Log level (default: 0)")
+    print( "            -c file   - Save comm to file")
+    print( "            -s        - Showkey")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
+    #print( " Needs debug level or verbose to have any output.")
     print()
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", version)
+    print( os.path.basename(sys.argv[0]), "Version", support.version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
+    ["c:",  "comm",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
+    ["s",   "showkey",  "",     None],      \
     ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
+    if conf.comm:
+        print("Save to filename", conf.comm)
+
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
+    hand.comm  = conf.comm
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    if conf.verbose:
-        resp3 = hand.client(["hello",] , "", False)
-        print("Hello Response:", resp3[1])
+    resp3 = hand.client(["hello", "world"] , "", False)
+    print("Hello Response: ", resp3)
 
-    #conf.sess_key = ""    #ret = ["OK",]
     ret = hand.start_session(conf)
 
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
+    print("Sess Key ACCEPTED:",  conf.sess_key[:12], '...' )
     #print("Post session, all is encrypted")
 
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    if conf.verbose:
-        print("Hello (plain) Response:", resp4)
-        #print("Hello (encrypted) Response:", resp4[1])
+    print("Server hello Response:", resp4[1])
 
     cresp = hand.client(["user", "admin"], conf.sess_key)
-    #print ("Server user response:", cresp[1])
+    print ("Server user  response:", cresp)
 
     cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print ("Server pass response:", cresp[1])
+    print ("Server pass  response:", cresp)
 
-    if conf.verbose:
-        cresp = hand.client(["ls", ], conf.sess_key)
-        print ("Server  ls response:", cresp)
-
-    cresp = hand.client(["file", "zeros"], conf.sess_key)
-    print ("Server file response:", cresp)
-    if cresp[0] != "OK":
-        #print("Err: ", cresp)
-        cresp = hand.client(["quit", ], conf.sess_key)
-        print ("Server quit response:", cresp)
-        sys.exit(0)
-
-    fp = open("zeros_local", "rb")
-    offs = 0
-    while 1:
-        buf = fp.read(1024)
-        #print("sending", buf)
-        cresp = hand.client(["data", offs, buf], conf.sess_key)
-        if conf.verbose:
-            print ("Server data response:", cresp)
-        if cresp[0] != "OK":
-            print("Cannot send", cresp)
-            break
-        blen = len(buf)
-        if blen == 0:
-            break
+    #resp = hand.client(["pass", "12345"], conf.sess_key)
+    #print ("Server pass  response:", cresp)
 
-        offs += blen
-
-    cresp = hand.client(["quit", ], conf.sess_key)
-    print ("Server quit response:", cresp)
-
-    sys.exit(0)
+    #resp = hand.client(["pass", "12345"], conf.sess_key)
+    #print ("Server pass response:", cresp)
 
+    #cresp = hand.client(["pass", "12345"], conf.sess_key)
+    #print ("Server pass response:", cresp[1])
+    #if(cresp[1][:2] != "OK"): sys.exit(1)
 
+    #cresp = hand.client(["pass", "1234"], conf.sess_key)
+    #print ("Server pass  response:", cresp[1])
 
+    #cresp = hand.client(["hello", "1234"], conf.sess_key)
+    #print ("Server hello response:", cresp[1])
 
+    cresp = hand.client(["quit",],conf.sess_key)
+    print ("Server quit  response:", cresp[1])
+    hand.close();
 
+    sys.exit(0)
 
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_fput.py` & `pyvserv-1.0.4/pyvclient/pyvcli_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,55 +2,60 @@
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
     print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
-    print( "            -f fname  - Send file")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["f:",  "fname",    "test.txt", None],      \
-    ["d:",  "pgdebug",  0,          None],      \
-    ["p:",  "port",     6666,       None],      \
-    ["v",   "verbose",  0,          None],      \
-    ["q",   "quiet",    0,          None],      \
-    ["t",   "test",     "x",        None],      \
-    ["V",   None,       None,       pversion],  \
-    ["h",   None,       None,       phelp]      \
+    ["d:",  "pgdebug",  0,      None],      \
+    ["p:",  "port",     6666,   None],      \
+    ["v",   "verbose",  0,      None],      \
+    ["q",   "quiet",    0,      None],      \
+    ["V",   None,       None,   pversion],  \
+    ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
@@ -74,55 +79,62 @@
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     if conf.verbose:
         resp3 = hand.client(["hello",] , "", False)
         print("Hello Response:", resp3[1])
 
-    #conf.sess_key = ""    #ret = ["OK",]
     ret = hand.start_session(conf)
 
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    if conf.verbose:
-        print("Hello (plain) Response:", resp4)
+    if not conf.quiet:
+        print("Hello (plain) Resp:", resp4)
 
     cresp = hand.client(["user", "admin"], conf.sess_key)
-    #print ("Server user response:", cresp[1])
+    if not conf.quiet:
+        print ("Server user response:", cresp[1])
 
     cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print ("Server pass response:", cresp[1])
+    if not conf.quiet:
+        print ("Server pass response:", cresp[1])
 
-    if conf.verbose:
-        cresp = hand.client(["ls", ], conf.sess_key)
-        print ("Server  ls response:", cresp)
+    cresp = hand.client(["ls", ], conf.sess_key)
+    if not conf.quiet:
+        print ("Server ls response:", cresp)
 
-    print("Started file ...", conf.fname)
-    ttt = time.time()
-    resp = hand.putfile(conf.fname, "", conf.sess_key)
-    filesize = support.fsize(conf.fname)/1024
-    #print("filesize", filesize)
-    if resp[0] != "OK":
-        print ("fput resp:", resp)
+    cresp = hand.client(["file", "test.txt"], conf.sess_key)
+    print ("Server file response:", cresp)
+    if cresp[0] != "OK":
         cresp = hand.client(["quit", ], conf.sess_key)
-        print ("Server quit response:", cresp)
-        sys.exit()
+        #print ("Server quit response:", cresp)
+        sys.exit(0)
 
-    if conf.verbose:
-        rate = filesize / (time.time() - ttt)
-        print ("fput resp:", resp, " %.2f kbytes/sec" % rate)
+    fp = open("test.txt_local", "rb")
+    offs = 0
+    while 1:
+        buf = fp.read(1024)
+        #print("sending", buf)
+        cresp = hand.client(["data", offs, buf], conf.sess_key)
+        if conf.verbose:
+            print ("Server data response:", cresp)
+        if cresp[0] != "OK":
+            print("Cannot send", cresp)
+            break
+        blen = len(buf)
+        if blen == 0:
+            break
 
-    cresp = hand.client(["ls", ], conf.sess_key)
-    print ("Server  ls response:", cresp)
+        offs += blen
 
     cresp = hand.client(["quit", ], conf.sess_key)
     print ("Server quit response:", cresp)
 
     sys.exit(0)
 
-# EOF
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_gethelp.py` & `pyvserv-1.0.4/pyvclient/pyvcli_fput.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,125 +1,61 @@
-#!/usr/bin/env python3
-
-from __future__ import print_function
+#!/usr/bin/env python
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. User add.
+# Test client for the pyserv project. Upload file.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
-# This repairs the path from local run to pip run.
-try:
-    from pyvcommon import support
-    base = os.path.dirname(os.path.realpath(support.__file__))
-    sys.path.append(os.path.join(base, "."))
-except:
-    base = os.path.dirname(os.path.realpath(__file__))
-    sys.path.append(os.path.join(base,  '..'))
-    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
-    from pyvcommon import support
+base = os.path.dirname(os.path.realpath(__file__))
+sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
-from pyvcommon import support, pycrypt, pyclisup
-from pyvcommon import pysyslog, comline
+import support, pycrypt, pyservsup, pyclisup
+import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-myhandler = None
-mydathand = None
-pgdebug = 0
-subhelp = ""
-verbose = 0
-port    = 6666
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
-# Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p port   - Port to use (default: 6666)")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
+    print( "            -f fname  - Send file")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
-    print( "            -s str    - Subhelp string")
-    print()
-    print( " Needs debug level or verbose to have any output.")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
+    # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,       None],      \
-    ["p:",  "port",     6666,    None],      \
-    ["v",   "verbose",  0,       None],      \
-    ["q",   "quiet",    0,       None],      \
-    ["t",   "test",     "x",     None],      \
-    ["s:",  "subhelp",  subhelp, None],      \
-    ["V",   None,       None,    pversion],  \
-    ["h",   None,       None,    phelp]      \
+    ["f:",  "fname",    "test.txt", None],      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
-# Send out our special buffer (short)len + (str)message
-
-'''def sendx(sock, message):
-    strx = struct.pack("!h", len(message)) + message
-    sock.send(strx)
-
-def sendfile(s1, fname, toname):
-
-    response = ""
-    try:
-        flen = os.stat(fname)[stat.ST_SIZE]
-        fh = open(fname)
-    except:
-        print( "Cannot open file", sys.exc_info()[1])
-        return
-
-    client(s1, "file " + toname)
-    client(s1, "data " + str(flen))
-    while 1:
-        buff = fh.read(pyservsup.buffsize)
-        if len(buff) == 0:
-            break
-        sendx(s1, buff)
-    response = myhandler.handle_one(mydathand)
-
-    if verbose:
-        print( "Received: '%s'" % response)
-
-    return response
-
 # ------------------------------------------------------------------------
 
-def client(sock, message):
-
-    sendx(sock, message)
-    if verbose:
-        print( "Sent: '%s'" % message)
-
-    response = myhandler.handle_one(mydathand)
-    if verbose:
-        print( "Received: '%s'" % response)
-
-    return response
-'''
-
-# ------------------------------------------------------------------------
-
-def mainfunct():
+if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
@@ -127,37 +63,65 @@
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
-    #print("subhelp", conf.subhelp);
-
     try:
-        resp2 = hand.connect(ip, conf.port)
+        respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #if conf.quiet == False:
-    #    print ("Server initial:", resp2[1])
+    resp3 = hand.client(["hello",] , "", False)
+    if not conf.quiet:
+        print("Hello Response:", resp3[1])
+
+    ret = hand.start_session(conf)
+    if ret[0] != "OK":
+        print("Error on setting session:", resp3[1])
+        hand.client(["quit"])
+        hand.close();
+        sys.exit(0)
+
+    # Session estabilished, try a simple command
+    resp4 = hand.client(["hello",], conf.sess_key)
+    if not conf.quiet:
+        print("Hello resp:", resp4)
+
+    cresp = hand.client(["user", "admin"], conf.sess_key)
+    if not conf.quiet:
+        print ("Server user response:", cresp[1])
+
+    cresp = hand.client(["pass", "1234"], conf.sess_key)
+    if not conf.quiet:
+        print ("Server pass response:", cresp[1])
+
+    if not conf.quiet:
+        print("Started file ...", conf.fname)
+
+    ttt = time.time()
+    resp = hand.putfile(conf.fname, "", conf.sess_key)
+    filesize = support.fsize(conf.fname)/1024
+    #print("filesize", filesize)
+    if resp[0] != "OK":
+        print ("fput resp:", resp)
+        cresp = hand.client(["quit", ], conf.sess_key)
+        print ("Server quit response:", cresp)
+        sys.exit()
+
+    if conf.verbose:
+        rate = filesize / (time.time() - ttt)
+        print ("fput resp:", resp, " %.2f kbytes/sec" % rate)
 
-    if conf.subhelp:
-        resp = hand.client(["help", conf.subhelp])
-    else:
-        resp = hand.client(["help",])
+    print("fput response:", resp)
 
-    if conf.quiet == False:
-        print ("Server response:", resp)
+    #cresp = hand.client(["ls", ], conf.sess_key)
+    #print ("Server  ls response:", cresp)
 
-    hand.client(["quit",])
-    hand.close();
+    cresp = hand.client(["quit", ], conf.sess_key)
+    #print ("Server quit response:", cresp)
 
     sys.exit(0)
 
-#def mainfunct():
-
-if __name__ == '__main__':
-    mainfunct()
-
-# EOF
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_hello.py` & `pyvserv-1.0.4/pyvclient/pyvcli_id.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,16 @@
 #!/usr/bin/env python3
 
 from __future__ import print_function
 
+import sys
+if sys.version_info[0] < 3:
+    print("Python 2 is not supported as of 1/1/2020")
+    sys.exit(1)
+
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat
 
 # This repairs the path from local run to pip run.
@@ -22,15 +27,15 @@
 from pyvcommon import support, pycrypt, pyclisup
 from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Functions from command line
 
 optarr =  comline.optarr
-optarr.append ( ["p:",  "port",     6666,   None, "Port to use (default: 6666)"] )
+optarr.append ( ["p:",  "port",  6666,   None, "Port to use (default: 6666)"] )
 
 #print (optarr)
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
@@ -70,15 +75,15 @@
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     if conf.quiet == False:
         respini = hand.pb.decode_data(resp2[1])[0]
         print ("Server initial:", respini)
 
-    resp = hand.client(["hello"])
+    resp = hand.client(["id"])
     if conf.quiet == False:
         print("resp", resp)
 
     resp2 = hand.client(["quit"])
     if conf.quiet == False:
         print ("Server quit response:", resp2)
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_id.py` & `pyvserv-1.0.4/pyvclient/pyvcli_ver.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,86 +1,114 @@
 #!/usr/bin/env python3
 
-from __future__ import print_function
-
-import sys
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
-
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# Test client for the pyserv project.
 
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
+
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+# For this file
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 # Functions from command line
 
-optarr =  comline.optarr
-optarr.append ( ["p:",  "port",     6666,   None, "Port to use (default: 6666)"] )
+def phelp():
+
+    print( "The pyvserv version query.")
+    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options] [hostname]")
+    print( "  hostname: host to connect to. (default: 127.0.0.1)")
+    print( "  options:    -d level  - Debug level 0-10")
+    print( "              -p port   - Port to use (default: 6666)")
+    print( "              -v        - Verbose")
+    print( "              -V        - Version")
+    print( "              -q        - Quiet")
+    print( "              -h        - Help")
+    sys.exit(0)
+
+def pversion():
+    print( os.path.basename(sys.argv[0]), "Version", version)
+    sys.exit(0)
 
-#print (optarr)
+    # option, var_name, initial_val, function
+optarr = \
+    ["d:",  "pgdebug",  0,      None],      \
+    ["p:",  "port",     6666,   None],      \
+    ["v",   "verbose",  0,      None],      \
+    ["q",   "quiet",    0,      None],      \
+    ["V",   None,       None,   pversion],  \
+    ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def mainfunct():
 
     if sys.version_info[0] < 3:
         print("Warning! This script was meant for python 3.x")
-        time.sleep(1)
-
-    args = conf.comline(sys.argv[1:])
-
-    #for aa in vars(conf):
-    #    print(aa, getattr(conf, aa))
+        sys.exit()
 
-    pyclisup.verbose = conf.verbose
+    try:
+        args = conf.comline(sys.argv[1:])
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
 
     if conf.verbose and conf.pgdebug:
         print("Debug level", conf.pgdebug)
 
+    pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
-    #print("dir".__doc__)
-
     try:
         resp2 = hand.connect(ip, conf.port)
     except:
         #support.put_exception("On connect")
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    if conf.quiet == False:
+    if conf.verbose:
         respini = hand.pb.decode_data(resp2[1])[0]
         print ("Server initial:", respini)
 
-    resp = hand.client(["id"])
-    if conf.quiet == False:
-        print("resp", resp)
-
-    resp2 = hand.client(["quit"])
-    if conf.quiet == False:
-        print ("Server quit response:", resp2)
+    resp = hand.client(["ver"])
+    print ("Version resp:", resp)
 
-    hand.close();
+    resp = hand.client(["quit"])
+    if conf.verbose:
+        print ("Server quit resp:", resp)
+    hand.close()
 
     sys.exit(0)
 
-# EOF
+if __name__ == '__main__':
+    mainfunct()
+
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_ihost.py` & `pyvserv-1.0.4/pyvclient/pyvcli_ihost.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,107 +8,119 @@
 from Crypto.Hash import SHA512
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, uuid
 
 from Crypto import Random
 
 # This repairs the path from local run to pip run.
-# Remove pip version for local tests
 try:
     from pyvcommon import support
 
     # Get Parent of module root
     sf = os.path.dirname(support.__file__)
     sf = os.path.dirname(sf)
-    print("sf", sf)
+    #print("sf", sf)
     sys.path.append(os.path.join(sf, "pyvcommon"))
-    sys.path.append(os.path.join(sf, "pyvserver"))
-    #sys.path.append(os.path.join(sf, "pyvgui"))
-    #sys.path.append(os.path.join(sf, "pyvgui", "guilib"))
 
 except:
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
-    sys.path.append(os.path.join(base,  '..', "pyvserver"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui"))
-    #sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
 from pyvcommon import support, pycrypt, pyservsup, pyclisup, pyvhash
 from pyvcommon import pysyslog, comline
 
 import pyvpacker
 
-'''
-# test encrypt with large keys
-rrr =  "mTQdnL51eKnblQflLGSMvnMKDG4XjhKa9Mbgm5ZY9YLd" \
-        "/SxqZZxwyKc/ZVzCVwMxiJ5X8LdX3X5VVO5zq/VBWQ=="
-sss = bluepy.encrypt(rrr, conf.sess_key)
-ttt = bluepy.decrypt(sss, conf.sess_key)
-print (rrr)
-print (ttt)
-'''
+# ------------------------------------------------------------------------
+# Globals
+
+version = "1.0.0"
+progn = os.path.basename(sys.argv[0])
+
+__doc__ = '''\
+The pyvserv replication host manager.
+Usage: %s  [options] [hostname]
+  hostname: host to connect to. (default: 127.0.0.1)
+  options:  -d level       - Debug level 0-10
+            -p port        - Port to use (default: 6666)
+            -l login       - Login Name; default: 'admin'
+            -s lpass       - Login Pass; default: '1234' (for !!testing only!!)
+            -t             - Prompt for login pass
+            -A  host:port  - Add host:port to replicate to
+            -D  host:port  - Delete host:port to replicate to
+            -S             - Show (list) remote replication hosts
+            -n             - Number of records to put
+            -v             - Verbose
+            -q             - Quiet
+            -h             - Help''' \
+    % (progn)
 
 # ------------------------------------------------------------------------
 # Functions from command line
 
-def phelp():
 
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level        - Debug level 0-10")
-    print( "            -p port         - Port to use (default: 6666)")
-    print( "            -l level        - Log level (default: 0)")
-    print( "            -A  host/port   - Add host/port to replicate to")
-    print( "            -D  host/port   - Delete host/port to replicate to")
-    print( "            -S              - Show (list) remote replication hosts")
-    print( "            -n              - Number of records to put")
-    print( "            -v              - Verbose")
-    print( "            -q              - Quiet")
-    print( "            -h              - Help")
-    #print( " Needs debug level or verbose to have any output.")
-    print()
+def phelp():
+    print(__doc__)
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", support.version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["s",   "showkey",  "",     None],      \
-    ["n:",  "numrec",   1,     None],      \
-    ["A:",  "addx",      "",    None],      \
-    ["D:",  "delx",      "",    None],      \
-    ["S",   "showx",     0,    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["c:",  "comm",     "",         None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["l:",  "login",    "admin",    None],      \
+    ["s:",  "lpass",    "1234",     None],      \
+    ["t",   "lprompt",  0,          None],      \
+    ["n:",  "numrec",   1,          None],      \
+    ["A:",  "addx",      "",        None],      \
+    ["D:",  "delx",      "",        None],      \
+    ["S",   "showx",     0,         None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
-    args = conf.comline(sys.argv[1:])
-    #print(vars(conf))
+    try:
+        args = conf.comline(sys.argv[1:])
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
+    if len(args) == 0:
+        ip = '127.0.0.1'
+    else:
+        ip = args[0]
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
+    if conf.lprompt:
+        import getpass
+        strx = getpass.getpass("Pass for login %s: " % conf.login)
+        if not strx:
+            print("Cannot login with empty pass, aborting ...")
+            sys.exit(0)
+        conf.lpass = strx
+
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
@@ -117,73 +129,76 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello", "world"] , "", False)
-    print("Hello Resp:", resp3)
+    if conf.verbose:
+        resp3 = hand.client(["hello",] , "", False)
+        print("Hello Resp:", resp3)
 
-    resp4 = hand.client(["tout", "30",], conf.sess_key)
-    print("Server tout Response:", resp4)
+    #resp4 = hand.client(["tout", "30",], conf.sess_key)
+    #print("Server tout Response:", resp4)
 
-    ret = hand.start_session(conf)
-
-    if ret[0] != "OK":
+    resp3 = hand.start_session(conf)
+    if resp3[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
     #print("Sess Key ACCEPTED:",  conf.sess_key[:12], '...' )
-    print(" ----- Post session, all is encrypted ----- ")
+    #print(" ----- Post session, all is encrypted ----- ")
 
-    resp4 = hand.client(["tout", "30",], conf.sess_key)
-    print("Server tout Response:", resp4)
+    #resp4 = hand.client(["tout", "30",], conf.sess_key)
+    #print("Server tout Response:", resp4)
 
     # Session estabilished, try a simple command
-    resp4 = hand.client(["hello",], conf.sess_key)
-    print("Server hello resp:", resp4[1])
-
-    cresp = hand.client(["user", "admin"], conf.sess_key)
-    print ("Server user respo:", cresp)
+    #resp4 = hand.client(["hello",], conf.sess_key)
+    #print("Server hello resp:", resp4[1])
 
-    cresp = hand.client(["pass", "1234"], conf.sess_key)
-    print ("Server pass resp:", cresp)
+    cresp = hand.login(conf.login, conf.lpass, conf)
+    if cresp[0] != 'OK':
+        print("Login Error:", cresp)
+        sys.exit(1)
 
     cresp = hand.client(["dmode",], conf.sess_key)
     #print("dmode", cresp)
     if cresp[1] == '0':
         print("Enter twofa code: (ret to skip)", end = "")
         sesscode = input()
         if sesscode:
             cresp = hand.client(["twofa", sesscode], conf.sess_key)
             print ("Server twofa resp:", cresp)
             if cresp[0] != "OK":
                 print ("Server twofa failed")
                 sys.exit(0)
 
-    # Interactive, need more time
-    tout = hand.client(["tout", "200",], conf.sess_key)
-    #print (tout)
-
     if conf.showx:
         cresp = hand.client(["ihost", "list", "",], conf.sess_key)
     elif conf.addx:
+        # Now the server will do it
+        #if conf.addx.find(":") < 0:
+        #    print("Missing ':' (colon). Entry must be in host:port format.")
+        #    sys.exit(1)
         cresp = hand.client(["ihost", "add", conf.addx,], conf.sess_key)
     elif conf.delx:
         cresp = hand.client(["ihost", "del", conf.delx,], conf.sess_key)
     else:
-        cresp = hand.client(["ihost", "add", "localhost:5555",], conf.sess_key)
+       pass
+       cresp = hand.client(["ihost", "add", "localhost:5555",], conf.sess_key)
 
-    print ("Server ihost response:", cresp)
+    if not conf.quiet:
+        print ("ihost resp:", end = " ")
+    print (cresp)
 
     cresp = hand.client(["quit",],conf.sess_key)
-    print ("Server quit  response:", cresp)
+    if conf.verbose:
+        print ("Quit  Resp:", cresp)
     hand.close();
 
     sys.exit(0)
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_login.py` & `pyvserv-1.0.4/pyvclient/pyvcli_lsd.py`

 * *Files 11% similar despite different names*

```diff
@@ -3,20 +3,16 @@
 from __future__ import print_function
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 from Crypto.Hash import SHA512
 import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat
+import  random, stat, datetime
 
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
 from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
@@ -27,17 +23,14 @@
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
     print( "            -p port   - Port to use (default: 6666)")
-    print( "            -l level  - Log level (default: 0)")
-    print( "            -c file   - Save comm to file")
-    print( "            -s        - Showkey")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
     #print( " Needs debug level or verbose to have any output.")
     print()
     sys.exit(0)
 
@@ -45,94 +38,105 @@
     print( os.path.basename(sys.argv[0]), "Version", support.version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
-    ["s",   "showkey",  "",     None],      \
-    ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
-
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
-    hand.comm  = conf.comm
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello", "world"] , "", False)
-    print("Hello Response: ", resp3)
+    resp3 = hand.client(["hello",] , "", False)
+    #print("Hello Response:", resp3[1])
 
     ret = hand.start_session(conf)
 
+    #if ret[0] == "OK":
+    #    print("Sess Key ACCEPTED:",  ret[1])
+
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
-    print("Sess Key ACCEPTED:",  conf.sess_key[:12], '...' )
-    #print("Post session, all is encrypted")
+    #print("Sess Key ACCEPTED:",  resp3[1])
+    print("Post session, all is encrypted")
 
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    print("Server hello Response:", resp4[1])
+    if not conf.quiet:
+        print("Hello Response:", resp4[1])
 
     cresp = hand.client(["user", "admin"], conf.sess_key)
-    print ("Server user  response:", cresp)
+    if not conf.quiet:
+        print ("Server user response:", cresp[1])
 
     cresp = hand.client(["pass", "1234"], conf.sess_key)
-    print ("Server pass  response:", cresp)
-
-    #resp = hand.client(["pass", "12345"], conf.sess_key)
-    #print ("Server pass  response:", cresp)
-
-    #resp = hand.client(["pass", "12345"], conf.sess_key)
-    #print ("Server pass response:", cresp)
-
-    #cresp = hand.client(["pass", "12345"], conf.sess_key)
-    #print ("Server pass response:", cresp[1])
-    #if(cresp[1][:2] != "OK"): sys.exit(1)
+    if not conf.quiet:
+        print ("Server pass response:", cresp[1])
 
-    #cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print ("Server pass  response:", cresp[1])
+    cresp = hand.client(["lsd",], conf.sess_key)
+    print ("Server lsd response:", cresp)
 
-    #cresp = hand.client(["hello", "1234"], conf.sess_key)
-    #print ("Server hello response:", cresp[1])
+    ''' Stat return values are as in python os.stat() + OK and name prefix
+    "OK", fname,
+    st_mode, st_ino, st_dev, st_nlink
+    st_uid, st_gid, st_size
+    st_atime, st_mtime, st_ctime
+    st_atime_ns
+    st_mtime_ns
+    st_ctime_ns '''
+
+    print ("Server stat response:")
+    for aa in cresp[1:]:
+        bb = support.unescape(aa)
+        cresp2 = hand.client(["stat", aa], conf.sess_key)
+        #print("cresp2", cresp2)
+        if cresp2[0] != "OK":
+            print("Bad entry from remote", cresp2)
+        else:
+            ddd = datetime.datetime.fromtimestamp(int(cresp2[10]))
+            print ("%s %-24s %-8d %s" %
+                (
+                support.mode2str(int(cresp2[2])), support.unescape(cresp2[1]),
+                        int(cresp2[8]), ddd)
+                )
+            #int(cresp2[9]), int(cresp2[10]), int(cresp2[11])
+            #print(ddd)
 
-    cresp = hand.client(["quit",],conf.sess_key)
-    print ("Server quit  response:", cresp[1])
+    hand.client(["quit",],conf.sess_key)
     hand.close();
 
     sys.exit(0)
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_ls.py` & `pyvserv-1.0.4/pyvclient/pyvcli_ls.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 from Crypto.Hash import SHA512
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat, datetime
 
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
 from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
@@ -89,30 +85,33 @@
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
     resp3 = hand.client(["hello",] , conf.sess_key, False)
-    print("Hello Response:", resp3)
+    if not conf.quiet:
+        print("Hello Response:", resp3)
 
     ret = hand.start_session(conf)
     if ret[0] != "OK":
         print("Error on setting session:", resp3)
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
     #print("Session Key ACCEPTED:",  ret, )
-    print("Session, with key:", conf.sess_key[:12], "...")
+    if not conf.quiet:
+        print("Session, with key:", conf.sess_key[:12], "...")
 
     # Session estabilished, try a simple command
-    #resp4 = hand.client(["hello",], conf.sess_key)
-    #print("Hello Response:", resp4[1])
+    resp4 = hand.client(["hello",], conf.sess_key)
+    if not conf.quiet:
+        print("Sess Response:", resp4)
 
     ret =  hand.login("admin", "1234", conf)
     if ret[0] != "OK":
         print ("Server login fail:", ret)
         hand.client(["quit"], conf.sess_key)
         hand.close();
         sys.exit(0)
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_lsd.py` & `pyvserv-1.0.4/pyvclient/pyvcli_rget.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,167 +1,171 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
-from __future__ import print_function
+import sys
+if sys.version_info[0] < 3:
+    print("Python 2 is not supported as of 1/1/2020")
+    sys.exit(1)
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# Test client for the pyserv project. Download file.
 
-from Crypto.Hash import SHA512
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, datetime
-
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
-from Crypto import Random
-
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
-
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
-
-'''
-# test encrypt with large keys
-rrr =  "mTQdnL51eKnblQflLGSMvnMKDG4XjhKa9Mbgm5ZY9YLd" \
-        "/SxqZZxwyKc/ZVzCVwMxiJ5X8LdX3X5VVO5zq/VBWQ=="
-sss = bluepy.encrypt(rrr, conf.sess_key)
-ttt = bluepy.decrypt(sss, conf.sess_key)
-print (rrr)
-print (ttt)
-'''
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat, datetime
+
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
+
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
+
+# ------------------------------------------------------------------------
+# Globals
+
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
-# Functions from command line
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p port   - Port to use (default: 6666)")
-    print( "            -l level  - Log level (default: 0)")
-    print( "            -c file   - Save comm to file")
-    print( "            -s        - Showkey")
+    print( "            -p        - Port to use (default: 6666)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
+    print( "            -r recids - Record IDs to get")
+    print( "            -b        - Start / Begin time. Format: 'Y-m-d+H:M' Default: now")
+    print( "            -i        - Interval in minutes. (Default: 1 day)")
     print( "            -h        - Help")
-    #print( " Needs debug level or verbose to have any output.")
     print()
+    print("  Use quotes for multiple arguments on recids.")
+    print()
+
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", support.version)
+    print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["s",   "showkey",  "",     None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["f:",  "fname",    "test.txt", None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["n",   "plain",    0,          None],      \
+    ["r:",  "rget",     "",         None],      \
+    ["b:",  "begin",    "",        None],      \
+    ["i:",  "inter",    0,          None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def    mainfunct():
 
     args = conf.comline(sys.argv[1:])
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
+    #print(dir(conf))
+
+    #if conf.comm:
+    #    print("Save to filename", conf.comm)
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
-    hand.comm  = conf.comm
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello",] , "", False)
-    #print("Hello Response:", resp3[1])
+    #resp3 = hand.client(["id",] , "", False)
+    #print("ID Response:", resp3[1])
 
+    #ret = ["OK",];  conf.sess_key = ""
     ret = hand.start_session(conf)
-
-    #if ret[0] == "OK":
-    #    print("Sess Key ACCEPTED:",  ret[1])
-
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
     #print("Sess Key ACCEPTED:",  resp3[1])
-    print("Post session, all is encrypted")
 
-    # Session estabilished, try a simple command
-    resp4 = hand.client(["hello",], conf.sess_key)
-    print("Hello Response:", resp4[1])
-
-    cresp = hand.client(["user", "admin"], conf.sess_key)
-    print ("Server user response:", cresp[1])
-
-    cresp = hand.client(["pass", "1234"], conf.sess_key)
-    print ("Server pass response:", cresp[1])
-
-    # Error responses
-    #cresp = hand.client(["pwd",], conf.sess_key)
-    #print ("Server pwd response:", cresp)
-
-    cresp = hand.client(["lsd",], conf.sess_key)
-    print ("Server lsd response:", cresp)
-
-    ''' Stat return values are as in python os.stat() + OK and name prefix
-    "OK", fname,
-    st_mode, st_ino, st_dev, st_nlink
-    st_uid, st_gid, st_size
-    st_atime, st_mtime, st_ctime
-    st_atime_ns
-    st_mtime_ns
-    st_ctime_ns '''
-
-    print ("Server stat response:")
-    for aa in cresp[1:]:
-        bb = support.unescape(aa)
-        cresp2 = hand.client(["stat", aa], conf.sess_key)
-        #print("cresp2", cresp2)
-        if cresp2[0] != "OK":
-            print("Bad entry from remote", cresp2)
-        else:
-            ddd = datetime.datetime.fromtimestamp(int(cresp2[10]))
-            print ("%s %-24s %-8d %s" %
-                (
-                support.mode2str(int(cresp2[2])), support.unescape(cresp2[1]),
-                        int(cresp2[8]), ddd)
-                )
-            #int(cresp2[9]), int(cresp2[10]), int(cresp2[11])
-            #print(ddd)
+    #if conf.sess_key:
+    #    print("Post session, session key:", conf.sess_key[:12], "...")
 
-    hand.client(["quit",],conf.sess_key)
-    hand.close();
+    resp3 = hand.client(["hello", ],  conf.sess_key, False)
+    #print("Hello Response:", resp3)
 
-    sys.exit(0)
+    cresp = hand.login("admin", "1234", conf)
+    #print ("Server login response:", cresp)
 
-# EOF
+    dd_beg, dd_end = pyclisup.inter_date(conf.begin, conf.inter)
+    print("date from:", dd_beg, "to:", dd_end);
+
+    if conf.rget:
+        rgetarr = conf.rget.split()
+        #print("rgetarr:", rgetarr)
+        cresp = hand.client(["rget", "vote", rgetarr], conf.sess_key)
+        if cresp[0] == "OK":
+            #print("rget resp:", cresp)
+            for aa in cresp[3]:
+                pyclisup.show_onerec(hand, aa, conf)
+
+                #dec = hand.pb.decode_data(aa[1])[0]
+                #if conf.verbose:
+                #    print("dec:", dec)
+                #pay = hand.pb.decode_data(dec['payload'])[0]
+                #if conf.verbose:
+                #    print("dec:", dec)
+                #else:
+                #    print("pay:", pay['PayLoad'])
+    else:
+        cresp = hand.client(["rlist", "vote", dd_beg.timestamp(),
+                         dd_end.timestamp()], conf.sess_key)
+        #print ("Server  rlist response:", cresp)
+        if cresp[0] != "OK":
+            print("Cannot get rlist", cresp)
+            cresp = hand.client(["quit", ], conf.sess_key)
+            sys.exit(0)
+        #print("rlist got", len(cresp[1]), "records")
+        for aaa in cresp[1]:
+            cresp2 = hand.client(["rget", "vote", [aaa]], conf.sess_key)
+            if cresp2[0] != "OK":
+                print("Cannot get record", cresp2)
+                continue
+            #print("cresp2:", cresp2)
+            for aa in cresp2[3]:
+                pyclisup.show_onerec(hand, aa, conf)
+        print("Listed", len(cresp[1]), "records.")
 
+    cresp = hand.client(["quit", ], conf.sess_key)
+    #print ("Server quit response:", cresp)
+
+if __name__ == '__main__':
+    mainfunct()
+
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_mkdir.py` & `pyvserv-1.0.4/pyvclient/pyvcli_mkdir.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,49 +16,45 @@
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level   - Debug level 0-10")
     print( "            -c dirname - Directory to create. default: test_3")
     print( "            -p         - Port to use (default: 6666)")
     print( "            -v         - Verbose")
     print( "            -q         - Quiet")
-    print( "            -n         - No encryption (plain)")
     print( "            -h         - Help")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["c:",  "fname",    "test_3", None],    \
-    ["p:",  "port",     6666,   None],      \
-    ["f:",  "file",     6666,   None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["n",   "plain",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["c:",  "fname",    "test_dir", None],    \
+    ["p:",  "port",     6666,       None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
@@ -85,54 +81,42 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #resp3 = hand.client(["id",] , "", False)
-    #print("ID Response:", resp3[1])
-
-    #ret = ["OK",];  conf.sess_key = ""
     ret = hand.start_session(conf)
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
-    # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
-
-    if conf.sess_key:
-        print("Post session, session key:", conf.sess_key[:12], "...")
+    if not conf.quiet:
+        print("Session key:", conf.sess_key[:12], "...")
 
     resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    print("Hello Response:", resp3)
-
-    # Session estabilished, try a simple command
-    #resp4 = hand.client(["hello",], conf.sess_key)
-    #print("Hello Response:", resp4[1])
+    if not conf.quiet:
+        print("Hello Response:", resp3)
 
     cresp = hand.login("admin", "1234", conf)
-    print ("Server login response:", cresp)
-
-    #cresp = hand.client(["ls", ], conf.sess_key)
-    #print ("Server  ls response:", cresp)
+    if not conf.quiet:
+        print ("Server login response:", cresp)
 
     #cresp = hand.client(["buff", "10", ], conf.sess_key)
     #print ("Server buff response:", cresp)
     #if cresp[0] != "OK":
     #    print("Error on buff command", cresp[1])
     #    hand.client(["quit"], conf.sess_key)
     #    hand.close();
     #    sys.exit(0)
 
     ret2 = hand.client(["mkdir", conf.fname], conf.sess_key)
     print ("Server mkdir response:", ret2)
 
     cresp = hand.client(["quit", ], conf.sess_key)
-    print ("Server quit response:", cresp)
+    #print ("Server quit response:", cresp)
 
     sys.exit(0)
 
-
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_pass.py` & `pyvserv-1.0.4/pyvclient/pyvcli_pass.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,18 +5,14 @@
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Encrypt test.
 
 from Crypto.Hash import SHA512
 import  os, sys, getopt, signal, select, socket, time, struct
 import  random, stat
 
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
 from Crypto import Random
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_ping.py` & `pyvserv-1.0.4/pyvclient/pyvcli_ping.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_qr.py` & `pyvserv-1.0.4/pyvclient/pyvcli_throt.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,9 @@
 #!/usr/bin/env python
 
-import sys, os
-import readline
-
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
-
 # ------------------------------------------------------------------------
 # Test client for the pyserv project.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
 # This repairs the path from local run to pip run.
@@ -26,61 +19,54 @@
 
 from pyvcommon import support, pycrypt, pyclisup
 from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
+    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options] [hostname]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
     print( "            -p        - Port to use (default: 6666)")
-    print( "            -f file   - Upload new QR image file")
+    print( "            -t flag   - Throttle on / off")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
-    print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["f:",  "file",     "",     None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["n",   "plain",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["t:",   "throt",   "",         None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-def mainfunct():
+if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
 
-    #print(vars(conf))
-    #if conf.comm:
-    #    print("Save to filename", conf.comm)
-
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
@@ -91,39 +77,46 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    conf.sess_key = ""
-    #ret = ["OK",];  conf.sess_key = ""
-    resp3 = hand.start_session(conf)
-    if resp3[0] != "OK":
+    ret = hand.start_session(conf)
+    if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
+        hand.client(["quit"])
+        hand.close();
         sys.exit(0)
 
-    if conf.file:
-        fp = open(conf.file, "rb")
-        buff = fp.read()
-        fp.close()
-        #print("len:", len(buff))
-        resp3 = hand.client(["qr", buff], conf.sess_key, False)
-        print("QR UP Response:", resp3)
+    # Session estabilished, try a simple command
+    resp4 = hand.client(["hello",], conf.sess_key)
+    if conf.verbose:
+        print("Hello Resp:", resp4)
+
+    cresp = hand.client(["user", "admin"], conf.sess_key)
+    #if not conf.quiet:
+    #    print ("Server user response:", cresp[1])
+
+    cresp = hand.client(["pass", "1234"], conf.sess_key)
+    if not conf.quiet:
+        print ("Server pass response:", cresp)
+
+    if not conf.throt:
+        cresp = hand.client(["throt", ], conf.sess_key)
     else:
-        resp3 = hand.client(["qr",], conf.sess_key, False)
-        #print("QR Response:", resp3)
-        fp = open("qr.png", 'wb')
-        if type(resp3[1]) != type(b""):
-            resp3[1] = resp3[1].encode()
-        fp.write(resp3[1])
-        fp.close()
+        cresp = hand.client(["throt", conf.throt,], conf.sess_key)
 
-    hand.client(["quit"], conf.sess_key)
-    hand.close();
+    print ("Server throt response:", cresp)
 
-    sys.exit(0)
+    if cresp[0] != "OK":
+        #print("Err: ", cresp)
+        cresp = hand.client(["quit", ], conf.sess_key)
+        #print ("Server quit response:", cresp)
+        sys.exit(0)
 
-if __name__ == '__main__':
-    mainfunct()
+    cresp = hand.client(["quit", ], conf.sess_key)
+    #print ("Server quit response:", cresp)
+
+    sys.exit(0)
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_replic.py` & `pyvserv-1.0.4/pyvclient/pyvcli_rman.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,300 +5,247 @@
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
 # ------------------------------------------------------------------------
 # Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
-import random, stat, datetime, atexit
-
-#from pyvcli_utils import *
+import random, stat, datetime, atexit, uuid
 
 # This repairs the path from local run to pip run.
-# Remove pip version for local tests
-
 try:
     from pyvcommon import support
-    #print("sf", sf)
-    # Get Parent of module root
-    sf = os.path.dirname(support.__file__)
-    sf = os.path.dirname(sf)
-    sys.path.append(os.path.join(sf, "pyvcommon"))
-    sys.path.append(os.path.join(sf, "pyvserver"))
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
 except:
-    #print("pathching")
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
-    sys.path.append(os.path.join(base,  '..', "pyvserver"))
     from pyvcommon import support
 
-def atexit_func(hand, conf):
-
-    ''' Severe connection on exit '''
-
-    try:
-        print("Atexit")
-        cresp = hand.client(["quit", ], conf.sess_key)
-        print ("Server quit response:", cresp)
-        hand.close();
-    except:
-        pass
-
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
-
-hand = None
-hand2 = None
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline, pyvhash
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
+#progn = os.path.basename(sys.argv[0])
+progn = os.path.basename(__file__)
+
+cdoc = '''\
+The pyvserv record manager.
+Usage: %s [options] [hostname]
+  hostname: host to connect to. (default: 127.0.0.1)
+  options:   -d level  - Debug level 0-10
+             -p        - Port to use (default: 6666)
+             -l login  - Login Name; default: 'admin'
+             -s lpass  - Login Pass; default: '1234' (for !!testing only!!)
+             -t        - prompt for login pass")
+             -a recpos - Get record by absolute pos. Negative for pos. from end
+             -r recids - Record IDs to get
+             -b date   - Start / Begin time. See format below. default:today
+             -i mins   - Interval in minutes. (default: 1 day)
+             -c        - Get records between specified dates
+             -u        - Upload record (randomly generated)
+             -o        - Count records in date range
+             -z        - Get remote database size
+             -v        - Verbose          -|-  -V        - Print version number
+             -q        - Quiet            -|-  -h        - Help (this screen)
+Use quotes for multiple arguments. (example: -a \"-1 -2 -3\" -- lists last 3)
+Possible date Formats: 'Y-m-d+H:M' 'Y-m-d' 'm-d' 'm-d+H-M'  '''  \
+% (progn)
+
+__doc__= "<pre>" + cdoc + "</pre>"
 
 # ------------------------------------------------------------------------
 
 def phelp():
-
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 6666)")
-    print( "            -v        - Verbose")
-    print( "            -q        - Quiet")
-    print( "            -n        - No encryption (plain)")
-    print( "            -h        - Help")
-    print()
+    ''' Present command line help '''
+    print(cdoc)
     sys.exit(0)
 
 def pversion():
+    ''' Display Version information '''
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,          None],      \
     ["p:",  "port",     6666,       None],      \
-    ["P:",  "port_to",  5555,       None],      \
-    ["f:",  "fname",    "test.txt", None],      \
+    ["l:",  "login",    "admin",    None],      \
+    ["s:",  "lpass",    "1234",     None],      \
+    ["t",   "lprompt",  0,          None],      \
     ["v",   "verbose",  0,          None],      \
     ["q",   "quiet",    0,          None],      \
-    ["n",   "plain",    0,          None],      \
-    ["t",   "test",     "x",        None],      \
+    ["u",   "upload",   0,          None],      \
+    ["c",   "cget",     0,          None],      \
+    ["z",   "size",    0,          None],       \
+    ["r:",  "rget",     "",         None],      \
+    ["a:",  "rabs",     "",         None],      \
+    ["b:",  "begin",     "",        None],      \
+    ["i:",  "inter",    0,          None],      \
+    ["o",   "count",    0,          None],      \
     ["V",   None,       None,       pversion],  \
     ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
-conf2 = comline.Config(optarr)
-
-def scanfordays(handx, handx2):
-
-    global hand, hand2
-    hand    = handx
-    hand2   = handx2
-
-    # Set beginning date range
-    dd = datetime.datetime.now()
-    dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
-
-    maxdays = 5; dayx = 0
-
-    dd = datetime.datetime.now()
-    dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
-    dd = dd - datetime.timedelta(maxdays)
-
-    # Scan which days have records
-    while True:
-        dd_beg = dd + datetime.timedelta(dayx)
-        dd_end = dd_beg + datetime.timedelta(1)
-
-        cresp = hand.client(["rcount", "vote", dd_beg.timestamp(),
-                                        dd_end.timestamp()], conf.sess_key)
-        if cresp[1] > 0:
-            print("from:", dd_beg, "to:", dd_end);
-            print ("Server rcount response:", cresp)
-
-            if cresp[1] >= 100:
-                scanhours(maxdays - dayx)
-            else:
-                print("getting day:", dd_bed, "-", dd_end)
-
-        #if cresp[1] > 100:
-        #    #print("record with more", cresp[1])
-        #    pass
-
-        dayx += 1
-        # We end one day late to include all timezone deviations
-        if dayx >= maxdays + 1:
-            break
-
-# Scan which hours of days that have records
-def scanhours(dayx):
-
-    # Set beginning date range
-    dd = datetime.datetime.now()
-    dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
-    dd = dd - datetime.timedelta(dayx)
-
-    maxhours = 24; hourx = 0
-
-    while True:
-        dd_beg = dd + datetime.timedelta(0, hourx * 3600)
-        dd_end = dd_beg + datetime.timedelta(0, 1 * 3600)
-
-        cresp = hand.client(["rcount", "vote", dd_beg.timestamp(),
-                                        dd_end.timestamp()], conf.sess_key)
-        if cresp[1] > 0:
-            print(" from:", dd_beg, "to:", dd_end);
-            print(" Server hour rcount response:", cresp)
-            if cresp[1] >= 100:
-                scanminutes(dayx, hourx)
-            else:
-                print(" getting hour:", dd_beg, " - ", dd_end)
-                cresp = hand.client(["rlist", "vote", dd_beg.timestamp(),
-                                    dd_end.timestamp()], conf.sess_key)
-
-        hourx += 1
-        if hourx > maxhours:
-            break
-
-def scanminutes(dayx, hourx):
-
-    # Set beginning date range
-    dd = datetime.datetime.now()
-    dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
-    dd = dd - datetime.timedelta(dayx)
-    dd = dd + datetime.timedelta(0, hourx * 3600)
-
-    maxmins = 60; minx = 0
-
-    while True:
-        dd_beg = dd + datetime.timedelta(0, minx * 60)
-        dd_end = dd_beg + datetime.timedelta(0, 60)
-
-        cresp = hand.client(["rcount", "vote", dd_beg.timestamp(),
-                                        dd_end.timestamp()], conf.sess_key)
-        if cresp[1] > 0:
-            print("    from:", dd_beg, "to:", dd_end);
-            print("    Server min  rcount response:", cresp)
-
-            if cresp[1] >= 100:
-                print("    ----------- big rec count")
-            else:
-                #print("    getting minutes:", dd_beg, "-", dd_end)
-                cresp = hand.client(["rlist", "vote", dd_beg.timestamp(),
-                                    dd_end.timestamp()], conf.sess_key)
-                if cresp[0] == "OK":
-                    crespr = hand.client(["rget", "vote", cresp[1]], conf.sess_key)
-                    #print("rget", crespr)
-                    for aa in crespr[1]:
-                        #print("aa", aa)
-                        dec = hand.pb.decode_data(aa[1])[0]
-                        #print("dec", dec)
-                        print(dec['header'], dec['payload'])
-
-                    #for aa in cresp[1]:
-                    #    #print("head", aa)
-                    #    #crespg = hand2.client(["rhave", "vote", aa], conf2.sess_key)
-                    #    #print("rhave", crespg)
-                    #    if 1: #crespg[0] != "OK":
-                    #        crespr = hand.client(["rget", "vote", aa], conf.sess_key)
-                    #        #print("Rec", crespr[1])
-                    #        cresp3 = hand2.client(
-                    #                ["rput", "vote", crespr[1][0], ], conf2.sess_key)
-                    #        if cresp3[0] == 'OK':
-                    #            print("rput", cresp3)
-                #print(cresp)
-
-        minx += 1
-        if minx > maxmins:
-            break
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
-
-    args = conf.comline(sys.argv[1:])
+def    mainfunct():
 
+    ''' Entry point for pip script '''
 
-    #print(dir(conf))
+    try:
+        args = conf.comline(sys.argv[1:])
 
-    #if conf.comm:
-    #    print("Save to filename", conf.comm)
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        #print(sys.exc_info())
+        sys.exit(1)
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
-        ip2 = '127.0.0.1'
     else:
         ip = args[0]
-        ip2 = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
+    dd_beg, dd_end = pyclisup.inter_date(conf.begin, conf.inter)
+    if conf.verbose:
+        print("Date begin:", dd_beg, "Date end", dd_end)
+    if conf.lprompt:
+        import getpass
+        strx = getpass.getpass("Pass for login %s: " % conf.login)
+        if not strx:
+            print("Cannot login with empty pass, aborting ...")
+            sys.exit(0)
+        conf.lpass = strx
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    atexit.register(atexit_func, hand, conf)
-
-    hand2 = pyclisup.CliSup()
-    hand2.verbose = conf.verbose
-    hand2.pgdebug = conf.pgdebug
-
-    try:
-        respc = hand2.connect(ip, conf.port_to)
-    except:
-        print( "Cannot connect to second server:", ip2 + ":" + str(conf.port_to), sys.exc_info()[1])
-        sys.exit(1)
-
-    atexit.register(atexit_func, hand2, conf2)
-
-    #resp3 = hand.client(["id",] , "", False)
-    #print("ID Response:", resp3[1])
+    atexit.register(pyclisup.atexit_func, hand, conf)
 
     #ret = ["OK",];  conf.sess_key = ""
     ret = hand.start_session(conf)
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
-    ret2 = hand2.start_session(conf2)
-    if ret2[0] != "OK":
-        print("Error on setting session:", resp3[1])
-        hand2.client(["quit"])
-        hand2.close();
+    cresp = hand.login(conf.login, conf.lpass, conf)
+    #print ("Server login response:", cresp)
+    if cresp[0] != "OK":
+        print("Error on logging in:", cresp)
+        hand.client(["quit"], conf.sess_key)
+        hand.close();
         sys.exit(0)
 
-    # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
+    if conf.upload:
 
-    if conf.sess_key:
-        print("Post session, session key:", conf.sess_key[:12], "...")
+        actstr = ["register", "unregister", "cast", "uncast", ]
+        act = actstr[random.randint(0, len(actstr)-1)]
 
-    #resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    #print("Hello Response:", resp3)
+        print("Calculating hash ....", end = " "); sys.stdout.flush()
+        #ttt = time.time()
+        pvh = pyvhash.BcData()
+        pvh.addpayload({"Vote": random.randint(0, 10), "UID":  str(uuid.uuid1()), })
+        pvh.addpayload({"SubVote": random.randint(0, 10), "TUID":  str(uuid.uuid1()), })
+        pvh.addpayload({"Action": act , "RUID":  str(uuid.uuid1()), })
+        pvh.hasharr();    pvh.powarr()
+        print("OK")
+        cresp = hand.client(["rput", "vote", pvh.datax], conf.sess_key)
+        print ("rput resp:", cresp)
+
+    elif conf.cget:
+        import shlex
+        shlex.split(conf.rget)
+        cresp = hand.client(["rlist", "vote", dd_beg.timestamp(),
+                         dd_end.timestamp()], conf.sess_key)
+
+        if cresp[0] != "OK":
+            print("Cannot get rlist", cresp)
+        else:
+            #print("cresp", cresp)
+            for aaa in cresp[1]:
+                cresp2 = hand.client(["rget", "vote", [aaa]], conf.sess_key)
+                if cresp2[0] != "OK":
+                    print("Cannot get record", cresp2)
+                    continue
+                #print("cresp2:", cresp2)
+                for aa in cresp2[3]:
+                    pyclisup.show_onerec(hand, aa, conf)
+
+            print("Listed", len(cresp[1]), "records.")
+
+    elif conf.rabs:
+        arrx = conf.rabs.split()
+        #print("getting", arrx)
+        cresp2 = hand.client(["rabs", "vote", *arrx], conf.sess_key)
+        #print("rabs got:", cresp2)
+        if cresp2[0] != "OK":
+            print("Cannot get rabs:", cresp2)
+            cresp = hand.client(["quit", ], conf.sess_key)
+            sys.exit()
+        for aa in cresp2[3]:
+            #print("aa", aa)
+            pyclisup.show_onerec(hand, aa, conf)
 
-    cresp = hand.login("admin", "1234", conf)
-    print ("Server login response:", cresp)
+        print("Listed", len(cresp2[3]), "records.")
 
-    cresp = hand.client(["rsize", "vote",], conf.sess_key)
-    print ("Server rsize response:", cresp)
+    elif conf.count:
+        cresp = hand.client(["rcount", "vote", dd_beg.timestamp(),
+                         dd_end.timestamp()], conf.sess_key)
 
-    cresp = hand2.login(conf2, "admin", "1234")
-    print ("Server login response:", cresp)
+        #cresp = hand.client(["rcount", "vote"], conf.sess_key)
+        print ("Server rcount response:", cresp)
 
-    cresp = hand2.client(["rsize", "vote",], conf2.sess_key)
-    print ("Server rsize response:", cresp)
+    elif conf.size:
+        cresp = hand.client(["rsize", "vote"], conf.sess_key)
+        print ("Server rsize response:", cresp)
+
+    elif conf.rget:
+        arrx = conf.rget.split()
+        print("getting", arrx)
+        cresp2 = hand.client(["rget", "vote", arrx], conf.sess_key)
+        #print("rabs got:", cresp2)
+        if cresp2[0] != "OK":
+            print("Error on rget:", cresp2)
+            sys.exit()
+
+        for aa in cresp2[3]:
+            #print("aa", aa)
+            pyclisup.show_onerec(hand, aa, conf)
 
-    scanfordays(hand, hand2)
+        print("Listed", len(cresp2[3]), "records.")
+
+    else:
+        # Get last record
+        cresp = hand.client(["rsize", "vote"], conf.sess_key)
+        if not conf.quiet:
+            print ("Server rsize response:", cresp)
+        # Offset is one less than count
+        cresp2 = hand.client(["rabs", "vote", cresp[1] - 1], conf.sess_key)
+        #print ("Server rabs response:", cresp2)
+        pyclisup.show_onerec(hand, cresp2[3][0], conf)
+
+    cresp = hand.client(["quit", ], conf.sess_key)
+    #print ("Server quit response:", cresp)
+
+if __name__ == '__main__':
+    mainfunct()
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_rget.py` & `pyvserv-1.0.4/pyvclient/pyvcli_rput.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,188 +1,191 @@
-#!/usr/bin/env python
-
-import sys
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
+#!/usr/bin/env python3
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Download file.
+# Test client for the pyserv project. Encrypt test.
+
+import  os, sys, getopt, signal, select, socket, time, struct
+import  random, stat, uuid, atexit
 
-import os, sys, getopt, signal, select, socket, time, struct
-import random, stat, datetime
+from Crypto import Random
 
 # This repairs the path from local run to pip run.
+# Remove pip version for local tests
+
 try:
     from pyvcommon import support
-    base = os.path.dirname(os.path.realpath(support.__file__))
-    sys.path.append(os.path.join(base, "."))
+    #print("sf", sf)
+    # Get Parent of module root
+    sf = os.path.dirname(support.__file__)
+    sf = os.path.dirname(sf)
+    sys.path.append(os.path.join(sf, "pyvcommon"))
+    sys.path.append(os.path.join(sf, "pyvserver"))
 except:
+    #print("pathching")
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    sys.path.append(os.path.join(base,  '..', "pyvserver"))
     from pyvcommon import support
 
-from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import support, pycrypt, pyservsup, pyclisup, pyvhash
 from pyvcommon import pysyslog, comline
 
-# ------------------------------------------------------------------------
-# Globals
-
-version = 1.0
+import pyvpacker
 
 # ------------------------------------------------------------------------
+# Functions from command line
+
+#print( "            -n        - Number of records to put")
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 6666)")
+    print( "            -p port   - Port to use (default: 6666)")
+    print( "            -k keyval - Put this key")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
-    print( "            -r        - Record ID to get")
-    print( "            -s        - Start time. Format: 'Y-m-d H:M'")
-    print( "            -i        - Interval in minutes. (Default: 1 day)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", version)
+    print( os.path.basename(sys.argv[0]), "Version", support.version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,          None],      \
-    ["p:",  "port",     6666,       None],      \
-    ["f:",  "fname",    "test.txt", None],      \
-    ["v",   "verbose",  0,          None],      \
-    ["q",   "quiet",    0,          None],      \
-    ["n",   "plain",    0,          None],      \
-    ["r:",  "rget",     "",         None],      \
-    ["s:",  "start",     "",        None],      \
-    ["i:",  "inter",    0,          None],      \
-    ["V",   None,       None,       pversion],  \
-    ["h",   None,       None,       phelp]      \
+    ["d:",  "pgdebug",  0,      None],      \
+    ["p:",  "port",     6666,   None],      \
+    ["c:",  "comm",     "",     None],      \
+    ["v",   "verbose",  0,      None],      \
+    ["q",   "quiet",    0,      None],      \
+    ["k:",  "putkey",   "",     None],      \
+    ["n:",  "numrec",   1,     None],      \
+    ["t",   "test",     "x",    None],      \
+    ["V",   None,       None,   pversion],  \
+    ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-def    mainfunct():
+def mainfunct():
 
     args = conf.comline(sys.argv[1:])
-
-    #print(dir(conf))
-
-    #if conf.comm:
-    #    print("Save to filename", conf.comm)
+    #print(vars(conf))
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
+    hand.comm  = conf.comm
+
+    actstr = ["register", "unregister", "cast", "uncast", ]
+    act = actstr[random.randint(0, len(actstr)-1)]
+
+    #ttt = time.time()
+    pvh = pyvhash.BcData()
+    pvh.addpayload({"Vote": random.randint(0, 10), "UID":  str(uuid.uuid1()), })
+    pvh.addpayload({"SubVote": random.randint(0, 10), "TUID":  str(uuid.uuid1()), })
+    pvh.addpayload({"Action": act , "RUID":  str(uuid.uuid1()), })
+    # We mark this as 'test' so it can stay in the chain, if desired
+    pvh.addpayload({"Test": "test" ,})
+
+
+    if conf.putkey:
+        pvh.datax['header'] = conf.putkey
+
+    print("Calculating hash ....", end = " "); sys.stdout.flush()
+    pvh.hasharr();    pvh.powarr()
+    print("OK")
+
+    if not pvh.checkhash():
+        print("Error on hashing payload .. retrying ...")
+    elif not pvh.checkpow():
+        print("Error on POW payload .. retrying ...")
+
+    if conf.verbose:
+        print(pvh.datax)
+        #!/usr/bin/env python3
+
+    #print("Chain cnt", pvh.cnt)
+    #print("chain %.3fms" % ((time.time() - ttt) * 1000) )
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #resp3 = hand.client(["id",] , "", False)
-    #print("ID Response:", resp3[1])
+    atexit.register(pyclisup.atexit_func, hand, conf)
+
+    #resp3 = hand.client(["hello", "world"] , "", False)
+    #print("Hello Resp:", resp3)
 
-    #ret = ["OK",];  conf.sess_key = ""
     ret = hand.start_session(conf)
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
-        hand.client(["quit"])
-        hand.close();
         sys.exit(0)
 
-    # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
-
-    #if conf.sess_key:
-    #    print("Post session, session key:", conf.sess_key[:12], "...")
-
-    resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    #print("Hello Response:", resp3)
-
-    cresp = hand.login("admin", "1234", conf)
-    #print ("Server login response:", cresp)
-
-    if conf.start:
-        dd = datetime.datetime.now()
-        #print(dd)
-        try:
-            dd = dd.strptime(conf.start, "%Y-%m-%d %H:%M")
-        except:
-            try:
-                dd = dd.strptime(conf.start, "%Y-%m-%d")
-            except:
-                raise
-        print("date from comline:", dd)
-    else:
-        # Beginning of today
-        dd = datetime.datetime.now()
-        dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
-
-    dd_beg = dd + datetime.timedelta(0)
-
-    if conf.inter:
-        dd_end = dd_beg + datetime.timedelta(0, conf.inter * 60)
-    else:
-        dd_end = dd_beg + datetime.timedelta(1)
+    #ttt = time.time()
+    # Session estabilished, try a simple command
+    #resp4 = hand.client(["hello",], conf.sess_key)
+    #print("hello %.3fms" % ((time.time() - ttt) * 1000) )
+    #if resp4[0] != "OK":
+    #    print("Server hello resp:", resp4[1])
+    #    sys.exit()
+
+    #ttt = time.time()
+    cresp = hand.client(["user", "admin"], conf.sess_key)
+    #print("user %.3fms" % ((time.time() - ttt) * 1000) )
+    #print ("Server user respo:", cresp)
+    #ttt = time.time()
+    cresp = hand.client(["pass", "1234"], conf.sess_key)
+    #print("pass %.3fms" % ((time.time() - ttt) * 1000) )
+    if cresp[0] != "OK":
+        print("Cannot log on")
+        sys.exit(1)
+    if not conf.quiet:
+        print ("Server pass resp:", cresp)
 
-    print("from:", dd_beg, "to:", dd_end);
-    if conf.rget:
-        rgetarr = conf.rget.split()
-        #print("rgetarr:", rgetarr)
-        cresp = hand.client(["rget", "vote", rgetarr], conf.sess_key)
-        if cresp[0] == "OK":
-            #print("rget resp:", cresp[1])
-            for bb in cresp[1]:
-                #print("rget bb:", bb)
-                if type(bb[1]) == type({}):
-                    print("Initial record. Skipping.")
-                    continue
-                #print("bb", bb)
-                dec = hand.pb.decode_data(bb[1])[0]
-                #print("dec", dec)
-                print(dec['header'], dec['payload'])
-    else:
-        cresp = hand.client(["rlist", "vote", dd_beg.timestamp(),
-                         dd_end.timestamp()], conf.sess_key)
-        #print ("Server  rlist response:", cresp)
-        if cresp[0] != "OK":
-            print("Cannot get rlist", cresp)
-            cresp = hand.client(["quit", ], conf.sess_key)
-            sys.exit(0)
-        print("rlist got", cresp[1], "records")
-        for aa in cresp[1]:
-            cresp2 = hand.client(["rget", "vote", [aa]], conf.sess_key)
-            if cresp2[0] != "OK":
-                print("Cannot get record", cresp)
-                #break
-            #print("cresp2:", cresp2)
-            for aa in cresp2[1]:
-                #print("aa", aa)
-                dec = hand.pb.decode_data(aa[1])
-                print("dec:", dec[0]['header'], dec[0]['now'], dec[0]['payload'])
+    cresp = hand.client(["dmode",], conf.sess_key)
+    #print("dmode", cresp)
+    if cresp[1] == '0':
+        print("Enter twofa code: (ret to skip)", end = "")
+        sesscode = input()
+        if sesscode:
+            cresp = hand.client(["twofa", sesscode], conf.sess_key)
+            print ("Server twofa resp:", cresp)
+            if cresp[0] != OK:
+                print ("Server twofa failed")
+                sys.exit(0)
+
+    if conf.pgdebug > 2:
+        print(pvh.datax)
+
+    if hand.verbose:
+        print("Sending Data:", pvh.datax)
+
+    #ttt = time.time()
+    for aa in range(conf.numrec):
+        cresp = hand.client(["rput", "vote", pvh.datax], conf.sess_key)
+        print ("rput resp:", cresp)
+    #print("rput %.3fms" % ((time.time() - ttt) * 1000) )
 
-    cresp = hand.client(["quit", ], conf.sess_key)
-    print ("Server quit response:", cresp)
+    sys.exit(0)
 
 if __name__ == '__main__':
     mainfunct()
 
 # EOF
+
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_rlist.py` & `pyvserv-1.0.4/pyvclient/pyvcli_rlist.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,48 +24,50 @@
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
     print( "            -p        - Port to use (default: 6666)")
+    print( "            -l login  - Login Name; default: 'admin'")
+    print( "            -s lpass  - Login Pass; default: '1234' (for !!testing only!!)")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
-    print( "            -s        - Start time. Format: 'Y-m-d H:M'")
+    print( "            -b        - Start / Begin time. See format below. Default:today")
     print( "            -i        - Interval in minutes. (Default: 1 day)")
-    print( "            -n        - No encryption (plain)")
     print( "            -h        - Help")
+    print("  Possible date Formats: 'Y-m-d+H:M' 'Y-m-d' 'm-d' 'm-d+H-M'")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,          None],      \
     ["p:",  "port",     6666,       None],      \
+    ["l:",  "login",    "admin",    None],      \
+    ["s:",  "lpass",    "1234",     None],      \
     ["v",   "verbose",  0,          None],      \
     ["q",   "quiet",    0,          None],      \
-    ["n",   "plain",    0,          None],      \
-    ["t",   "test",     "x",        None],      \
+    ["b:",  "begin",    "",         None],      \
     ["i:",  "inter",    0,          None],      \
-    ["s:",  "start",    "",         None],      \
     ["V",   None,       None,       pversion],  \
     ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
@@ -105,54 +107,43 @@
     ret = hand.start_session(conf)
     if ret[0] != "OK":
         print("Error on setting session:", resp3[1])
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
-    # Make a note of the session key
-    #print("Sess Key ACCEPTED:",  resp3[1])
+    cresp = hand.login(conf.login, conf.lpass, conf)
+    pyclisup.exit_if_err(cresp)
 
-    if conf.sess_key:
-        print("Post session, session key:", conf.sess_key[:12], "...")
+    #if not conf.quiet:
+    #    print ("Server login response:", cresp)
 
-    resp3 = hand.client(["hello", ],  conf.sess_key, False)
-    print("Hello Response:", resp3)
+    dd_beg, dd_end = pyclisup.inter_date(conf.begin, conf.inter)
 
-    cresp = hand.login("admin", "1234", conf)
-    print ("Server login response:", cresp)
-
-    # Set date range
-    if conf.start:
-        dd = datetime.datetime.now()
-        dd = dd.strptime(conf.start, "%Y-%m-%d %H:%M")
-    else:
-        dd = datetime.datetime.now()
-        dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
+    cresp = hand.client(["rsize", "vote"], conf.sess_key)
+    print ("Server rsize response:", cresp)
 
-    #print(dd)
-    dd_beg = dd + datetime.timedelta(0)
-    if conf.inter:
-        dd_end = dd_beg + datetime.timedelta(0, conf.inter * 60)
-    else:
-        dd_end = dd_beg + datetime.timedelta(1)
+    if not conf.quiet:
+        print("listing from:", dd_beg, "to:", dd_end);
 
-    print("from:", dd_beg, "to:", dd_end);
     cresp = hand.client(["rcount", "vote", dd_beg.timestamp(),
                                     dd_end.timestamp()], conf.sess_key)
     print ("Server  rcount response:", cresp)
+    if cresp[0] != "OK":
+        sys.exit()
 
     if cresp[1] < 100:
         cresp = hand.client(["rlist", "vote", dd_beg.timestamp(),
                                     dd_end.timestamp()], conf.sess_key)
         #print ("Server  rlist response:", cresp)
         if cresp[0] == "OK":
             for aa in cresp[1]:
                 #print("aa", aa)
                 if aa:
                     ttt = pyservsup.uuid2date(uuid.UUID(aa))
                     print(aa, ":", ttt)
+        print("Listed", len(cresp[1]), "records.")
 
 if __name__ == '__main__':
     mainfunct()
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_rput.py` & `pyvserv-1.0.4/pyvclient/pyvcli_uini.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,216 +1,154 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
-
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat, uuid, atexit
-
-#from Crypto.Hash import SHA512
-#from Crypto.PublicKey import RSA
-#from Crypto.Cipher import PKCS1_v1_5
-#from Crypto.PublicKey import RSA
-#from Crypto.Hash import SHA
-
-from Crypto import Random
+import sys
+if  sys.version_info[0] < 3:
+    print(("Needs python 3 or better."))
+    sys.exit(1)
+
+__doc__ =\
+'''
+    Test client for the pyvserv project. Default user initialiser.
+    This command can only be used from the local network, loopback
+    interface. The command is used to create the initial user,
+    and will not do anything if there is a user present already.
+
+'''
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
 
 # This repairs the path from local run to pip run.
-# Remove pip version for local tests
-
 try:
     from pyvcommon import support
-    #print("sf", sf)
-    # Get Parent of module root
-    sf = os.path.dirname(support.__file__)
-    sf = os.path.dirname(sf)
-    sys.path.append(os.path.join(sf, "pyvcommon"))
-    sys.path.append(os.path.join(sf, "pyvserver"))
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
 except:
-    #print("pathching")
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
-    sys.path.append(os.path.join(base,  '..', "pyvserver"))
     from pyvcommon import support
 
-from pyvcommon import support, pycrypt, pyservsup, pyclisup, pyvhash
+from pyvcommon import support, pycrypt, pyclisup
 from pyvcommon import pysyslog, comline
 
-import pyvpacker
-
 # ------------------------------------------------------------------------
-# Functions from command line
+# Globals
+
+version = "1.0.0"
 
 def phelp():
 
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p port   - Port to use (default: 6666)")
-    print( "            -l level  - Log level (default: 0)")
-    print( "            -c file   - Save comm to file")
-    print( "            -k keyval - Put this key")
-    print( "            -n        - Number of records to put")
-    print( "            -v        - Verbose")
-    print( "            -q        - Quiet")
-    print( "            -h        - Help")
-    #print( " Needs debug level or verbose to have any output.")
-    print()
+    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options] [hostname]")
+    print( "  hostname: host to connect to. (default: 127.0.0.1)")
+    print( "  options:    -d level  - Debug level 0-10 default: 0")
+    print( "              -p        - Port to use (default: 6666)")
+    print( "              -v        - Verbose. Present more info.")
+    print( "              -q        - Quiet. Present less info.")
+    print( "              -u user   - User Name; default: 'admin'")
+    print( "              -l pass   - Password; default: '1234' (!! for tests only !!)")
+    print( "              -t        - Prompt for password.")
+    print( "              -f        - Force, No prompt for demo.")
+    print( "              -h        - Help (this screen)")
+    print( "The user will be prompted for confirmation if demosystem is created.")
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", support.version)
+    print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["k:",  "putkey",   "",     None],      \
-    ["n:",  "numrec",   1,     None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["u:",  "userx",    "admin",    None],      \
+    ["l:",  "passx",    "1234",     None],      \
+    ["t",   "prompt",    0,         None],      \
+    ["f",   "noprompt",  0,         None],      \
+    ["V",   None,        None,      pversion],  \
+    ["h",   None,        None,      phelp]      \
 
 conf = comline.Config(optarr)
+conf.sess_key = ""
 
 # ------------------------------------------------------------------------
 
-def mainfunct():
+def    mainfunct():
 
-    args = conf.comline(sys.argv[1:])
-    #print(vars(conf))
+    ''' Initialize test user 'admin' with password '1234'
+        Naturally, this is for testing.
+        On production server, add a real password.
+    '''
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
+    try:
+        args = conf.comline(sys.argv[1:])
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
+
+    if conf.verbose and conf.pgdebug:
+        print("Debug level", conf.pgdebug)
 
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
+    if conf.prompt:
+        import getpass
+        strx = getpass.getpass("Enter Pass for initial user: ")
+        if not strx:
+            print("Empty pass, aborting ...")
+            sys.exit(0)
+        conf.passx =  strx
+
+    if conf.passx == "1234":
+
+        if not conf.noprompt:
+            print("This creates credentials for a demo / test system.")
+            print("Are you sure? (y/N) ", end = ""); sys.stdout.flush()
+            sss = input().strip().lower()
+            #print(sss)
+            if sss != "y" and sss != "yes":
+                print("You may use the -t option for password prompt. Exiting ...")
+                sys.exit()
+
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
-    hand.comm  = conf.comm
-
-    actstr = ["register", "unregister", "cast", "uncast", ]
-    act = actstr[random.randint(0, len(actstr)-1)]
-
-    print("Calculating hash ....", end = " "); sys.stdout.flush()
-    #ttt = time.time()
-    pvh = pyvhash.BcData()
-    pvh.addpayload({"Vote": random.randint(0, 10), "UID":  str(uuid.uuid1()), })
-    pvh.addpayload({"SubVote": random.randint(0, 10), "TUID":  str(uuid.uuid1()), })
-    pvh.addpayload({"Action": act , "RUID":  str(uuid.uuid1()), })
-    #print(pvh.datax)
-
-    if conf.putkey:
-        pvh.datax['header'] = conf.putkey
-
-    pvh.hasharr();    pvh.powarr()
-    print("OK")
-
-
-    if not pvh.checkhash():
-        print("Error on hashing payload .. retrying ...")
-    elif not pvh.checkpow():
-        print("Error on POW payload .. retrying ...")
-
-    if conf.verbose:
-        print(pvh.datax)
-
-    #print("Chain cnt", pvh.cnt)
-    #print("chain %.3fms" % ((time.time() - ttt) * 1000) )
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    atexit.register(pyclisup.atexit_func, hand, conf)
-
-    resp3 = hand.client(["hello", "world"] , "", False)
-    print("Hello Resp:", resp3)
+    #print("Connect Response:", respc)
 
-    ret = hand.start_session(conf)
+    resp3 = hand.start_session(conf)
+    if not conf.quiet:
+        print("Sess Response:", resp3)
 
-    if ret[0] != "OK":
-        print("Error on setting session:", resp3[1])
-        sys.exit(0)
+    resp3 = hand.client(["hello",] , conf.sess_key, False)
+    #print("Hello sess Response:", resp3[1])
 
-    # Make a note of the session key
-    if conf.verbose:
-        print("Sess Key ACCEPTED:",  conf.sess_key[:12], '...' )
-
-    #print(" ----- Post session, all is encrypted ----- ")
-
-    #resp4 = hand.client(["tout", "30",], conf.sess_key)
-    #if resp4[0] != "OK":
-    #    print("Server tout Response:", resp4)
-    #    sys.exit()
-
-    #ttt = time.time()
-    # Session estabilished, try a simple command
-    resp4 = hand.client(["hello",], conf.sess_key)
-    #print("hello %.3fms" % ((time.time() - ttt) * 1000) )
-    if resp4[0] != "OK":
-        print("Server hello resp:", resp4[1])
-        sys.exit()
-
-    #ttt = time.time()
-    cresp = hand.client(["user", "admin"], conf.sess_key)
-    #print("user %.3fms" % ((time.time() - ttt) * 1000) )
-    print ("Server user respo:", cresp)
-
-    #ttt = time.time()
-    cresp = hand.client(["pass", "1234"], conf.sess_key)
-    #print("pass %.3fms" % ((time.time() - ttt) * 1000) )
-    if cresp[0] != "OK":
-        print("Cannot log on")
-        sys.exit(1)
-    print ("Server pass resp:", cresp)
+    resp = hand.client(["uini", conf.userx, conf.passx], conf.sess_key)
+    print("resp", resp)
 
-    cresp = hand.client(["dmode",], conf.sess_key)
-    #print("dmode", cresp)
-    if cresp[1] == '0':
-        print("Enter twofa code: (ret to skip)", end = "")
-        sesscode = input()
-        if sesscode:
-            cresp = hand.client(["twofa", sesscode], conf.sess_key)
-            print ("Server twofa resp:", cresp)
-            if cresp[0] != OK:
-                print ("Server twofa failed")
-                sys.exit(0)
-
-    # Interactive, need more time
-    #tout = hand.client(["tout", "200",], conf.sess_key)
-    #print (tout)
-
-    if conf.pgdebug > 2:
-        print(pvh.datax)
-
-    if hand.verbose:
-        print("Sending Data:", pvh.datax)
-
-    #ttt = time.time()
-    for aa in range(conf.numrec):
-        cresp = hand.client(["rput", "vote", pvh.datax], conf.sess_key)
-        print ("Server rput response:", cresp)
-    #print("rput %.3fms" % ((time.time() - ttt) * 1000) )
+    hand.client(["quit"], conf.sess_key)
+    hand.close();
 
     sys.exit(0)
 
 if __name__ == '__main__':
     mainfunct()
 
 # EOF
-
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_sess.py` & `pyvserv-1.0.4/pyvclient/pyvcli_sess.py`

 * *Files 4% similar despite different names*

```diff
@@ -43,46 +43,39 @@
     print( os.path.basename(sys.argv[0]), "Version", support.version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
-    ["s",   "showkey",  "",     None],      \
-    ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
     args = conf.comline(sys.argv[1:])
     #print(vars(conf))
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
-
     pyclisup.verbose = conf.verbose
     pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
-    hand.comm  = conf.comm
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
@@ -168,19 +161,19 @@
     if resp3[0] != "OK":
         print("Error on setting session:", resp3)
         hand.client(["quit"])
         hand.close();
         sys.exit(0)
 
     # Make a note of the session key
-    print("Session key:", conf.sess_key[:24] , "..." )
+    print("Session key:", conf.sess_key)
 
     # Session estabilished, try a simple command
     resp4 = hand.client(["hello",], conf.sess_key)
-    print("Encrypted Resp:", resp4)
+    print("Hello Resp:", resp4)
 
     # --------------------------------------------------------------------
     # Generate communication key, second session and second run
 
     conf.sess_key2 = base64.b64encode(Random.new().read(128))
     sss2 = SHA256.new(); sss2.update(conf.sess_key2)
 
@@ -203,19 +196,19 @@
         print("Err: ", resp4)
         cresp = hand.client(["quit", ], conf.sess_key)
         print ("Server quit response:", cresp)
         sys.exit(0)
 
     conf.sess_key = conf.sess_key2
     # Make a note of the session key
-    print("Session key:", conf.sess_key[:24] , "..." )
+    print("Session key2:", conf.sess_key)
 
     # Session estabilished, try a simple command
     resp5 = hand.client(["hello",], conf.sess_key)
-    print("Hello2 Response:", resp5)
+    print("Hello2 Resp:", resp5)
 
     hand.client(["quit",],conf.sess_key)
     hand.close();
 
     sys.exit(0)
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_sess_tout.py` & `pyvserv-1.0.4/pyvclient/pyvcli_uman.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,246 +1,203 @@
-#!/usr/bin/env python3
-
-from __future__ import print_function
+#!/usr/bin/env python
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# Test client for the pyserv project. User add.
+
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
 
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-from Crypto.Hash import SHA512
-from Crypto.PublicKey import RSA
-from Crypto.Cipher import PKCS1_v1_5
-from Crypto.PublicKey import RSA
-from Crypto.Hash import SHA
-from Crypto import Random
-
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
-
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
-
-'''
-# test encrypt with large keys
-rrr =  "mTQdnL51eKnblQflLGSMvnMKDG4XjhKa9Mbgm5ZY9YLd" \
-        "/SxqZZxwyKc/ZVzCVwMxiJ5X8LdX3X5VVO5zq/VBWQ=="
-sss = bluepy.encrypt(rrr, conf.sess_key)
-ttt = bluepy.decrypt(sss, conf.sess_key)
-print (rrr)
-print (ttt)
-'''
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
-# Functions from command line
+# Globals
 
-def phelp():
+version = "1.0.0"
+#progn = os.path.basename(sys.argv[0])
+progn = os.path.basename(__file__)
+
+cdoc = '''\
+The pyvserv user manager.
+Usage: %s [options] [hostname]
+  hostname: host to connect to. (default: 127.0.0.1)
+  options:  -d level  - Debug level 0-10
+            -p        - Port to use (default: 6666)
+            -l login  - Login Name; default: 'admin'
+            -s lpass  - Login Pass; default: '1234' (for !!testing only!!)
+            -t        - prompt for login pass
+            -u user   - New/Op User Name; default: 'test_user'
+            -x npass  - New/Op User Pass; default: '1234'
+            -a        - Add user flag. Must be a unique user name
+            -m        - Add admin flag. Add admin instead of a regular user
+            -i kind   - List users. (kind = user / admin / disabled / initial)
+            -e enflag - Enable / Disable user flag
+            -T        - Prompt for new/op user pass / change pass
+            -r        - Remove user flag -|-  -c        - Change pass flag
+            -v        - Verbose          -|-  -V        - Print version number
+            -q        - Quiet            -|-  -h        - Help (this screen)
+If no action is specified, defaults to list users. ''' \
+ % (progn)
+
+__doc__= "<pre>" + cdoc + "</pre>"
 
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p port   - Port to use (default: 6666)")
-    print( "            -l level  - Log level (default: 0)")
-    print( "            -c file   - Save comm to file")
-    print( "            -s        - Showkey")
-    print( "            -v        - Verbose")
-    print( "            -q        - Quiet")
-    print( "            -h        - Help")
-    #print( " Needs debug level or verbose to have any output.")
-    print()
+def phelp():
+    ''' Present command line help '''
+    print(cdoc)
     sys.exit(0)
 
 def pversion():
-    print( os.path.basename(sys.argv[0]), "Version", support.version)
+    ''' Display Version information '''
+    print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["c:",  "comm",     "",     None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["s",   "showkey",  "",     None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",      0,              None],      \
+    ["p:",  "port",         6666,           None],      \
+    ["l:",  "login",        "admin",        None],      \
+    ["s:",  "lpass",        "1234",         None],      \
+    ["t",   "lprompt",      0,              None],      \
+    ["v",   "verbose",      0,              None],      \
+    ["q",   "quiet",        0,              None],      \
+    ["m",   "admin",        0,              None],      \
+    ["a",   "add",          0,              None],      \
+    ["r",   "remove",       0,              None],      \
+    ["c",   "change",       "",             None],      \
+    ["u:",  "userx",        "test_user",    None],      \
+    ["x:",  "passx",        "1234",         None],      \
+    ["X:",  "chpass",       "",             None],      \
+    ["T",   "prompt",       0,              None],      \
+    ["e:",  "encomm",       "",             None],      \
+    ["i:",  "listx",        "",             None],  \
+    ["V",   None,           None,           pversion],  \
+    ["h",   None,           None,           phelp]      \
 
 conf = comline.Config(optarr)
+conf.sess_key = ""
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def    mainfunct():
 
-    args = conf.comline(sys.argv[1:])
+    ''' Entry point for pip script '''
+    try:
+        args = conf.comline(sys.argv[1:])
 
-    if conf.comm:
-        print("Save to filename", conf.comm)
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
 
-    pyclisup.verbose = conf.verbose
-    pyclisup.pgdebug = conf.pgdebug
+    #if not conf.add and not conf.remove and not conf.encomm \
+    #            and not conf.listx and not conf.change:
+    #    print("One of: Add / Remove / Change / Enable / List option should be specified.")
+    #    print("Use [ -a | -r | -p | -e  | -i ] options or the -h option for help.")
+    #    sys.exit()
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
-    hand.comm  = conf.comm
+
+    if conf.lprompt:
+        import getpass
+        strx = getpass.getpass("Pass for login %s: " % conf.login)
+        if not strx:
+            print("Cannot login with empty pass, aborting ...")
+            sys.exit(0)
+        conf.lpass = strx
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #print("IP:", ip, respc);
-    #print("Initial:", respc);
-
-    resp = hand.client(["akey"])
-    #print("akey response", resp)
-
+    resp3 = hand.start_session(conf)
+    if not conf.quiet:
+        print("Sess Response:", resp3)
+
+    #resp3 = hand.client(["hello",] , conf.sess_key, False)
+    #if not conf.quiet:
+    #    print("Hello sess Response:", resp3[1])
+
+    resp = hand.client(["user", conf.login], conf.sess_key)
+    if not conf.quiet:
+        print("user Response:", resp)
     if resp[0] != "OK":
-        print("Error on getting key:", resp[1])
-        hand.client(["quit"])
+        hand.client(["quit"], conf.sess_key)
         hand.close();
-        sys.exit(0)
-
-    if conf.verbose:
-        print("Got akey hash:", "'" + resp[1] + "'")
-        pass
-
-    #if conf.pgdebug > 4:
-    #    print ("Server response2:\n" +  "'" + resp[1].decode("cp437") +  "'\n")
-
-    hhh = SHA512.new();
-    hhh.update(resp[2])
-    #hhh.update(bytes(resp[2], "cp437"))
-
-    if conf.pgdebug > 3:
-        print("Hash1:  '" + resp[1] + "'")
-        print("Hash2:  '" + hhh.hexdigest() + "'")
-
-    # Remember key
-    if hhh.hexdigest() !=  resp[1]:
-        print("Tainted key, aborting.")
-        hand.client(["quit"])
-        hand.close();
-        sys.exit(0)
-
-    hand.pkey = resp[2]
-
-    #if conf.quiet == False:
-    #     print("Key response:", resp[0], resp[2][:32], "...")
-
-    if conf.pgdebug > 4:
-         print(hand.pkey)
-
-    if conf.pgdebug > 2:
-        print ("Server response:", "'" + hhh.hexdigest() + "'")
-
-    if conf.showkey or conf.pgdebug > 5:
-        #print("Key:")
-        print(hand.pkey)
-
-    try:
-        hand.pubkey = RSA.importKey(hand.pkey)
-        if conf.pgdebug > 4:
-            print (hand.pubkey)
-    except:
-        print("Cannot import public key.")
-        support.put_exception("import key")
-        hand.client(["quit"])
-        hand.close();
-        sys.exit(0)
-
-    resp0 = hand.client(["hello",], )
-    print("Hello (unencrypted) Response:", resp0[1])
 
-    #if conf.pgdebug > 1:
-    #    print("Got pub key", hand.pubkey, "size =", hand.pubkey.size_in_bits())
-
-    # Generate communication key
-    conf.sess_key = Random.new().read(512)
-    sss = SHA512.new(); sss.update(conf.sess_key)
-
-    cipher = PKCS1_v1_5.new(hand.pubkey)
-    #print ("cipher", cipher.can_encrypt())
-
-    if conf.pgdebug > 2:
-        support.shortdump("conf.sess_key", conf.sess_key )
-
-    sess_keyx = cipher.encrypt(conf.sess_key)
-    ttt = SHA512.new(); ttt.update(sess_keyx)
-
-    if conf.pgdebug > 2:
-        support.shortdump("sess_keyx", sess_keyx )
-
-    resp3 = hand.client(["sess", sss.hexdigest(), ttt.hexdigest(), sess_keyx], "", False)
-    #print("Sess Response:", resp3)
-
-    if resp3[0] != "OK":
-        print("Error on setting session:", resp3[1])
-        hand.client(["quit"])
+    resp = hand.client(["pass", conf.lpass], conf.sess_key)
+    if not conf.quiet:
+        print("pass Response:", resp)
+    if resp[0] != "OK":
+        hand.client(["quit"], conf.sess_key)
         hand.close();
-        sys.exit(0)
-
-    # Make a note of the session key
-    #print(resp3[1])
-    support.shortdump(" All is encrypted with", conf.sess_key )
-
-    # Session estabilished, try a simple command
-    resp4 = hand.client(["hello",], conf.sess_key)
-    print("Hello (encrypted) Response:", resp4[1])
-
-    # --------------------------------------------------------------------
-    # Generate communication key, second session and second run
-
-    conf.sess_key2 = Random.new().read(512)
-    sss2 = SHA512.new(); sss2.update(conf.sess_key2)
-
-    #cipher = PKCS1_v1_5.new(hand.pubkey)
-    #print ("cipher", cipher.can_encrypt())
-
-    if conf.pgdebug > 2:
-        support.shortdump("conf.sess_key2", conf.sess_key2 )
-
-    sess_keyx2 = cipher.encrypt(conf.sess_key2)
-    ttt2 = SHA512.new(); ttt2.update(sess_keyx2)
-
-    if conf.pgdebug > 2:
-        support.shortdump("sess_keyx", sess_keyx )
-
-    #print("Key Hexdigest", ttt2.hexdigest()[:16])
-
-    resp4 = hand.client(["sess", sss2.hexdigest(), ttt2.hexdigest(), sess_keyx2],
-                                conf.sess_key, False)
-
-    if resp4[0] != "OK":
-        print("Err: ", resp4)
-        cresp = hand.client(["quit", ], conf.sess_key)
-        print ("Server quit response:", cresp)
-        sys.exit(0)
-
-    # Make a note of the session key
-    #print(resp4[1])
-    support.shortdump(" All is encrypted with", conf.sess_key2 )
-
-    # Session estabilished, try a simple command
-    resp5 = hand.client(["hello",], conf.sess_key2)
-    print("Hello (encrypted2) Response:", resp5)
-
-    time.sleep(10)
+        print("Error on login, exiting.", resp)
+        sys.exit(1)
 
-    resp5 = hand.client(["hello",], conf.sess_key2)
-    print("Hello (encrypted2) Response:", resp5)
+    if conf.prompt:
+        import getpass
+        strx = getpass.getpass("Pass for new user %s: " % conf.userx)
+        if not strx:
+            print("Empty pass, aborting ...")
+            sys.exit(0)
+        conf.passx = strx
+
+    if conf.encomm:
+        resp = hand.client(["uena", conf.userx, conf.encomm, ], conf.sess_key)
+        print("uen Response:", resp)
+    elif conf.add:
+        if conf.admin:
+            resp = hand.client(["aadd", conf.userx, conf.passx], conf.sess_key)
+        else:
+            resp = hand.client(["uadd", conf.userx, conf.passx], conf.sess_key)
+        print("uadd Response:", resp)
+    elif conf.remove:
+        resp = hand.client(["udel", conf.userx, conf.passx], conf.sess_key)
+        print("udel Response:", resp)
+    elif conf.change:
+        if not conf.chpass:
+            import getpass
+            strx = getpass.getpass("Pass for change pass %s: " % conf.userx)
+            if not strx:
+                print("Empty pass, aborting ...")
+                sys.exit(0)
+            conf.chpass = strx
+        resp = hand.client(["chpass", conf.userx, conf.passx, conf.chpass, ], conf.sess_key)
+        print("uchpass Response:", resp)
+    else:
+        if not conf.listx:
+            conf.listx = "user"
+        resp = hand.client(["ulist", conf.listx], conf.sess_key)
+        print("ulist Response:", resp)
 
-    hand.client(["quit",],conf.sess_key2)
+    hand.client(["quit"], conf.sess_key)
     hand.close();
 
     sys.exit(0)
 
-# EOF
+if __name__ == '__main__':
+    mainfunct()
+
+
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_tout.py` & `pyvserv-1.0.4/pyvclient/pyvcli_gethelp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,114 +1,112 @@
 #!/usr/bin/env python3
 
 from __future__ import print_function
 
-import sys
-if sys.version_info[0] < 3:
-    print("Python 2 is not supported as of 1/1/2020")
-    sys.exit(1)
-
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# Test client for the pyserv project. User add.
+
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
+
+# This repairs the path from local run to pip run.
+try:
+    from pyvcommon import support
+    base = os.path.dirname(os.path.realpath(support.__file__))
+    sys.path.append(os.path.join(base, "."))
+except:
+    base = os.path.dirname(os.path.realpath(__file__))
+    sys.path.append(os.path.join(base,  '..'))
+    sys.path.append(os.path.join(base,  '..', "pyvcommon"))
+    from pyvcommon import support
 
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat
+from pyvcommon import support, pycrypt, pyclisup
+from pyvcommon import pysyslog, comline
 
-base = os.path.dirname(os.path.realpath(__file__))
-sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
+# ------------------------------------------------------------------------
+# Globals
 
-import support, pycrypt, pyservsup, pyclisup
-import pysyslog, comline
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
 # Functions from command line
 
 def phelp():
 
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level  - Debug level 0-10")
+    print( "The pyvserv help program.")
+    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options] [hostname]")
+    print( "  hostname: host to connect to. (default: 127.0.0.1)")
+    print( "  options:  -d level  - Debug level 0-10")
     print( "            -p port   - Port to use (default: 6666)")
+    print( "            -s str    - Subhelp string")
     print( "            -v        - Verbose")
+    print( "            -V        - Print version number")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
-    print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["p:",  "port",     6666,       None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["t",   "test",     "x",        None],      \
+    ["s:",  "subhelp",  "",         None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def mainfunct():
 
-    if sys.version_info[0] < 3:
-        print("Warning! This script was meant for python 3.x")
-        time.sleep(1)
-
-    #if  sys.version_info[0] < 3:
-    #    print("Needs python 3 or better.")
-    #    sys.exit(1)
-    #
     args = conf.comline(sys.argv[1:])
 
+    pyclisup.verbose = conf.verbose
+    pyclisup.pgdebug = conf.pgdebug
+
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
+    if conf.subhelp:
+        if conf.verbose:
+            print("subhelp", conf.subhelp);
+
     try:
         resp2 = hand.connect(ip, conf.port)
     except:
-        support.put_exception("On connect")
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #if conf.quiet == False:
-    #    print ("Server initial:", resp2)
-
-    resp = hand.client(["ver"])
-
-    if conf.quiet == False:
-        print ("Server response:", resp)
+    if conf.verbose:
+        print ("Server initial:", hand.pb.decode_data(resp2[1])[0])
 
-    time.sleep(10)
+    if conf.subhelp:
+        resp = hand.client(["help", conf.subhelp])
+    else:
+        resp = hand.client(["help",])
 
-    resp = hand.client(["quit"])
-    if conf.quiet == False:
-        print ("Server response:", resp)
+    print ("help resp:", resp)
 
-    hand.close()
+    hand.client(["quit",])
+    hand.close();
 
     sys.exit(0)
 
-# EOF
-
-
-
-
-
-
-
-
-
-
+#def mainfunct():
 
+if __name__ == '__main__':
+    mainfunct()
 
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_uadd.py` & `pyvserv-1.0.4/pyvclient/pyvcli_uadd.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
@@ -91,15 +91,15 @@
     resp = hand.client(["pass", "1234"], conf.sess_key)
     print("pass Response:", resp)
     if resp[0] != "OK":
         hand.client(["quit"], conf.sess_key)
         hand.close();
         raise ValueError("Not authorized", resp[1])
 
-    resp = hand.client(["uadd", "peter", "1234"], conf.sess_key)
+    resp = hand.client(["uadd", "peter3", "1234"], conf.sess_key)
     print("uadd Response:", resp)
 
     resp = hand.client(["uadd", "peter2", "1234"], conf.sess_key)
     print("uadd Response:", resp)
 
     resp = hand.client(["uadd", "peter3,comma", "1234"], conf.sess_key)
     print("uadd Response:", resp)
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_uchpass.py` & `pyvserv-1.0.4/pyvclient/pyvcli_uena.py`

 * *Files 27% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
@@ -68,81 +68,89 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.client(["hello",] , "", False)
-    print("Hello Response:", resp3)
+    #resp3 = hand.client(["hello",] , "", False)
+    #print("Hello Response:", resp3)
 
     resp3 = hand.start_session(conf)
-    print("Sess Response:", resp3)
+    if not conf.quiet:
+        print("Sess Response:", resp3)
 
-    #resp3 = hand.client(["hello",] , conf.sess_key, False)
-    #print("Hello Response:", resp3[1])
+    resp3 = hand.client(["hello",] , conf.sess_key, False)
+    if not conf.quiet:
+        print("Hello Response:", resp3)
 
     resp = hand.client(["user", "admin"], conf.sess_key)
-    print("user Response:", resp)
-    if resp[0] != "OK":
-        hand.client(["quit"], conf.sess_key)
-        hand.close();
-        raise ValueError("No user", resp[1])
+    if not conf.quiet:
+        print("user Response:", resp)
 
     resp = hand.client(["pass", "1234"], conf.sess_key)
     print("pass Response:", resp)
     if resp[0] != "OK":
-        hand.client(["quit"], conf.sess_key)
-        hand.close();
         raise ValueError("Not authorized", resp[1])
 
-    resp = hand.client(["udel", "admin2", "1234"], conf.sess_key)
-    print("udel Response:", resp)
+    resp = hand.client(["uena", "peter2", "enable"], conf.sess_key)
+    if not conf.quiet:
+        print("uena Response:", resp)
 
-    resp = hand.client(["aadd", "admin2", "1234"], conf.sess_key)
-    print("aadd Response:", resp)
+    resp = hand.client(["logout",], conf.sess_key)
+    if not conf.quiet:
+        print("logout Response:", resp)
 
-    resp = hand.client(["udel", "peter", "1234"], conf.sess_key)
-    print("udel Response:", resp)
+    resp = hand.client(["uena", "peter2", "enable"], conf.sess_key)
+    if not conf.quiet:
+        print("uena Response:", resp)
+
+    resp = hand.client(["user", "admin"], conf.sess_key)
+    if not conf.quiet:
+        print("user Response:", resp)
 
-    resp = hand.client(["uadd", "peter", "1234"], conf.sess_key)
-    print("uadd Response:", resp)
+    resp = hand.client(["pass", "1234"], conf.sess_key)
+    print("pass Response:", resp)
+    if resp[0] != "OK":
+        raise ValueError("Not authorized", resp[1])
+
+    resp = hand.client(["uena", "peter2", "disable"], conf.sess_key)
+    if not conf.quiet:
+        print("uena Response:", resp)
 
     resp = hand.client(["logout",], conf.sess_key)
-    print("logout Response:", resp)
+    if not conf.quiet:
+        print("logout Response:", resp)
+
+    resp = hand.client(["user", "peter2"], conf.sess_key)
+    if not conf.quiet:
+        print("user Response:", resp)
+
+    resp = hand.client(["pass", "1234"], conf.sess_key)
+    if not conf.quiet:
+        print("pass Response:", resp)
+
+    hand.client(["quit"], conf.sess_key)
+    hand.close();
+
+    sys.exit(0)
+
+
+
+
+
+
+
+
 
-    resp = hand.login("peter", "1234", conf)
-    print("login Response:", resp)
 
-    resp = hand.client(["chpass", "1234", "12345"], conf.sess_key)
-    print("chpass Response:", resp)
 
-    resp = hand.client(["logout",], conf.sess_key)
-    print("logout Response:", resp)
 
-    resp = hand.login("peter", "12345", conf)
-    print("login Response:", resp)
 
-    resp3 = hand.client(["hello",] , conf.sess_key, False)
-    print("Hello Response:", resp3)
 
-    resp = hand.client(["logout",], conf.sess_key)
-    print("logout Response:", resp)
 
-    resp = hand.login("admin2", "1234", conf)
-    print("login Response:", resp)
 
-    resp = hand.client(["chpass", "1234", "12345"], conf.sess_key)
-    print("chpass Response:", resp)
 
-    resp = hand.client(["logout",], conf.sess_key)
-    print("logout Response:", resp)
 
-    resp = hand.login("admin2", "12345", conf)
-    print("login Response:", resp)
 
-    hand.client(["quit"], conf.sess_key)
-    hand.close();
 
-    sys.exit(0)
 
-# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_udel.py` & `pyvserv-1.0.4/pyvclient/pyvcli_udel.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
@@ -87,15 +87,15 @@
         raise ValueError("No user", resp[1])
 
     resp = hand.client(["pass", "1234"], conf.sess_key)
     print("pass Response:", resp)
     if resp[0] != "OK":
         raise ValueError("Not authorized", resp[1])
 
-    resp = hand.client(["udel", "peter",], conf.sess_key)
+    resp = hand.client(["udel", "peter3",], conf.sess_key)
     print("udel Response:", resp)
 
     resp = hand.client(["udel", "peter2",], conf.sess_key)
     print("udel Response:", resp)
 
     resp = hand.client(["udel", "peter3,comma"], conf.sess_key)
     print("udel Response:", resp)
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_uena.py` & `pyvserv-1.0.4/pyvclient/pyvcli_rmdir.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,145 +1,122 @@
 #!/usr/bin/env python
 
+import sys
+if sys.version_info[0] < 3:
+    print("Python 2 is not supported as of 1/1/2020")
+    sys.exit(1)
+
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. User add.
+# Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
 import random, stat
 
 base = os.path.dirname(os.path.realpath(__file__))
 sys.path.append(os.path.join(base,  '..' + os.sep + 'pyvcommon'))
 
 import support, pycrypt, pyservsup, pyclisup
 import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
+
+# ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
-    print( "Options:    -d level  - Debug level 0-10")
-    print( "            -p        - Port to use (default: 6666)")
-    print( "            -v        - Verbose")
-    print( "            -q        - Quiet")
-    print( "            -h        - Help")
+    print( "Options:    -d level   - Debug level 0-10")
+    print( "            -c dirname - Directory to remove. default: test_3")
+    print( "            -p         - Port to use (default: 6666)")
+    print( "            -v         - Verbose")
+    print( "            -q         - Quiet")
+    print( "            -h         - Help")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,      None],      \
-    ["p:",  "port",     6666,   None],      \
-    ["v",   "verbose",  0,      None],      \
-    ["q",   "quiet",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
-    ["V",   None,       None,   pversion],  \
-    ["h",   None,       None,   phelp]      \
+    ["d:",  "pgdebug",  0,          None],      \
+    ["c:",  "fname",    "test_dir", None],    \
+    ["p:",  "port",     6666,       None],      \
+    ["v",   "verbose",  0,          None],      \
+    ["q",   "quiet",    0,          None],      \
+    ["V",   None,       None,       pversion],  \
+    ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
-conf.sess_key = ""
 
 # ------------------------------------------------------------------------
 
 if __name__ == '__main__':
 
-    '''if  sys.version_info[0] < 3:
-        print(("Needs python 3 or better."))
-        sys.exit(1)'''
-
     args = conf.comline(sys.argv[1:])
 
+    #print(dir(conf))
+
+    #if conf.comm:
+    #    print("Save to filename", conf.comm)
+
+    pyclisup.verbose = conf.verbose
+    pyclisup.pgdebug = conf.pgdebug
+
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
+    #hand.comm  = conf.comm
+
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #resp3 = hand.client(["hello",] , "", False)
-    #print("Hello Response:", resp3)
-
-    resp3 = hand.start_session(conf)
-    print("Sess Response:", resp3)
-
-    resp3 = hand.client(["hello",] , conf.sess_key, False)
-    print("Hello Response:", resp3)
-
-    resp = hand.client(["user", "admin"], conf.sess_key)
-    print("user Response:", resp)
-
-    resp = hand.client(["pass", "1234"], conf.sess_key)
-    print("pass Response:", resp)
-    if resp[0] != "OK":
-        raise ValueError("Not authorized", resp[1])
-
-    resp = hand.client(["uena", "peter2", "enable"], conf.sess_key)
-    print("uena Response:", resp)
-
-    resp = hand.client(["logout",], conf.sess_key)
-    print("logout Response:", resp)
-
-    resp = hand.client(["uena", "peter2", "enable"], conf.sess_key)
-    print("uena Response:", resp)
-
-    resp = hand.client(["user", "admin"], conf.sess_key)
-    print("user Response:", resp)
-
-    resp = hand.client(["pass", "1234"], conf.sess_key)
-    print("pass Response:", resp)
-    if resp[0] != "OK":
-        raise ValueError("Not authorized", resp[1])
-
-    resp = hand.client(["uena", "peter2", "disable"], conf.sess_key)
-    print("uena Response:", resp)
-
-    resp = hand.client(["logout",], conf.sess_key)
-    print("logout Response:", resp)
-
-    resp = hand.client(["user", "peter2"], conf.sess_key)
-    print("user Response:", resp)
+    ret = hand.start_session(conf)
+    if ret[0] != "OK":
+        print("Error on setting session:", resp3[1])
+        hand.client(["quit"])
+        hand.close();
+        sys.exit(0)
+
+    if not conf.quiet:
+        print("Session key:", conf.sess_key[:12], "...")
+
+    resp3 = hand.client(["hello", ],  conf.sess_key, False)
+    if not conf.quiet:
+        print("Hello Response:", resp3)
+
+    cresp = hand.login("admin", "1234", conf)
+    if not conf.quiet:
+        print ("Server login response:", cresp)
+
+    #cresp = hand.client(["buff", "10", ], conf.sess_key)
+    #print ("Server buff response:", cresp)
+    #if cresp[0] != "OK":
+    #    print("Error on buff command", cresp[1])
+    #    hand.client(["quit"], conf.sess_key)
+    #    hand.close();
+    #    sys.exit(0)
 
-    resp = hand.client(["pass", "1234"], conf.sess_key)
-    print("pass Response:", resp)
+    ret2 = hand.client(["rmdir", conf.fname], conf.sess_key)
+    print ("Server rmdir response:", ret2)
 
-    hand.client(["quit"], conf.sess_key)
-    hand.close();
+    cresp = hand.client(["quit", ], conf.sess_key)
+    #print ("Server quit response:", cresp)
 
     sys.exit(0)
 
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
-
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_uini.py` & `pyvserv-1.0.4/pyvclient/pyvcli_hello.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,16 @@
-#!/usr/bin/env python
+#!/usr/bin/env python3
+
+from __future__ import print_function
 
 # ------------------------------------------------------------------------
-import sys
-if  sys.version_info[0] < 3:
-    print(("Needs python 3 or better."))
-    sys.exit(1)
-
-__doc__ =\
-'''
-    Test client for the pyvserv project. Default user initialiser.
-    This command can only be used from the local network, loopback
-    interface. The command is used to create the initial user,
-    and will not do anything if there is a user present already.
-
-'''
-import os, sys, getopt, signal, select, socket, time, struct
-import random, stat
+# Test client for the pyserv project. Encrypt test.
+
+import  os, sys, getopt, signal, select, socket, time, struct
+import  random, stat
 
 # This repairs the path from local run to pip run.
 try:
     from pyvcommon import support
     base = os.path.dirname(os.path.realpath(support.__file__))
     sys.path.append(os.path.join(base, "."))
 except:
@@ -30,88 +21,107 @@
 
 from pyvcommon import support, pycrypt, pyclisup
 from pyvcommon import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
+progn = os.path.basename(sys.argv[0])
 
-def phelp():
+__doc__ = '''\
+The pyvserv hello.
+Usage: %s  [options] [hostname]
+  hostname: host to connect to. (default: 127.0.0.1)
+  options:  -d level  - Debug level 0-10
+            -p        - Port to use (default: 6666)
+            -v        - Verbose
+            -V        - Print version number
+            -q        - Quiet
+            -h        - Help ''' \
+ % (progn)
+
+# ------------------------------------------------------------------------
+# Functions from command line
 
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level  - Debug level 0-10 default: 0")
-    print( "            -p        - Port to use (default: 6666)")
-    print( "            -v        - Verbose. Present more info")
-    print( "            -u user   - User Name; default: 'admin'")
-    print( "            -p pass   - Password; default: '1234' (!!! for tests only)")
-    print( "            -q        - Quiet. Prrsent less info")
-    print( "            -h        - Help (this screen)")
-    print()
+#print (optarr)
+def phelp():
+    print(__doc__)
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
-    ["d:",  "pgdebug",  0,          None],      \
-    ["p:",  "port",     6666,       None],      \
-    ["v",   "verbose",  0,          None],      \
-    ["q",   "quiet",    0,          None],      \
-    ["u:",  "userx",    "admin",    None],      \
-    ["p:",  "passx",    "1234",     None],      \
-    ["t",   "test",     "x",        None],      \
-    ["V",   None,       None,       pversion],  \
-    ["h",   None,       None,       phelp]      \
+    ["d:",  "pgdebug",      0,          None],      \
+    ["p:",  "port",         6666,       None],      \
+    ["g",   "long",         0,          None],      \
+    ["v",   "verbose",      0,          None],      \
+    ["q",   "quiet",        0,          None],      \
+    ["V",   None,           None,       pversion],  \
+    ["h",   None,           None,       phelp]      \
 
 conf = comline.Config(optarr)
-conf.sess_key = ""
 
 # ------------------------------------------------------------------------
 
-def    mainfunct():
+def mainfunct():
+
+    if sys.version_info[0] < 3:
+        print("Warning! This script was meant for python 3.x")
+        time.sleep(1)
 
-    ''' Initialize test user 'admin' with password '1234'
-    Naturally, this is for testing. '''
+    try:
+        args = conf.comline(sys.argv[1:])
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
 
+    if conf.verbose and conf.pgdebug:
+        print("Debug level", conf.pgdebug)
 
-    args = conf.comline(sys.argv[1:])
+    pyclisup.verbose = conf.verbose
+    pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
+    #print("dir".__doc__)
+
     try:
-        respc = hand.connect(ip, conf.port)
+        resp2 = hand.connect(ip, conf.port)
     except:
+        #support.put_exception("On connect")
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    #print("Connect Response:", respc)
-
-    resp3 = hand.start_session(conf)
-    print("Sess Response:", resp3)
-
-    resp3 = hand.client(["hello",] , conf.sess_key, False)
-    #print("Hello sess Response:", resp3[1])
-
-    resp = hand.client(["uini", conf.userx, conf.passx], conf.sess_key)
-    print("resp", resp)
+    if conf.verbose:
+        respini = hand.pb.decode_data(resp2[1])[0]
+        print ("Server initial:", respini)
+
+    resp = hand.client(["hello"])
+    if not conf.quiet:
+        print("hello resp", resp)
+    else:
+        print(resp)
 
-    hand.client(["quit"], conf.sess_key)
+    resp2 = hand.client(["quit"])
+    if conf.verbose:
+        print ("Server quit response:", resp2)
     hand.close();
 
-    sys.exit(0)
-
 if __name__ == '__main__':
     mainfunct()
 
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_uman.py` & `pyvserv-1.0.4/pyvclient/pyvcli_rcheck.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,92 +1,92 @@
 #!/usr/bin/env python
 
+import sys
+if sys.version_info[0] < 3:
+    print("Python 2 is not supported as of 1/1/2020")
+    sys.exit(1)
+
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. User add.
+# Test client for the pyserv project. Download file.
 
 import os, sys, getopt, signal, select, socket, time, struct
-import random, stat
+import random, stat, datetime, uuid, atexit
 
 # This repairs the path from local run to pip run.
 try:
     from pyvcommon import support
     base = os.path.dirname(os.path.realpath(support.__file__))
     sys.path.append(os.path.join(base, "."))
 except:
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     from pyvcommon import support
 
-from pyvcommon import support, pycrypt, pyclisup
-from pyvcommon import pysyslog, comline
+import support, pycrypt, pyservsup, pyclisup
+import pysyslog, comline
 
 # ------------------------------------------------------------------------
 # Globals
 
-version = 1.0
+version = "1.0.0"
+
+# ------------------------------------------------------------------------
 
 def phelp():
 
     print()
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
     print()
     print( "Options:    -d level  - Debug level 0-10")
     print( "            -p        - Port to use (default: 6666)")
-    print( "            -l login  - Login Name; default: 'user'")
-    print( "            -s lpass  - Login Pass; default: '1234'")
-    print( "            -u user   - User Name; default: 'user'")
-    print( "            -a        - Add user. Must be unique.")
-    print( "            -r        - Remove user (one of add or remove needed.")
-    print( "            -u user   - User Name; default: 'user'")
-    print( "            -p pass   - User pssword; default: '1234' (!!! for tests only)")
-    print( "            -m        - Add admin instead of regular user")
+    print( "            -l login  - Login Name; default: 'admin'")
+    print( "            -s lpass  - Login Pass; default: '1234' (for !!testing only!!)")
+    print( "            -r header - Test item")
     print( "            -v        - Verbose")
     print( "            -q        - Quiet")
+    print( "            -s        - Start time. Format: 'Y-m-d H:M'")
+    print( "            -i        - Interval in minutes. (Default: 1 day)")
     print( "            -h        - Help")
     print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,          None],      \
     ["p:",  "port",     6666,       None],      \
-    ["l:",  "login",    "admin",    None],      \
-    ["s:",  "lpass",    "1234",    None],      \
     ["v",   "verbose",  0,          None],      \
     ["q",   "quiet",    0,          None],      \
-    ["m",   "admin",    0,          None],      \
-    ["a",   "add",      0,          None],      \
-    ["r",   "remove",    0,         None],      \
-    ["u:",  "userx",    "user",     None],      \
-    ["p:",  "passx",    "1234",     None],      \
-    ["t",   "prompt",    0,         None],      \
+    ["n",   "plain",    0,          None],      \
+    ["i:",  "inter",    0,          None],      \
+    ["l:",  "login",    "admin",    None],      \
+    ["s:",  "lpass",    "1234",     None],      \
+    ["r:",  "rtest",    "",         None],      \
     ["V",   None,       None,       pversion],  \
     ["h",   None,       None,       phelp]      \
 
 conf = comline.Config(optarr)
-conf.sess_key = ""
 
 # ------------------------------------------------------------------------
 
-def    mainfunct():
-
-    '''if  sys.version_info[0] < 3:
-        print(("Needs python 3 or better."))
-        sys.exit(1)'''
+def mainfunct():
 
     args = conf.comline(sys.argv[1:])
 
-    if not conf.add and not conf.remove:
-        print("One of Add / Remove [ -a | -r ] should be specified.")
-        sys.exit()
+    #print(dir(conf))
+
+    #if conf.comm:
+    #    print("Save to filename", conf.comm)
+
+    pyclisup.verbose = conf.verbose
+    pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
@@ -95,57 +95,64 @@
 
     try:
         respc = hand.connect(ip, conf.port)
     except:
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp3 = hand.start_session(conf)
-    print("Sess Response:", resp3)
+    atexit.register(pyclisup.atexit_func, hand, conf)
 
-    resp3 = hand.client(["hello",] , conf.sess_key, False)
-    print("Hello sess Response:", resp3[1])
+    #resp3 = hand.client(["id",] , "", False)
+    #print("ID Response:", resp3[1])
 
-    resp = hand.client(["user", conf.login], conf.sess_key)
-    print("user Response:", resp)
-    if resp[0] != "OK":
+    #ret = ["OK",];  conf.sess_key = ""
+    ret = hand.start_session(conf)
+    if ret[0] != "OK":
+        print("Error on setting session:", ret)
         hand.client(["quit"], conf.sess_key)
         hand.close();
+        sys.exit(0)
+
+    cresp = hand.login(conf.login, conf.lpass, conf)
 
-    resp = hand.client(["pass", conf.lpass], conf.sess_key)
-    print("pass Response:", resp)
-    if resp[0] != "OK":
+    if cresp[0] != "OK":
+        print("Error on logging in:", cresp)
         hand.client(["quit"], conf.sess_key)
         hand.close();
-        print("Error on authentication, exiting.")
-        sys.exit(1)
+        sys.exit(0)
 
-    if conf.prompt:
-        import getpass
-        #print("Pass for new user %s:" % conf.userx, end = " ");
-        #sys.stdout.flush()
-        #strx = input()
-        strx = getpass.getpass("Pass for new user %s: " % conf.userx)
-        if not strx:
-            print("Aborting ...")
-            sys.exit(0)
-        conf.passx = strx
-    if conf.add:
-        if conf.admin:
-            resp = hand.client(["aadd", conf.userx, conf.passx], conf.sess_key)
-        else:
-            resp = hand.client(["uadd", conf.userx, conf.passx], conf.sess_key)
-        print("uadd Response:", resp)
-    elif conf.remove:
-        resp = hand.client(["udel", conf.userx, conf.passx], conf.sess_key)
-        print("udel Response:", resp)
+    if not conf.quiet:
+        print ("Server login response:", cresp)
 
-    hand.client(["quit"], conf.sess_key)
-    hand.close();
+    # Set date range
+    #if conf.start:
+    #    dd = datetime.datetime.now()
+    #    dd = dd.strptime(conf.start, "%Y-%m-%d %H:%M")
+    #else:
+    #    dd = datetime.datetime.now()
+    #    dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
+    #print(dd)
+    #dd_beg = dd + datetime.timedelta(0)
+    #if conf.inter:
+    #    dd_end = dd_beg + datetime.timedelta(0, conf.inter * 60)
+    #else:
+    #    dd_end = dd_beg + datetime.timedelta(1)
+
+    if conf.rtest:
+        import shlex
+        zzz = shlex.split(conf.rtest)
+        #print("zzz", zzz)
+        cresp = hand.client(["rtest", "vote", "sum", *zzz], conf.sess_key)
+        print ("rtest response:", cresp)
+    else:
+        cresp = hand.client(["rcheck", "vote", "sum"], conf.sess_key)
+        print ("rcheck sum response:", cresp)
 
-    sys.exit(0)
+        cresp = hand.client(["rcheck", "vote", "link"], conf.sess_key)
+        print ("rcheck link response:", cresp)
+        if cresp[0] != "OK":
+            sys.exit()
 
 if __name__ == '__main__':
     mainfunct()
 
-
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvclient/pyvcli_ver.py` & `pyvserv-1.0.4/pyvclient/pyvcli_qr.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-#!/usr/bin/env python3
+#!/usr/bin/env python
 
-from __future__ import print_function
+import sys, os
+import readline
 
-import sys
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
 # ------------------------------------------------------------------------
-# Test client for the pyserv project. Encrypt test.
+# Test client for the pyserv project.
 
-import  os, sys, getopt, signal, select, socket, time, struct
-import  random, stat
+import os, sys, getopt, signal, select, socket, time, struct
+import random, stat
 
 # This repairs the path from local run to pip run.
 try:
     from pyvcommon import support
     base = os.path.dirname(os.path.realpath(support.__file__))
     sys.path.append(os.path.join(base, "."))
 except:
@@ -23,90 +23,123 @@
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     from pyvcommon import support
 
 from pyvcommon import support, pycrypt, pyclisup
 from pyvcommon import pysyslog, comline
 
-version = "1,0"
+# ------------------------------------------------------------------------
+# Globals
+
+version = "1.0.0"
 
 # ------------------------------------------------------------------------
-# Functions from command line
 
 def phelp():
 
-    print()
+    print( "The pyvserv QR code downloader.")
     print( "Usage: " + os.path.basename(sys.argv[0]) + " [options]")
-    print()
-    print( "Options:    -d level  - Debug level 0-10")
+    print( "  hostname: host to connect to. (default: 127.0.0.1)")
+    print( "  options:  -d level  - Debug level 0-10")
     print( "            -p port   - Port to use (default: 6666)")
+    print( "            -f file   - Upload new QR image file. Admin only.")
     print( "            -v        - Verbose")
+    print( "            -V        - Version")
     print( "            -q        - Quiet")
     print( "            -h        - Help")
-    print()
     sys.exit(0)
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
     # option, var_name, initial_val, function
 optarr = \
     ["d:",  "pgdebug",  0,      None],      \
     ["p:",  "port",     6666,   None],      \
+    ["f:",  "file",     "",     None],      \
     ["v",   "verbose",  0,      None],      \
     ["q",   "quiet",    0,      None],      \
-    ["t",   "test",     "x",    None],      \
     ["V",   None,       None,   pversion],  \
     ["h",   None,       None,   phelp]      \
 
 conf = comline.Config(optarr)
 
 # ------------------------------------------------------------------------
 
-if __name__ == '__main__':
+def mainfunct():
 
-    if sys.version_info[0] < 3:
-        print("Warning! This script was meant for python 3.x")
-        sys.exit()
+    try:
+        args = conf.comline(sys.argv[1:])
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
 
-    args = conf.comline(sys.argv[1:])
+    pyclisup.verbose = conf.verbose
+    pyclisup.pgdebug = conf.pgdebug
 
     if len(args) == 0:
         ip = '127.0.0.1'
     else:
         ip = args[0]
 
     hand = pyclisup.CliSup()
     hand.verbose = conf.verbose
     hand.pgdebug = conf.pgdebug
 
     try:
-        resp2 = hand.connect(ip, conf.port)
+        respc = hand.connect(ip, conf.port)
     except:
-        #support.put_exception("On connect")
         print( "Cannot connect to:", ip + ":" + str(conf.port), sys.exc_info()[1])
         sys.exit(1)
 
-    resp = hand.client(["ver"])
-
-    if conf.quiet == False:
-        print ("Server response:", resp)
-
-    hand.client(["quit"])
-    hand.close()
+    resp3 = hand.start_session(conf)
+    if resp3[0] != "OK":
+        print("Error on setting session:", resp3[1])
+        sys.exit(0)
+
+    if conf.verbose:
+        resp = hand.client(["hello"], conf.sess_key)
+        print("Hello resp:", resp)
+
+    if conf.file:
+        resp = hand.login("admin", "1234", conf)
+        if resp[0] != "OK":
+            print("Login Response:", resp)
+            sys.exit()
+
+        fp = open(conf.file, "rb")
+        buff = fp.read()
+        fp.close()
+        #print("len:", len(buff))
+        resp3 = hand.client(["qr", buff], conf.sess_key, False)
+        print("QR UP Response:", resp3)
+    else:
+        resp3 = hand.client(["qr",], conf.sess_key, False)
+        if resp3[0] != "OK":
+            print("QR Response:", resp3)
+            sys.exit()
+
+        # Save
+        fp = open("qr.png", 'wb')
+        if type(resp3[1]) != type(b""):
+            resp3[1] = resp3[1].encode()
+        fp.write(resp3[1])
+        fp.close()
+        if not conf.quiet:
+            print("Downloaded QR code, saved to 'qr.png'", len(resp3[1]), "bytes")
+
+    rrr = hand.client(["quit"], conf.sess_key)
+    if conf.verbose:
+        print("Quit resp:", rrr)
+    hand.close();
 
     sys.exit(0)
 
-# EOF
-
-
-
-
-
-
-
-
-
-
-
+if __name__ == '__main__':
+    mainfunct()
 
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvcommon/comline.py` & `pyvserv-1.0.4/pyvcommon/comline.py`

 * *Files 12% similar despite different names*

```diff
@@ -9,63 +9,102 @@
 # ------------------------------------------------------------------------
 
 def pversion():
     print( os.path.basename(sys.argv[0]), "Version", version)
     sys.exit(0)
 
 glargs = ""
+glhead = ""
 glfoot = ""
 
+glprog = "proname"
+gloptarr = []
+glsoptarr = []
+
 def setargs(args):
     global glargs
     glargs = args
 
 def setfoot(args):
     global glfoot
     glfoot = args
 
+def sethead(args):
+    global glhead
+    glhead = args
+
+def setprog(args):
+    global glprog
+    glprog = args
+
 # ------------------------------------------------------------------------
 
+def dupoptcheck(optarr):
+        optdup = {}
+        for bb in range(len(optarr)):
+            kkk = optarr[bb][0][0]
+            try:
+                optdup[kkk] += 1
+            except KeyError:
+                optdup[kkk] = 1
+            except:
+                print(sys.exc_info())
+        #print(optdup)
+        found = False
+        for cc in optdup.keys():
+            if optdup[cc] > 1:
+                #print("found dup", cc)
+                found = cc
+        return found
+
 def phelp():
 
-    print()
+    if glhead:
+        print("head", glhead)
     print( "Usage: " + os.path.basename(sys.argv[0]), "[options]", glargs)
-    print()
-    print( "Options:")
+    print( "options:")
 
     for aa in optarr:
         pad = " " * (9 - len(aa[1]))
         print("        ", "-" + aa[0][0], " ", aa[1], pad, " - ", aa[4])
 
     print()
     if glfoot:
-        print(glfoot)
+        print("s", glfoot)
 
     sys.exit(0)
 
 # ------------------------------------------------------------------------
-# option [:], var_name, initial_val, function, helpstr
+# option [:],  var_name, initial_val, function, helpstr
 # Add colon ':' to option with argument.
 
 optarr = [\
-    ["d:",  "pgdebug",  0,      None,       "Debug level 0-10" ], \
-    ["p:",  "port",     6666,   None,       "Listen on port"],    \
-    ["v",   "verbose",  0,      None,       "Verbose"],           \
-    ["q",   "quiet",    0,      None,       "Quiet"],             \
-    ["V",   "version",  None,   pversion,   "Print Version"],     \
-    ["h",   "help",     None,   phelp,      "Show Help"]          \
-    ]
+ ["d:",  "pgdebug",  0,      None,       "Debug level 0-10" ], \
+ ["p:",  "port",     6666,   None,       "Listen on port"],    \
+ ["v",   "verbose",  0,      None,       "Verbose. . More info on screen."],           \
+ ["q",   "quiet",    0,      None,       "Quiet. Less info on screen."],             \
+ ["V",   "version",  None,   pversion,   "Print Version."],     \
+ ["h",   "help",     None,   phelp,      "Show Help. (this screen)"]          \
+]
 
 # ------------------------------------------------------------------------
 # Handle command line. Interpret optarray and decorate the class
 # This allows a lot of sub utils to have a common set of options.
 
 class Config:
 
     def __init__(self, optarr):
+
+        ddd = dupoptcheck(optarr)
+        if ddd:
+            raise ValueError("Duplicate options on comline.", ddd)
+
+        global glsoptarr
+        glsoptarr = optarr
+
         self.optarr = optarr
         self.verbose = False
         self.debug = False
         self.sess_key = ""
 
     def comline(self, argv):
         optletters = ""
@@ -75,14 +114,16 @@
         # Create defaults:
         err = 0
         for bb in range(len(self.optarr)):
             if self.optarr[bb][1]:
                 # Coerse type
                 if type(self.optarr[bb][2]) == type(0):
                     self.__dict__[self.optarr[bb][1]] = int(self.optarr[bb][2])
+                if type(self.optarr[bb][2]) == type(.0):
+                    self.__dict__[self.optarr[bb][1]] = float(self.optarr[bb][2])
                 if type(self.optarr[bb][2]) == type(""):
                     self.__dict__[self.optarr[bb][1]] = str(self.optarr[bb][2])
         try:
             opts, args = getopt.getopt(argv, optletters)
         except getopt.GetoptError as err:
             print( "Invalid option(s) on command line:", err)
             raise
@@ -92,56 +133,58 @@
 
         #print( "opts", opts, "args", args)
         for aa in opts:
             for bb in range(len(self.optarr)):
                 if aa[0][1] == self.optarr[bb][0][0]:
                     #print( "match", aa, self.optarr[bb])
                     if len(self.optarr[bb][0]) > 1:
-                        #print( "arg", self.optarr[bb][1], aa[1])
+                        print( "arg", self.optarr[bb][1], aa[1])
                         if self.optarr[bb][2] != None:
                             if type(self.optarr[bb][2]) == type(0):
                                 self.__dict__[self.optarr[bb][1]] = int(aa[1])
+                            if type(self.optarr[bb][2]) == type(.0):
+                                self.__dict__[self.optarr[bb][1]] = float(aa[1])
                             if type(self.optarr[bb][2]) == type(""):
                                 self.__dict__[self.optarr[bb][1]] = str(aa[1])
                     else:
                         #print( "set", self.optarr[bb][1], self.optarr[bb][2])
                         if self.optarr[bb][2] != None:
                             self.__dict__[self.optarr[bb][1]] = 1
                         #print( "call", self.optarr[bb][3])
                         if self.optarr[bb][3] != None:
                             self.optarr[bb][3]()
         return args
 
+# ------------------------------------------------------------------------
+# Long form help
 
 def phelplong():
 
-    print()
-    print( "Usage: " + os.path.basename(sys.argv[0]), "[options]", glargs)
-    print()
-    print( "Options:")
+    if glhead:
+        print(glhead)
 
-    for aa in optarrlong:
+    print( "Usage:", glprog, glargs)
+    print( "  options:")
+    for aa in gloptarr:
         longop = aa[1].replace("=", "")
         if "=" in aa[1]:
-            arg = longop
+            arg = aa[2]
         else:
             arg = " "
 
         pad  = " " * (8 - len(longop))
         pad2 = " " * (8 - len(arg))
 
-        print("       ", "-" + aa[0][0], " ", "--" + longop, pad, arg, pad2," - ", aa[5])
-
-    print()
+        print("   ", "-" + aa[0][0], " ",
+                        "--" + longop, pad, arg, pad2,"- ", aa[5])
     if glfoot:
         print(glfoot)
 
     sys.exit(0)
 
-
 # ------------------------------------------------------------------------
 # Handle command line. Interpret optarray and decorate the class;
 # Uses UNIX getopt for compatibility;
 #
 # Option parameters:
 #
 # option, long_option,  var_name,   initial_value, function
@@ -157,26 +200,34 @@
 #    ["v",     "verbose",     "verbose",  0,              None],      \
 #    ["t",     "test",        "test",     "x",            None],      \
 #    ["V",     "version",     None,       None,           pversion],  \
 #    ["h",     "help",        None,       None,           phelp],     \
 #    ["i:",    "input=",      "input",      "-",          None],      \
 #    ]
 
+# option [:], long_option[=],  var_name,   initial_value, function, helpstr
 optarrlong = [\
-    ["d:",  "debug=",  "pgdebug",  0,      None,       "Debug level 0-10" ], \
-    ["p:",  "port=",   "port",     6666,   None,       "Listen on port"],    \
-    ["v",   "verbose", "verbose",  0,      None,       "Verbose"],           \
-    ["q",   "quiet",   "quiet",    0,      None,       "Quiet"],             \
-    ["V",   "version", "version",  None,   pversion,   "Print Version"],     \
-    ["h",   "help",    "help",     None,   phelplong,  "Show Help"]          \
-    ]
+ ["d:",  "debug=",  "pgdebug",  0,      None,       "Debug level. 0=none 10=noisy default=0" ],
+ ["p:",  "port=",   "port",     6666,   None,       "Listen on port. default=6666"],
+ ["v",   "verbose", "verbose",  0,      None,       "Verbose. Show more info."],
+ ["q",   "quiet",   "quiet",    0,      None,       "Quiet. Show less info."],
+ ["V",   "version", "version",  None,   pversion,   "Print Version string."],
+ ["h",   "help",    "help",     None,   phelplong,  "Show Help. (this screen)"]
+]
 
 class ConfigLong:
 
     def __init__(self, optarr):
+
+        ddd = dupoptcheck(optarr)
+        if ddd:
+            raise ValueError("Duplicate options on comline.", ddd)
+
+        global gloptarr
+        gloptarr = optarr
         self._optarr = optarr
         self.err = None
 
         # Create defaults:
         for bb in range(len(self._optarr)):
             if self._optarr[bb][2]:
                 #print("init", self._optarr[bb][2],
@@ -189,14 +240,15 @@
                 elif type(self._optarr[bb][3]) == type(""):
                     self.__dict__[self._optarr[bb][2]] = str(self._optarr[bb][3])
                 else:
                     print("Can only have int and str type not", type(self._optarr[bb][3]))
                     raise ValueError("Can only None, have int and string - not %s" \
                                              % (type(self._optarr[bb][3])))
 
+
     def printvars(self):
         print("Variables -----")
         for aa in dir(self):
             try:
                 if aa[:2] == "__" :
                     continue
                 if  aa != "_optarr" and  aa != "comline" and \
@@ -222,18 +274,16 @@
 
         #print("optleters", optletters, "longopt", longopt)
 
         try:
             opts, args = getopt.getopt(argv, optletters, longopt)
         #except getopt.GetoptError, err:
         except getopt.GetoptError as err:
-            #print("Invalid option(s) on command line: %s" % err)
-            #self.err =  str("Invalid option(s) on command line: %s" % err)
+            print("Invalid option(s) on command line: %s" % err)
             raise
-            return None
 
         #print ("opts", opts, "args", args)
         for aa in opts:
             for bb in range(len(self._optarr)):
                 ddd = None
                 if aa[0][1] == "-":
                     ddd = "--" + self._optarr[bb][0]
```

### Comparing `pyvserv-1.0.3/pyvcommon/crysupp.py` & `pyvserv-1.0.4/pyvcommon/crysupp.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvcommon/genstrerr.py` & `pyvserv-1.0.4/pyvcommon/genstrerr.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvcommon/pyclisup.py` & `pyvserv-1.0.4/pyvcommon/pyclisup.py`

 * *Files 9% similar despite different names*

```diff
@@ -19,14 +19,17 @@
 from Crypto.PublicKey import RSA
 from Crypto.Cipher import PKCS1_v1_5
 from Crypto.Cipher import PKCS1_OAEP
 
 #rbuffsize = 1024
 rbuffsize = 4096
 
+OK  = "OK"
+ERR = "ERR"
+
 privtest = '''\
 -----BEGIN PRIVATE ECC-----
 ZMOOwr3Dg0sSw7oTAQAAQMOpM8O+D8O2w53ClsOjwr4KwpRxZcKmCMOVwrZ8w54/McOqY8K7w7VtD8KTBcKKwq4uwosvMHLDj3TDgMOtw6w+wrHDqRtCecO5w5vCmnE6w5jDi8KAw58Gw7vCqcKLw5XDn8KEwpsAIC56akoEOsO6w5hYwpwfADHCrcOvwrxIwqMUwrXClkXDsW8OJcO/fMOaT8O+w7c=
 -----END PRVATE ECC-----
 '''
 
 # -----------------------------------------------------------------------
@@ -81,15 +84,15 @@
         self.sock.close();
 
     # ------------------------------------------------------------------------
     # Send out our special buffer (short)len + (str)message
 
     def sendx(self, message):
 
-        if self.pgdebug > 5:
+        if self.pgdebug > 7:
             print("sending message:", message  )
 
         if sys.version_info[0] < 3:
             strx = struct.pack("!h", len(message)) + message
         else:
             if type(message) == type(""):
                  message = message.encode("cp437")
@@ -101,18 +104,18 @@
             fp.write(strx.decode("cp437"))
             fp.close()
 
         self.sock.sendall(strx)
 
     def recvx(self, key):
         resp = self.getreply(key)
-        if self.pgdebug > 3:
+        if self.pgdebug > 5:
             print("resp:", resp[:24])
         response = self.pb.decode_data(resp[1])
-        if self.pgdebug > 2:
+        if self.pgdebug > 7:
             print( "    recvx: '%s'" % response[:24])
         return response[0]
 
     # ------------------------------------------------------------------------
     # Set encryption key. New key returned. Raises ValuError.
 
     def set_key(self, newkey, oldkey):
@@ -175,67 +178,77 @@
         return response
 
     # ------------------------------------------------------------------------
     # Receive File. Return True for success.
 
     def getfile(self, fname, toname, key = ""):
 
+        if not fname:
+            cresp = ["ERR", "Must specify file name."]
+            return cresp
+
+        if not toname:
+            toname = fname  #+ "_local"
+
         if self.verbose:
             print( "getting ", fname, "to", toname)
 
         try:
             fh = open(toname, "wb+")
         except:
-            cresp = [ERR, "Cannot create local file: '" + toname + "'", ]
+            cresp = ["ERR", "Cannot create local file: '" + toname + "'", ]
             return cresp
 
         cresp = self.client(["fget", fname], key)
         if self.verbose:
-            print ("fget  response:", cresp)
+            print ("fget response:", cresp)
 
         if cresp[0] != "OK":
+            #print("remove:", toname)
+            try:
+                os.remove(toname)
+            except:
+                print(sys.exc_info())
             return cresp
 
         fsize = int(cresp[1])
-
         cipher = AES.new(key[:32], AES.MODE_CTR,
                         use_aesni=True, nonce = key[-8:])
         while(True):
             response = self.myhandler.handle_one(self.mydathand)
-            if self.pgdebug > 2:
+            if self.pgdebug > 8:
                 print("getfile resp", response[:12])
+            # possibly EOF
             if not response:
                 break
             response = cipher.encrypt(response)
             try:
                 fh.write(response)
             except:
                 #if self.verbose:
                 print( "Cannot write to local file: '" + toname + "'", sys.exc_info())
                 fh.close()
-                cresp = [ERR,"Cannot write local file",]
+                cresp = ["ERR" ,"Cannot write local file",]
                 return cresp
             fsize -= len(response)
+            # Detect the end of file bythe empty packet
             #if fsize <= 0:
             #   break
             #if not response:
             #    break
-
         fh.close()
-
         resp = self.recvx(key)
         return  resp
 
     def  getreply(self, key = "", rand = True):
-        response = self.myhandler.handle_one(self.mydathand)
 
-        if self.pgdebug > 3:
+        response = self.myhandler.handle_one(self.mydathand)
+        if self.pgdebug > 6:
             print( "Got reply:")
             print (crysupp.hexdump(response, len(response)))
-
         dstr = self.wr.unwrap_data(key, response)
         return dstr
 
     ''' Stat return values are as in python os.stat() + OK and name prefix
     "OK", fname (1),
     st_mode (2), st_ino, st_dev, st_nlink
     st_uid, st_gid, st_size (8)
@@ -286,15 +299,15 @@
 
     #@support.timeit2
     def client(self, message, key = "", rand = True):
 
         if type(message) != type([]):
             raise TypeError("Argument one to client() must be list")
 
-        if self.pgdebug > 0:
+        if self.pgdebug > 5:
             cnt = 0
             for aa in message:
                 try:
                     if len(aa) > 30:
                         aa = aa[:24]
                 except:
                     # Not iterable
@@ -312,33 +325,33 @@
         self.sendx(dstr)
 
         #if self.pgdebug > 0:
         #    print("    waiting for answer ...")
 
         response =  self.recvx(key)
 
-        if self.pgdebug > 0:
+        if self.pgdebug > 5:
             cnt = 0
             for aa in response:
 
                 try:
                     if len(aa) > 30:
                         aa = aa[:12]
                 except:
                     # Not iterable
                     pass
                 print( "   response %d:" % cnt, aa, end=' ')
                 cnt += 1
             print()
 
         '''resp = self.getreply(key)
-        if self.pgdebug > 1:
+        if self.pgdebug > 5:
             print("resp:", resp)
         response = self.pb.decode_data(resp[1])
-        if self.pgdebug > 0:
+        if self.pgdebug > 5:
             print( "    get: '%s'" % response)
         '''
         return response
 
     # ------------------------------------------------------------------------
     #  Login
 
@@ -376,59 +389,59 @@
         conf.sess_key2 = conf.sess_key[:]
 
         #if conf.verbose:
         #    print("Got akey:", resp)
 
         resp = self.client(["akey"], conf.sess_key2)
 
-        if conf.verbose:
+        if self.pgdebug > 5:
             print("Got akey:", resp)
 
         if resp[0] != "OK":
             print("Error on getting key:", resp)
             self.client(["quit"])
             self.close();
             sys.exit(0)
 
-        if conf.verbose:
+        if self.pgdebug > 5:
             print("Got hash:", "'" + resp[1] + "'")
 
         #hhh = SHA512.new(); hhh.update(bytes(resp[2], "cp437"))
         hhh = SHA256.new(); hhh.update(resp[2].encode())
 
-        if self.pgdebug > 1:
+        if self.pgdebug > 16:
             print("Hash1:  '" + resp[1] + "'")
             print("Hash2:  '" + hhh.hexdigest() + "'")
 
         # Remember key
         if hhh.hexdigest() !=  resp[1]:
             print("Tainted key, aborting.")
             self.client(["quit"])
             self.close();
             sys.exit(0)
 
         self.pkey = resp[2]
 
         #print("Key response:", resp[0], resp[2][:32], "...")
 
-        if self.pgdebug > 4:
+        if self.pgdebug > 5:
              print(self.pkey)
 
-        if self.pgdebug > 2:
+        if self.pgdebug > 5:
             print ("Server response:", "'" + hhh.hexdigest() + "'")
 
         try:
             #print(self.pkey)
             #self.pubkey = RSA.importKey(self.pkey)
             #self.pubkey = ECC.import_key(self.pkey)
             self.pubkey = Key.import_pub(self.pkey)
             #print("finger", self.pubkey.fingerprint())
             #print("validate", self.pubkey.validate())
 
-            if conf.pgdebug > 4:
+            if conf.pgdebug > 6:
                 print (self.pubkey)
         except:
             print("Cannot import public key.", sys.exc_info())
             support.put_exception("import key")
             self.client(["quit"])
             self.close();
             sys.exit(0)
@@ -443,30 +456,30 @@
         #print("sess_key", conf.sess_key[:24])
         #cipher = PKCS1_v1_5.new(self.pubkey)
         #cipher = PKCS1_OAEP.new(self.pubkey)
         cipher = self.pubkey
         #print(dir(cipher))
         #print ("cipher", cipher.can_encrypt())
 
-        if conf.pgdebug > 2:
+        if conf.pgdebug > 3:
             support.shortdump("conf.sess_key", conf.sess_key )
 
         if conf.sess_key:
             sess_keyx = cipher.encrypt(conf.sess_key)
             #print("sess_keyx", sess_keyx.encode()[:24])
 
             #self.privkey = Key.import_priv(privtest)
             #print("validate", self.privkey.validate())
             #print("finger", self.privkey.fingerprint())
             #sess_keyx3 = self.privkey.decrypt(sess_keyx)
             #print(sess_keyx3)
 
             ttt = SHA256.new(); ttt.update(sess_keyx.encode())
 
-            if conf.pgdebug > 2:
+            if conf.pgdebug > 5:
                 print("sess_keyx", crysupp.hexdump(sess_keyx.encode(), 24))
         else:
             sess_keyx = ""
 
         #print("Key Hexdigest", ttt.hexdigest()[:16])
         resp3 = self.client(["sess", sss.hexdigest(), ttt.hexdigest(), sess_keyx],
             conf.sess_key2,  False)
@@ -489,8 +502,78 @@
         #print("Atexit")
         cresp = hand.client(["quit", ], conf.sess_key)
         #print ("Server quit response:", cresp)
         hand.close();
     except:
         pass
 
+def expect(val, expx, ifyes = "", context = "", ifno = "" ):
+
+    if val == expx:
+        #print(ifyes)   # silent if OK
+        pass
+    else:
+        if not ifno:
+            ifno = "Unexpected result:",
+        print(ifno, "'" + val + "'"  , "!=",  "'" + expx + "'",
+                        "Context:", context)
+
+def formatstat(resp, dateidx = 0):
+    #print(resp)
+    ddd = datetime.datetime.fromtimestamp(int(resp[10 + dateidx]))
+    retx = ("%s %-24s %-8d %s" % (
+        support.mode2str(int(resp[2])), support.unescape(resp[1]),
+                int(resp[8]), ddd) )
+    return retx
+
+def show_onerec(hand, aa, conf):
+    dec = hand.pb.decode_data(aa[1])[0]
+    if conf.pgdebug > 2:
+        print("dec:", dec)
+    pay = hand.pb.decode_data(dec['payload'])[0]
+    if conf.verbose:
+        print("pay:", pay)
+    else:
+        print("payload:", pay['PayLoad'])
+
+def inter_date(begin = None, inter = None):
+
+    dd = datetime.datetime.now()
+    if not begin:
+        # Beginning of today
+        dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
+    else:
+        try:
+            dd = dd.strptime(begin, "%Y-%m-%d+%H:%M")
+        except:
+            try:
+                dd = dd.strptime(begin, "%Y-%m-%d")
+                dd = dd.replace(hour=0, minute=0, second=0, microsecond=0)
+            except:
+                try:
+                    yyyy = dd.year
+                    dd = dd.strptime(begin, "%m-%d+%H:%M")
+                    # Merge it with this year
+                    dd = dd.replace(year=yyyy, second=0, microsecond=0)
+                except:
+                    try:
+                        yyyy = dd.year; hhh = dd.hour; mmm = dd.minute
+                        dd = dd.strptime(begin, "%m-%d")
+                        # Merge it with this year, reset HH:MM
+                        dd = dd.replace(year=yyyy, hour=0, minute=0, second=0, microsecond=0)
+                    except:
+                        raise
+
+    dd_beg = dd + datetime.timedelta(0)
+    if inter:
+        dd_end = dd_beg + datetime.timedelta(0, inter * 60)
+    else:
+        dd_end = dd_beg + datetime.timedelta(1)
+
+    return dd_beg, dd_end
+
+def     exit_if_err(cresp, strx = "Exiting:"):
+    if cresp[0] != OK:
+        print(strx, cresp)
+        sys.exit(1)
+
 # EOF
```

### Comparing `pyvserv-1.0.3/pyvcommon/pycrypt.py` & `pyvserv-1.0.4/pyvcommon/pycrypt.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvcommon/pydata.py` & `pyvserv-1.0.4/pyvcommon/pydata.py`

 * *Files 3% similar despite different names*

```diff
@@ -56,33 +56,36 @@
         while True:
             time.sleep(1)
             #print (self.timex)
             if self.sock._closed:
                 break
             self.timex += 1
             if self.timex > self.timeout:
-                #print (self.timex)
                 self.handler_timeout()
                 break
 
     def handler_timeout(self):
-
         try:
             #self.tout.cancel()
             if self.pgdebug > 0:
                 print( "in handler_timeout %s" % self.name )
 
-            if self.verbose:
-                print( "handler_timeout()")
+            #if self.verbose:
+            #    print( "handler_timeout()")
 
             if self.pglog > 0:
-                pysyslog.syslog("Timeout on " + " " + str(self.par.client_address))
+                pysyslog.syslog("Timeout on ", str(self.par.client_address))
 
             #print(dir(self))
             #print(dir(self.par))
+
+            # Forcably close ... dead already but cleanup can start
+            self.sock.shutdown(socket.SHUT_RDWR)
+            self.sock.close()
+
         except:
             pass
         self.toutflag = True
 
     def putencode(self, ddd, key = "", rand = True):
 
         if type(ddd) == str:
```

### Comparing `pyvserv-1.0.3/pyvcommon/pyservsup.py` & `pyvserv-1.0.4/pyvcommon/pyservsup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 #!/usr/bin/env python
 
 from __future__ import print_function
 
 import os, sys, string, time, traceback, random, uuid
 import datetime, base64
 
+import multiprocessing as mp
+
 try:
     import fcntl
 except:
     fcntl = None
 
 #base = os.path.dirname(os.path.realpath(__file__))
 #sys.path.append(os.path.join(base, '../pyvcommon'))
@@ -17,55 +19,62 @@
 
 #from Crypto.Hash import SHA512
 from Crypto.Hash import SHA256
 from Crypto import Random
 
 # Globals and configurables
 
-version = "1.0"
+# Update it here from setup
+version = "1.0.4"
 
 # Actions
 USER_AUTH  = 0;  USER_ADD = 1;   USER_DEL = 2;   USER_CHPASS = 3;
 USER_CHMOD = 4;
 
 # Permissions
 PERM_NONE = 0;  PERM_INI = 1;   PERM_ADMIN = 2;   PERM_DIS = 4;
 PERM_NON = 8;
 
 # Modes
 RESET_MODE = 0x80;
 
+# ------------------------------------------------------------------------
+# Globals
+
 pgdebug = 0
 
 #buffsize = 1024;
 buffsize = 4096;
 
 chainfname  = "initial"
 repfname    = "pyvreplic"
 logfname    = "pyvserver"
 
-lock_pgdebug = 0
 lock_locktout = 5
+shared_logons = None
 
 # Configure the server by customizing this class
 
 class   Global_Vars:
 
     def __init__(self, scriptname, dataroot):
 
         # Underscore names are definitions - others are calculated
 
         self.verbose = 0
-        self._script_home = scriptname    # where the original script lives
+        # where the original script lives
+        self.script_home = os.path.abspath(scriptname)
+        #print("script:", self._script_home)
 
         self._dataroot  =   dataroot
         self._passfile  =  "passwd.secret"
         self._keyfile   =  "keys.secret"
         self._idfile    =  "pyservid.init"
 
+        # Force relative to home
         if self._dataroot[0] != os.sep:
             self.myhome     =  os.path.expanduser(
                                 "~" + os.sep + self._dataroot + os.sep)
         else:
             self.myhome     =  self._dataroot + os.sep
 
         self.myhome    = os.path.normpath(self.myhome) + os.sep
@@ -117,14 +126,17 @@
         self.throt_time       =  3    # throttle by this many sec
 
         #print("init globals");
         #global globals
         #globals = self
         pass
 
+    def softmkdir(self, ddd):
+        self._softmkdir(ddd)
+
     # Soft make dir
     def _softmkdir(self, ddd, fff="data"):
 
         if not os.path.isdir(ddd):
             try:
                 os.mkdir(ddd, 0o700)
             except:
@@ -133,22 +145,21 @@
 
     # --------------------------------------------------------------------
 
     def config(self, realp, conf):
 
         self.verbose = conf.verbose
         self.pgdebug = conf.pgdebug
-
         #if conf.verbose:
         #    print("Script home:     ", self._script_home)
-
         if conf.pgdebug:
-                print ("Debug level:     ", conf.pgdebug)
+            print ("Debug level:     ", conf.pgdebug)
 
-        #self._datadir = self.script_home + self._datadir
+        globals.siteid = create_read_idfile \
+                        (globals.idfile)
 
 # ------------------------------------------------------------------------
 # This will create the server's UUID
 
 def  create_read_idfile(fname):
 
     # Create globals file, read it if exists
@@ -201,83 +212,149 @@
                 #print("Badly formed UUID");
                 pass
             break
     fp2.close
 
     return uuuu
 
-# ------------------------------------------------------------------------
-
 class   FileLock():
 
-    ''' A working file lock in Linux '''
+    ''' A working file lock in Linux and Windows '''
 
-    def __init__(self):
+    def __init__(self, lockname = ""):
 
-        ''' Create the lock file '''
-        self.lockname = None
+        ''' Create the lock file, else just remember the name '''
+
+        #if not lockname:
+        #    raise ValueError("Must specify lockfile")
+
+        self.lockname = lockname
+
+        if pgdebug > 0:
+            print("lockname init", self.lockname)
+
+        if fcntl:
+            if self.lockname:
+                try:
+                    self.fpx = open(lockname, "wb")
+                except:
+                    if pgdebug > 1:
+                        print("Cannot create lock file")
+                    raise ValueError("Cannot create lock file")
 
     def waitlock(self):
 
+        # If no lockfilename specified, grab one
         if not self.lockname:
             self.lockname = globals.passfile + ".lock"
-            #print("lockname", self.lockname)
+
+            if pgdebug > 5:
+                print("lockname", self.lockname)
 
             try:
-                self.fpx = open(self.lockname, "rb+")
+                self.fpx = open(self.lockname, "wb")
             except:
+                if pgdebug > 1:
+                    print("Cannot create lock file")
+
+        if pgdebug > 5:
+            print("Waitlock", self.lockname)
+
+        if fcntl:
+            cnt2 = 0
+            while True:
                 try:
-                    self.fpx = open(self.lockname, "wb+")
+                    fcntl.flock(self.fpx, fcntl.LOCK_EX | fcntl.LOCK_NB)
+                    break
                 except:
-                    if lock_pgdebug > 1:
-                        print("Cannot create lock file")
-                    raise
+                    pass
+                    if pgdebug > 1:
+                        print("waiting in fcntl", self.lockname,
+                                            os.getpid()) #sys.exc_info())
+                cnt2 += 1
+                time.sleep(1)
+                if cnt2 > lock_locktout:
+                    # Taking too long; break in
+                    if pgdebug > 1:
+                        print("Lock held too long",
+                                            os.getpid(), self.lockname)
+                    self.unlock()
+                    break
+        else:
+            cnt = 0
+            while True:
+                try:
+                    if os.path.exists(self.lockname):
+                        if pgdebug:
+                           print("Waiting ... ", self.lockname)
+                        pass
+                    else:
+                        fp = open(self.lockname, "wb")
+                        fp.write(str(os.getpid()).encode())
+                        fp.close()
+                        break
+                except:
+                    if pgdebug:
+                        print("locked",  self.lockname, cnt, sys.exc_info())
+                    pass
+                time.sleep(1)
+                cnt += 1
+                if cnt > lock_locktout:
+                    if pgdebug:
+                        print("breaking lock", self.lockname)
+                    break
 
-        if lock_pgdebug > 1:
-            print("Waitlock", self.lockname)
+    def unlock(self):
+
+        if pgdebug > 5:
+            print("Unlock", self.lockname)
 
-        cnt = 0
-        while True:
+        if fcntl:
             try:
-                buff = self.fpx.read()
-                self.fpx.seek(0, os.SEEK_SET)
-                self.fpx.write(buff)
-                break;
+                fcntl.flock(self.fpx, fcntl.LOCK_UN | fcntl.LOCK_NB)
             except:
-                if lock_pgdebug > 1:
-                    print("waiting", sys.exc_info())
+                pass
+        else:
+            try:
+                os.remove(self.lockname)
+            except:
+                pass
+                if pgdebug:
+                    print("unlock", self.lockname, sys.exc_info())
 
-            if cnt > lock_locktout :
-                # Taking too long; break in
-                if 1: #lock_pgdebug > 1:
-                    print("Lock held too long pid =", os.getpid(), cnt)
-                self.unlock()
-                break
-            cnt += 1
-            time.sleep(1)
-        # Lock NOW
-        if fcntl:
-            fcntl.lockf(self.fpx, fcntl.LOCK_EX)
+    def __del__(self):
 
-    def unlock(self):
-        if fcntl:
-            fcntl.lockf(self.fpx, fcntl.LOCK_UN)
+        #print("__del__ lock", self.lockname)
+        try:
+            if fcntl:
+                # Do not remove, others may have locked it
+                if hasattr(self, "fpx"):
+                    fcntl.flock(self.fpx, fcntl.LOCK_UN | fcntl.LOCK_NB)
+                pass
+
+            # Always remove file
+            try:
+                os.remove(self.lockname)
+            except:
+                pass
+                #print("cannot delete lock", self.lockname, sys.exc_info())
+        except:
+            print("exc on del (ignored)", self.lockname, sys.exc_info())
+            pass
 
 # ------------------------------------------------------------------------
 # This class will maintain a passwd database, similar to
 #  the system database
 
 class Passwd():
 
     def __init__(self):
         self.pgdebug = 0
         self.verbose = 0
-        global lock_pgdebug
-        lock_pgdebug = 0
-        self.lock = FileLock()
+        self.lock = FileLock(globals.passfile + ".lock")
 
     def     _xjoin(self, iterx, charx):
         sss = ""
         try:
             for aa in iterx:
                 if sss != "":
                     sss += charx
@@ -612,15 +689,45 @@
             ret = 7, "User permissions:", 0
 
         self.lock.unlock()
         #print("   perms 4 %.3f" % ((time.time() - ttt) * 1000) )
 
         return ret
 
-passwd = Passwd()
+    def listusers(self, umode):
+
+        self.lock.waitlock()
+        fields = ""; haveusr = False
+        try:
+            fh = open(globals.passfile, "r")
+        except:
+            try:
+                fh = open(globals.passfile, "w+")
+            except:
+                #self._unlock()
+                return -1, "Cannot open / create pass file " + globals.passfile
+
+        passdb = fh.readlines()
+        fh.close()
+        userlist = []
+        if not passdb:
+            self.lock.unlock()
+            return userlist
+
+        for line in passdb:
+            fields = line.split(",")
+            fff = int(fields[1])
+            #print(fields[:2])
+            if umode == 0 and fff == 0:
+                userlist.append(fields[0])
+            elif fff & umode:
+                userlist.append(fields[0])
+
+        self.lock.unlock()
+        return userlist
 
 # ------------------------------------------------------------------------
 # Save key to local file. Return err code and cause.
 #   kadd = 0 -> Authenticate
 #   kadd = 1 -> add
 #   kadd = 2 -> delete
 #   kadd = 3 -> chpass
@@ -713,88 +820,24 @@
 
 # Return basename for key file
 
 def pickkey(keydir):
 
     #print("Getting keys", keydir)
     dl = os.listdir(keydir)
-    if dl == 0:
-        print("No keys yet", keydir)
-        raise (Valuerror("No keys generated yet"))
-
+    #print("dl:", dl)
+    if not dl:
+        #print("No keys yet", keydir)
+        raise (ValueError("No keys generated yet"))
     dust = random.randint(0, len(dl)-1)
     eee = os.path.splitext(os.path.basename(dl[dust]))
     #print("picking key", eee[0])
     return eee[0]
 
 # ------------------------------------------------------------------------
-# Simple file system based locking system
-# !!!!! does not work on Linux !!!!!
-# Linux can access the filesystem differently than windosw, however the
-# file based locking system work well
-
-#def _createlock(fname, raisex = True):
-#
-#    ''' Open for read / write. Create if needed. '''
-#
-#    fp = None
-#    try:
-#        fp = open(fname, "wb")
-#    except:
-#        print("Cannot open / create ", fname, sys.exc_info())
-#        if raisex:
-#            raise
-#    return fp
-#
-#def dellock(lockname):
-#
-#    ''' Lock removal;
-#        Test for stale lock;
-#    '''
-#
-#    try:
-#        if os.path.isfile(lockname):
-#            os.unlink(lockname)
-#    except:
-#        if pgdebug > 1:
-#            print("Del lock failed", sys.exc_info())
-#
-#def waitlock(lockname, locktout = 30):
-#
-#    ''' Wait for lock file to become available. '''
-#
-#    cnt = 0
-#    while True:
-#        if os.path.isfile(lockname):
-#            if pgdebug > 1:
-#                print("Waiting on", lockname)
-#            #if cnt == 0:
-#            #    try:
-#            #        fpx = open(lockname)
-#            #        pid = int(fpx.read())
-#            #        fpx.close()
-#            #    except:
-#            #        print("Exc in pid test", sys.exc_info())
-#            cnt += 1
-#            time.sleep(0.3)
-#            if cnt > locktout:
-#                # Taking too long; break in
-#                if pgdebug > 1:
-#                    print("Warn: main Lock held too long ... pid =", os.getpid(), cnt)
-#                dellock(lockname)
-#                break
-#        else:
-#            break
-#
-#    # Finally, create lock
-#    xfp = _createlock(lockname)
-#    xfp.write(str(os.getpid()).encode())
-#    xfp.close()
-
-# ------------------------------------------------------------------------
 # Get date out of UUID
 
 def uuid2date(uuu):
 
     UUID_EPOCH = 0x01b21dd213814000
     dd = datetime.datetime.fromtimestamp(\
                     (uuu.time - UUID_EPOCH)*100/1e9)
@@ -804,14 +847,190 @@
 def uuid2timestamp(uuu):
 
     UUID_EPOCH = 0x01b21dd213814000
     dd = datetime.datetime.fromtimestamp(\
                     (uuu.time - UUID_EPOCH)*100/1e9)
     return dd.timestamp()
 
-if __name__ == '__main__':
-    print( "This module was not meant to be used directly.")
+class SharedData():
+
+    '''  Common space for mydata for remebering connecting client data.
+    '''
+    def __init__(self):
+
+        if fcntl:
+            # This is for forkmixin
+            self.sem  = mp.Semaphore()
+            self.man  = mp.Manager()
+            self.mydata = self.man.dict()
+        else:
+            self.sem     = threading.Semaphore()
+            self.mydata = {}
+
+    def setdat(self, newkey, newdat):
+
+        self.sem.acquire()
+        try:
+            self.mydata[newkey] = newdat
+        except:
+            print("setdat", sys.exc_info())
+        self.sem.release()
 
+    def getdat(self, key):
 
-# EOF
+        self.sem.acquire()
+        ddd = None
+        try:
+            ddd = self.mydata[key]
+        except:
+            print("getdat", self.man, self.sem, sys.exc_info())
+        self.sem.release()
+
+        return ddd
+
+    def getall(self):
+
+        self.sem.acquire()
+        ddd = None
+        try:
+            ddd = self.mydata.copy()
+        except:
+            print("getall", sys.exc_info())
+        self.sem.release()
+
+        return ddd
+
+    def deldat(self, keyx):
+
+        self.sem.acquire()
+        try:
+            del self.mydata[keyx]
+        except:
+            print("deldat", sys.exc_info())
+        self.sem.release()
+        return
+
+# ------------------------------------------------------------------------
+
+class Throttle():
+
+    '''  Catch clients that are connecting too fast. This needs a serious
+        upgrade if in large volume production.
+    '''
+    def __init__(self):
+
+        if fcntl:
+            # This is for forkmixin
+            self.sem  = mp.Semaphore()
+            self.man  = mp.Manager()
+            self.connlist = self.man.list()
+            #self.enabled = self.man.list()
+            #self.enabled.append(1)
+            self.enabled = self.man.Value("i", 1)
+        else:
+            self.sem     = threading.Semaphore()
+            self.connlist = []
+            self.enabled = True
+
+    def throttle(self, peer):
+
+        '''
+            Catch clients that are connecting too fast.
+            Throttle to N sec frequency, if number of connections from
+            the same ip exceeds throt_instances.
+        '''
+
+        wantsleep = 0; sss = 0;
+        now = time.time()
+
+        self.sem.acquire()
+        # Throttle disabled, return zero delay
+        if not self.enabled.value:
+        #if not self.enabled[0]:
+            self.sem.release()
+            return 0
+
+        # Calculate recents
+        for aa in self.connlist:
+            if aa[0] == peer[0]:
+                if now - aa[1] <  globals.throt_sec:
+                    sss += 1
+
+        if sss >  globals.throt_instances:
+            # Clean old entries for this host
+            for aa in range(len(self.connlist)-1, -1 ,-1):
+                if self.connlist[aa][0] == peer[0]:
+                    if now - self.connlist[aa][1] > globals.throt_sec:
+                        del self.connlist[aa]
+            wantsleep = globals.throt_time
+
+        # Clean throtle data periodically
+        if len(self.connlist) > globals.throt_maxdat:
+            #print("Cleaning throttle list", len(self.connlist))
+            for aa in range(len(self.connlist)-1, -1 ,-1):
+                if now - self.connlist[aa][1] > globals.throt_maxsec:
+                    del self.connlist[aa]
+
+        # Flatten list for the multiprocessing context manager
+        self.connlist.append((peer[0], now))
+
+        #print("connlist", self.connlist)  # Make sure it cycles
+        #print()
+
+        self.sem.release()
+        return wantsleep
+
+    def setflag(self, flag):
+
+        ''' Enable / disable throttleing '''
+
+        #print("setting flag", flag)
+
+        self.sem.acquire()
+        #self.enabled[0] = flag
+        self.enabled.value = flag
+        self.sem.release()
+
+    def getflag(self):
+
+        ''' report throttling status '''
+
+        self.sem.acquire()
+        #self.enabled[0] = flag
+        ret = self.enabled.value
+        self.sem.release()
+        return ret
+
+# The one and only instance
+gl_throttle = Throttle()
+
+bool_yes = [ "on", "yes", "true", "enable" ]
+bool_no = [ "off", "no", "false", "disable" ]
+
+def str2bool(strx, default = False):
+
+    ''' Turn a string into a boolean value.
+        If value is recognized, turn it. Otherwise assume passed default.
+    '''
+
+    boolx = -1
+    strx = strx.lower()
+    for aa in bool_yes:
+        if strx == aa:
+            boolx = True
+            break
+    if boolx == -1:
+        for aa in bool_no:
+            if strx == aa:
+                boolx = False
+                break
+    # Response not found, default it
+    if boolx == -1:
+        boolx = default
+
+    return boolx
+
+if __name__ == '__main__':
+    print( "This module was not meant to be used directly.")
 
 
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvcommon/pysyslog.py` & `pyvserv-1.0.4/pyvcommon/pysyslog.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvcommon/pyv2fa.py` & `pyvserv-1.0.4/pyvcommon/pyv2fa.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvcommon/pyvhash.py` & `pyvserv-1.0.4/pyvcommon/pyvhash.py`

 * *Files 8% similar despite different names*

```diff
@@ -34,29 +34,40 @@
 
 Hash     = "_Hash"
 Link     = "_Link"
 PrevHash = "_PrevHash"
 PowRand  = "_PowRand"
 Proof    = "_Proof"
 Repli    = "Replicated"
-PayLoad  = "payload"
+PayLoad  = "PayLoad"
 Header   = "header"
 Now      = "now"
+Stamp    = "stamp"
+Iso      = "iso"
+
+datefmt = '%a, %d %b %Y %H:%M:%S'
+isostr  = "%Y-%m-%dT%H:%M:%S"
 
 def DefPayload():
     return {PayLoad : { "Default": "None"}}
 
 def DefHeader():
     return {Header : str(uuid.uuid1())}
 
-def DefNow():
-    dt = datetime.datetime.now()
-    fdt = dt.strftime('%a, %d %b %Y %H:%M:%S`')
+def DefNow(dt):
+    fdt = dt.strftime(datefmt)
     return {'now' : fdt}
 
+def DefISO(dt):
+    fdt = dt.isoformat()
+    return {'iso' : fdt}
+
+def DefStamp(dt):
+    return {'stamp' : str(dt.timestamp())}
+
 def DefRep():
     return {Repli : 0}
 
 class NoProof(Exception):
 
     def __init__(self, strx):
         self.strx = strx
@@ -70,15 +81,15 @@
     ''' Shorthand to exec hash op '''
 
     hh = USEHASH.new();
     hh.update(val)
     hhh = hh.hexdigest()
     return hhh
 
-# Enable the bigger one for production
+# Enable the bigger one if needed.
 #USEHASH = SHA512
 USEHASH = SHA256
 
 class BcData():
 
     '''
         This class manipulates the block chain data.
@@ -110,21 +121,35 @@
             for aa in range(len(old_data) // 2):
                 tmpx |= { old_data[aa]: old_data[aa+1], }
                 self.datax = copy.deepcopy(tmpx)
         elif type(old_data) == type(None):
             self.newdata()
         else:
             raise TypeError("Cannot create class from %s" % type(old_data))
+
         # Add Expected fields:
+        dt = datetime.datetime.now()
+        dt = dt.replace(microsecond=0)
         if not PayLoad in self.datax:
             self.datax |= DefPayload()
         if not Header in self.datax:
             self.datax |= DefHeader()
+
+        # This is a lot of datetime variations. The rational is:
+        #   a human readable
+        #   a machine readable and
+        #   an ISO standard date.
+        # This is to assist internationalzation and possible hand count.
+
         if not Now in self.datax:
-            self.datax |= DefNow()
+            self.datax |= DefNow(dt)
+        if not Stamp in self.datax:
+            self.datax |= DefStamp(dt)
+        if not Iso in self.datax:
+            self.datax |= DefISO(dt)
         if not Repli in self.datax:
             self.datax |= DefRep()
 
         if self.pgdebug:
             print(self.datax)
 
     def newdata(self):
```

### Comparing `pyvserv-1.0.3/pyvcommon/pywrap.py` & `pyvserv-1.0.4/pyvcommon/pywrap.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvcommon/support.py` & `pyvserv-1.0.4/pyvcommon/support.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,14 +22,15 @@
     rr = random.randint(0, 100)
     #print("rr", rr)
 
 # ------------------------------------------------------------------------
 # A more informative exception print
 
 def put_debug(xstr):
+
     try:
         if os.isatty(sys.stdout.fileno()):
             print( xstr)
         else:
             syslog.syslog(xstr)
     except:
         print( "Failed on debug output.")
@@ -274,15 +275,15 @@
 # ------------------------------------------------------------------------
 
 def unlock_process(lockfile):
     try:
         os.unlink(lockfile)
     except:
         pass
-        print("Cannot unlink lockfile.", lockfile, sys.exc_info())
+        #print("Cannot unlink lockfile.", lockfile, sys.exc_info())
 
 def lock_process(lockfile):
 
     closeit = 0; pidstr = ""
     pid = os.getpid()
 
     try:
```

### Comparing `pyvserv-1.0.3/pyvgui/guilib/mainwin.py` & `pyvserv-1.0.4/pyvgui/guilib/mainwin.py`

 * *Files 2% similar despite different names*

```diff
@@ -168,19 +168,19 @@
         ##butt1.connect("clicked", self.show_new, window)
         #hbox4p.pack_start(butt1, False, 0, 2)
 
         butt1 = Gtk.Button.new_with_mnemonic("    _Start Log Mon.  ")
         butt1.connect("clicked", self.mon_log)
         hbox4p.pack_start(butt1, False, 0, 2)
 
-        butt1 = Gtk.Button.new_with_mnemonic("    _Stop Log Mon.  ")
+        butt1 = Gtk.Button.new_with_mnemonic("    Stop Log Mon.  ")
         butt1.connect("clicked", self.mon_log_off)
         hbox4p.pack_start(butt1, False, 0, 2)
 
-        butt1 = Gtk.Button.new_with_mnemonic("    Start Replic. Mon.  ")
+        butt1 = Gtk.Button.new_with_mnemonic("    Start _Replic. Mon.  ")
         butt1.connect("clicked", self.enable_replic)
         hbox4p.pack_start(butt1, False, 0, 2)
 
         butt1 = Gtk.Button.new_with_mnemonic("    Stop Replic. Mon. ")
         butt1.connect("clicked", self.disable_replic)
         hbox4p.pack_start(butt1, False, 0, 2)
 
@@ -192,15 +192,15 @@
         lab2a = Gtk.Label(" buttom ");  hbox4.pack_start(lab2a, 1, 1, 0)
         lab2a.set_xalign(0)
         lab2a.set_size_request(300, -1)
         self.status = lab2a
 
         lab1 = Gtk.Label("  ");  hbox4.pack_start(lab1, 1, 1, 0)
 
-        butt1 = Gtk.Button.new_with_mnemonic("    _Start Data Mon.  ")
+        butt1 = Gtk.Button.new_with_mnemonic("    Start _Data Mon.  ")
         butt1.connect("clicked", self.datamon_on)
         hbox4.pack_start(butt1, False, 0, 2)
 
         butt1 = Gtk.Button.new_with_mnemonic("    S_top Data Mon.   ")
         butt1.connect("clicked", self.datamon_off)
         hbox4.pack_start(butt1, False, 0, 2)
 
@@ -407,18 +407,18 @@
                         continue
                     #print("Datamon", rec)
                     pb = pyvpacker.packbin()
                     dec = pb.decode_data(rec[1])[0]
                     #print("dec", dec)
                     decpay   = pb.decode_data(dec['payload'])[0]
                     #print("decpay", decpay)
-                    for bb in sorted(decpay.keys()):
-                        strx = ""
-                        if bb[0] != "_":
-                            strx += bb + " : " + str(decpay[bb]) + "  "
+                    strx = ""
+                    for bb in sorted(decpay['PayLoad'].keys()):
+                        if 1: #bb[0] != "_":
+                            strx += bb + " : " + str(decpay['PayLoad'][bb]) + "  "
                     #print("append:", strx)
                     self.tree3.append([dec['header'], strx])
                 self.old_sss = sss
                 self.tree3.sel_last()
                 self.led2.set_color("00ff00")
                 GLib.timeout_add(400, self.led_off, self.led2, "#aaaaaa")
```

### Comparing `pyvserv-1.0.3/pyvgui/guilib/mainwinserv.py` & `pyvserv-1.0.4/pyvgui/guilib/mainwinserv.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvgui/guilib/pgui.py` & `pyvserv-1.0.4/pyvgui/guilib/pgui.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvgui/guilib/pymenu.py` & `pyvserv-1.0.4/pyvgui/guilib/pymenu.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvgui/pyvcpanel.py` & `pyvserv-1.0.4/pyvgui/pyvcpanel.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvgui/pyvservui.py` & `pyvserv-1.0.4/pyvgui/pyvservui.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvgui/pyvtally.py` & `pyvserv-1.0.4/pyvgui/pyvtally.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvserv.egg-info/PKG-INFO` & `pyvserv-1.0.4/pyvserv.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyvserv
-Version: 1.0.3
+Version: 1.0.4
 Summary: High power secure server with blockchain backend.
 Home-page: https://github.com/pglen/pyvserv
 Author: Peter Glen
 Author-email: peterglen99@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -115,53 +115,82 @@
 #### Start server
 
  The python server can be added to the system servers with the Makefile targets
 'make genservice' and 'make instservice'
  The scripts will generate the service file to run under current user's
  credentials, and install it onto the running system. (requires sudo)
 
-#### Platform:
+#### Platforms:
 
  This project was developed on Ubuntu 22.x. Most linux distributions should work.
 It is ported to Windows MSYS2, with all major functions operating as expected.
 
  On Fedora, the service files need to be re-written to accomodate the
 quirk that the Fedora systectl does not allow user executables. Install
 the 'pip pyvserv' as root, and adjust the service file accordingly. If you want
 to use pyvserv with  particular data directory, use the -r option.
 
+ On Debian and newer (23+) Ubuntu the system needs the --break-system-packages
+ on pip. (unless one creates a venv for it) This is a cutionary arrangement
+ for the OS, pyvserv does not break anything.
+
+    pip install pyvserv --break-system-packages
+
+Also the scripts are installed in ~/.local/bin, so add the following line
+  to the end of ~/.bashrc:
+
+    PATH=$PATH:~/.local/bin
+
+This workaround is not needed if one installs pyvserv in a virtual environment.
+
+    python3 -m venv pip_pyvserv
+    cd pip_pyvserv
+    source ./bin/avtivate
+    pip install pyvserv
+    ... continue as needed.
+
+The makefile target 'make installvirt' will install pyvserv in a virtual
+environment.
+
+ Running pyvserv as a system daemon from virtual environment needs extra
+configuration steps. You may use the make target: 'make genservice_virt'
+and activate with 'make instservice'
+Please see the relevant systemctl manuals.
+
 #### Quick map:
 
     Server.     subdir: pyvserver       -- Server has most all the commands done
     Client.     subdir: pyvclient       -- Exercise server commands / demo code
     Test Suite. subdir: pyvclient/tests -- official pytest tests
     Tool Suite. subdir: pyvtools        -- Key generation etc ...
     GUI base    subdir: pyvgui          -- Monitoring / administering the server
     Studies.    subdir: study           -- testing/learning subsystems (ignore it)
 
 #### Quick start:
 
  One can mimic global connectivity on a single machine. This would allow the study
 of the client / server interaction before live deployment. This chapter assumes
-installation from github, replicating directory structure on the local drive.
+installation / clone from github, replicating directory structure on the
+local drive.
 
     open terminal window
     navigate to the server's pyvserver subdir
     type: ./pyvserv.py
 
     open another terminal window
     navigate to the pyvclient subdir
     type: ./pyvcli_hello.py
 
 The following (and more) should be printed on the command line:
 
     ./pyvcli_hello.py
-    Server initial: ['OK', 'pyvserv 1.0 ready']
-    resp ['OK', 'Hello', '6ccdaaf1-a22d-4140-9608-8fb93a8845af', '11812']
-    Server quit response: ['OK', 'Bye', '11812']
+
+    Server initial: ['OK', 'pyvserv 1.0.4 ready']
+    resp ['OK', 'Hello', '4814b46a-9489-4720-af7d-aa14ba19f2be', '11367']
+    Server quit response: ['OK', 'Bye', '11367']
 
 Quick rundown of the above test:
 
     1.) Server responds to connection with signin message
     2.) Delivers OK status, hello message, server serial number, and a unique id
     3.) Server signs off. Repeats unique id / session number.
 
@@ -184,15 +213,22 @@
  (two factor authentication)
 
  The command line client can be started as:
 
     pyvcli_cli
 
   In the command line client most of the server functions can be exercised.
-See the pyvcli_* utils for more examples of driving the server.
+See the pyvcli_* utils for more examples of driving the server. On a
+fresh install, one may need to execute the pyvcli_uini.py to create an initial
+admin user, with password 1234. The uini command will prompt if this is
+what was intended.
+
+ The cli utility command 'help' will deliver information on the available commands.
+
+!!! IMPORTANT !!! Make sure you change this when testing / learning is over.
 
 ## Command line help
 
     Usage: pyvserv.py [options]
 
     Options:
             -n   --host                 -  Set server hostname / interface.
@@ -209,36 +245,72 @@
             -h   --help                 -  Show Help
 
 ## Client command line help example:
 
  While most command line clients have their own help screen, here as a typical
 client utility's help screen:
 
-    Usage: pyvcli_uman.py [options]
+    Usage: pyvcli_uman.py [options] [hostname]
 
     Options:    -d level  - Debug level 0-10
                 -p        - Port to use (default: 6666)
                 -l login  - Login Name; default: 'user'
                 -s lpass  - Login Pass; default: '1234'
                 -u user   - User Name; default: 'user'
-                -a        - Add user. Must be unique.
-                -r        - Remove user (one of add or remove needed.
+                -t        - prompt for login pass
+                -a        - Add user. Must be a unique user name.
+                -r        - Remove user
                 -u user   - User Name; default: 'user'
-                -p pass   - User pssword; default: '1234' (!!! for tests only)
+                -p pass   - User password; default: '1234' (!!for tests only!!)
+                -T        - prompt for new pass
                 -m        - Add admin instead of regular user
+                -e enflag - Enable / Disable user.
+                -i kind   - List users (user or admin
                 -v        - Verbose
                 -q        - Quiet
                 -h        - Help
 
+     One of Add / Remove / Enable / List option is needed.
+
+## pyvser clients
+
+ Some client programs are supplied to administer / drive / monitor pyvserv.
+ The -h option on the client programs give a brief help of usage / purpose.
+
+ | Client name  | Description               |        Purpose                |
+ | -----------  |  -----------              |  ------------------------     |
+ | pyvcli_cli   | Command line interface    | All aspects of pyvserv        |
+ | pyvcli_uini  | Create initial user       | Create initial admin user     |
+ | pyvcli_fman  | File manager              | Upload / Download files       |
+ | pyvcli_uman  | User manager              | Add remove users / admins     |
+ | pyvcli_rman  | Record manager            | Get / Put Blockchain Records  |
+ | pyvcli_hello | Get hello message         | Connectivity test             |
+ | pyvcli_ver   | Get Version number        | Check for server version      |
+
+ The utilities can also be executed from the 'pyvclient' sub directory by
+ post fixing with script extension. (add the .py extension like: ./pyvcli_cli.py)
+
+ The date formats for specifying record date filter dates are:
+
+   'Y-m-d+H:M' 'Y-m-d' 'm-d' 'm-d+H-M'
+
+Where Y=year m=month d=day H=hour M=minutes, just like in strftime.
+The hour is in 24 hour notation.
+
+The following are all valid dates specs, specifying the same date
+(in 2024 apr 15 at 00:00):
+
+    2024-04-15 2024-04-15+0:0 04-15 04-15+00:00
+
 ## Testing:
 
- All pytest cases pass. Note that the for the pytest client tests one needs to
- start the 'pyvserv.py' server.
- The server --port and --dataroot option can ba used to start the server in an alternate
- universe. Please make sure it does not interfere with production.
+ All pytest cases pass successfully. Note that for the pytest client
+ tests one needs to start the server. ('./pyvserv.py' or pyvserv if installed)
+ The server --port and --dataroot option can be used to start the server in
+ an alternate 'universe', so it does not interfere with production.
 
     ============================ test session starts ==============================
     platform linux -- Python 3.10.12, pytest-7.4.3, pluggy-1.0.0
     rootdir: /home/<homedir>/pgpygtk/pyvserv
     collected 15 items
 
     test_afirst.py .                                                         [  6%]
@@ -253,45 +325,56 @@
     test_rput.py .                                                           [ 73%]
     test_sess.py ..                                                          [ 86%]
     test_user.py .                                                           [ 93%]
     test_ver.py .                                                            [100%]
 
     ============================== 15 passed in 9.47s ==============================
 
-Additional tests can be found in the tests/ directory. The pyvcli_* files may also
-serve as test cases.
+Additional tests can be found in the tests/ directory. The pyvcli_* files in the
+'pyvclient' directory may also serve as test cases.
+
+## Production:
 
-More test coming soon ....
+Once the testing phase is complete, deploying it for production needs a
+complete wipe of the data. There are Makefile targets that do that
+(make cleanall). Restarting the server will create the new environment without
+any users. To allow operation one may create the initial user with the uini
+functions and / or scripts.
+The uini command can only operate successfully if there are no users present in the
+pyvserv system, and it is executed from the loopback interface. For example,
+the command line utility ./pyvcli_uini.py can be used;
+For production, it can executed with the -t option to prompt for a password.
 
 ## Screen shots:
 
 Screen shot of the Monitoring tool:
 
 ![Screen Shot](montool.png)
 
  This screen shot depicts the monitoring (control panel) application 'pyvcpanel'.
 The top left area contains a live view of the pyvserver syslog. The top right
 contains a live view of the replicator log.
 
  The bottom area of the window contains a live view of the incoming data, as it is
 originally formatted, without the blockchain and hash details.
 
-  All views monitor the live files, on the default setup, without interfering
-with any of the operations.
+  All views monitor the live log files, on the default setup. The montor functions
+operate, without interfering with any of the operations.
 
 ## Windows compatibility
 
- Pyvserv now functions in the Windows MSYS2 subsystem. All the major
+  Pyvserv now functions in the Windows MSYS2 subsystem. All the major
 functionalities are ported. The file locking mechanism works, and all the
 pytests pass. Naturally, logging and readline etc ... works with the usual
 windows caveat.
 
-  For the GUI functions install the PyGobject subsystem. Instructions can
-be found very easily for that. Below, a screenshot of the pyvserv control panel
-in MSYS2.
+  For the GUI functions ona my need to install the PyGobject subsystem.
+Instructions can be found very easily for that.
+
+Below, a screenshot of the pyvserv control panel in MSYS2.
 
 ![Screen Shot](winscreen.png)
 
 The project is functional in MSYS2, but for real deployment we recommend Linux.
 
 ## History:
 
@@ -299,31 +382,34 @@
 
     1.0.0   Sun 03.Mar.2024    Beta ready
     1.0.0   Mon 11.Mar.2024    PIP installation with utils
     1.0.0   Wed 13.Mar.2024    rget rput and family (rget=BC record get)
     1.0.0   Thu 14.Mar.2024    Started GUI tools
     1.0.1   Fri 15.Mar.2024    Added LIC, verification, doc, tally
     1.0.3   Wed 03.Apr.2024    Ported to MSYS2, throttle, for multiprocess
+    1.0.4   Tue 09.Apr.2024    Cleanup, uman fman rman completed
 
 ## Statistics
 
     Project name
         pyvserv
+    Generated
+        2024-04-09 20:45:56
     Report Period
-        2018-12-31 20:50:04 to 2024-03-15 04:47:25
+        2018-12-31 20:50:04 to 2024-04-09 20:41:24
     Age
-        1901 days, 101 active days (5.31%)
+        1927 days, 111 active days (5.76%)
     Total Files
-        287
+        211
     Total Lines of Code
-        70286 (235368 added, 165082 removed)
+        44443 (258657 added, 214214 removed)
     Total Commits
-        216 (average 2.1 commits per active day, 0.1 per all days)
+        257 (average 2.3 commits per active day, 0.1 per all days)
     Authors
-        6 (average 36.0 commits per author)
+        6 (average 42.8 commits per author)
 
 ![Screen Shot](commits_by_year_month.png)
 
 ## Security review:
 
  &nbsp;  As of today, (Fri 15.Mar.2024) the 256 bit AES is considered unbreakable by
 available state of the art means. The key exchange algorithm ECC 384 bit is
@@ -331,15 +417,15 @@
 key is used in every session. The session is also able to dynamically change keys
 mid flight, on command.
 
  &nbsp; The checksum verification and link verification both use SHA256 (256 bit)
 hashes. This is generated every time a transaction is created.
 
  &nbsp; The proof of work is a modest 3 generations deep. This can be calculated
-with an everyday desktop in one - to - three seconds. Even though this looks like
+with an everyday desktop in one ... to ... three seconds. Even though this looks like
 a small amount, it adds up if one wants to re-generate (fake) a whole chain.
 Additionally, the check sum, the link sum, and proof of work interact, changing one
 will effect the other. This way a sum verification and link verification and the
 proof of work verification together create an ironclad safety solution.
 
 Written by Peter Glen, 2022, 2023, 2024
 Released under MIT License (MIT)
```

### Comparing `pyvserv-1.0.3/pyvserv.egg-info/entry_points.txt` & `pyvserv-1.0.4/pyvserv.egg-info/entry_points.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 [console_scripts]
 pyvcli_cli = pyvcli_cli:mainfunct
+pyvcli_fman = pyvcli_fman:mainfunct
 pyvcli_gethelp = pyvcli_gethelp:mainfunct
 pyvcli_hello = pyvcli_hello:mainfunct
+pyvcli_ihost = pyvcli_ihost:mainfunct
 pyvcli_qr = pyvcli_qr:mainfunct
-pyvcli_rget = pyvcli_rget:mainfunct
-pyvcli_rlist = pyvcli_rlist:mainfunct
-pyvcli_rput = pyvcli_rput:mainfunct
+pyvcli_replic = pyvcli_replic:mainfunct
+pyvcli_rman = pyvcli_rman:mainfunct
 pyvcli_uini = pyvcli_uini:mainfunct
 pyvcli_uman = pyvcli_uman:mainfunct
+pyvcli_ver = pyvcli_ver:mainfunct
 pyvcpanel = pyvcpanel:mainfunct
 pyvgenkey = pyvgenkey:mainfunct
 pyvgenkeys = pyvgenkeys:mainfunct
-pyvpuller = pyvpuller:mainfunct
 pyvreplic = pyvreplic:mainfunct
 pyvserv = pyvserv:mainfunct
 pyvservui = pyvservui:mainfunct
 pyvtally = pyvtally:mainfunct
```

### Comparing `pyvserv-1.0.3/pyvserver/pyvfunc.py` & `pyvserv-1.0.4/pyvserver/pyvfunc.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,21 @@
 #!/usr/bin/env python
 
-#from __future__ import print_function
-#from __future__ import absolute_import
-
 try:
     import pyotp
 except:
     pyotp = None
 
 import os, sys, getopt, signal, select, string
 import datetime,  time, stat, base64, uuid
 
 from pyvecc.Key import Key
 
-#from Crypto.Cipher import PKCS1_v1_5
-#from Crypto.PublicKey import RSA
 from Crypto import Random
 from Crypto.Cipher import AES
-#from Crypto.Hash import SHA
 #from Crypto.Hash import SHA512
 from Crypto.Hash import SHA256
 
 import pyvpacker
 
 from pyvcommon import support, pyservsup, pyclisup, pysyslog, pyvhash
 from pyvserver import pyvstate
@@ -33,22 +27,38 @@
     Server functions. The pyvstate calls routines from this module. The reason
     this is not made into a class is for speed. (Class was too big, and we are still
     adding functions for new commands.)
     This module executes the functions corresponding to keywords.
     The keyword is embedded into the function name.
 '''
 
-#chainfname = "initial"
+fields_help =  '''
+    stat fields2:
+       1.  ST_MODE Inode protection mode.
+       2.  ST_INO Inode number.
+       3.  ST_DEV Device inode resides on.
+       4.  ST_NLINK  Number of links to the inode.
+       5.  ST_UID User id of the owner.
+       6.  ST_GID Group id of the owner.
+       7.  ST_SIZE Size in bytes of a plain file.
+       8.  ST_ATIME Time of last access.
+       9.  ST_MTIME Time of last modification.
+       10. ST_CTIME Time of last metadata change.
+    '''
 repfname = "replic"
 
 OK = "OK"
 ERR = "ERR"
 
 #pgdebug = 0
 
+def _wr(strx):
+    ''' Wrap string with single quotes '''
+    return "'" + strx + "'"
+
 def _print_handles(self):
         ''' Debug helper '''
         open_file_handles = os.listdir('/proc/self/fd')
         print('open file handles: ' + ', '.join(map(str, open_file_handles)))
 
 def check_chain_path(self, strp):
 
@@ -111,45 +121,65 @@
 
     return dname4
 
 # ------------------------------------------------------------------------
 # State transition and action functions
 
 def get_exit_func(self, strx):
-    #print( "get_exit_func", strx)
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_exit_func()", strx)
+
+    # Clean up logouts
+    if self.resp.user:
+        pyservsup.SHARED_LOGINS.deldat(self.resp.user)
+
+    if pyservsup.globals.conf.pglog > 0:
+        stry = "Quit", _wr(self.resp.user), str(self.resp.client_address)
+        pysyslog.syslog(*stry)
+
+    # This instance will go away, but just to make sure
+    self.resp.user = ""
+
     self.resp.datahandler.putencode([OK, "Bye", self.name], self.resp.ekey)
-    #self.resp.datahandler.par.shutdown(socket.SHUT_RDWR)
 
     # Cancel **after** sending bye
     if self.resp.datahandler.tout:
         self.resp.datahandler.tout.cancel()
 
     return True
 
 # ------------------------------------------------------------------------
 # Also stop timeouts
 
 def get_tout_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_tout_func()", strx)
+
     tout = self.resp.datahandler.timeout
     if len(strx) > 1:
-        tout = int(strx[1])
-        self.resp.datahandler.timeout = tout
-        resp = [OK, "Timeout set to ", str(tout)],
+        try:
+            tout = int(strx[1])
+            self.resp.datahandler.timeout = tout
+            resp = [OK, "Timeout set to ", str(tout)],
+        except:
+            resp = [OK, "Timeout value must be an integer", strx[1]],
     else:
         resp = [OK, "Current timeout", str(self.resp.datahandler.timeout)],
 
     #if self.resp.datahandler.tout:
     #    self.resp.datahandler.tout.cancel()
 
     self.resp.datahandler.putencode(resp, self.resp.ekey)
 
-
 def get_mkdir_func(self, strx):
-    #print("make dir", strx[1])
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_mkdir_func()", strx)
 
     if len(strx) == 1:
         response = [ERR, "Must specify directory name.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     dname = contain_path(self, strx[1])
@@ -163,24 +193,89 @@
 
     if os.path.isdir(dname):
         response = [ERR, "Directory already exist.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     try:
-        response = [OK, "Made directory:", strx[1]]
         os.mkdir(dname)
+        response = [OK, "Made directory:", strx[1]]
     except:
         response = [ERR, "Cannot make directory.", strx[1]]
 
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
+def get_rmdir_func(self, strx):
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rmdir_func()", strx)
+
+    if len(strx) == 1:
+        response = [ERR, "Must specify directory name.", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    dname = contain_path(self, strx[1])
+
+    if not dname:
+        response = [ERR, "No Access to directory.", strx[1]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    #print("remove dir", dname)
+
+    if not os.path.isdir(dname):
+        response = [ERR, "Directory does not exist.", strx[1]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    try:
+        os.rmdir(dname)
+        response = [OK, "Deleted directory:", strx[1]]
+    except:
+        response = [ERR, "Cannot delete directory.", str(sys.exc_info()[1]), strx[1]]
+
+    self.resp.datahandler.putencode(response, self.resp.ekey)
+
+def get_throt_func(self, strx):
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_throt_func()", strx)
+
+    if len(strx) < 2:
+        if pyservsup.gl_throttle.getflag():
+            boolstr = "ON"
+        else:
+            boolstr = "OFF"
+        rrr = [OK, "Throttle is", boolstr]
+        self.resp.datahandler.putencode(rrr, self.resp.ekey)
+        return
+
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
+    if not int(ret[2]) & pyservsup.PERM_ADMIN:
+        rrr = [ERR, "Only admin can control throttle"]
+        self.resp.datahandler.putencode(rrr, self.resp.ekey)
+        return
+
+    boolx = pyservsup.str2bool(strx[1], True)
+    #print("boolx:", boolx, strx[1], hex(id(strx[1])))
+    if  boolx:
+        boolstr = "ON"
+        pyservsup.gl_throttle.setflag(True)
+    else:
+        boolstr = "OFF"
+        pyservsup.gl_throttle.setflag(False)
+
+    rrr = [OK, "Throttle turned %s" %  boolstr]
+    self.resp.datahandler.putencode(rrr, self.resp.ekey)
 
 def get_buff_func(self, strx):
-    #print("buffer str", strx[1])
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_buff_func()", strx)
 
     if len(strx) < 2:
         response = [ERR, "Must specify buffer size.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     # Set to an number that most short based (2 bytes) routines can handle
@@ -195,19 +290,22 @@
 
     self.buffsize = num
     response = [OK, "Buffer set to:", pyservsup.buffsize]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_lsd_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_lsd_func()", strx)
+
     sss = ""
     dname2 = self.resp.cwd + os.sep + self.resp.dir + os.sep
     dname2 = support.dirclean(dname2)
 
-    if pyservsup.globals.conf.pgdebug > 1:
+    if pyservsup.globals.conf.pgdebug > 3:
         print("get_lsd_func", dname2)
 
     response = [ OK, ]
 
     try:
         ddd = os.listdir(dname2)
         for aa in ddd:
@@ -222,14 +320,17 @@
         support.put_exception("lsd")
         response = [ERR, str(sys.exc_info()[1] ), strx[0]]
 
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_ls_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_ls_func()", strx)
+
     dname = ""; sss = ""
     if len(strx) < 2:
         strx.append(".")
     try:
         dname = support.unescape(strx[1]);
     except:
         pass
@@ -262,15 +363,15 @@
 
     #print("response", response)
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_fget_func(self, strx):
 
     if pyservsup.globals.conf.pgdebug > 1:
-        print("fget strx", strx)
+        print("get_fget_func()", strx)
 
     dname = ""
     if len(strx) == 1:
         response = [ERR, "Must specify file name.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
@@ -334,29 +435,26 @@
         #    break
 
         if ret == 0:
             break
         if blen == 0:
             break
 
-    response = [OK, "Sent File", strx[1]]
-    self.resp.datahandler.putencode(response, self.resp.ekey)
-
-    #ret = self.resp.datahandler.wfile.write(b" ")
-    #self.resp.datahandler.wfile.flush()
+    #if pyservsup.globals.conf.pglog > 1:
+    #    stry = "Server sent file: '" + dname + "' " + str(flen) + " bytes",
+    #    pysyslog.syslog(stry)
 
-    # Lof and set state to IDLE
-    xstr = "Sent file: '" + dname + \
-                "' " + str(flen) + " bytes"
+    response = [OK, "Server sent file", strx[1]]
+    self.resp.datahandler.putencode(response, self.resp.ekey)
 
-    #print(xstr)
-    pysyslog.syslog(xstr)
 
 def get_fput_func(self, strx):
-    #print("fput strx", strx)
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_fput_func()", strx)
 
     if len(strx) < 2:
         response = [ERR, "Must specify file name.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     dname = contain_path(self, strx[1])
@@ -411,117 +509,163 @@
         dstr = self.wr.unwrap_data(self.resp.ekey, data)
         #print("dstr[1]", dstr[1])
         if not dstr[1]:
             break
         fh.write(dstr[1])
 
     fh.close()
-    response = [OK, "File received.", strx[1]]
+    response = [OK, "Server received file.", strx[1]]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
+def get_pwd_func(self, strx):
 
-def get_ekey_func(self, strx):
-
-    oldkey = self.resp.ekey[:]
-    response = ERR ,  "Not implemented."
-    self.resp.datahandler.putencode(response, oldkey)
-    return
-
-    if len(strx) < 2:
-        self.resp.ekey = ""
-        response = OK ,  "Key reset (no encryption)"
-    else:
-        self.resp.ekey = strx[1]
-        response = OK ,  "Key Set"
-
-    # Encrypt reply to ekey with old the key
-    self.resp.datahandler.putencode(response, oldkey)
-
-def get_xkey_func(self, strx):
-    oldkey = self.resp.ekey[:]
-
-    oldkey = self.resp.ekey[:]
-    response = ERR ,  "Not implemented."
-    self.resp.datahandler.putencode(response, oldkey)
-    return
-
-    if len(strx) < 2:
-        self.resp.ekey = ""
-        response = OK ,  "Key reset (no encryption)"
-    else:
-        # Lookup if it is a named key:
-        retx = pyservsup.kauth(strx[1], "", 0)
-        if retx[0] == 1:
-            print( "key set", "'" + retx[1] + "'")
-            self.resp.ekey = retx[1]
-            response = OK,  "Key Set"
-        else:
-            response = ERR, strx[1], strx[0]
-
-    # Encrypt reply to xkey with old the key
-    self.resp.datahandler.putencode(response, oldkey)
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_pwd_func()", strx)
 
-def get_pwd_func(self, strx):
     dname2 = self.resp.dir
     dname2 = support.dirclean(dname2)
     if dname2 == "": dname2 = os.sep
     response = [OK,  dname2]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_rcheck_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rcheck_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify blockchain kind", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     if len(strx) < 3:
         response = [ERR, "Must specify link or sum", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
+    if int(ret[2]) & pyservsup.PERM_ADMIN != pyservsup.PERM_ADMIN:
+        response = [ERR, "Only admin can check integrity", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
     tmpname = os.path.join(pyservsup.globals.chaindir, strx[1])
     dname = check_chain_path(self, tmpname)
 
     if not dname:
         response = [ERR, "No Access to directory.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
     if not os.path.isdir(dname):
-        response = [ERR, "Directory does not exis.t", strx[1]]
+        response = [ERR, "Directory does not exist.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     core = twinchain.TwinChain(os.path.join(dname, pyservsup.chainfname + ".pydb"), 0)
 
     errx = False; cnt = -1; arrx = []
     sss = core.getdbsize()
-    for aa in range(sss-1, 0, -1):
-        if  strx[2] == "sum":
+    if  strx[2] == "sum":
+        for aa in range(sss-1, -1, -1):
             ppp = core.checkdata(aa)
             if not ppp:
                 arrx.append(aa)
-        elif strx[2] == "link":
-            ppp = core.linkintegrity(aa)
-            if not ppp:
+    elif strx[2] == "link":
+        for aa in range(sss-1, -1, -1):
+            ppp2 = core.linkintegrity(aa)
+            if not ppp2:
                 arrx.append(aa)
-        else:
-            response = [ERR, "One of 'link' or 'sum' is required.", strx[0]]
+    else:
+        response = [ERR, "One of 'link' or 'sum' is required.", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    if len(arrx):
+        response = [ERR,  arrx, len(arrx), "errors", strx[2], sss, "total"]
+    else:
+        response = [OK,  "No errors.", strx[2], sss, "total"]
+    self.resp.datahandler.putencode(response, self.resp.ekey)
+
+def get_rtest_func(self, strx):
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rtest_func()", strx[:4])
+
+    if len(strx) < 2:
+        response = [ERR, "Must specify blockchain kind", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    if len(strx) < 3:
+        response = [ERR, "Must specify link or sum", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    if len(strx) < 4:
+        response = [ERR, "Must specify record id or ids", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    tmpname = os.path.join(pyservsup.globals.chaindir, strx[1])
+    dname = check_chain_path(self, tmpname)
+
+    if not dname:
+        response = [ERR, "No Access to directory.", strx[1]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+    if not os.path.isdir(dname):
+        response = [ERR, "Directory does not exis.t", strx[1]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    core = twinchain.TwinChain(os.path.join(dname, pyservsup.chainfname + ".pydb"), 0)
+
+    if  strx[2] == "sum":
+        funcx = core.checkdata
+    elif strx[2] == "link":
+        funcx = core.linkintegrity
+    else:
+        response = [ERR, "One of 'link' or 'sum' is required.", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    errx = False; cnt = -1; arrx = []
+    sss = len(strx[3:])
+    for aa in strx[3:]:
+        #print("test:", aa)
+        try:
+            ddd = core.get_payoffs_bykey(aa)
+        except:
+            pass
+        if len(ddd) == 0:
+            response = [ERR, "Data not found.", aa,]
             self.resp.datahandler.putencode(response, self.resp.ekey)
             return
+        if self.pgdebug > 4:
+            try:
+                rec = core.get_rec(ddd[0])
+                print("rec:", rec)
+            except:
+                print("exc: get_header", sys.exc_info())
+                raise
+        ppp = funcx(ddd[0])
+        if not ppp:
+            arrx.append(aa)
 
     if len(arrx):
         response = [ERR,  arrx, len(arrx), "errors", strx[2]]
     else:
-        response = [OK,  "No errors.", strx[2]]
+        response = [OK,  "No errors.", strx[2], sss, "records checked."]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
-
 def get_rsize_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rsize_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify blockchain kind.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     tmpname = os.path.join(pyservsup.globals.chaindir, strx[1])
     dname = check_chain_path(self, tmpname)
@@ -543,14 +687,17 @@
 
     response = [OK,  dbsize, "records"]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 
 def get_rcount_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rcount_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify blockchain kind.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     if len(strx) < 3:
         response = [ERR, "Must specify starting point.", strx[0]]
@@ -590,25 +737,28 @@
     dbsize = core.getdbsize()
     for aa in range(dbsize - 1, -1, -1):
         rec = core.get_header(aa)
         ddd = pyservsup.uuid2timestamp(uuid.UUID(rec))
         #ttt = pyservsup.uuid2date(uuid.UUID(rec))
         #print(ddd, ttt)
 
-        if ddd > strx[2] and ddd < strx[3]:
+        if ddd >= strx[2] and ddd <= strx[3]:
             rcnt += 1
 
     if self.pgdebug > 2:
         print("rcnt", "total: %d records" % dbsize, "got: %d records" % rcnt)
 
     response = [OK,  rcnt, "records"]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_rlist_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rlisr_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify blockchain kind.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     if len(strx) < 3:
         response = [ERR, "Must specify starting point.", strx[0]]
@@ -656,23 +806,27 @@
         if len(arr) > 100:
             break
 
     #print("rec", "%d records" % dbsize, "got: %d" % len(arr))
 
     # Prevent overload from
     if len(arr) > 100:
-        response = [ERR,  "Too many records, narrow date range."]
+        # Return error and some data
+        response = [ERR,  "Too many records, narrow date range.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     response = [OK,  arr]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_rhave_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rhave_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify blockchain kind.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     if len(strx) < 3:
         response = [ERR, "Must specify data header.", strx[0]]
@@ -683,41 +837,113 @@
     dname = check_chain_path(self, tmpname)
 
     if not dname:
         response = [ERR, "No Access to directory.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
-    #print("dname", dname)
+    if pyservsup.globals.conf.pgdebug > 3:
+        print("dname", dname)
+
     if not os.path.isdir(dname):
         response = [ERR, "Blockchain 'kind' directory does not exist.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
-    if pyservsup.globals.conf.pgdebug > 2:
-        print("rget", strx[1], strx[2])
-
     core = twinchain.TwinChain(os.path.join(dname, pyservsup.chainfname + ".pydb"), 0)
     #print("db op2 %.3f" % ((time.time() - ttt) * 1000) )
     ddd = []
     try:
-        ddd = core.get_payoffs_bykey(strx[2])
+        # use the faster hash based function
+        ddd = core.retrieve(strx[2])
     except:
         pass
     if len(ddd) == 0:
         response = [ERR, "Data not found.", strx[2],]
     else:
         response = [OK, "Data found", strx[2],]
 
     #_print_handles(self)
+    self.resp.datahandler.putencode(response, self.resp.ekey)
+
+def get_rabs_func(self, strx):
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rabs_func()", strx)
+
+    if len(strx) < 2:
+        response = [ERR, "Must specify blockchain kind.", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    if len(strx) < 3:
+        response = [ERR, "Must specify absolute position.", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    tmpname = os.path.join(pyservsup.globals.chaindir, strx[1])
+    dname = check_chain_path(self, tmpname)
+
+    if not dname:
+        response = [ERR, "No Access to directory.", strx[1]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
 
+    #print("dname", dname)
+    if not os.path.isdir(dname):
+        response = [ERR, "Blockchain 'kind' directory does not exist.", strx[1]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    if pyservsup.globals.conf.pgdebug > 2:
+        print("rabs", strx[1], strx[2])
+
+    core = twinchain.TwinChain(os.path.join(dname, pyservsup.chainfname + ".pydb"), 0)
+    #print("db op2 %.3f" % ((time.time() - ttt) * 1000) )
+    datax = []
+    dbsize = core.getdbsize()
+    for aa in strx[2:]:
+        aa = int(aa)
+        #convert to offsets
+        if aa < 0:
+            aa = dbsize + aa
+        #print("aa", aa)
+        if not core.checkdata(aa):
+            data = [ERR, "Invalid Record, bad checksum.", aa]
+            self.resp.datahandler.putencode(data, self.resp.ekey)
+            return
+
+        if not core.linkintegrity(aa):
+            data = [ERR, "Invalid Record, link damaged.", aa]
+            self.resp.datahandler.putencode(data, self.resp.ekey)
+            return
+        try:
+            data = core.get_rec(aa)
+        except:
+            data = ""
+            print(str(sys.exc_info()))
+
+        if self.pgdebug > 4:
+            print("rec data", data)
+        if not data:
+            response = [ERR, "Record not found.", aa,]
+            self.resp.datahandler.putencode(response, self.resp.ekey)
+            return
+
+        datax.append(data)
+        #print("data:", data)
+
+    response = [OK, len(datax), "records", datax]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_rget_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rget_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify blockchain kind.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     if len(strx) < 3:
         response = [ERR, "Must specify data header.", strx[0]]
@@ -740,18 +966,33 @@
 
     if pyservsup.globals.conf.pgdebug > 2:
         print("rget", strx[1], strx[2])
 
     core = twinchain.TwinChain(os.path.join(dname, pyservsup.chainfname + ".pydb"), 0)
     #print("db op2 %.3f" % ((time.time() - ttt) * 1000) )
     datax = []
+    if type(strx[2]) == type(""):
+        strx[2] = strx[2].split()
     for aa in strx[2]:
+        #print("aa", aa)
+        # Validate uuid
+        try:
+            uuidx = uuid.UUID(aa)
+        except:
+            print("getting UUID", sys.exc_info())
+            #response = [ERR, "Header must be a real UUID.", strx[2],]
+            #self.resp.datahandler.putencode(response, self.resp.ekey)
+            #return
+            continue
+
         data = []; ddd = []
         try:
             ddd = core.get_payoffs_bykey(aa)
+            if pyservsup.globals.conf.pgdebug > 2:
+                    print("ddd", ddd)
         except:
             pass
         if len(ddd) == 0:
             response = [ERR, "Data not found.", aa,]
             self.resp.datahandler.putencode(response, self.resp.ekey)
             return
         try:
@@ -765,39 +1006,45 @@
             return
 
         if self.pgdebug > 2:
             print("got rechead", rechead)
 
         if not core.checkdata(ddd[0]):
             data = [ERR, "Invalid Record, bad checksum.", aa]
-            self.resp.datahandler.putencode(response, self.resp.ekey)
+            self.resp.datahandler.putencode(data, self.resp.ekey)
             return
 
         if not core.linkintegrity(ddd[0]):
             data = [ERR, "Invalid Record, link damaged.", aa]
-            self.resp.datahandler.putencode(response, self.resp.ekey)
+            self.resp.datahandler.putencode(data, self.resp.ekey)
             return
-        else:
-            try:
-                data = core.get_payload(ddd[0])
-            except:
-                data = "error on get data.", str(sys.exc_info())
-            if self.pgdebug > 4:
-                print("rec data", data)
+
+        try:
+            data = core.get_rec(ddd[0])
+        except:
+            data = ""
+            print(str(sys.exc_info()))
+
+        if self.pgdebug > 4:
+            print("rec data", data)
         if not data:
             response = [ERR, "Record not found.", aa,]
             self.resp.datahandler.putencode(response, self.resp.ekey)
             return
+
         datax.append(data)
 
-    response = [OK, datax, datax, len(datax), "records"]
+    response = [OK, len(datax), "records", datax,]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_rput_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_rput_func()")
+
     if len(strx) < 3:
         response = [ERR, "Must specify blockchain kind and data.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     #print("strx[1]", strx[1])
     #print('curr', self.resp.dir)
@@ -841,30 +1088,20 @@
     savecore = twinchain.TwinChain(cfname)
     #print("db op2 %.3f" % ((time.time() - ttt) * 1000) )
 
     #print("Got:", strx[2])
 
     # Do we have it already?:
     #ttt = time.time()
-    #rethas = savecore.get_data_bykey(strx[2]['header'])
-    #print("db get data  %.3f" % ((time.time() - ttt) * 1000) )
-    #if rethas:
-    #    if self.pgdebug > 1:
-    #        print("Duplicate block, rethas", rethas[0][0])
-    #    response = [ERR, "Duplicate block, not saved.", strx[0]]
-    #    self.resp.datahandler.putencode(response, self.resp.ekey)
-    #    return
-
-    #ttt = time.time()
     retoffs = savecore.get_payoffs_bykey(strx[2]['header'])
     #print("db get offs  %.3f" % ((time.time() - ttt) * 1000) )
     if retoffs:
         if self.pgdebug > 2:
-            print("Duplicate block, retoffs", retoffs)
-        response = [ERR, "Duplicate block, not saved.", strx[2]['header']]
+            print("Duplicate block, retoffs", retoffs[0])
+        response = [ERR, "Duplicate block, not saved.", strx[2]['header'], retoffs[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     undec = self.pb.encode_data("", strx[2])
 
     if  self.pgdebug > 5:
         print("Save_data header:", strx[2]["header"])
@@ -879,22 +1116,28 @@
         del savecore
         print("exc save_data", sys.exc_info()[1])
         response = [ERR, "Cannot save record.", str(sys.exc_info()[1]) ]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
     del savecore
 
-    # if it no replicated, replicate
+    # if it is not replicated already, add replicate request
     if not strx[2]["Replicated"]:
         # Prepare data. Do strings so it can be re-written in place
-        rrr = {'count1': "00000", 'count2' : "00000",
-                        'count3' : "00000",  'header' : strx[2]['header'],
-                            'now' : strx[2]['now'],}
-        if self.pgdebug > 2:
-            print("replic", rrr)
+        rrr = {
+                # Sun 14.Apr.2024 removed counts, shifted to state data
+                #'count1': "00000", 'count2' : "00000", 'count3' : "00000",
+                'header' : strx[2]['header'],
+                'now' : strx[2]['now'], 'iso' : strx[2]['iso'],
+                'stamp' : strx[2]['stamp'],
+                "processed" : "00000",
+                }
+
+        if self.pgdebug > 3:
+            print("replic req", rrr)
 
         undec2 = self.pb.encode_data("", rrr)
         frname = os.path.join(dname, repfname + ".pydb")
         #print("Saving at", frname)
         repcore = twincore.TwinCore(frname, 0)
         #if self.pgdebug > 5:
         #print("repl save_data", strx[2]["Header"], undec2)
@@ -906,69 +1149,94 @@
             response = [ERR,  "Cannot save replicator.",  str(sys.exc_info()[1]) ]
             support.put_exception("save_data")
             self.resp.datahandler.putencode(response, self.resp.ekey)
             return
 
         del repcore
     else:
-        if self.pgdebug > 2:
+        if self.pgdebug > 3:
             print("Not replicating", strx[2]['header'])
         pass
 
         #print("db op3 %.3f" % ((time.time() - ttt) * 1000) )
         #dbsize = repcore.getdbsize()
         #print("replicator %d total records" % dbsize)
 
     response = [OK,  "Blockchain data added.",  strx[2]['header']]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
     #open_file_handles = os.listdir('/proc/self/fd')
     #print('open file handles: ' + ', '.join(map(str, open_file_handles)))
 
-    pysyslog.syslog("BCD %s" % strx[2]['header'])
+    if pyservsup.globals.conf.pglog > 1:
+        stry = "Block Chain Data %s" % strx[2]['header'], \
+                _wr(self.resp.user), str(self.resp.client_address)
+        pysyslog.syslog(*stry)
 
 
 def get_ihost_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_ihost_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify operation (add / remove).", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
-    if len(strx) < 3:
-        response = [ERR, "Must specify host/port.", strx[0]]
-        self.resp.datahandler.putencode(response, self.resp.ekey)
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
+    if not int(ret[2]) & pyservsup.PERM_ADMIN:
+        rrr = [ERR, "Only admin can control / view ihosts"]
+        self.resp.datahandler.putencode(rrr, self.resp.ekey)
         return
 
-    #print(strx)
-    ihname = "ihosts.pydb"
+    if strx[1] != 'list':
+        if len(strx) < 3:
+            response = [ERR, "Must specify host:port.", strx[0]]
+            self.resp.datahandler.putencode(response, self.resp.ekey)
+            return
+
+        if strx[2].find(":") < 0:
+            response = [ERR, "Entry must be in host:port format.", strx[2]]
+            self.resp.datahandler.putencode(response, self.resp.ekey)
+            return
+
+    ihname = os.path.realpath("ihosts.pydb")
+    if self.pgdebug > 2:
+        print("ihost:", ihname)
     repcore = twincore.TwinCore(ihname)
+    #repcore.pgdebug = 10
 
     if strx[1] == 'add':
         ddd = self.pb.encode_data("", strx[2])
         rec = repcore.retrieve(strx[2])
+        if self.pgdebug > 9:
+            print("rec:", rec)
         if rec:
             if rec[0][0].decode() == strx[2]:
                 #print("Identical", rec[0][0])
-                response = [ERR, "This entry is already in the list.", strx[2]]
+                response = [ERR, "Duplicate entry.", strx[2]]
                 self.resp.datahandler.putencode(response, self.resp.ekey)
                 return
-        ret = repcore.save_data(strx[2], ddd, True)
-        response = [OK, "Added replication host/port.", strx[2]]
+        ret = repcore.save_data(strx[2], ddd)
+        if self.pgdebug > 8:
+            print("repcore save:", ret, ddd)
+        response = [OK, "Added replication host:port.", strx[2]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
 
     elif strx[1] == 'del':
         rec = repcore.retrieve(strx[2])
         if not rec:
-            response = [ERR, "This entry does not exist.", strx[2]]
+            response = [ERR, "This entry is not in the list.", strx[2]]
             self.resp.datahandler.putencode(response, self.resp.ekey)
             return
+        if self.pgdebug > 4:
+            print("delete ihost rec:", strx[2])
         ret = repcore.del_rec_bykey(strx[2])
-        #print("del ret", ret, strx[2])
-        response = [OK, "Deleted replication host/port.", strx[2]]
+        response = [OK, "Deleted replication host:port.", strx[2]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
 
     elif strx[1] == 'list':
         arr = []
         for aa in range(repcore.getdbsize()-1, -1, -1):
             ddd = repcore.get_rec(aa)
             if ddd:
@@ -976,35 +1244,19 @@
         #print("got recs", arr)
         response = [OK,  arr, strx[2]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
     else:
         response = [ERR, "Operation must be 'add' or 'del or list'.", strx[2]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
 
-
-def get_ihave_func(self, strx):
-
-    if len(strx) < 2:
-        response = [ERR, "Must specify blockchain kind.", strx[0]]
-        self.resp.datahandler.putencode(response, self.resp.ekey)
-        return
-
-    if len(strx) < 3:
-        response = [ERR, "Must specify record header.", strx[0]]
-        self.resp.datahandler.putencode(response, self.resp.ekey)
-        return
-
-    uuid = uuid.UUID(strx[2])
-
-    print("ihave", strx[1], strx[2])
-    response = [OK,  "Ihave processed", strx[0], ]
-    self.resp.datahandler.putencode(response, self.resp.ekey)
-
 def get_cd_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_cd_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Directory name cannot be empty.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     dname = contain_path(self, strx[1])
 
@@ -1025,14 +1277,17 @@
     except:
         support.put_exception("cd")
         response = [ERR, "Must specify directory name.", strx[0]]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_del_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_del_func()", strx)
+
     if len(strx) == 1:
         response = [ERR, "Must specify file name to delete.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     try:
         dname = contain_path(self, strx[1])
@@ -1055,47 +1310,45 @@
         support.put_exception("del")
         response = [ERR, "Must specify file name to delete.", strx[0]]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 # ------------------------------------------------------------------------
 
 def get_ver_func(self, strx):
+
     if pyservsup.globals.conf.pgdebug > 1:
         print( "get_ver_func()", strx)
 
     res = [OK, "%s" % pyservsup.version,
-                        "%s" % pyservsup.globals.siteid]
+                        "%s" % pyservsup.globals.siteid, self.name]
 
-    if pyservsup.globals.conf.pgdebug > 2:
+    if pyservsup.globals.conf.pgdebug > 4:
         print( "get_ver_func->output", res)
 
     self.resp.datahandler.putencode(res, self.resp.ekey)
 
-
 def get_id_func(self, strx):
     if pyservsup.globals.conf.pgdebug > 1:
         print( "get_id_func()", strx)
-    res = []
-    res.append(OK);   res.append("%s" % pyservsup.globals.siteid)
-    res.append("ID")
-    if pyservsup.globals.conf.pgdebug > 2:
-        print( "get_ver_func->output", res)
+
+    res = [OK, str(pyservsup.globals.siteid), str(self.name)]
     self.resp.datahandler.putencode(res, self.resp.ekey)
 
 #@support.timeit
 def get_hello_func(self, strx):
     if pyservsup.globals.conf.pgdebug > 3:
         print( "get_hello_func()", strx)
     strres = [OK, "Hello", str(pyservsup.globals.siteid), self.name]
-    if pyservsup.globals.conf.pgdebug > 4:
-        print( "get_hello_func->output", "'" + str(strres) + "'")
     self.resp.datahandler.putencode(strres, self.resp.ekey)
 
 def get_stat_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_stat_func()", strx)
+
     if len(strx) < 2:
         response = [ERR, "Must specify file name.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     fname = ""; aaa = " "
     #print("stat_func", strx[1])
@@ -1120,41 +1373,65 @@
         response = [ERR, str(sys.exc_info()[1]) , strx[0]]
     except:
         response = [ERR, "Must specify file name.", strx[0]]
         #print( sys.exc_info())
 
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
-def get_logout_func(self, strx):
+def get_lout_func(self, strx):
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_lout_func()", strx)
 
     if not self.resp.user:
         response = [ERR, "Not logged in.", strx[0], ]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
-    olduser = self.resp.user
+    if pyservsup.globals.conf.pglog > 0:
+        stry = "Logout", _wr(resp.user), \
+                str(self.resp.client_address)
+        pysyslog.syslog(*stry)
+
+    if self.pgdebug > 3:
+        print("logout", self.resp.user)
+
+    if resp.user:
+        pyservsup.SHARED_LOGINS.deldat(resp.user)
+
     self.resp.user = ""
-    #print("logout", self.resp.user)
 
     response = [OK, "Logged out.", olduser, ]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 #@support.timeit
 def get_user_func(self, strx):
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_user_func()", strx)
+
     if len(strx) < 2:
-        self.resp.datahandler.putencode(
-                [ERR, "Must specify user name.", strx[0]], self.resp.ekey)
+        resp = [ERR, "Must specify user name.", strx[0]]
+        self.resp.datahandler.putencode(resp, self.resp.ekey)
+        return
+
+    if self.resp.user:
+        self.resp.datahandler.putencode([ERR, "Already logged in"], self.resp.ekey)
         return
-    self.resp.user = strx[1]
-    self.resp.datahandler.putencode([OK, "Send pass ..."], self.resp.ekey)
+
+    self.resp.preuser = strx[1]
+    self.resp.datahandler.putencode([OK, "Send pass for", strx[1]], self.resp.ekey)
 
 # ------------------------------------------------------------------------
 
 def get_sess_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_sess_func()")
+
     if len(strx) < 4:
         response = [ERR, "Not enough arguments for session."]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     #sss = SHA512.new(); sss.update(bytes(strx[3], "cp437"))
     sss = SHA256.new(); sss.update(strx[3].encode())
@@ -1171,15 +1448,15 @@
     message2 = self.priv_cipher.decrypt(strx[3])
 
     #print("sess_key", message2[:24])
 
     # Decoded OK?
     ttt = SHA256.new(); ttt.update(message2.encode())
 
-    if pyservsup.globals.conf.pgdebug > 4:
+    if pyservsup.globals.conf.pgdebug > 6:
         print("Hash1:", strx[1])
         print("Hash2:", ttt.hexdigest())
 
     if ttt.hexdigest() != strx[1]:
         self.resp.datahandler.putencode(\
             [ERR, "session key damaged on decoding."], self.resp.ekey, strx[0])
         return
@@ -1191,27 +1468,34 @@
         support.shortdump("session key:", self.resp.ekey.encode() )
 
 # ------------------------------------------------------------------------
 
 #@support.timeit
 def get_akey_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_akey_func()", strx)
+
     ttt = time.time()
 
     if pyservsup.globals.conf.pgdebug > 4:
         print("get_akey_func() called")
 
     ddd = os.path.abspath("keys")
     ppp = os.path.abspath("private")
 
     try:
         self.keyfroot = pyservsup.pickkey(ddd)
     except:
-        print("No keys generated yet.", sys.exc_info()[1])
-        support.put_exception("no keys yet")
+        if self.verbose:
+            print("No keys generated yet.", sys.exc_info()[1])
+
+        if self.pgdebug > 2:
+            support.put_exception("no keys yet")
+
         rrr = [ERR, "No keys yet. Run keygen.", strx[0]]
         self.resp.datahandler.putencode(rrr, self.resp.ekey)
         return
 
     if pyservsup.globals.conf.pgdebug > 4:
        print("self.keyfroot", self.keyfroot)
 
@@ -1222,15 +1506,15 @@
 
     try:
         # Do public import
         fp = open(ddd + os.sep + self.keyfroot + ".pub", "rt")
         self.keyx = fp.read()
         fp.close()
 
-        if pyservsup.globals.conf.pgdebug > 4:
+        if pyservsup.globals.conf.pgdebug > 7:
             print("Key read: \n'" + self.keyx + "'\n")
     except:
         print("Cannot read key:", self.keyfroot, sys.exc_info()[1])
         support.put_exception("read key")
         rrr = [ERR, "cannot open keyfile.", strx[0]]
         self.resp.datahandler.putencode(rrr, self.resp.ekey)
 
@@ -1285,147 +1569,189 @@
     # Deliver the answer in two parts:
     rrr = [OK, "%s" % hh.hexdigest(), self.keyx]
     self.resp.datahandler.putencode(rrr, self.resp.ekey)
 
 #@support.timeit
 def get_pass_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_pass_func()")
+
     ret = "";  retval = True
 
     #ttt = time.time()
 
     if len(strx) < 2:
         self.resp.datahandler.putencode(
                 [ERR, "Must specify pass.", strx[0]], self.resp.ekey)
         return retval
+
     # Make sure there is a trace of the attempt
-    stry = "Logon  '" + self.resp.user + "' " + \
+    if pyservsup.globals.conf.pglog > 0:
+        stry = "Attempted login", _wr(self.resp.preuser), \
                 str(self.resp.client_address)
-    pysyslog.syslog(stry)
+        pysyslog.syslog(*stry)
 
     #print("pass 1 %.3f" % ((time.time() - ttt) * 1000) )
 
-    ret = pyservsup.passwd.perms(self.resp.user)
+    ret = pyservsup.gl_passwd.perms(self.resp.preuser)
     #print("pass 2 %.3f" % ((time.time() - ttt) * 1000) )
 
     if int(ret[2]) & pyservsup.PERM_DIS:
         rrr = [ERR, "this user is temporarily disabled", strx[1]]
         self.resp.datahandler.putencode(rrr, self.resp.ekey)
         return retval
 
-    xret = pyservsup.passwd.auth(self.resp.user, strx[1], 0, pyservsup.USER_AUTH)
+    xret = pyservsup.gl_passwd.auth(self.resp.preuser, strx[1], 0, pyservsup.USER_AUTH)
     #print("pass 3 %.3f" % ((time.time() - ttt) * 1000) )
 
     rrr = []
     if xret[0] == 3:
-        stry = "No such user  '" + self.resp.user + "' " + \
+        if pyservsup.globals.conf.pglog > 0:
+            stry = "No such user", _wr(self.resp.preuser), \
                 str(self.resp.client_address)
-        pysyslog.syslog(stry)
-        rrr = [ERR, "No such user.", self.resp.user]
+            pysyslog.syslog(*stry)
+        rrr = [ERR, "No such user.", self.resp.preuser]
     elif xret[0] == 1:
-        stry = "Successful logon '" + self.resp.user + "' " + \
-                            str(self.resp.client_address)
-        pysyslog.syslog(stry)
 
         if self.pgdebug > 3:
-            print("Authenticated", self.resp.user)
+            print("Authenticated", self.resp.preuser)
 
-        userdir2 = pyservsup.globals.paydir + os.sep + self.resp.user
+        userdir2 = pyservsup.globals.paydir + os.sep + self.resp.preuser
         self.userdir = check_payload_path(self, userdir2)
         #print("Contained",  self.userdir)
         if not self.userdir:
             rrr = [ERR, "No access to this path", userdir2]
             self.resp.datahandler.putencode(rrr, self.resp.ekey)
             return
 
         if not os.path.isdir(self.userdir):
             os.mkdir(self.userdir)
         self.resp.cwd = self.userdir
+
+        if pyservsup.globals.conf.pglog > 0:
+            stry = "Successful login", _wr(self.resp.preuser),  \
+                            str(self.resp.client_address)
+            pysyslog.syslog(*stry)
+
+        # Commit  user
+        self.resp.user = self.resp.preuser
+        self.resp.preuser = ""
+
+        # Anounce it to global stats
+        if self.resp.user:
+            logttt = time.time()
+            pyservsup.SHARED_LOGINS.setdat(self.resp.user, logttt)
+
         rrr = [OK,  "Authenticated.", self.resp.user]
         retval = False
     else:
-        stry = "Error on logon  '" + self.resp.user + "' " + \
+        if pyservsup.globals.conf.pglog > 0:
+            stry = "Error on login", _wr(self.resp.preuser), \
                 str(self.resp.client_address)
-        pysyslog.syslog(stry)
+            pysyslog.syslog(*stry)
         rrr = [ERR,  xret[1], strx[0]]
 
     self.resp.datahandler.putencode(rrr, self.resp.ekey)
     return retval
 
 def get_chpass_func(self, strx):
 
-    if len(strx) < 1:
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_chpass_func()")
+
+    if len(strx) < 2:
+        response = [ERR, "Must specify user to change.", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return
+
+    if len(strx) < 3:
         response = [ERR, "Must specify old_pass.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
-    if len(strx) < 2:
+    if len(strx) < 4:
         response = [ERR, "Must specify new_pass.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
-
-    #print("chpass", strx[1], strx[2])
-
+    #print("chpass", strx)
     # Make sure there is a trace of the attempt
-    stry = "chpass  '" + self.resp.user + "' " + str(self.resp.client_address)
-    pysyslog.syslog(stry)
+    if pyservsup.globals.conf.pglog > 1:
+        stry = "chpass", _wr(self.resp.user), \
+                 str(self.resp.client_address)
+        pysyslog.syslog(*stry)
 
-    # Authenticate
-    xret = pyservsup.passwd.auth(self.resp.user, strx[1], 0, pyservsup.USER_AUTH)
-    if xret[0] != 1:
-        response = [ERR, "Old pass must match", strx[0]]
-        self.resp.datahandler.putencode(response, self.resp.ekey )
-        return
+    # Are we allowed to change pass?
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
+    if int(ret[2]) & pyservsup.PERM_ADMIN != pyservsup.PERM_ADMIN:
+        # Authenticate
+        if strx[1] !=  self.resp.user:
+            response = [ERR, "Non admins can only change their own password.", strx[0]]
+            self.resp.datahandler.putencode(response, self.resp.ekey )
+            return
 
+        xret = pyservsup.gl_passwd.auth(strx[1], strx[2], 0, pyservsup.USER_AUTH)
+        if xret[0] != 1:
+            response = [ERR, "Old pass must match", strx[0]]
+            self.resp.datahandler.putencode(response, self.resp.ekey )
+            return
     # Change
-    xret = pyservsup.passwd.auth(self.resp.user, strx[2], 0, pyservsup.USER_CHPASS)
+    xret = pyservsup.gl_passwd.auth(strx[1], strx[3], 0, pyservsup.USER_CHPASS)
 
     ret = ""
     if xret[0] == 5:
-        stry = "Pass changed '" + self.resp.user + "' " + \
+        if pyservsup.globals.conf.pglog > 1:
+            stry = "Pass changed", _wr(resp.user), \
                 str(self.resp.client_address)
-        pysyslog.syslog(stry)
-        ret = [OK, "Pass changed", self.resp.user]
+            pysyslog.syslog(*stry)
+        ret = [OK, "Pass changed", strx[1]]
     elif xret[0] == 3:
-        stry = "No such user  '" + self.resp.user + "' " + \
+        if pyservsup.globals.conf.pglog > 1:
+            stry = "No such user", _wr(strx[1]),  \
                 str(self.resp.client_address)
-        pysyslog.syslog(stry)
-        ret = [ERR, "No such user.", self.resp.user]
+            pysyslog.syslog(*stry)
+        ret = [ERR, "No such user.", strx[1]]
     elif xret[0] == 1:
-        pysyslog.syslog("Successful logon", self.resp.user,
-                                            str(self.resp.client_address))
+        if pyservsup.globals.conf.pglog > 1:
+            stry = "Successful login", strx[1], \
+                           str(self.resp.client_address)
+            pysyslog.syslog(*stry)
         ret = ["OK ", self.resp.user, " Authenticated."]
         retval = False
     else:
-        stry = "Error on logon  '" + self.resp.user + "' " + \
-                str(self.resp.client_address)
-        pysyslog.syslog(stry)
+        if pyservsup.globals.conf.pglog > 1:
+            stry = "Error on login", _wr(strx[1]), \
+                    str(self.resp.client_address)
+            pysyslog.syslog(*stry)
         ret = [ERR, xret[1], strx[0]]
 
     self.resp.datahandler.putencode(ret, self.resp.ekey)
     return
 
 def get_uadd_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_uadd_func()", strx)
+
     if len(strx) < 3:
         response = ERR, "Must specify user name and pass.", strx[0]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return retval
 
     #print("uadd", strx)
 
     # Are we allowed to add users?
-    ret = pyservsup.passwd.perms(self.resp.user)
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
     if int(ret[2]) & pyservsup.PERM_ADMIN != pyservsup.PERM_ADMIN:
         response = [ERR, "Only admin can add/delete users", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     # Add this user if not exist
-    ret = pyservsup.passwd.auth(strx[1], strx[2], 0, pyservsup.USER_ADD)
+    ret = pyservsup.gl_passwd.auth(strx[1], strx[2], 0, pyservsup.USER_ADD)
     if ret[0] <= 0:
         response = [ERR, ret[1], strx[1]]
     elif ret[0] == 1:
         response = [ERR, "User already exists.", strx[1]]
     elif ret[0] == 2:
         response = ["OK", "Added user.", strx[1]]
     else:
@@ -1433,45 +1759,51 @@
 
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 # Add Admin
 
 def get_aadd_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_aadd_func()", strx)
+
     # Are we allowed to add users?
-    ret = pyservsup.passwd.perms(self.resp.user)
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
     if int(ret[2]) & pyservsup.PERM_ADMIN != pyservsup.PERM_ADMIN:
         response = [ERR, "only admin can add/delete users.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return retval
 
     if len(strx) < 3:
         response = [ERR, "must specify user name and pass.", strx[1]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     # Add this admin in not exist
-    ret = pyservsup.passwd.auth(strx[1], strx[2], pyservsup.PERM_ADMIN, pyservsup.USER_ADD)
+    ret = pyservsup.gl_passwd.auth(strx[1], strx[2], pyservsup.PERM_ADMIN, pyservsup.USER_ADD)
     if ret[0] <= 0:
         response = [ERR, ret[1], strx[0]]
     elif ret[0] == 1:
         response = ERR, ["Admin already exists.", strx[1]]
     elif ret[0] == 2:
         response = [OK, "Added admin.", strx[1]]
     else:
         response = [ERR, ret[1], strx[1]]
 
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def get_uena_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_uena_func()", strx)
+
     retval = 0
 
     # Are we allowed to add users?
-    ret = pyservsup.passwd.perms(self.resp.user)
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
     if int(ret[2]) & pyservsup.PERM_ADMIN != pyservsup.PERM_ADMIN:
         response = ERR, "only admin can modify users.", strx[0]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return retval
 
     if len(strx) < 2:
         response = ERR, "Must specify user name and flag.", strx[0]
@@ -1479,132 +1811,136 @@
         return retval
 
     if strx[2] == "enable":
         mode = pyservsup.PERM_DIS  | pyservsup.RESET_MODE
     elif strx[2] == "disable":
         mode = pyservsup.PERM_DIS
     else:
-        response = [ERR, "Must specify 'enable' or 'disable'.", strx[0]]
+        response = [ERR, "Must specify 'enable' or 'disable'", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return retval
 
     # Add this user in not exist
-    ret = pyservsup.passwd.auth(strx[1], strx[2], mode, pyservsup.USER_CHMOD)
+    ret = pyservsup.gl_passwd.auth(strx[1], strx[2], mode, pyservsup.USER_CHMOD)
 
     if ret[0] == 0:
         response = ERR, ret[1], strx[1]
     elif ret[0] == 8:
         response = OK,  strx[1], strx[2] + "d"
     else:
         response = ERR, ret[1], strx[1]
 
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 
+def get_ulist_func(self, strx):
+
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_ulist_func()", strx)
+
+    retval = 0
+
+    # Are we allowed to add users?
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
+    if int(ret[2]) & pyservsup.PERM_ADMIN != pyservsup.PERM_ADMIN:
+        response = ERR, "only admin can view users.", strx[0]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return retval
+
+    if len(strx) < 2:
+        response = ERR, "Must specify user / admin flag", strx[0]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return retval
+
+    if strx[1] == "user":
+        mode = pyservsup.PERM_NONE
+    elif strx[1] == "admin":
+        mode = pyservsup.PERM_ADMIN
+    elif strx[1] == "initial":
+        mode = pyservsup.PERM_INI
+    elif strx[1] == "disabled":
+        mode = pyservsup.PERM_DIS
+    else:
+        response = [ERR, "Must specify 'user' or 'admin' or 'disabled' or 'initial'", strx[0]]
+        self.resp.datahandler.putencode(response, self.resp.ekey)
+        return retval
+
+    response = pyservsup.gl_passwd.listusers(mode)
+
+    self.resp.datahandler.putencode(response, self.resp.ekey)
+
+
 def get_uini_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_uini_func()")
+
     # Test for local client
     if str(self.resp.client_address[0]) != "127.0.0.1":
         response = [ERR,  "Must connect from loopback interface.", strx[0]]
 
-    elif  pyservsup.passwd.count() != 0:
+    elif  pyservsup.gl_passwd.count() != 0:
         response = [ERR, "Already has initial user", strx[0]]
 
     elif len(strx) < 3:
         response = [ERR, "Must specify user name and pass.", strx[0]]
     else:
-        ret = pyservsup.passwd.auth(strx[1], strx[2],
+        ret = pyservsup.gl_passwd.auth(strx[1], strx[2],
                     pyservsup.PERM_INI | pyservsup.PERM_ADMIN,
                         pyservsup.USER_ADD)
         if ret[0] == 0:
             response = [ERR, ret[1], strx[0]]
         elif ret[0] == 1:
             response = [ERR,
             "User already exists, no change. Use pass function.", strx[0]];
         elif ret[0] == 2:
+
+            if pyservsup.globals.conf.pglog > 1:
+                stry = "Added initial user",  strx[1], \
+                        str(self.resp.client_address)
+                pysyslog.syslog(*stry)
             response = [OK, "Added initial user", strx[1]]
         else:
             response = [ERR, ret[1], strx[0]]
 
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
-#def get_kini_func(self, strx):
-#
-#    # Test for local client
-#    if str(self.resp.client_address[0]) != "127.0.0.1":
-#        response = ERR, "Must connect from loopback.", strx[0]
-#    elif len(strx) < 3:
-#        response = ERR, "Must specify key_name and key_value.", strx[0]
-#    else:
-#        # See if there is a key file
-#        if os.path.isfile(pyservsup.keyfile):
-#            response = ERR, "Initial key already exists", strx[0]
-#        else:
-#            #tmp2 = bluepy.bluepy.decrypt(self.resp.passwd, "1234")
-#            #tmp = bluepy.bluepy.encrypt(strx[2], tmp2)
-#            #ret = pyservsup.kauth(strx[1], tmp, 1)
-#            ret = pyservsup.kauth(strx[1], strx[2], 1)
-#            #bluepy.bluepy.destroy(tmp)
-#
-#            if ret[0] == 0:
-#                response = OK, "Added key",  strx[1]
-#            else:
-#                response = ERR, ret[1], strx[0]
-#    self.resp.datahandler.putencode(response, self.resp.ekey)
-#
-#def get_kadd_func(self, strx):
-#
-#    response = ERR, "Not Implemented", strx[0]
-#    self.resp.datahandler.putencode(response, self.resp.ekey)
-#    return
-#
-#    if not os.path.isfile(pyservsup.keyfile):
-#        response = ERR, "No initial keys yet. Please add some.", strx[0]
-#    if len(strx) < 3:
-#        response = ERR, "Must specify key_name and key_value.", strx[0]
-#    else:
-#        # See if there is a key by this name
-#        ret = pyservsup.kauth(strx[1], strx[2], 1)
-#        if ret[0]  < 0:
-#            response = ERR, ret[1], strx[0]
-#        elif ret[0] == 2:
-#            response = ERR, "Key already exists, no keys are changed ", strx[0]
-#        elif ret[0] == 0:
-#            response = "OK added key '" + strx[1] + "'"
-#        else:
-#            response = ERR, "Invalid return code from auth.", strx[0]
-#    self.resp.datahandler.putencode(response, self.resp.ekey)
-
 def get_udel_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "get_udel_func()", strx)
+
     retval = 0
      # Are we allowed to add users?
-    ret = pyservsup.passwd.perms(self.resp.user)
+    ret = pyservsup.gl_passwd.perms(self.resp.user)
     if int(ret[2]) & pyservsup.PERM_ADMIN != pyservsup.PERM_ADMIN:
         response = ERR, "Only admin can add/delete users", strx[0]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return retval
     if len(strx) < 2:
         response = [ERR, "Must specify user name to delete", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return retval
     # Delete user
-    ret = pyservsup.passwd.auth(strx[1], "",
+    ret = pyservsup.gl_passwd.auth(strx[1], "",
                     pyservsup.PERM_NONE, pyservsup.USER_DEL)
     #print("udel ret", ret)
     if ret[0] == 0:
         response = [ERR, ret[1], strx[1]]
     elif ret[0] == 4:
         response = [OK, "deleted user", strx[1]]
     else:
         response = [ERR, ret[1], strx[1]]
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def put_file_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "put_file_func()", strx)
+
     if len(strx) == 1:
         response = [ERR, "Must specify file name.", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
     # Close possible pending
     if  self.resp.fh:
@@ -1628,19 +1964,22 @@
             self.resp.fh = open(dname, "wb")
             self.resp.fname = strx[1]
             response = [OK, "Send file", self.resp.fname]
         except:
             response = [ERR, "Cannot create file", self.resp.fname, strx[0]]
     except:
         response = [ERR,  "Must specify file name", strx[0]]
-    #pysyslog.syslog("Opened", xstr[1])
+
     self.resp.datahandler.putencode(response, self.resp.ekey)
 
 def put_data_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "put_data_func()", strx)
+
     #print("fname", self.resp.fname, "data:", strx)
 
     if self.resp.fname == "":
         response = [ERR, "No filename for data", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
@@ -1665,39 +2004,49 @@
         self.resp.fh.write(strx[2])
     except:
         #print(sys.exc_info())
         response = [ERR, "Cannot save data on server", strx[0]]
         self.resp.datahandler.putencode(response, self.resp.ekey)
         return
 
-    xstr = "Received chunk: '" + self.resp.fname + \
-                "' " + str(dlen) + " bytes"
+    #xstr = "Received chunk: '" + self.resp.fname + \
+    #            "'" + str(dlen) + " bytes"
     #print( xstr)
-    #pysyslog.syslog(xstr)
-    #self.resp.datahandler.putencode("OK Got data", self.resp.ekey)
+
     self.resp.datahandler.putencode([OK,  "Got data"], self.resp.ekey)
 
 def get_qr_func(self, strx):
 
     if pyservsup.globals.conf.pgdebug > 1:
-        print("QRfunc called", len(strx))
+        print("get_qr_func()", len(strx))
 
     #print("cwd:", self.resp.cwd)
     if len(strx) == 1:
-        fp = open('qr.png', 'rb')
-        buff = fp.read()
-        fp.close()
-        self.resp.datahandler.putencode([OK, buff], self.resp.ekey)
+        try:
+            fp = open('qr.png', 'rb')
+            buff = fp.read()
+            fp.close()
+            self.resp.datahandler.putencode([OK, buff], self.resp.ekey)
+        except:
+            self.resp.datahandler.putencode([ERR, "No QR image on server"], self.resp.ekey)
     else:
+        ret = pyservsup.gl_passwd.perms(self.resp.user)
+        if not int(ret[2]) & pyservsup.PERM_ADMIN:
+            rrr = [ERR, "Only admin can upload QR image", self.name]
+            self.resp.datahandler.putencode(rrr, self.resp.ekey)
+
         if type(strx[1]) != type(b""):
             strx[1] = strx[1].encode()
-        fp = open('qr.png', 'wb')
-        fp.write(strx[1])
-        fp.close()
-        self.resp.datahandler.putencode([OK, "Written new QR image", len(strx[1])], self.resp.ekey)
+        try:
+            fp = open('qr.png', 'wb')
+            fp.write(strx[1])
+            fp.close()
+            self.resp.datahandler.putencode([OK, "Written new QR image", len(strx[1])], self.resp.ekey)
+        except:
+            self.resp.datahandler.putencode([ERR, "Cannot save QR image"], self.resp.ekey)
 
 def get_twofa_func(self, strx):
 
     if pyservsup.globals.conf.pgdebug > 1:
         print("get_twofa_func called")
 
     retval = True
@@ -1721,39 +2070,43 @@
         self.resp.datahandler.putencode(["OK", "Code Auth OK",],  self.resp.ekey)
         retval = False
 
     return retval
 
 def get_dmode_func(self, strx):
 
+    if pyservsup.globals.conf.pgdebug > 1:
+        print( "getdmode_func()", strx)
+
     flag = not pyservsup.globals.conf.pmode
     self.resp.datahandler.putencode(["OK", "%d" % flag],  self.resp.ekey)
 
 def get_help_func(self, strx):
 
     if pyservsup.globals.conf.pgdebug > 1:
         print( "get_help_func()", strx)
 
     harr = []
     if len(strx) == 1:
         harr.append(OK)
         for aa in pyvstate.state_table:
             harr.append(aa[0])
+        harr.append("fields")
     else:
         ff = False
         for aa in pyvstate.state_table:
             if strx[1] == aa[0]:
-                harr.append(OK)
-                harr.append(aa[5])
+                harr = [OK, aa[5], ]
                 ff = True
                 break
         if not ff:
-                harr.append(ERR)
-                harr.append("No such command")
-                harr.append(strx[0])
+            if strx[1] == "fields":
+                harr = [OK, fields_help, ]
+            else:
+                harr = [ERR, "No such command", strx[1], ]
 
     if pyservsup.globals.conf.pgdebug > 2:
         print( "get_help_func->output", harr)
 
     self.resp.datahandler.putencode(harr, self.resp.ekey)
 
 if __name__ == '__main__':
```

### Comparing `pyvserv-1.0.3/pyvserver/pyvserv.py` & `pyvserv-1.0.4/pyvserver/pyvserv.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,43 +1,66 @@
 #!/usr/bin/env python3
 
+# Too many misc crappers like dyn properties
+# pylint: disable=E1101
+# pylint: disable=C0103
+# pylint: disable=C0413
+# pylint: disable=C0209
+# pylint: disable=W0201
+# pylint: disable=W0702     # Bare exceptions
+# pylint: disable=W0602     # No global assignment
+
 __doc__ = \
 '''
 Server module.
 '''
 import sys
+import os
+import getopt
+import signal
+import time
+import subprocess
+import platform
+import socket
+import threading
+import tracemalloc
+import datetime
+import distro
 
 if sys.version_info[0] < 3:
     print("Python 2 is not supported as of 1/1/2020")
     sys.exit(1)
 
-import os, getopt, signal, select, string, time
-import subprocess,  platform, queue, ctypes
-import socket, threading, tracemalloc, copy, random
-
-import multiprocessing as mp
-
 try:
     import fcntl
-except:
+except ImportError:
     fcntl = None
+except:
+    print(sys.exc_info())
 
 if sys.version_info[0] < 3:
     import SocketServer as socketserver
 else:
     import socketserver
 
-import pyvpacker
-
-#import gi
-#gi.require_version("Gtk", "3.0")
-#from gi.repository import GLib
-
-# Create a placeholder for the main server var
-server = None
+__doc__ = ''' <pre>\
+The main pyvserv excutable.
+Usage: pyvserv.py [options]
+  options:
+        -n   --host      host       -  Set server hostname / interface.
+        -r   --dataroot  droot      -  Set data root for server.
+        -l   --loglevel  pglog      -  Log level (0 - 10) default = 1
+        -d   --debug     pgdebug    -  Debug level 0-10
+        -p   --port      port       -  Listen on port
+        -v   --verbose              -  Verbose. Show more info.
+        -q   --quiet                -  Quiet. Show less info.
+        -V   --version              -  Print Version string
+        -h   --help                 -  Show Help. (this screen)
+        -P   --pmode                -  Production mode ON. (allow 2FA)
+Use quotes for multiple option strings. </pre>'''
 
 progname = os.path.split(sys.argv[0])[1]
 
 # This repairs the path from local run to pip run.
 # Remove pip version for local tests
 try:
     from pyvcommon import support
@@ -51,359 +74,336 @@
 except:
     base = os.path.dirname(os.path.realpath(__file__))
     sys.path.append(os.path.join(base,  '..'))
     sys.path.append(os.path.join(base,  '..', "pyvcommon"))
     sys.path.append(os.path.join(base,  '..', "pyvserver"))
     from pyvcommon import support
 
-from pyvcommon import support, pyservsup, pyclisup
+from pyvcommon import support, pyservsup
 from pyvcommon import pydata, pysyslog, comline
 
 from pyvserver import pyvstate
 from pyvserver import pyvfunc
 
-# Update it from setup
-version = "1.0.3"
+# Create a placeholders
 
-mydata = {}
+SHARED_MYDATA   = None
+gl_server       = None
+args            = None
 
 # ------------------------------------------------------------------------
 
 class InvalidArg(Exception):
 
     ''' Exception for bad arguments '''
 
     def __init__(self, message):
-         self.message = message
-
-# Using globals here; class instances fooled by threading
-#gl_sem = threading.Semaphore()
-#gl_queue = queue.Queue()
-#global gl_queue
-#gl_queue.put((peer, now))
-#print("qsize", gl_queue.qsize)
-
-# ------------------------------------------------------------------------
-
-class Throttle():
-
-    '''  Catch clients that are connecting too fast. This needs a serious
-        upgrade if in large volume production.
-    '''
-    def __init__(self):
-
-        if fcntl:
-            # This is for forkmixin
-            self.sem  = mp.Semaphore()
-            self.man  = mp.Manager()
-            self.connlist = self.man.list()
-        else:
-            self.sem     = threading.Semaphore()
-            self.connlist = []
-
-    def throttle(self, peer):
-
-        '''
-            Catch clients that are connecting too fast.
-            Throttle to N sec frequency, if number of connections from
-            the same ip exceeds throt_instances.
-        '''
-
-        wantsleep = 0; sss = 0;
-        now = time.time()
-        self.sem.acquire()
-
-        for aa in self.connlist:
-            if aa[0] == peer[0]:
-                if now - aa[1] <  pyservsup.globals.throt_sec:
-                    sss += 1
-
-        if sss >  pyservsup.globals.throt_instances:
-            # Clean old entries fot this host
-            for aa in range(len(self.connlist)-1, -1 ,-1):
-                if self.connlist[aa][0] == peer[0]:
-                    if now - self.connlist[aa][1] > pyservsup.globals.throt_sec:
-                        del self.connlist[aa]
-            wantsleep = pyservsup.globals.throt_time
-
-        # Clean throtle data periodically
-        if len(self.connlist) > pyservsup.globals.throt_maxdat:
-            #print("Cleaning throttle list", len(self.connlist))
-            for aa in range(len(self.connlist)-1, -1 ,-1):
-                if now - self.connlist[aa][1] > pyservsup.globals.throt_maxsec:
-                    del self.connlist[aa]
-
-        # Flatten list for the multiprocessing context manager
-        self.connlist.append((peer[0], now))
-
-        #print("connlist", self.connlist)  # Make sure it cycles
-        #print()
-
-        self.sem.release()
-        return wantsleep
-
-# The one and only instance
-gl_throttle = Throttle()
+        super().__init__(self)  #InvalidArg, self)
+        self.message = message
 
 class ThreadedTCPRequestHandler(socketserver.BaseRequestHandler):
 
     ''' Request handler. '''
 
     def __init__(self, a1, a2, a3):
 
         self.verbose = conf.verbose
-        self.a1 = a1
-        self.a2 = a2
+        self.pgdebug = conf.pgdebug
+        self.peer = a2
         self.fname = ""
         self.user = ""
+        self.preuser = ""
         self.cwd = os.getcwd()
         self.dir = ""
         self.ekey = ""
 
-        ttt = gl_throttle.throttle(self.a1.getpeername())
+        #print("a1", a1, "a2", a2, "a3", a3)
+
+        # Throttle for multiple connectiond from one host
+        ttt = pyservsup.gl_throttle.throttle(a1.getpeername())
         if ttt > 0:
-            if self.verbose > 0:
+            if self.pgdebug > 2:
                 print("Throttle sleep",  a1.getpeername())
             time.sleep(ttt)
 
         socketserver.BaseRequestHandler.__init__(self, a1, a2, a3)
 
     def setup(self):
 
         ''' Start server '''
 
-        global mydata
+        global SHARED_MYDATA
 
         #print("thread", self)
         #print(dir(self))
 
         cur_thread = threading.current_thread()
         #print(dir(cur_thread))
 
         self.name  = str(cur_thread._native_id) #name #getName()
         #self.name  = cur_thread.name #getName()
         #print( "Logoff '" + usr + "'", cli)
+
         if self.verbose:
-            print( "Connection from ", self.a2, "as", self.name)
+            print( "Connection from ", self.peer, "as", self.name)
 
         self.statehandler = pyvstate.StateHandler(self)
-        self.statehandler.verbose = conf.verbose
-        self.statehandler.pglog = conf.pglog
-        self.statehandler.pgdebug = conf.pgdebug
-        self.statehandler.name    = self.name
-
-        #print(self.request)
-        mydata[self.name] = self
-
-        #print(dir(self))
-        #print(self.name)
-        #if conf.verbose:
-        #    print("Connected " + " " + str(self.client_address))
+        self.statehandler.verbose   = conf.verbose
+        self.statehandler.pglog     = conf.pglog
+        self.statehandler.pgdebug   = conf.pgdebug
+        self.statehandler.name      = self.name
+
+        # Remeber globally, add to shared dicrtionary
+        ddd = (os.getpid(), self.peer[0], self.peer[1],  self.request)
+
+        if conf.pgdebug > 4:
+            print("Adding mydata:", ddd)
+        SHARED_MYDATA.setdat(self.name, ddd)
 
         self.datahandler            =  pydata.DataHandler(self.request)
         self.datahandler.pgdebug    = conf.pgdebug
         self.datahandler.pglog      = conf.pglog
         self.datahandler.verbose    = conf.verbose
         self.datahandler.par        = self
 
         self.request.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
 
         if conf.pglog > 0:
             pysyslog.syslog("Connected " + " " + str(self.client_address))
 
-        response =  ["OK", "pyvserv %s ready" % version]
+        response =  ["OK", "pyvserv %s ready" % pyservsup.version, self.name]
+
         # Connected, acknowledge it
         self.datahandler.putencode(response, "")
 
-    def handle_error(request, client_address):
+    def handle_error(self, request, client_address):
 
         ''' Placeholder '''
 
         print("pyvserv Error", request, client_address)
 
     def handle(self):
 
         ''' Request comes in here '''
 
         if conf.mem:
             tracemalloc.start()
         try:
             while 1:
                 ret = self.datahandler.handle_one(self)
-                if not ret: break
+                if not ret:
+                    break
                 ret2 = self.statehandler.run_state(ret)
                 if ret2:
                     #response2 = ["err", "Too many tries, disconnecting."]
                     response2 = ["ERR", "Disconnected."]
                     self.datahandler.putencode(response2, self.statehandler.resp.ekey)
                     #time.sleep(.1)
                     #self.datahandler.par.request.shutdown(socket.SHUT_RDWR)
                     break
         except:
             #print( sys.exc_info())
             support.put_exception("state handler")
 
         if self.verbose:
-            print( "Connection closed on", self.name)
+            print( "Connection closed on", self.peer)
 
         if conf.mem:
-            #print( "Memory trace")
+            print( "Memory trace")
             snapshot = tracemalloc.take_snapshot()
             top_stats = snapshot.statistics('lineno')
-
             print("[ Top 10 ]")
             for stat in top_stats[:10]:
                 print(stat)
 
         #if conf.pglog > 0:
         #    pysyslog.syslog("Disconn " + " " + str(self.client_address))
 
     def finish(self):
 
         ''' Wind down, remove globals '''
 
-        global mydata, conf
-
-        cli = str(mydata[self.name].client_address)
-        usr = str(mydata[self.name].user)
-        #print( "Logoff '" + usr + "'", cli)
-        del mydata[self.name]
-
-        if conf.verbose:
-            print( "Closed socket on", self.name)
-
-        if conf.pglog > 0:
-            pysyslog.syslog("Logoff '" + usr + "' " + cli)
-
-        #server.socket.shutdown(socket.SHUT_RDWR)
-        #server.socket.close()
+        global SHARED_MYDATA
+        if conf.pgdebug > 4:
+            ddd = SHARED_MYDATA.getdat(self.name)
+            print("Removing mydata:", self.name, ddd)
+
+        SHARED_MYDATA.deldat(self.name)
+        if self.statehandler.resp.user:
+            pyservsup.SHARED_LOGINS.deldat(self.statehandler.resp.user)
 
 # ------------------------------------------------------------------------
 # Override stock methods. Windows has no ForkinMixin
 
 if not fcntl:
     mixin = socketserver.ThreadingMixIn
 else:
     mixin = socketserver.ForkingMixIn
 
-# Overriding it for throttle development
+# Overriding it for throttle and cleanup development !! TEST !!
 #mixin = socketserver.ThreadingMixIn
 
 class ThreadedTCPServer(mixin, socketserver.TCPServer):
 
     ''' Overridden socket server '''
 
     #def __init__(self, arg1, arg2):
     #    self._BaseServer__shutdown_request = True
 
     def stop(self):
+        ''' breakout '''
+
         self._BaseServer__shutdown_request = True
-        if verbose:
+
+        if conf.verbose:
             print( "Stop called")
+
         #self.shutdown()
         #self.server_close()
-        pass
-
 
-def usersig(arg1, arg2):
+def usersig1(arg1, arg2):
 
     ''' signal comes in here, list current clients '''
 
-    global mydata, server
-    print("usersig", arg1, arg2)
-    if conf.pglog > 0:
+    global SHARED_MYDATA, gl_server
+    if conf.pgdebug > 1:
+        print("usersig", arg1)
+
+    if conf.pgdebug > 6:
+        print("usersig", arg1, arg2)
+
+    if conf.pglog > 2:
         pysyslog.syslog("Got user signal %d" % arg1)
 
     print("Current clients:")
-    print( mydata)
+    print( SHARED_MYDATA.getall())
+
+    print("Current logins:")
+    ddd = pyservsup.SHARED_LOGINS.getall()
+    if ddd:
+        for aa in ddd.keys():
+            dt = datetime.datetime.fromtimestamp(ddd[aa])
+            print("Login:", "'" + aa + "'", "Login time:", dt)
 
 def usersig2(arg1, arg2):
 
-    global mydata, server
-    print("usersig2", arg1, arg2)
-    if conf.pglog > 0:
-        pysyslog.syslog("Got user signal2 %d" % arg1)
+    ''' respond to user signaal '''
 
-def soft_terminate(arg1, arg2):
+    if conf.pgdebug > 1:
+        print("usersig2", arg1)
 
-    ''' Terminate app.  Did not behave as expected. '''
+    if conf.pgdebug > 6:
+        print("usersig2", arg1, arg2)
 
-    #global mydata, server
-    ##print("soft_terminate")
-    #try:
-    #
-    #    for aa in mydata:
-    #        print(aa, mydata[aa])
-    #        mydata[aa].finish()
-    #except:
-    #    pass
-    #
-
-    terminate(0, 0)
-
-    #while True:
-    #    print( "Dumping connection info:")
-    #    print( mydata)
-    #    if mydata == {}:
-    #        terminate(0, 0);
-    #        break
-    #    time.sleep (1)
+    if conf.pglog > 2:
+        pysyslog.syslog("Got user signal2 %d" % arg1)
 
-# ------------------------------------------------------------------------
+    print("Current configuration:")
+    print("Full server path:    ", pyservsup.globals.script_home)
+    print("Data root:           ", pyservsup.globals.myhome)
+    print("Pass Dir:            ", pyservsup.globals.passdir)
+    print("Key Dir:             ", pyservsup.globals.keydir)
+    print("Payload Dir:         ", pyservsup.globals.paydir)
+    print("Blockchain Dir:      ", pyservsup.globals.chaindir)
+    print("Log dir:             ", pyservsup.globals.logdir)
+    print("Temp dir:            ", pyservsup.globals.tmpdir)
+    print("Lockfile:            ", pyservsup.globals.lockfname)
+    print("IDfile:              ", pyservsup.globals.idfile)
+    print("Current operationals:")
+    print("Server hostname:     ", pyservsup.globals.conf.host)
+    print("Port listening on:   ", pyservsup.globals.conf.port)
+    print("Debug level:         ", pyservsup.globals.conf.pgdebug)
+    print("Verbose:             ", pyservsup.globals.conf.verbose)
+    print("Loglevel:            ", pyservsup.globals.conf.pglog)
+    print("Production Mode:     ", pyservsup.globals.conf.pmode)
+
+def soft_terminate(arg1 = 0, arg2 = 0):
+
+    # pylint: disable=unused-argument
+
+    ''' Terminate app. Did not behave as expected ... fixed. '''
+
+    if conf.pgdebug > 1:
+        print("   soft_terminate")
+
+    if conf.pgdebug > 1:
+        print( "Dumping connection info:")
+        ddd = SHARED_MYDATA.getall()
+        for aa in ddd.keys():
+            print(os.getpid(), ddd[aa])
 
-def terminate(arg1, arg2):
+    terminate() #0, 0)
 
-    global mydata, server
+# ------------------------------------------------------------------------
 
-    #print("terminate")
-    #if mydata != {}:
-    #    print( "Dumping connection info:")
-    #    print( mydata)
+def terminate(arg1 = 0, arg2 = 0):
 
-    try:
-        if server:
-            server.socket.shutdown(socket.SHUT_RDWR)
-            server.socket.close()
-            server.shutdown()
-    except:
-        print("Exception in shutdown", sys.exc_info())
-        pass
+    ''' Terminate app.  Wind down all sockets. Free locks. '''
 
-    if not conf.quiet:
-        print( "Terminated", progname)
+    # pylint: disable=unused-argument
+    global SHARED_MYDATA, gl_server
 
-    #if conf.pglog > 0:
-    #    pysyslog.syslog("Terminated Server")
+    # Attempt to unhook all pending clients
+    #print( "Closing active clients:")
+    pid = os.getpid()
+    ddd = SHARED_MYDATA.getall()
+    if ddd:
+        for aa in ddd.keys():
+            if conf.pgdebug > 5:
+                print( "Shared data:", ddd[aa])
+            if pid == ddd[aa][0]:
+                if conf.pgdebug > 1:
+                    print( "Closing connection:", ddd[aa])
+                try:
+                    ddd[aa][3].shutdown(socket.SHUT_RDWR)
+                    ddd[aa][3].close()
+                except:
+                    print("exc on close conn", sys.exc_info())
+
+    if conf.pglog > 0:
+        pysyslog.syslog("Terminated Server" )
 
     support.unlock_process(pyservsup.globals.lockfname)
 
-    # Attempt to unhook all pending clients
+    if not conf.quiet:
+        print( "Terminated", progname)
+
     sys.exit(2)
 
 # ------------------------------------------------------------------------
 # Execute one server cycle
 
-class serve_one():
+# pylint: disable=too-few-public-methods
 
-    ''' Simplifies server for testing. '''
+class serve_one():
 
+    ''' Simplified server for testing. Kept in case we want to
+        temporarily revert.
+    '''
     def __init__(self, *argx):
         self.cnt = 0
         self.fname = ""
         self.user = ""
         self.cwd = os.getcwd()
         self.dir = ""
         self.ekey = ""
         self.argx = argx
         server_thread = threading.Thread(target=self.run)
         server_thread.start()
+        self.verbose = False
+        self.argx = argx
+        self.name = ""
+        self.statehandler = None
+        self.datahandler =  None
+
+    def run(self, argx):
 
-    def run(self, *argx):
+        ''' run '''
 
-        self.client, self.client_address, self.args = self.argx
+        self.client, self.client_address, self.args = argx
         cur_thread = threading.current_thread()
         self.name = cur_thread.name #getName()
         #print( "Logoff '" + usr + "'", cli)
 
         self.verbose = conf.verbose
 
         if self.verbose:
@@ -416,269 +416,300 @@
         #    put_debug("Connection from %s" % self.a2)
 
         self.statehandler = pyvstate.StateHandler(self)
         self.statehandler.verbose = conf.verbose
         self.statehandler.pglog = conf.pglog
         self.statehandler.pgdebug = conf.pgdebug
 
-        #print(self.request)
-        #mydata[self.name] = self
-
         #if conf.verbose:
         #    print("Connected " + " " + str(self.client_address))
 
         self.datahandler =  pydata.DataHandler(self.client)
         self.datahandler.pgdebug = conf.pgdebug
         self.datahandler.pglog = conf.pglog
         self.datahandler.verbose = conf.verbose
         self.datahandler.par = self
 
         self.client.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
 
         if conf.pglog > 0:
-            pysyslog.syslog("Connected " + " " + str(self.client_address))
+            pysyslog.syslog("Connected ", str(self.client_address))
 
-        response =  ["OK", "pyvserv %s ready" % version]
+        response =  ["OK", "pyvserv %s ready" % pyservsup.version]
         # Connected, acknowledge it
         self.datahandler.putencode(response, "")
 
         try:
             while 1:
                 ret = self.datahandler.handle_one(self)
-                if not ret: break
+                if not ret:
+                    break
                 ret2 = self.statehandler.run_state(ret)
                 if ret2:
                     #response2 = ["err", "Too many tries, disconnecting."]
                     response2 = ["ERR", "Disconnected."]
                     self.datahandler.putencode(response2, self.statehandler.resp.ekey)
                     break
         except:
             #print( sys.exc_info())
             support.put_exception("state handler")
 
-        if self.verbose:
-            print( "Connection closed on", self.name)
-
         if conf.mem:
             #print( "Memory trace")
-            snapshot = tracemalloc.take_snapshot()
-            top_stats = snapshot.statistics('lineno')
+            #snapshot = tracemalloc.take_snapshot()
+            #top_stats = snapshot.statistics('lineno')
+            pass
 
         if self.verbose:
             print("ended thread", self.name)
 
-
-def simple_server(HOST, PORT):
+def simple_server(Host, Port):
 
     ''' This was a test server, left it in for future refernence.
         It was marginally faster than the stock version, also less features,
          so the stock servers stayed.
     '''
 
+    global args
+
     with socket.socket() as server:
         server.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
 
-        server.bind((HOST, PORT))
+        server.bind((Host, Port))
         server.listen()
         while True:
             client, addr = server.accept()
-            client.setsockopt(socket.IPPROTO_TCP, socket.TCP_NODELAY, 1)
+            client.setsockopt(socket.IPPROTO_TCP,
+                            socket.TCP_NODELAY, 1)
             serve_one(client, addr, args)
 
 # ------------------------------------------------------------------------
 
-optarr =  [] #comline.optarrlong
-#optarr.append ( ["e",   "detach=",   "detach",      0,       None, "Detach from terminal."] )
-optarr.append ( ["n:",  "host",      "host",   "127.0.0.1",  None, "Set server hostname / interface."] )
-optarr.append ( ["r:",  "dataroot=", "droot",  "pyvserver",  None, "Set data root for server. "] )
-optarr.append ( ["P",   "pmode",     "pmode",       0,       None, "Production mode ON. (allow 2FA)"] )
-optarr.append ( ["l:",  "loglevel",  "pglog",       1,       None, "Log level (0 - 10) default = 1"] )
-optarr.append ( ["m",   "mem",       "mem",         0,       None, "Show memory trace."] )
-optarr.append ( ["N",   "norepl",    "norepl",      0,       None, "No replication. (for testing)"] )
-
-for aa in comline.optarrlong:
-    optarr.append(aa)
-
-comline.optarrlong = optarr
-
 # Tue 02.Apr.2024 made devmode default
 
-#print (optarr)
-comline.setargs("")
-comline.setfoot("Use quotes for argument separations.")
+optarr =  []
+optarr.append ( ["n:",  "host=",     "host",   "127.0.0.1",
+            None, "Set server hostname / interface. default=127.0.0.1"] )
+optarr.append ( ["r:",  "dataroot=", "droot",  "pyvserver",
+            None, "Set data root for server. default:~/pyvserver "] )
+optarr.append ( ["l:",  "loglevel=", "pglog",       1,
+            None, "Log level. 0=none 10=noisy default=1"] )
+
+optarr += comline.optarrlong
+
+optarr.append ( ["m",   "mem",       "mem",         0,
+                                None, "Show memory trace. (Advanced users only.)"] )
+#optarr.append ( ["N",   "norepl",    "norepl",      0,
+#                            None, "No replication. (for testing)"] )
+optarr.append ( ["P",   "pmode",     "pmode",       0,
+                            None, "Production mode ON. (allow 2FA)"] )
+
+comline.sethead("The main pyvserv excutable.")
+#comline.setprog(os.path.basename(sys.argv[0]))
+comline.setprog(os.path.basename(__file__))
+comline.setargs("[options]")
+comline.setfoot("Use quotes for multiple option strings.")
 
 conf = comline.ConfigLong(optarr)
 #conf.printvars()
 
-def mainfunct():
-
-    ''' Main entry point. The pip install will call this script. '''
-
-    if sys.version_info[0] < 3:
-        print("This script was meant for python 3.x")
-        time.sleep(.1)
-        sys.exit(0)
-
-    args = conf.comline(sys.argv[1:])
-    #print(args)
-
-    # Print comline args
-    if conf.pgdebug > 7:
-        for aa in vars(conf):
-            if aa != "_optarr":
-                print(aa, "=", getattr(conf, aa), end = "    ")
-        print()
-
-    if conf.pgdebug > 4:
-        print("This script:     ", os.path.realpath(__file__))
-        print("Full path argv:  ", os.path.abspath(sys.argv[0]))
-        print("Script name:     ", __file__)
-        print("Exec argv:       ", sys.argv[0])
-
-    pyservsup.globals  = pyservsup.Global_Vars(__file__, conf.droot)
-    pyservsup.globals.conf = conf
-    pyservsup.globals.lockfname += "_" + str(conf.port) + "_" + str(conf.host)
-    pyservsup.globals._softmkdir(pyservsup.globals.myhome)
+def do_keys():
+    ''' breakout '''
+    try:
+        #keyfroot =
+        pyservsup.pickkey(pyservsup.globals.keydir)
+    except:
+        if conf.pgdebug > 4:
+            print("Could pick keys", sys.exc_info())
+        if conf.pgdebug > 5:
+            support.put_exception("pick keys")
 
-    # Change directory to the data dir
-    os.chdir(pyservsup.globals.myhome)
-    #print("cwd", os.getcwd())
+        #print("No keys generated yet. Please run pyvgenkey.py first.")
+        print("Notice: Generating key in", "'" + pyservsup.globals.keydir + "'")
+        execx = os.path.dirname(pyservsup.globals.script_home) + os.sep
+        execx += "../pyvtools/pyvgenkey.py"
+        try:
+            if conf.pgdebug > 4:
+                print("Generating keys", execx)
+            # Try local
+            if os.path.isfile(execx):
+                rrr = [execx, "-q", "-m", pyservsup.globals.myhome]
+                with subprocess.Popen(rrr):
+                    pass
+            else:
+                # Try with full install version ... executable
+                execx = "pyvgenkey"
+                rrr = [execx, "-q", "-m", pyservsup.globals.myhome]
+                with subprocess.Popen(rrr):
+                    pass
+        except:
+            if conf.pgdebug > 4:
+                print("Could not exec", sys.exc_info())
+            if conf.pgdebug > 5:
+                support.put_exception("generate keys")
+            print("Could not generate key. Keydir was:", pyservsup.globals.keydir)
+            print("Please try again manually with the 'pvgenkey' utility.")
+        print("For added security please generate more keys with 'pyvgenkeys'")
 
-    pyservsup.globals.config(pyservsup.globals.myhome, conf)
+def print_stats():
 
+    ''' breakout '''
     if conf.verbose:
-        #print("Script Dir:      ", pyservsup.globals._script_home)
+        print("Serve exe path:  ", pyservsup.globals.script_home)
+        print("Data root:       ", pyservsup.globals.myhome)
         print("Pass Dir:        ", pyservsup.globals.passdir)
         print("Key Dir:         ", pyservsup.globals.keydir)
         print("Payload Dir:     ", pyservsup.globals.paydir)
-        print("Lockfile:        ", pyservsup.globals.lockfname)
-        print("Passfile:        ", pyservsup.globals.passfile)
-        print("IDfile:          ", pyservsup.globals.idfile)
-        #print("Keyfile:         ", pyservsup.globals .keyfile)
+        print("Lock file:       ", pyservsup.globals.lockfname)
+        print("ID file:         ", pyservsup.globals.idfile)
+        #print("Passfile:        ", pyservsup.globals.passfile)
+
+def start_server():
+
+    ''' breakout '''
+    global gl_server
     try:
-        keyfroot = pyservsup.pickkey(pyservsup.globals.keydir)
+        gl_server = ThreadedTCPServer((conf.host, conf.port), ThreadedTCPRequestHandler)
+        gl_server.allow_reuse_address = True
+        #ip, port = server.server_address
+        gl_server.verbose = conf.verbose
+
+        # Start a thread with the server -- that thread will then start one
+        # or more threads for each request
+        server_thread = threading.Thread(target=gl_server.serve_forever)
+
+        # Exit the server thread when the main thread terminates
+        server_thread.verbose = conf.verbose
+        server_thread.daemon = True
+        #server_thread.paydir =  pyservsup.globals.paydir
+        server_thread.start()
+
     except:
-        #print("No keys generated yet. Please run pyvgenkey.py first.")
-        exec = os.path.dirname(os.path.split(pyservsup.globals._script_home)[0]) + os.sep
-        exec += "../pyvtools/pyvgenkey.py"
-        print("Notice: Generating key in", "'" + pyservsup.globals.keydir + "'")
+        print( "Cannot start server. ", sys.exc_info())
+        if conf.pglog > 0:
+            pysyslog.syslog("Cannot start server ", sys.exc_info())
+            #print("Try again later.")
+            #terminate(None, None)
+            sys.exit(1)
+
+def signon_message():
+
+    ''' message for the terminal '''
+    if not conf.quiet:
+        if not pyservsup.globals.conf.pmode:
+            print("Warning! Devmode ON. Use -P to allow 2FA auth")
         try:
-            if conf.pgdebug > 2:
-                print("Generating keys", exec)
-            # Early out for no script
-            if not os.path.isfile(exec):
-                raise
-            ret = subprocess.Popen([exec, "-q", "-m", pyservsup.globals.myhome])
+            strx = distro.name()
         except:
-            try:
-                # Try with full install version
-                #print("Executing with installed version")
-                exec = "pyvgenkey"
-                ret = subprocess.Popen([exec, "-q", "-m", pyservsup.globals.myhome])
-            except:
-                print("Could not generate key. Keydir was:", pyservsup.globals.keydir)
-                print("Please try again manually with the 'pvgenkey' utility.")
-
-            print("For added security please generate more keys with 'pyvgenkeys'");
-            #sys.exit(1)
-
-    iii = pyservsup.create_read_idfile(pyservsup.globals.idfile)
-    if not iii:
-        print("Cannot read / create site ID, exiting.")
-        sys.exit(1)
-
-    pyservsup.globals.siteid = iii
+            strx = "Win or Unkn."
+        print("MainSiteID:      ", pyservsup.globals.siteid)
+        print("Server running: ", "'"+conf.host+"'", "Port:", conf.port)
+        #pyver = support.list2str(sys.version_info) #[0:3], ".")
+        print("Running python", platform.python_version(), "on", platform.system(), strx)
 
-    #if conf.verbose:
-    #    print("Current dir:     ", os.getcwd())
+def set_sigs():
 
+    '''  set up signal handlers '''
     # Set termination handlers, so lock will be deleted
     signal.signal(signal.SIGTERM, terminate)
     signal.signal(signal.SIGINT, soft_terminate)
     try:
-        signal.signal(signal.SIGUSR1, usersig)
+        signal.signal(signal.SIGUSR1, usersig1)
         signal.signal(signal.SIGUSR2, usersig2)
     except:
         print("User signals may not be available.")
 
     sys.stdout = support.Unbuffered(sys.stdout)
     sys.stderr = support.Unbuffered(sys.stderr)
 
+def mainfunct():
+
+    ''' Main entry point. The pip install will call this script. '''
+
+    global args
+
+    if sys.version_info[0] < 3:
+        print("This script was meant for python 3.x")
+        time.sleep(.1)
+        sys.exit(0)
+    try:
+        args = conf.comline(sys.argv[1:])
+    except getopt.GetoptError:
+        sys.exit(1)
+    except SystemExit:
+        sys.exit(0)
+    except:
+        print(sys.exc_info())
+        sys.exit(1)
+    #print(args)
+
+    # Print comline args
+    #if conf.pgdebug > 7:
+    #    for aa in vars(conf):
+    #        if aa != "_optarr":
+    #            print(aa, "=", getattr(conf, aa), end = "    ")
+    #    print()
+
+    #if conf.pgdebug > 4:
+    #    print("This script:     ", os.path.realpath(__file__))
+    #    print("Full path argv:  ", os.path.abspath(sys.argv[0]))
+    #    print("Script name:     ", __file__)
+    #    print("Exec argv:       ", sys.argv[0])
+
+    # Just for testing
+    #pyservsup.pgdebug = conf.pgdebug
+    pyservsup.globals  = pyservsup.Global_Vars(__file__, conf.droot)
+    pyservsup.globals.conf = conf
+    pyservsup.globals.lockfname += "_" + str(conf.host) +  "_" + str(conf.port)
+    pyservsup.globals.softmkdir(pyservsup.globals.myhome)
+
+    # Change directory to the data dir
+    os.chdir(pyservsup.globals.myhome)
+    if conf.verbose:
+        print("cwd", os.getcwd())
+
+    # Create support objects
+    pyservsup.globals.config(pyservsup.globals.myhome, conf)
+    pyservsup.gl_passwd = pyservsup.Passwd()
+
+    # This is out of process, but create a 'vote' chain directory
+    # As testing will create it ... no harm
+    Vd = os.path.join(pyservsup.globals.chaindir, "vote")
+    pyservsup.globals.softmkdir(Vd)
+
+    print_stats()
+    do_keys()
+
+    set_sigs()
+
     # Comline processed, go
     support.lock_process(pyservsup.globals.lockfname)
 
     pyvfunc.pgdebug = conf.pgdebug
     pyvfunc.pglog = conf.pglog
 
     slogfile = os.path.join(pyservsup.globals.logdir, pyservsup.logfname + ".log")
     rlogfile = os.path.join(pyservsup.globals.logdir, pyservsup.repfname +".log")
 
     pysyslog.init_loggers(
             ("system", slogfile), ("replic", rlogfile))
     #pysyslog.syslog("Started Server")
 
-    if not conf.quiet:
-        if not pyservsup.globals.conf.pmode:
-            print("Warning! Devmode ON. Use -P to allow 2FA auth")
-        try:
-            import distro
-            strx = distro.name()
-        except:
-            strx = "Win or Unkn."
-
-        print("MainSiteID:      ", pyservsup.globals.siteid)
-        print("Server running: ", "'"+conf.host+"'", "Port:", conf.port)
-        pyver = support.list2str(sys.version_info) #[0:3], ".")
-        print("Running python", platform.python_version(), "on", platform.system(), strx)
-
+    signon_message()
     pyvstate.init_state_table()
 
-    # Parse multiple host (interace) options (disabled)
-    #hostarr = []
-    #import shlex
-    #hostarr = shlex.split(conf.host)
-    #print("hostarr", hostarr)
+    global SHARED_MYDATA
+    SHARED_MYDATA = pyservsup.SharedData()
+    pyservsup.SHARED_LOGINS = pyservsup.SharedData()
 
-    global server
-    try:
-        server = ThreadedTCPServer((conf.host, conf.port), ThreadedTCPRequestHandler)
-        server.allow_reuse_address = True
-        ip, port = server.server_address
-        server.allow_reuse_address = True
-        server.verbose = conf.verbose
-
-        # Start a thread with the server -- that thread will then start one
-        # or more threads for each request
-        server_thread = threading.Thread(target=server.serve_forever)
-
-        # Exit the server thread when the main thread terminates
-        server_thread.verbose = conf.verbose
-        server_thread.daemon = True
-        #server_thread.paydir =  pyservsup.globals.paydir
-        server_thread.start()
-
-    except:
-        print( "Cannot start server. ", sys.exc_info())
-        if conf.pglog > 0:
-            pysyslog.syslog("Cannot start server ", sys.exc_info())
-            #print("Try again later.")
-            #terminate(None, None)
-            sys.exit(1)
-
-    #if conf.pglog > 0:
-    #     pysyslog.syslog("Started Server")
+    start_server()
 
     if conf.pglog > 0:
         pysyslog.syslog("Server started. Prodmode %d" % conf.pmode)
 
-    #simple_server(HOST, PORT)
     # Block
-    server.serve_forever()
-
-    #if conf.detach:
-    #    print("Detach from terminal:)
-
+    gl_server.serve_forever()
 
 if __name__ == '__main__':
     mainfunct()
 
-# EOF
+# EOF
```

### Comparing `pyvserv-1.0.3/pyvserver/pyvstate.py` & `pyvserv-1.0.4/pyvserver/pyvstate.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,140 +42,135 @@
 
 # The commands in this state do not set new state
 none_in      = 120
 
 # ------------------------------------------------------------------------
 # Help stings
 
-user_help   = "Usage: user logon_name -- set session user name"
-akey_help   = "Usage: akey -- get asymmetric key"
-pass_help   = "Usage: pass logon_pass -- password"
-chpass_help = "Usage: chpass oldpass, newpass"
-file_help   = "Usage: file fname -- Specify name for upload"
-fget_help   = "Usage: fget fname -- Download (get) file"
-fput_help   = "Usage: fput fname -- Upload (put) file"
-del_help    = "Usage: del  fname -- Delete file"
-uadd_help   = "Usage: uadd user_name user_pass -- Create new user"
-#kadd_help   = "Usage: kadd key_name key_val -- Add new encryption key"
-uini_help   = "Usage: uini user_name user_pass -- Create initial user. "\
-                "Must be from local net."
-#kini_help  = "Usage: kini key_name key_pass -- Create initial key. " \
-#                "Must be from local net."
-uena_help  = "Usage: uena user_name  flag --  enable / disable user"
-aadd_help  = "Usage: aadd user_name user_pass -- create admin user"
-udel_help  = "Usage: udel user_name -- Delete user"
-data_help  = "Usage: data datalen -- Specify length of file to follow"
-vers_help  = "Usage: ver -- Get protocol version. alias: vers"
-id_help    = "Usage: id -- Get site id string"
-hello_help = "Usage: hello -- Say Hello - test connectivity."
-quit_help  = "Usage: quit -- Terminate connection. alias: exit"
-help_help  = "Usage: help [command] -- Offer help on command"
-lsls_help  = "Usage: ls [dir] -- List files in dir"
-lsld_help  = "Usage: lsd [dir] -- List dirs in dir"
-cdcd_help  = "Usage: cd dir -- Change to dir. Capped to server root"
-pwdd_help  = "Usage: pwd -- Show current dir"
-stat_help  = "Usage: stat fname  -- Get file stat. Field list:\n"\
-    "   1.  ST_MODE Inode protection mode.\n"\
-    "   2.  ST_INO Inode number.\n"\
-    "   3.  ST_DEV Device inode resides on.\n"\
-    "   4.  ST_NLINK  Number of links to the inode.\n"\
-    "   5.  ST_UID User id of the owner.\n"\
-    "   6.  ST_GID Group id of the owner.\n"\
-    "   7.  ST_SIZE Size in bytes of a plain file.\n"\
-    "   8.  ST_ATIME Time of last access.\n"\
-    "   9.  ST_MTIME Time of last modification.\n"\
-    "   10. ST_CTIME Time of last metadata change."
-tout_help  = "Usage: tout new_val -- Set / Reset timeout in seconds"
-ekey_help  = "Usage: ekey encryption_key -- Set encryption key "
-sess_help  = "Usage: sess session data -- Start session "
-logout_help = "Usage: logout -- log out user"
-buff_help  = "Usage: buff buff_size -- limited to 64k"
-
-rput_help  =  "Usage: rcheck kind link | sum -- check records. Link check or sum check"
-rcheck_help = "Usage: rput kind header, [field1, field2] ... -- put record in blockcain."
-rlist_help =  "Usage: rlist kind beg_date end_date -- get records from blockcain."
-rcount_help=  "Usage: rcount kind beg_date end_date -- get record count from blockcain."
-rsize_help =  "Usage: rsize kind -- get total record count from blockcain."
-rget_help  =  "Usage: rget kind header -- get record from blockcain."
-rhave_help =  "Usage: rhave kind header -- is record in blockcain."
-
-qr_help    = "Usage: qr -- get qrcode image for 2fa"
-twofa_help = "Usage: twofa -- two factor authentication"
-dmode_help = "Usage: dmode -- get dmode (Developer Mode) flag"
-ihave_help = "Usage: ihave -- 'i have you have' protocol entry point"
-ihost_help = "Usage: ihost -- add / delete replicator host"
-xxxx_help  = "Usage: no data -- Template for new halp"
+usage = "Usage:"
+user_help   = usage + " user logon_name -- set session user name"
+akey_help   = usage + " akey -- get asymmetric key"
+pass_help   = usage + " pass logon_pass -- password"
+chpass_help = usage + " chpass user  oldpass, newpass"
+file_help   = usage + " file fname -- Specify name for upload"
+mkdir_help  = usage + " mkdir dirname -- Specify name for new dir"
+rmdir_help  = usage + " rmdir dirname -- Specify dir name to delete"
+fget_help   = usage + " fget fname -- Download (get) file"
+fput_help   = usage + " fput fname -- Upload (put) file"
+del_help    = usage + " del  fname -- Delete file"
+uadd_help   = usage + " uadd user_name user_pass -- Create new user"
+uini_help   = usage + " uini user_name user_pass -- Create initial user. Loopback only."
+uena_help   = usage + " uena user_name  flag -- enable / disable user"
+ulist_help  = usage + " ulist flag  -- list users. Flag: user / admin / initial / disabled"
+aadd_help   = usage + " aadd user_name user_pass -- create admin user"
+udel_help   = usage + " udel user_name -- Delete user"
+data_help   = usage + " data datalen -- Specify length of file to follow"
+vers_help   = usage + " ver -- Get server version."
+id_help     = usage + " id -- Get site id string"
+hello_help  = usage + " hello -- Say Hello - test connectivity."
+quit_help   = usage + " quit -- Terminate connection. alias: exit"
+exit_help   = usage + " exit -- Terminate connection. alias: quit"
+help_help   = usage + " help [command] -- Offer help on command"
+lsls_help   = usage + " ls [dir] -- List files in dir"
+lsld_help   = usage + " lsd [dir] -- List dirs in dir"
+cdcd_help   = usage + " cd dir -- Change to dir. Capped to server root"
+pwdd_help   = usage + " pwd -- Show current dir"
+tout_help   = usage + " tout [val] -- Get / Set timeout value. (seconds)"
+ekey_help   = usage + " ekey encryption_key -- Set encryption key "
+sess_help   = usage + " sess session data -- Start session "
+logout_help = usage + " logout -- log out user"
+buff_help   = usage + " buff buff_size -- limited to 64k"
+throt_help  = usage + " throt flag -- turn on or off throttling"
+rput_help   = usage + " rcheck kind link | sum -- check records. Link check or sum check"
+rtest_help  = usage + " rtest link | sum recids -- check a list of records. Link check or sum check"
+rcheck_help = usage + " rput kind header, [field1, field2] ... -- put record in blockchain."
+rlist_help  = usage + " rlist kind beg_date end_date -- get records from blockchain."
+rcount_help = usage + " rcount kind beg_date end_date -- get record count from blockchain."
+rsize_help  = usage + " rsize kind -- get total record count from blockchain."
+rget_help   = usage + " rget kind header -- get record from blockchain."
+rabs_help   = usage + " rabs kind pos -- get record by absolute position from blockchain."
+rhave_help  = usage + " rhave kind header -- is record in blockchain."
+qr_help     = usage + " qr -- get QR code image for 2fa"
+twofa_help  = usage + " twofa pass -- two factor authentication credentials"
+dmode_help  = usage + " dmode -- get current dmode (Developer Mode) flag"
+ihost_help  = usage + " ihost -- add / del / list 'host:port' replicator host."
+stat_help   = usage + " stat fname  -- Get file stat"
+xxxx_help   = usage + " no data -- Template for new help"
 
 # ------------------------------------------------------------------------
 # Table driven server state machine.
 # The table is searched for a mathing start_state, and the corresponding
 # function is executed. The new state set to end_state
 
 def init_state_table():
 
-    global state_table
+    ''' Initialize state table '''
+
     #print("pystate init table")
+    global state_table
+
     # This is to develop without entering auth code every time
     if not pyservsup.globals.conf.pmode:
         minauth =  auth_pass
     else:
         minauth =  auth_twofa
 
     state_table = \
     [
-        # Command; start_state; end_state; min_auth; action func;   help func
-        ("ver",     all_in,     none_in,    initial,  get_ver_func,   vers_help),
-        ("id",      all_in,     none_in,    initial,  get_id_func,    id_help),
-        ("hello",   all_in,     none_in,    initial,  get_hello_func, hello_help),
-        ("helo",    all_in,     none_in,    initial,  get_hello_func, hello_help),
-        ("quit",    all_in,     none_in,    initial,  get_exit_func,  quit_help),
-        ("exit",    all_in,     none_in,    initial,  get_exit_func,  quit_help),
-        ("help",    all_in,     none_in,    initial,  get_help_func,  help_help),
-        #("xkey",    all_in,     none_in,    initial,  get_xkey_func,  ekey_help),
-        #("ekey",    all_in,     none_in,    initial,  get_ekey_func,  ekey_help),
-        ("akey",    all_in,     none_in,    initial,  get_akey_func,  akey_help),
-        ("uini",    all_in,     none_in,    initial,  get_uini_func,  uini_help),
-        #("kadd",    all_in,     none_in,    initial,  get_kadd_func,  kadd_help),
-        ("user",    all_in,     none_in,    initial,  get_user_func,  user_help),
-        ("pass",    all_in,     auth_pass,  initial,  get_pass_func,  pass_help),
-        ("logout",  all_in,     initial,    auth_pass,get_logout_func,  logout_help),
-        ("sess",    all_in,     none_in,    initial,  get_sess_func,  sess_help),
-        ("tout",    all_in,     none_in,    initial,  get_tout_func,  tout_help),
-        ("qr",      all_in,     none_in,    initial,  get_qr_func,    qr_help),
+        # Command; start_state; end_state; min_auth; action func;  help func
+        ("ver",     all_in,  none_in,    initial,   get_ver_func,     vers_help),
+        ("id",      all_in,  none_in,    initial,   get_id_func,      id_help),
+        ("hello",   all_in,  none_in,    initial,   get_hello_func,   hello_help),
+        ("helo",    all_in,  none_in,    initial,   get_hello_func,   hello_help),
+        ("quit",    all_in,  none_in,    initial,   get_exit_func,    quit_help),
+        ("exit",    all_in,  none_in,    initial,   get_exit_func,    exit_help),
+        ("help",    all_in,  none_in,    initial,   get_help_func,    help_help),
+        ("akey",    all_in,  none_in,    initial,   get_akey_func,    akey_help),
+        ("uini",    all_in,  none_in,    initial,   get_uini_func,    uini_help),
+        ("user",    all_in,  none_in,    initial,   get_user_func,    user_help),
+        ("pass",    all_in,  auth_pass,  initial,   get_pass_func,    pass_help),
+        ("logout",  all_in,  initial,    auth_pass, get_lout_func,    logout_help),
+        ("sess",    all_in,  none_in,    initial,   get_sess_func,    sess_help),
+        ("tout",    all_in,  none_in,    initial,   get_tout_func,    tout_help),
+        ("qr",      all_in,  none_in,    initial,   get_qr_func,      qr_help),
         ("chpass",  all_in,  none_in,    auth_pass, get_chpass_func,  chpass_help),
-        ("file",    all_in,  none_in,    auth_pass, put_file_func, file_help),
-        ("mkdir",   all_in,  none_in,    auth_pass, get_mkdir_func, file_help),
-        ("data",    all_in,  none_in,    auth_pass, put_data_func,  data_help),
-        ("fget",    all_in,  none_in,    auth_pass, get_fget_func,  fget_help),
-        ("fput",    all_in,  none_in,    auth_pass, get_fput_func,  fput_help),
-        ("del",     all_in,  none_in,    auth_pass, get_del_func,   del_help),
-        ("uadd",    all_in,  none_in,    auth_pass, get_uadd_func,  uadd_help),
-        ("uena",    all_in,  none_in,    auth_pass, get_uena_func,  uena_help),
-        ("aadd",    all_in,  none_in,    auth_pass, get_aadd_func,  aadd_help),
-        ("udel",    all_in,  none_in,    auth_pass, get_udel_func,  udel_help),
-        ("ls",      all_in,  none_in,    auth_pass, get_ls_func,    lsls_help),
-        ("lsd",     all_in,  none_in,    auth_pass, get_lsd_func,   lsld_help),
-        ("cd",      all_in,  none_in,    auth_pass, get_cd_func,    cdcd_help),
-        ("pwd",     all_in,  none_in,    auth_pass, get_pwd_func,   pwdd_help),
-        ("stat",    all_in,  none_in,    auth_pass, get_stat_func,  stat_help),
-        ("buff",    all_in,  none_in,    auth_pass, get_buff_func,  buff_help),
-        ("twofa",   all_in,  auth_twofa, auth_pass, get_twofa_func,  twofa_help),
-
-        ("dmode",   all_in,  none_in,    initial, get_dmode_func,  dmode_help),
-        ("ihave",   all_in,  none_in,    initial, get_ihave_func,  ihave_help),
-        ("ihost",   all_in,  none_in,    initial, get_ihost_func,  ihost_help),
-
-        # Following the two factor auth commands. Disabled during development
-        ("rput",     all_in,  none_in,    minauth,   get_rput_func,   rput_help),
-        ("rcheck",   all_in,  none_in,    minauth,   get_rcheck_func,  rcheck_help),
-        ("rlist",    all_in,  none_in,    auth_pass, get_rlist_func,  rlist_help),
-        ("rcount",   all_in,  none_in,    auth_pass, get_rcount_func, rcount_help),
-        ("rsize",    all_in,  none_in,    auth_pass, get_rsize_func,  rsize_help),
-        ("rget",     all_in,  none_in,    auth_pass, get_rget_func,   rget_help),
-        ("rhave",    all_in,  none_in,    auth_pass, get_rhave_func,   rhave_help),
+        ("file",    all_in,  none_in,    auth_pass, put_file_func,    file_help),
+        ("mkdir",   all_in,  none_in,    auth_pass, get_mkdir_func,   mkdir_help),
+        ("rmdir",   all_in,  none_in,    auth_pass, get_rmdir_func,   rmdir_help),
+        ("data",    all_in,  none_in,    auth_pass, put_data_func,    data_help),
+        ("fget",    all_in,  none_in,    auth_pass, get_fget_func,    fget_help),
+        ("fput",    all_in,  none_in,    auth_pass, get_fput_func,    fput_help),
+        ("del",     all_in,  none_in,    auth_pass, get_del_func,     del_help),
+        ("uadd",    all_in,  none_in,    auth_pass, get_uadd_func,    uadd_help),
+        ("udel",    all_in,  none_in,    auth_pass, get_udel_func,    udel_help),
+        ("uena",    all_in,  none_in,    auth_pass, get_uena_func,    uena_help),
+        ("ulist",   all_in,  none_in,    auth_pass, get_ulist_func,   ulist_help),
+        ("aadd",    all_in,  none_in,    auth_pass, get_aadd_func,    aadd_help),
+        ("ls",      all_in,  none_in,    auth_pass, get_ls_func,      lsls_help),
+        ("dir",     all_in,  none_in,    auth_pass, get_ls_func,      lsls_help),
+        ("lsd",     all_in,  none_in,    auth_pass, get_lsd_func,     lsld_help),
+        ("cd",      all_in,  none_in,    auth_pass, get_cd_func,      cdcd_help),
+        ("pwd",     all_in,  none_in,    auth_pass, get_pwd_func,     pwdd_help),
+        ("stat",    all_in,  none_in,    auth_pass, get_stat_func,    stat_help),
+        ("buff",    all_in,  none_in,    auth_pass, get_buff_func,    buff_help),
+        ("throt",   all_in,  none_in,    auth_pass, get_throt_func,   throt_help),
+        ("twofa",   all_in,  auth_twofa, auth_pass, get_twofa_func,   twofa_help),
+        ("dmode",   all_in,  none_in,    initial,   get_dmode_func,   dmode_help),
+        ("ihost",   all_in,  none_in,    initial,   get_ihost_func,   ihost_help),
+        ("rlist",    all_in,  none_in,   auth_pass, get_rlist_func,   rlist_help),
+        ("rcount",   all_in,  none_in,   auth_pass, get_rcount_func,  rcount_help),
+        ("rsize",    all_in,  none_in,   auth_pass, get_rsize_func,   rsize_help),
+        ("rget",     all_in,  none_in,   auth_pass, get_rget_func,    rget_help),
+        ("rabs",     all_in,  none_in,   auth_pass, get_rabs_func,    rabs_help),
+        ("rhave",    all_in,  none_in,   auth_pass, get_rhave_func,   rhave_help),
+        ("rtest",    all_in,  none_in,   auth_pass, get_rtest_func, rtest_help),
+
+        # The two factor auth commands. 2FA not required during development
+        ("rput",     all_in,  none_in,   minauth,   get_rput_func,   rput_help),
+        ("rcheck",   all_in,  none_in,   minauth,   get_rcheck_func, rcheck_help),
     ]
 # ------------------------------------------------------------------------
 
 class StateHandler():
 
     def __init__(self, resp):
 
@@ -310,15 +305,14 @@
         # Not found in the state table for the current state, complain
         if not got:
             #print( "Invalid command or out of sequence command ", "'" + comx[0] + "'")
             if not comok:
                 sss =  ["ERR", "Invalid command issued",  comx[0]]
             else:
                 sss =  ["ERR", "Out of Sequence command issued", comx[0]]
-            #self.resp.datahandler.putdata(sss.encode("cp437"), self.resp.ekey)
             self.resp.datahandler.putencode(sss, self.resp.ekey)
             # Do not quit, just signal the error
             ret = False
         return ret
 
     def __del(self):
         print("del state handler")
```

### Comparing `pyvserv-1.0.3/pyvtools/pyvgenkey.py` & `pyvserv-1.0.4/pyvtools/pyvgenkey.py`

 * *Files identical despite different names*

### Comparing `pyvserv-1.0.3/pyvtools/pyvgenkeys.py` & `pyvserv-1.0.4/pyvtools/pyvgenkeys.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
     #sys.path.append(os.path.join(base, "..", "pyvgui"))
     #sys.path.append(os.path.join(base, "..", "pyvgui", "guilib"))
     from pyvcommon import support
 
 #for aa in sys.path:
 #    print(aa)
 
-print("Load:", sys.path[-1])
+#print("Load:", sys.path[-1])
 
 import pyvgenkey
 import argparse
 
 parser = argparse.ArgumentParser(description='Genetrate ECC keypair for pyvserv.')
 
 parser.add_argument("-v", '--verbose', dest='verbose',
```

### Comparing `pyvserv-1.0.3/setup.py` & `pyvserv-1.0.4/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,132 +1,155 @@
+import sys, os
 import setuptools
 
 descx = '''
         pyvserv is modern multi-process data server.
         '''
 
 classx = [
-          'Development Status :: Mature',
-          'Environment :: GUI',
+          'Development Status :: 6 - Mature',
           'Intended Audience :: End Users/Desktop',
           'Intended Audience :: Developers',
           'Intended Audience :: System Administrators',
           'License :: OSI Approved :: Python Software Foundation License',
           'Operating System :: Microsoft :: Windows',
           'Operating System :: POSIX',
           'Programming Language :: Python',
-          'Topic :: Editors',
           'Topic :: Software Development :: Servers',
         ]
 
 includex = ["*", "pyvgui/", "pyvgui/guilib/", "pyvclient/", "pyvserver/",
                     "pyvcommon/", "pyvtools/", ]
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 # The shortlist of starter applications
 
 test_root = [\
-"pyvcli_cli",
-"pyvcli_gethelp",
-"pyvcli_hello",
-"pyvcli_rget",
-"pyvcli_rlist",
-"pyvcli_rput",
-"pyvcli_uini",
-"pyvcli_uman",
-"pyvcli_qr",
-]
+    "pyvcli_cli",
+    "pyvcli_gethelp",
+    "pyvcli_ver",
+    "pyvcli_hello",
+    "pyvcli_uini",
+    "pyvcli_uman",
+    "pyvcli_fman",
+    "pyvcli_rman",
+    "pyvcli_qr",
+    "pyvcli_ihost",
+    "pyvcli_replic",
+    ]
 
-# Generate script details
-
-test_scripts = []
+# Generate script and loadable details
+test_scripts = []; test_exec = []
 for aa in test_root:
     test_scripts.append("pyvclient/" + aa + ".py")
-#print(test_scripts)
-
-test_exec = []
-for aa in test_root:
     test_exec.append(aa+"="+aa+":mainfunct")
-#print(test_exec)
 
-# Get it from main file:
-fp = open("pyvserver/pyvserv.py", "rt")
+#print(test_scripts); #print(test_exec)
+
+# Get version number  from the server support file:
+fp = open("pyvcommon/pyservsup.py", "rt")
 vvv = fp.read(); fp.close()
 loc_vers =  '1.0.0'     # Default
 for aa in vvv.split("\n"):
     idx = aa.find("version =")
-    if idx == 0:        # At th beginning of line
+    if idx == 0:        # At the beginning of line
         try:
             loc_vers = aa.split()[2].replace('"', "")
             break
         except:
             pass
 #print("loc_vers:", loc_vers)
 
-# Dependency list, generate for windows
+# Dependency list, generate separate for windows
+# Sat 06.Apr.2024 same for all
 try:
     import fcntl
     #deplist = ["pyvpacker", "pydbase", "pycryptodome",
     #                    "pyvecc", "pyvguicom", "readline"],
 
     # Thu 04.Apr.2024 abandoned readline; may install by hand
     deplist = ["pyvpacker", "pydbase", "pycryptodome",
                         "pyvecc", "pyvguicom", ],
 except:
+    # No fnctl, windows
     deplist = ["pyvpacker", "pydbase", "pycryptodome",
                         "pyvecc", "pyvguicom"],
 
+doclist = []; droot = "pyvserver/docs/"
+doclistx = os.listdir(droot)
+for aa in doclistx:
+    doclist.append("docs/" + aa)
+
+cdoclist = []; droot2 = "pyvclient/docs/"
+cdoclistx = os.listdir(droot2)
+for aa in cdoclistx:
+    cdoclist.append("docs/" + aa)
+
+tdoclist = []; droot3 = "pyvtools/docs/"
+tdoclistx = os.listdir(droot3)
+for aa in tdoclistx:
+    tdoclist.append("docs/" + aa)
+
+# This was needed to verify lists ...
+#print("includex:", includex)
+#print("find packages:", setuptools.find_packages(include=includex))
+#print("deplist:", deplist)
+#print("doclist:", doclist)
+#print("cdoclist:", cdoclist)
+#print("tdoclist:", tdoclist)
+#sys.exit(1)
+
 setuptools.setup(
     name="pyvserv",
     version=loc_vers,
     author="Peter Glen",
     author_email="peterglen99@gmail.com",
     description="High power secure server with blockchain backend.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pglen/pyvserv",
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
-    include_package_data=True,
     packages=setuptools.find_packages(include=includex),
-
+    include_package_data = True,
     scripts = [
                 "pyvserver/pyvserv.py",
                 "pyvserver/pyvreplic.py",
-                "pyvserver/pyvpuller.py",
                 "pyvtools/pyvgenkey.py", "pyvtools/pyvgenkeys.py",
                 "pyvgui/pyvservui.py", "pyvgui/pyvcpanel.py",
                 "pyvgui/pyvtally.py",
                 *test_scripts,
                 ],
-
     package_dir = {
                     'pyvgui':           'pyvgui',
                     'pyvgui/guilib':    'pyvgui/guilib',
                     'pyvcommon':        'pyvcommon',
                     'pyvserver':        'pyvserver',
                     'pyvclient':        'pyvclient',
                     'pyvtools':         'pyvtools',
                    },
 
+    package_data = {    "pyvserver" :  doclist,
+                        "pyvclient" : cdoclist,
+                        "pyvtools"  : tdoclist,
+                   },
     python_requires='>=3',
     install_requires=deplist,
     entry_points={
         'console_scripts': [ "pyvserv=pyvserv:mainfunct",
                              "pyvreplic=pyvreplic:mainfunct",
                              "pyvgenkey=pyvgenkey:mainfunct",
                              "pyvgenkeys=pyvgenkeys:mainfunct",
                              "pyvservui=pyvservui:mainfunct",
                              "pyvcpanel=pyvcpanel:mainfunct",
                              "pyvtally=pyvtally:mainfunct",
-                             "pyvpuller=pyvpuller:mainfunct",
                              test_exec,
             ],
     },
 )
 
 # EOF
```

