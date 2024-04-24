# Comparing `tmp/perun.proxygui-5.1.0.tar.gz` & `tmp/perun.proxygui-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxygui-5.1.0.tar", last modified: Wed Apr 24 09:26:48 2024, max compression
+gzip compressed data, was "perun.proxygui-5.1.1.tar", last modified: Wed Apr 24 09:58:03 2024, max compression
```

## Comparing `perun.proxygui-5.1.0.tar` & `perun.proxygui-5.1.1.tar`

### file list

```diff
@@ -1,291 +1,292 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.328771 perun.proxygui-5.1.0/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/LICENSE
--rw-rw-rw-   0     1001 root         (0)       46 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/MANIFEST.in
--rw-r--r--   0     1001 root         (0)     9351 2024-04-24 09:26:48.328771 perun.proxygui-5.1.0/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)     8072 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/proxygui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/__init__.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.248772 perun.proxygui-5.1.0/perun/proxygui/api/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/api/__init__.py
--rw-rw-rw-   0     1001 root         (0)     2478 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/api/backchannel_logout_api.py
--rw-rw-rw-   0     1001 root         (0)     4517 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/api/ban_api.py
--rw-rw-rw-   0     1001 root         (0)     4900 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/api/consent_api.py
--rw-rw-rw-   0     1001 root         (0)    10671 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/api/heuristic_api.py
--rw-rw-rw-   0     1001 root         (0)     3089 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/api/kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)     6919 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/app.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.248772 perun.proxygui-5.1.0/perun/proxygui/gui/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/__init__.py
--rw-rw-rw-   0     1001 root         (0)    21850 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/gui.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.248772 perun.proxygui-5.1.0/perun/proxygui/gui/static/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.240772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.240772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.248772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.248772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
--rw-rw-rw-   0     1001 root         (0)   141520 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)       99 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
--rw-rw-rw-   0     1001 root         (0)      612 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
--rw-rw-rw-   0     1001 root         (0)       67 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.248772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
--rw-rw-rw-   0     1001 root         (0)      688 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
--rw-rw-rw-   0     1001 root         (0)       19 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)      949 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
--rw-rw-rw-   0     1001 root         (0)     1663 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.248772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
--rw-rw-rw-   0     1001 root         (0)      477 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.240772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.252772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
--rw-rw-rw-   0     1001 root         (0)      631 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
--rw-rw-rw-   0     1001 root         (0)     1451 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
--rw-rw-rw-   0     1001 root         (0)     3089 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
--rw-rw-rw-   0     1001 root         (0)     1617 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
--rw-rw-rw-   0     1001 root         (0)     1776 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
--rw-rw-rw-   0     1001 root         (0)      437 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
--rw-rw-rw-   0     1001 root         (0)      387 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
--rw-rw-rw-   0     1001 root         (0)     2945 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
--rw-rw-rw-   0     1001 root         (0)     2624 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
--rw-rw-rw-   0     1001 root         (0)      713 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
--rw-rw-rw-   0     1001 root         (0)     1899 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.252772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
--rw-rw-rw-   0     1001 root         (0)      815 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
--rw-rw-rw-   0     1001 root         (0)      571 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.252772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
--rw-rw-rw-   0     1001 root         (0)      421 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
--rw-rw-rw-   0     1001 root         (0)      403 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
--rw-rw-rw-   0     1001 root         (0)     2758 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.252772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
--rw-rw-rw-   0     1001 root         (0)      198 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
--rw-rw-rw-   0     1001 root         (0)      684 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
--rw-rw-rw-   0     1001 root         (0)    29997 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
--rw-rw-rw-   0     1001 root         (0)      244 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.240772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.256772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
--rw-rw-rw-   0     1001 root         (0)    22637 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
--rw-rw-rw-   0     1001 root         (0)    21057 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
--rw-rw-rw-   0     1001 root         (0)    22481 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
--rw-rw-rw-   0     1001 root         (0)    35533 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
--rw-rw-rw-   0     1001 root         (0)    34805 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
--rw-rw-rw-   0     1001 root         (0)    28733 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
--rw-rw-rw-   0     1001 root         (0)    20267 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28025 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
--rw-rw-rw-   0     1001 root         (0)    25884 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
--rw-rw-rw-   0     1001 root         (0)   363233 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
--rw-rw-rw-   0     1001 root         (0)    27013 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
--rw-rw-rw-   0     1001 root         (0)    33321 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
--rw-rw-rw-   0     1001 root         (0)    31511 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
--rw-rw-rw-   0     1001 root         (0)    34010 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
--rw-rw-rw-   0     1001 root         (0)    28152 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
--rw-rw-rw-   0     1001 root         (0)    36726 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
--rw-rw-rw-   0     1001 root         (0)    28663 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
--rw-rw-rw-   0     1001 root         (0)    22030 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.264772 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.280771 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/
--rw-rw-rw-   0     1001 root         (0)   125046 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
--rw-rw-rw-   0     1001 root         (0)   252563 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
--rw-rw-rw-   0     1001 root         (0)  1052500 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
--rw-rw-rw-   0     1001 root         (0)  1125125 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
--rw-rw-rw-   0     1001 root         (0)  1125144 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
--rw-rw-rw-   0     1001 root         (0)  1125123 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
--rw-rw-rw-   0     1001 root         (0)  1125119 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
--rw-rw-rw-   0     1001 root         (0)  1125120 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
--rw-rw-rw-   0     1001 root         (0)  1125147 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
--rw-rw-rw-   0     1001 root         (0)  1125545 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
--rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
--rw-rw-rw-   0     1001 root         (0)  1126098 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
--rw-rw-rw-   0     1001 root         (0)   139176 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
--rw-rw-rw-   0     1001 root         (0)     2596 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css
--rw-rw-rw-   0     1001 root         (0)    48080 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/print.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.288771 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/
--rw-rw-rw-   0     1001 root         (0)     2596 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
--rw-rw-rw-   0     1001 root         (0)    46987 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
--rw-rw-rw-   0     1001 root         (0)   303728 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   332353 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   332557 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
--rw-rw-rw-   0     1001 root         (0)     5778 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
--rw-rw-rw-   0     1001 root         (0)   312236 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
--rw-rw-rw-   0     1001 root         (0)   341456 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
--rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
--rw-rw-rw-   0     1001 root         (0)   341664 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style.css
--rw-rw-rw-   0     1001 root         (0)     5772 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.288771 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/
--rw-rw-rw-   0     1001 root         (0)    87048 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    74284 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)   208892 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
--rw-rw-rw-   0     1001 root         (0)   159376 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
--rw-rw-rw-   0     1001 root         (0)     1632 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
--rw-rw-rw-   0     1001 root         (0)     1837 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
--rw-rw-rw-   0     1001 root         (0)     1484 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
--rw-rw-rw-   0     1001 root         (0)      988 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
--rw-rw-rw-   0     1001 root         (0)    12252 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
--rw-rw-rw-   0     1001 root         (0)     9596 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.288771 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.292771 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/
--rw-rw-rw-   0     1001 root         (0)    70841 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
--rw-rw-rw-   0     1001 root         (0)     4348 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
--rw-rw-rw-   0     1001 root         (0)      151 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
--rw-rw-rw-   0     1001 root         (0)      279 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
--rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
--rw-rw-rw-   0     1001 root         (0)      281 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
--rw-rw-rw-   0     1001 root         (0)      280 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
--rw-rw-rw-   0     1001 root         (0)      149 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
--rw-rw-rw-   0     1001 root         (0)      304 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
--rw-rw-rw-   0     1001 root         (0)     7406 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
--rw-rw-rw-   0     1001 root         (0)     4426 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
--rw-rw-rw-   0     1001 root         (0)      443 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/logo.svg
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.296771 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/
--rw-rw-rw-   0     1001 root         (0)   218591 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js
--rw-rw-rw-   0     1001 root         (0)   659454 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map
--rw-rw-rw-   0     1001 root         (0)   337945 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/d3.js
--rw-rw-rw-   0     1001 root         (0)     2707 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js
--rw-rw-rw-   0     1001 root         (0)     8806 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js
--rw-rw-rw-   0     1001 root         (0)    26171 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
--rw-rw-rw-   0     1001 root         (0)     4075 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
--rw-rw-rw-   0     1001 root         (0)   284394 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js
--rw-rw-rw-   0     1001 root         (0)   610160 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.296771 perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/css/
--rw-rw-rw-   0     1001 root         (0)   155845 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
--rw-rw-rw-   0     1001 root         (0)   431289 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.296771 perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/js/
--rw-rw-rw-   0     1001 root         (0)    78743 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-rw-   0     1001 root         (0)   325834 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-rw-   0     1001 root         (0)       78 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/campus-idp-muni.js
--rw-rw-rw-   0     1001 root         (0)     7336 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/campus-idp.css
--rw-rw-rw-   0     1001 root         (0)     4859 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/campus-idp.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.296771 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/css/
--rw-rw-rw-   0     1001 root         (0)    73577 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/css/all.css
--rw-rw-rw-   0     1001 root         (0)    59305 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/css/all.min.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.320771 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/
--rw-rw-rw-   0     1001 root         (0)   134294 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
--rw-rw-rw-   0     1001 root         (0)   747927 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
--rw-rw-rw-   0     1001 root         (0)   133988 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
--rw-rw-rw-   0     1001 root         (0)    89988 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
--rw-rw-rw-   0     1001 root         (0)    76736 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
--rw-rw-rw-   0     1001 root         (0)    34034 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
--rw-rw-rw-   0     1001 root         (0)   144714 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
--rw-rw-rw-   0     1001 root         (0)    33736 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
--rw-rw-rw-   0     1001 root         (0)    16276 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
--rw-rw-rw-   0     1001 root         (0)    13224 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
--rw-rw-rw-   0     1001 root         (0)   203030 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
--rw-rw-rw-   0     1001 root         (0)   918991 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
--rw-rw-rw-   0     1001 root         (0)   202744 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
--rw-rw-rw-   0     1001 root         (0)   101648 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
--rw-rw-rw-   0     1001 root         (0)    78268 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.320771 perun.proxygui-5.1.0/perun/proxygui/gui/static/images/
--rw-rw-rw-   0     1001 root         (0)      490 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/images/check.svg
--rw-rw-rw-   0     1001 root         (0)      536 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/images/circle-check-regular.svg
--rw-rw-rw-   0     1001 root         (0)      483 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
--rw-rw-rw-   0     1001 root         (0)      730 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/images/questionmark.svg
--rw-rw-rw-   0     1001 root         (0)      625 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/images/spinner.svg
--rw-rw-rw-   0     1001 root         (0)    89501 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/jquery-3.6.0.min.js
--rw-rw-rw-   0     1001 root         (0)      627 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/proxygui.css
--rw-rw-rw-   0     1001 root         (0)     1427 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/proxygui.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.320771 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/
--rw-rw-rw-   0     1001 root         (0)    15836 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
--rw-rw-rw-   0     1001 root         (0)     8266 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
--rw-rw-rw-   0     1001 root         (0)     8862 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
--rw-rw-rw-   0     1001 root         (0)     8873 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
--rw-rw-rw-   0     1001 root         (0)     7692 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.css
--rw-rw-rw-   0     1001 root         (0)     8344 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.default.css
--rw-rw-rw-   0     1001 root         (0)    11438 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/js/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.320771 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/js/standalone/
--rw-rw-rw-   0     1001 root         (0)    64906 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.324771 perun.proxygui-5.1.0/perun/proxygui/gui/templates/
--rw-rw-rw-   0     1001 root         (0)    15205 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/ConsentRegistration.html
--rw-rw-rw-   0     1001 root         (0)     9192 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/HeuristicData.html
--rw-rw-rw-   0     1001 root         (0)      747 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/IsTestingSP.html
--rw-rw-rw-   0     1001 root         (0)     3091 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/Logout.html
--rw-rw-rw-   0     1001 root         (0)     1131 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResetEmailSent.html
--rw-rw-rw-   0     1001 root         (0)     1942 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResetInitiated.html
--rw-rw-rw-   0     1001 root         (0)     1133 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
--rw-rw-rw-   0     1001 root         (0)     1021 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResult.html
--rw-rw-rw-   0     1001 root         (0)      795 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/MissingAuth.html
--rw-rw-rw-   0     1001 root         (0)     1019 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/OidcError.html
--rw-rw-rw-   0     1001 root         (0)     1223 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/Post-logout.html
--rw-rw-rw-   0     1001 root         (0)      907 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/SPAuthorization.html
--rw-rw-rw-   0     1001 root         (0)     2490 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/_footer.html
--rw-rw-rw-   0     1001 root         (0)     8119 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/_header.html
--rw-rw-rw-   0     1001 root         (0)     1175 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/authorization.html
--rw-rw-rw-   0     1001 root         (0)     3477 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/base.html
--rw-rw-rw-   0     1001 root         (0)      561 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/logout-iframe.html
--rw-rw-rw-   0     1001 root         (0)     3769 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/templates/logout-state.html
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/proxygui/gui/translations/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun/proxygui/gui/translations/cs/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.324771 perun.proxygui-5.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/
--rw-rw-rw-   0     1001 root         (0)     2973 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
--rw-rw-rw-   0     1001 root         (0)     8108 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
--rw-rw-rw-   0     1001 root         (0)     5372 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/jwt.py
--rw-rw-rw-   0     1001 root         (0)    20220 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/logout_manager.py
--rw-rw-rw-   0     1001 root         (0)     2480 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/oauth.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.324771 perun.proxygui-5.1.0/perun/proxygui/openapi/
--rw-rw-rw-   0     1001 root         (0)     6107 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/openapi/openapi.py
--rw-rw-rw-   0     1001 root         (0)    12933 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/openapi/openapi_data.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.324771 perun.proxygui-5.1.0/perun/proxygui/openapi/schemas/
--rw-rw-rw-   0     1001 root         (0)      997 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/openapi/schemas/arguments_schemas.py
--rw-rw-rw-   0     1001 root         (0)     1446 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/openapi/schemas/response_schemas.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.324771 perun.proxygui-5.1.0/perun/proxygui/tests/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1816 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/shared_test_data.py
--rw-rw-rw-   0     1001 root         (0)     6409 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/test_ban_api.py
--rw-rw-rw-   0     1001 root         (0)     6635 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/test_consent_api.py
--rw-rw-rw-   0     1001 root         (0)     4713 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/test_consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2160 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/test_consent_request_db.py
--rw-rw-rw-   0     1001 root         (0)     6826 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/test_gui.py
--rw-rw-rw-   0     1001 root         (0)     1111 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/tests/test_kerberos_auth_api.py
--rw-rw-rw-   0     1001 root         (0)    22361 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/proxygui/user_manager.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.328771 perun.proxygui-5.1.0/perun/utils/
--rw-rw-rw-   0     1001 root         (0)     2496 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/ConfigStore.py
--rw-rw-rw-   0     1001 root         (0)       43 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/CustomExceptions.py
--rw-rw-rw-   0     1001 root         (0)     2555 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/CustomRPHandler.py
--rw-rw-rw-   0     1001 root         (0)     1354 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/DatabaseService.py
--rw-rw-rw-   0     1001 root         (0)     4414 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/EmailService.py
--rw-rw-rw-   0     1001 root         (0)       96 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/Notification.py
--rw-rw-rw-   0     1001 root         (0)      816 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/Utils.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.328771 perun.proxygui-5.1.0/perun/utils/auth_event_loggig/
--rw-rw-rw-   0     1001 root         (0)     2070 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.328771 perun.proxygui-5.1.0/perun/utils/consent_framework/
--rw-rw-rw-   0     1001 root         (0)     1241 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/consent_framework/consent.py
--rw-rw-rw-   0     1001 root         (0)     2226 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/consent_framework/consent_db.py
--rw-rw-rw-   0     1001 root         (0)     2274 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/consent_framework/consent_manager.py
--rw-rw-rw-   0     1001 root         (0)      730 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/consent_framework/consent_request.py
--rw-rw-rw-   0     1001 root         (0)     1371 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/consent_framework/consent_request_db.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.328771 perun.proxygui-5.1.0/perun/utils/logout_requests/
--rw-rw-rw-   0     1001 root         (0)     2001 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/logout_requests/BackchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)      832 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     3841 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/logout_requests/GraphLogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     1361 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/logout_requests/LogoutRequest.py
--rw-rw-rw-   0     1001 root         (0)     2229 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/perun/utils/logout_requests/SamlLogoutRequest.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:26:48.244772 perun.proxygui-5.1.0/perun.proxygui.egg-info/
--rw-r--r--   0     1001 root         (0)     9351 2024-04-24 09:26:48.000000 perun.proxygui-5.1.0/perun.proxygui.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)    12842 2024-04-24 09:26:48.000000 perun.proxygui-5.1.0/perun.proxygui.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-04-24 09:26:48.000000 perun.proxygui-5.1.0/perun.proxygui.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)      557 2024-04-24 09:26:48.000000 perun.proxygui-5.1.0/perun.proxygui.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)        6 2024-04-24 09:26:48.000000 perun.proxygui-5.1.0/perun.proxygui.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)       90 2024-04-24 09:26:48.328771 perun.proxygui-5.1.0/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     1485 2024-04-24 09:26:07.000000 perun.proxygui-5.1.0/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.874444 perun.proxygui-5.1.1/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/LICENSE
+-rw-rw-rw-   0     1001 root         (0)       46 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/MANIFEST.in
+-rw-r--r--   0     1001 root         (0)     9351 2024-04-24 09:58:03.874444 perun.proxygui-5.1.1/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)     8072 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/__init__.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/api/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/api/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     2478 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/api/backchannel_logout_api.py
+-rw-rw-rw-   0     1001 root         (0)     4517 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/api/ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     4900 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/api/consent_api.py
+-rw-rw-rw-   0     1001 root         (0)    10671 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/api/heuristic_api.py
+-rw-rw-rw-   0     1001 root         (0)     3089 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/api/kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)     6919 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/app.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/gui/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/__init__.py
+-rw-rw-rw-   0     1001 root         (0)    21869 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/gui.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/gui/static/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.822443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.822443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   141520 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)       99 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_atoms.scss
+-rw-rw-rw-   0     1001 root         (0)      612 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss
+-rw-rw-rw-   0     1001 root         (0)       67 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_organisms.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/
+-rw-rw-rw-   0     1001 root         (0)      688 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss
+-rw-rw-rw-   0     1001 root         (0)       19 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)      949 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss
+-rw-rw-rw-   0     1001 root         (0)     1663 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.830443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/
+-rw-rw-rw-   0     1001 root         (0)      477 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/lib/_icons.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.822443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.834443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/
+-rw-rw-rw-   0     1001 root         (0)      631 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss
+-rw-rw-rw-   0     1001 root         (0)     1451 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss
+-rw-rw-rw-   0     1001 root         (0)     3089 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss
+-rw-rw-rw-   0     1001 root         (0)     1617 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss
+-rw-rw-rw-   0     1001 root         (0)     1776 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss
+-rw-rw-rw-   0     1001 root         (0)      437 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_food-menu.scss
+-rw-rw-rw-   0     1001 root         (0)      387 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_images.scss
+-rw-rw-rw-   0     1001 root         (0)     2945 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss
+-rw-rw-rw-   0     1001 root         (0)     2624 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss
+-rw-rw-rw-   0     1001 root         (0)      713 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss
+-rw-rw-rw-   0     1001 root         (0)     1899 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.834443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/
+-rw-rw-rw-   0     1001 root         (0)      815 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss
+-rw-rw-rw-   0     1001 root         (0)      571 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.834443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/
+-rw-rw-rw-   0     1001 root         (0)      421 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_mega.scss
+-rw-rw-rw-   0     1001 root         (0)      403 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_primary.scss
+-rw-rw-rw-   0     1001 root         (0)     2758 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.834443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/
+-rw-rw-rw-   0     1001 root         (0)      198 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_footer.scss
+-rw-rw-rw-   0     1001 root         (0)      684 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss
+-rw-rw-rw-   0     1001 root         (0)    29997 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css
+-rw-rw-rw-   0     1001 root         (0)      244 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.scss
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.822443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.838443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/
+-rw-rw-rw-   0     1001 root         (0)    22637 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    21057 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    22481 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg
+-rw-rw-rw-   0     1001 root         (0)    35533 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    34805 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    28733 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    20267 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28025 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    25884 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg
+-rw-rw-rw-   0     1001 root         (0)   363233 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg
+-rw-rw-rw-   0     1001 root         (0)    27013 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg
+-rw-rw-rw-   0     1001 root         (0)    33321 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg
+-rw-rw-rw-   0     1001 root         (0)    31511 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg
+-rw-rw-rw-   0     1001 root         (0)    34010 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg
+-rw-rw-rw-   0     1001 root         (0)    28152 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg
+-rw-rw-rw-   0     1001 root         (0)    36726 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg
+-rw-rw-rw-   0     1001 root         (0)    28663 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg
+-rw-rw-rw-   0     1001 root         (0)    22030 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.842443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.850443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/
+-rw-rw-rw-   0     1001 root         (0)   125046 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map
+-rw-rw-rw-   0     1001 root         (0)   252563 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map
+-rw-rw-rw-   0     1001 root         (0)  1052500 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125125 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125144 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125123 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125119 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125120 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125147 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125545 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map
+-rw-rw-rw-   0     1001 root         (0)  1125121 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map
+-rw-rw-rw-   0     1001 root         (0)  1126098 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map
+-rw-rw-rw-   0     1001 root         (0)   139176 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    48080 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/print.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.854443 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/
+-rw-rw-rw-   0     1001 root         (0)     2596 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css
+-rw-rw-rw-   0     1001 root         (0)    46987 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css
+-rw-rw-rw-   0     1001 root         (0)   303728 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   332353 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   332243 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   332557 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css
+-rw-rw-rw-   0     1001 root         (0)     5778 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css
+-rw-rw-rw-   0     1001 root         (0)   312236 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css
+-rw-rw-rw-   0     1001 root         (0)   341456 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css
+-rw-rw-rw-   0     1001 root         (0)   341340 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css
+-rw-rw-rw-   0     1001 root         (0)   341664 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style.css
+-rw-rw-rw-   0     1001 root         (0)     5772 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.858444 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/
+-rw-rw-rw-   0     1001 root         (0)    87048 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    74284 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   208892 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff
+-rw-rw-rw-   0     1001 root         (0)   159376 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2
+-rw-rw-rw-   0     1001 root         (0)     1632 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot
+-rw-rw-rw-   0     1001 root         (0)     1837 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg
+-rw-rw-rw-   0     1001 root         (0)     1484 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf
+-rw-rw-rw-   0     1001 root         (0)      988 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff
+-rw-rw-rw-   0     1001 root         (0)    12252 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff
+-rw-rw-rw-   0     1001 root         (0)     9596 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.858444 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.858444 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/
+-rw-rw-rw-   0     1001 root         (0)    70841 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg
+-rw-rw-rw-   0     1001 root         (0)     4348 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif
+-rw-rw-rw-   0     1001 root         (0)      151 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/ico-external.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ciisb.png
+-rw-rw-rw-   0     1001 root         (0)      279 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-crc.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-econ.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fi.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fsps.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-fss.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-law.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-med.png
+-rw-rw-rw-   0     1001 root         (0)      282 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-ped.png
+-rw-rw-rw-   0     1001 root         (0)      281 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-phil.png
+-rw-rw-rw-   0     1001 root         (0)      280 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-sci.png
+-rw-rw-rw-   0     1001 root         (0)      149 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select-small.png
+-rw-rw-rw-   0     1001 root         (0)      304 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/select.png
+-rw-rw-rw-   0     1001 root         (0)     7406 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico
+-rw-rw-rw-   0     1001 root         (0)     4426 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png
+-rw-rw-rw-   0     1001 root         (0)      443 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/logo.svg
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.862444 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/
+-rw-rw-rw-   0     1001 root         (0)   218591 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js
+-rw-rw-rw-   0     1001 root         (0)   659454 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map
+-rw-rw-rw-   0     1001 root         (0)   337945 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/d3.js
+-rw-rw-rw-   0     1001 root         (0)     2707 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js
+-rw-rw-rw-   0     1001 root         (0)     8806 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js
+-rw-rw-rw-   0     1001 root         (0)    26171 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js
+-rw-rw-rw-   0     1001 root         (0)     4075 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js
+-rw-rw-rw-   0     1001 root         (0)   284394 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js
+-rw-rw-rw-   0     1001 root         (0)   610160 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.862444 perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/css/
+-rw-rw-rw-   0     1001 root         (0)   155845 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css
+-rw-rw-rw-   0     1001 root         (0)   431289 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.862444 perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/js/
+-rw-rw-rw-   0     1001 root         (0)    78743 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-rw-   0     1001 root         (0)   325834 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-rw-   0     1001 root         (0)       78 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/campus-idp-muni.js
+-rw-rw-rw-   0     1001 root         (0)     7336 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/campus-idp.css
+-rw-rw-rw-   0     1001 root         (0)     4859 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/campus-idp.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.862444 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/css/
+-rw-rw-rw-   0     1001 root         (0)    73577 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/css/all.css
+-rw-rw-rw-   0     1001 root         (0)    59305 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/css/all.min.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.866444 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/
+-rw-rw-rw-   0     1001 root         (0)   134294 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot
+-rw-rw-rw-   0     1001 root         (0)   747927 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg
+-rw-rw-rw-   0     1001 root         (0)   133988 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    89988 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff
+-rw-rw-rw-   0     1001 root         (0)    76736 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2
+-rw-rw-rw-   0     1001 root         (0)    34034 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot
+-rw-rw-rw-   0     1001 root         (0)   144714 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg
+-rw-rw-rw-   0     1001 root         (0)    33736 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf
+-rw-rw-rw-   0     1001 root         (0)    16276 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff
+-rw-rw-rw-   0     1001 root         (0)    13224 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2
+-rw-rw-rw-   0     1001 root         (0)   203030 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot
+-rw-rw-rw-   0     1001 root         (0)   918991 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg
+-rw-rw-rw-   0     1001 root         (0)   202744 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf
+-rw-rw-rw-   0     1001 root         (0)   101648 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff
+-rw-rw-rw-   0     1001 root         (0)    78268 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.866444 perun.proxygui-5.1.1/perun/proxygui/gui/static/images/
+-rw-rw-rw-   0     1001 root         (0)      490 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/images/check.svg
+-rw-rw-rw-   0     1001 root         (0)      536 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/images/circle-check-regular.svg
+-rw-rw-rw-   0     1001 root         (0)      483 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/images/circle-exclamation-solid.svg
+-rw-rw-rw-   0     1001 root         (0)      730 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/images/questionmark.svg
+-rw-rw-rw-   0     1001 root         (0)      625 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/images/spinner.svg
+-rw-rw-rw-   0     1001 root         (0)    89501 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/jquery-3.6.0.min.js
+-rw-rw-rw-   0     1001 root         (0)      627 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/proxygui.css
+-rw-rw-rw-   0     1001 root         (0)     1427 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/proxygui.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.870444 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/
+-rw-rw-rw-   0     1001 root         (0)    15836 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css
+-rw-rw-rw-   0     1001 root         (0)     8266 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css
+-rw-rw-rw-   0     1001 root         (0)     8862 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css
+-rw-rw-rw-   0     1001 root         (0)     8873 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css
+-rw-rw-rw-   0     1001 root         (0)     7692 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.css
+-rw-rw-rw-   0     1001 root         (0)     8344 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.default.css
+-rw-rw-rw-   0     1001 root         (0)    11438 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/js/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.870444 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/js/standalone/
+-rw-rw-rw-   0     1001 root         (0)    64906 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.870444 perun.proxygui-5.1.1/perun/proxygui/gui/templates/
+-rw-rw-rw-   0     1001 root         (0)    15205 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/ConsentRegistration.html
+-rw-rw-rw-   0     1001 root         (0)     9192 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/HeuristicData.html
+-rw-rw-rw-   0     1001 root         (0)      747 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/IsTestingSP.html
+-rw-rw-rw-   0     1001 root         (0)     3101 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/Logout.html
+-rw-rw-rw-   0     1001 root         (0)     1131 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResetEmailSent.html
+-rw-rw-rw-   0     1001 root         (0)     1942 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResetInitiated.html
+-rw-rw-rw-   0     1001 root         (0)     1133 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html
+-rw-rw-rw-   0     1001 root         (0)     1021 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResult.html
+-rw-rw-rw-   0     1001 root         (0)      795 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/MissingAuth.html
+-rw-rw-rw-   0     1001 root         (0)     1019 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/OidcError.html
+-rw-rw-rw-   0     1001 root         (0)     1223 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/Post-logout.html
+-rw-rw-rw-   0     1001 root         (0)      907 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/SPAuthorization.html
+-rw-rw-rw-   0     1001 root         (0)     2490 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/_footer.html
+-rw-rw-rw-   0     1001 root         (0)     8119 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/_header.html
+-rw-rw-rw-   0     1001 root         (0)     1175 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/authorization.html
+-rw-rw-rw-   0     1001 root         (0)     3477 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/base.html
+-rw-rw-rw-   0     1001 root         (0)      734 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/logout-canceled.html
+-rw-rw-rw-   0     1001 root         (0)      561 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/logout-iframe.html
+-rw-rw-rw-   0     1001 root         (0)     3769 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/templates/logout-state.html
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun/proxygui/gui/translations/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun/proxygui/gui/translations/cs/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.870444 perun.proxygui-5.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/
+-rw-rw-rw-   0     1001 root         (0)     2973 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
+-rw-rw-rw-   0     1001 root         (0)     8108 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
+-rw-rw-rw-   0     1001 root         (0)     5372 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/jwt.py
+-rw-rw-rw-   0     1001 root         (0)    20220 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/logout_manager.py
+-rw-rw-rw-   0     1001 root         (0)     2480 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/oauth.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.870444 perun.proxygui-5.1.1/perun/proxygui/openapi/
+-rw-rw-rw-   0     1001 root         (0)     6107 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/openapi/openapi.py
+-rw-rw-rw-   0     1001 root         (0)    12933 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/openapi/openapi_data.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.870444 perun.proxygui-5.1.1/perun/proxygui/openapi/schemas/
+-rw-rw-rw-   0     1001 root         (0)      997 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/openapi/schemas/arguments_schemas.py
+-rw-rw-rw-   0     1001 root         (0)     1446 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/openapi/schemas/response_schemas.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.874444 perun.proxygui-5.1.1/perun/proxygui/tests/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1816 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/shared_test_data.py
+-rw-rw-rw-   0     1001 root         (0)     6409 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/test_ban_api.py
+-rw-rw-rw-   0     1001 root         (0)     6635 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/test_consent_api.py
+-rw-rw-rw-   0     1001 root         (0)     4713 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/test_consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2160 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/test_consent_request_db.py
+-rw-rw-rw-   0     1001 root         (0)     6826 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/test_gui.py
+-rw-rw-rw-   0     1001 root         (0)     1111 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/tests/test_kerberos_auth_api.py
+-rw-rw-rw-   0     1001 root         (0)    22361 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/proxygui/user_manager.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.874444 perun.proxygui-5.1.1/perun/utils/
+-rw-rw-rw-   0     1001 root         (0)     2496 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/ConfigStore.py
+-rw-rw-rw-   0     1001 root         (0)       43 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/CustomExceptions.py
+-rw-rw-rw-   0     1001 root         (0)     2555 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/CustomRPHandler.py
+-rw-rw-rw-   0     1001 root         (0)     1354 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/DatabaseService.py
+-rw-rw-rw-   0     1001 root         (0)     4414 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/EmailService.py
+-rw-rw-rw-   0     1001 root         (0)       96 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/Notification.py
+-rw-rw-rw-   0     1001 root         (0)      816 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/Utils.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.874444 perun.proxygui-5.1.1/perun/utils/auth_event_loggig/
+-rw-rw-rw-   0     1001 root         (0)     2070 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.874444 perun.proxygui-5.1.1/perun/utils/consent_framework/
+-rw-rw-rw-   0     1001 root         (0)     1241 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/consent_framework/consent.py
+-rw-rw-rw-   0     1001 root         (0)     2226 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/consent_framework/consent_db.py
+-rw-rw-rw-   0     1001 root         (0)     2274 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/consent_framework/consent_manager.py
+-rw-rw-rw-   0     1001 root         (0)      730 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/consent_framework/consent_request.py
+-rw-rw-rw-   0     1001 root         (0)     1371 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/consent_framework/consent_request_db.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.874444 perun.proxygui-5.1.1/perun/utils/logout_requests/
+-rw-rw-rw-   0     1001 root         (0)     2001 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/logout_requests/BackchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)      832 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     3841 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/logout_requests/GraphLogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     1361 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/logout_requests/LogoutRequest.py
+-rw-rw-rw-   0     1001 root         (0)     2229 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/perun/utils/logout_requests/SamlLogoutRequest.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-24 09:58:03.826443 perun.proxygui-5.1.1/perun.proxygui.egg-info/
+-rw-r--r--   0     1001 root         (0)     9351 2024-04-24 09:58:03.000000 perun.proxygui-5.1.1/perun.proxygui.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)    12892 2024-04-24 09:58:03.000000 perun.proxygui-5.1.1/perun.proxygui.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-04-24 09:58:03.000000 perun.proxygui-5.1.1/perun.proxygui.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)      557 2024-04-24 09:58:03.000000 perun.proxygui-5.1.1/perun.proxygui.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)        6 2024-04-24 09:58:03.000000 perun.proxygui-5.1.1/perun.proxygui.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)       90 2024-04-24 09:58:03.878444 perun.proxygui-5.1.1/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     1485 2024-04-24 09:57:30.000000 perun.proxygui-5.1.1/setup.py
```

### Comparing `perun.proxygui-5.1.0/LICENSE` & `perun.proxygui-5.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/PKG-INFO` & `perun.proxygui-5.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 5.1.0
+Version: 5.1.1
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
@@ -12,15 +12,15 @@
 Requires-Dist: Flask==2.3.3
 Requires-Dist: Flask-pyoidc==3.14.3
 Requires-Dist: Flask-Babel==3.1.0
 Requires-Dist: perun.connector==3.8.1
 Requires-Dist: python-smail==0.9.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: pymongo==3.13.0
-Requires-Dist: validators==0.22.0
+Requires-Dist: validators==0.28.1
 Requires-Dist: idpyoidc==2.0.0
 Requires-Dist: python-dateutil==2.9.0
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: Flask-Session==0.5.0
 Requires-Dist: pysaml2==7.4.2
 Requires-Dist: cryptojwt==1.8.3
```

### Comparing `perun.proxygui-5.1.0/README.md` & `perun.proxygui-5.1.1/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/api/backchannel_logout_api.py` & `perun.proxygui-5.1.1/perun/proxygui/api/backchannel_logout_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/api/ban_api.py` & `perun.proxygui-5.1.1/perun/proxygui/api/ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/api/consent_api.py` & `perun.proxygui-5.1.1/perun/proxygui/api/consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/api/heuristic_api.py` & `perun.proxygui-5.1.1/perun/proxygui/api/heuristic_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/api/kerberos_auth_api.py` & `perun.proxygui-5.1.1/perun/proxygui/api/kerberos_auth_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/app.py` & `perun.proxygui-5.1.1/perun/proxygui/app.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/gui.py` & `perun.proxygui-5.1.1/perun/proxygui/gui/gui.py`

 * *Files 1% similar despite different names*

```diff
@@ -187,21 +187,24 @@
 
             resp = make_response(
                 render_template(
                     "Logout.html",
                     logged_out_service=logged_out_service,
                     session_services=session_services,
                     device_services=device_services,
-                    default_postlogout_uri=cfg.get("logout", {}).get(
-                        "default_postlogout_uri"
-                    ),
                 )
             )
             return resp
 
+        @gui.route("/logout_canceled")
+        def logout_canceled():
+            return render_template(
+                "logout-canceled.html",
+            )
+
         @gui.route("/logout_state", methods=["GET"])
         def logout_state():
             if session.get("logout_params") is None:
                 # at least empty dict should be set, or logout endpoint was not visited
                 return redirect(url_for("gui.logout", _external=True))
 
             ssp_session_id = request.cookies.get("SimpleSAMLSessionID")
```

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/_molecules.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_avatar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_dropdown.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/atoms/_modal.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_article.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_calendar.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_chat-message.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_dashboard-header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_documents.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_notifications.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_settings.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_summary.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/box/_widget.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/crossroad/_reactions.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/molecules/menu/_profile.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/organisms/_header.scss`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/article-ins-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/avatar.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/chat-message-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/dashboard-header.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-01.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-02.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-03.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-04.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-05.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-06.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-07.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/_ins/img/illust/menu-08.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/documentation.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/print.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-custom.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-econ.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fi.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fsps.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-fss.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-law.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-med.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-ped.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-phil.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style-sci.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/style.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/.map/wysiwyg.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/documentation.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/print.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/documentation.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/print.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/rtl/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-custom.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-custom.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-econ.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-econ.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fi.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fi.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fsps.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-fss.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-fss.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-law.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-law.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-med.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-med.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-ped.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-ped.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-phil.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-phil.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style-sci.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style-sci.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/style.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/style.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/css/wysiwyg.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/fa-light-300.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/ico.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/fonts/muni-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/box-category.jpg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/bg/fancybox_loading.gif`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/favicon.ico` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/favicon.ico`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/img/logo-masarykova-univerzita.png`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/app.js.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/app.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/d3.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/documentation.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/documentation.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/graphs.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/graphs.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/highlight.pack.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.fancybox-thumbs.custom.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/jquery.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/jquery.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/MuniWeb/js/nv.d3.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/campus-idp.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/campus-idp.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/campus-idp.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/campus-idp.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/css/all.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/css/all.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/css/all.min.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/css/all.min.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/font_awesome/webfonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/images/circle-check-regular.svg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/images/circle-check-regular.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/images/questionmark.svg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/images/questionmark.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/images/spinner.svg` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/images/spinner.svg`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/jquery-3.6.0.min.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/jquery-3.6.0.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/proxygui.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/proxygui.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/proxygui.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/proxygui.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap2.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap3.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap4.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.bootstrap5.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.default.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.default.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/css/selectize.legacy.css` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/css/selectize.legacy.css`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js` & `perun.proxygui-5.1.1/perun/proxygui/gui/static/selectize/js/standalone/selectize.min.js`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/ConsentRegistration.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/ConsentRegistration.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/HeuristicData.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/HeuristicData.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/IsTestingSP.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/IsTestingSP.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/Logout.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/Logout.html`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
                         </a>
                         {% if logged_out_service != {} %}
                           <a href="{{ url_for('gui.post_logout') }}"
                              class="btn {% if cfg.css_framework == 'MUNI' %}btn-primary{% else %}btn-secondary{% endif %} btn-s btn-border">
                               <span class="no-uppercase">{{ _('No') }}</span>
                           </a>
                         {% else %}
-                          <a href="{{default_postlogout_uri}}"
+                          <a href="{{ url_for('gui.logout_canceled') }}"
                              class="btn {% if cfg.css_framework == 'MUNI' %}btn-primary{% else %}btn-secondary{% endif %} btn-s btn-border">
                               <span class="no-uppercase">{{ _('No') }}</span>
                           </a>
                         {% endif %}
                     </p>
                     <h2 class="h5">{{ _("You can log out from the following services:") }}</h2>
                     <ul>
```

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResetEmailSent.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResetEmailSent.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResetInitiated.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResetInitiated.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResetVerifyConfirmationFail.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/MfaResult.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/MfaResult.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/MissingAuth.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/MissingAuth.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/OidcError.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/OidcError.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/Post-logout.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/Post-logout.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/SPAuthorization.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/SPAuthorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/_footer.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/_footer.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/_header.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/_header.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/authorization.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/authorization.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/base.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/base.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/logout-iframe.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/logout-iframe.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/templates/logout-state.html` & `perun.proxygui-5.1.1/perun/proxygui/gui/templates/logout-state.html`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo` & `perun.proxygui-5.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po` & `perun.proxygui-5.1.1/perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/jwt.py` & `perun.proxygui-5.1.1/perun/proxygui/jwt.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/logout_manager.py` & `perun.proxygui-5.1.1/perun/proxygui/logout_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/oauth.py` & `perun.proxygui-5.1.1/perun/proxygui/oauth.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/openapi/openapi.py` & `perun.proxygui-5.1.1/perun/proxygui/openapi/openapi.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/openapi/openapi_data.py` & `perun.proxygui-5.1.1/perun/proxygui/openapi/openapi_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/openapi/schemas/arguments_schemas.py` & `perun.proxygui-5.1.1/perun/proxygui/openapi/schemas/arguments_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/openapi/schemas/response_schemas.py` & `perun.proxygui-5.1.1/perun/proxygui/openapi/schemas/response_schemas.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/tests/shared_test_data.py` & `perun.proxygui-5.1.1/perun/proxygui/tests/shared_test_data.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/tests/test_ban_api.py` & `perun.proxygui-5.1.1/perun/proxygui/tests/test_ban_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/tests/test_consent_api.py` & `perun.proxygui-5.1.1/perun/proxygui/tests/test_consent_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/tests/test_consent_db.py` & `perun.proxygui-5.1.1/perun/proxygui/tests/test_consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/tests/test_consent_request_db.py` & `perun.proxygui-5.1.1/perun/proxygui/tests/test_consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/tests/test_gui.py` & `perun.proxygui-5.1.1/perun/proxygui/tests/test_gui.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/tests/test_kerberos_auth_api.py` & `perun.proxygui-5.1.1/perun/proxygui/tests/test_kerberos_auth_api.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/proxygui/user_manager.py` & `perun.proxygui-5.1.1/perun/proxygui/user_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/ConfigStore.py` & `perun.proxygui-5.1.1/perun/utils/ConfigStore.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/CustomRPHandler.py` & `perun.proxygui-5.1.1/perun/utils/CustomRPHandler.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/DatabaseService.py` & `perun.proxygui-5.1.1/perun/utils/DatabaseService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/EmailService.py` & `perun.proxygui-5.1.1/perun/utils/EmailService.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/Utils.py` & `perun.proxygui-5.1.1/perun/utils/Utils.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py` & `perun.proxygui-5.1.1/perun/utils/auth_event_loggig/AuthEventLoggingDbModels.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/consent_framework/consent.py` & `perun.proxygui-5.1.1/perun/utils/consent_framework/consent.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/consent_framework/consent_db.py` & `perun.proxygui-5.1.1/perun/utils/consent_framework/consent_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/consent_framework/consent_manager.py` & `perun.proxygui-5.1.1/perun/utils/consent_framework/consent_manager.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/consent_framework/consent_request.py` & `perun.proxygui-5.1.1/perun/utils/consent_framework/consent_request.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/consent_framework/consent_request_db.py` & `perun.proxygui-5.1.1/perun/utils/consent_framework/consent_request_db.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/logout_requests/BackchannelLogoutRequest.py` & `perun.proxygui-5.1.1/perun/utils/logout_requests/BackchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/logout_requests/FrontchannelLogoutRequest.py` & `perun.proxygui-5.1.1/perun/utils/logout_requests/FrontchannelLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/logout_requests/GraphLogoutRequest.py` & `perun.proxygui-5.1.1/perun/utils/logout_requests/GraphLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/logout_requests/LogoutRequest.py` & `perun.proxygui-5.1.1/perun/utils/logout_requests/LogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun/utils/logout_requests/SamlLogoutRequest.py` & `perun.proxygui-5.1.1/perun/utils/logout_requests/SamlLogoutRequest.py`

 * *Files identical despite different names*

### Comparing `perun.proxygui-5.1.0/perun.proxygui.egg-info/PKG-INFO` & `perun.proxygui-5.1.1/perun.proxygui.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxygui
-Version: 5.1.0
+Version: 5.1.1
 Summary: Module with GUI and API for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/proxyidp-gui.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: Authlib==1.3.0
 Requires-Dist: setuptools
@@ -12,15 +12,15 @@
 Requires-Dist: Flask==2.3.3
 Requires-Dist: Flask-pyoidc==3.14.3
 Requires-Dist: Flask-Babel==3.1.0
 Requires-Dist: perun.connector==3.8.1
 Requires-Dist: python-smail==0.9.0
 Requires-Dist: SQLAlchemy==2.0.29
 Requires-Dist: pymongo==3.13.0
-Requires-Dist: validators==0.22.0
+Requires-Dist: validators==0.28.1
 Requires-Dist: idpyoidc==2.0.0
 Requires-Dist: python-dateutil==2.9.0
 Requires-Dist: Jinja2==3.1.3
 Requires-Dist: requests==2.31.0
 Requires-Dist: Flask-Session==0.5.0
 Requires-Dist: pysaml2==7.4.2
 Requires-Dist: cryptojwt==1.8.3
```

### Comparing `perun.proxygui-5.1.0/perun.proxygui.egg-info/SOURCES.txt` & `perun.proxygui-5.1.1/perun.proxygui.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -201,14 +201,15 @@
 perun/proxygui/gui/templates/OidcError.html
 perun/proxygui/gui/templates/Post-logout.html
 perun/proxygui/gui/templates/SPAuthorization.html
 perun/proxygui/gui/templates/_footer.html
 perun/proxygui/gui/templates/_header.html
 perun/proxygui/gui/templates/authorization.html
 perun/proxygui/gui/templates/base.html
+perun/proxygui/gui/templates/logout-canceled.html
 perun/proxygui/gui/templates/logout-iframe.html
 perun/proxygui/gui/templates/logout-state.html
 perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.mo
 perun/proxygui/gui/translations/cs/LC_MESSAGES/messages.po
 perun/proxygui/openapi/openapi.py
 perun/proxygui/openapi/openapi_data.py
 perun/proxygui/openapi/schemas/arguments_schemas.py
```

### Comparing `perun.proxygui-5.1.0/perun.proxygui.egg-info/requires.txt` & `perun.proxygui-5.1.1/perun.proxygui.egg-info/requires.txt`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 Flask==2.3.3
 Flask-pyoidc==3.14.3
 Flask-Babel==3.1.0
 perun.connector==3.8.1
 python-smail==0.9.0
 SQLAlchemy==2.0.29
 pymongo==3.13.0
-validators==0.22.0
+validators==0.28.1
 idpyoidc==2.0.0
 python-dateutil==2.9.0
 Jinja2==3.1.3
 requests==2.31.0
 Flask-Session==0.5.0
 pysaml2==7.4.2
 cryptojwt==1.8.3
```

### Comparing `perun.proxygui-5.1.0/setup.py` & `perun.proxygui-5.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         "Flask==2.3.3",
         "Flask-pyoidc==3.14.3",
         "Flask-Babel==3.1.0",
         "perun.connector==3.8.1",
         "python-smail==0.9.0",
         "SQLAlchemy==2.0.29",
         "pymongo==3.13.0",  # downgrade pymongo for Flask (internal) Sessions to work
-        "validators==0.22.0",
+        "validators==0.28.1",
         "idpyoidc==2.0.0",
         "python-dateutil==2.9.0",
         "Jinja2==3.1.3",
         "requests==2.31.0",
         "Flask-Session==0.5.0",
         "pysaml2==7.4.2",
         "cryptojwt==1.8.3",
```
