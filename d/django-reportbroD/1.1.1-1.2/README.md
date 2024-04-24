# Comparing `tmp/django-reportbroD-1.1.1.tar.gz` & `tmp/django-reportbroD-1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-reportbroD-1.1.1.tar", last modified: Thu Apr 11 17:08:37 2024, max compression
+gzip compressed data, was "django-reportbroD-1.2.tar", last modified: Wed Apr 24 11:24:16 2024, max compression
```

## Comparing `django-reportbroD-1.1.1.tar` & `django-reportbroD-1.2.tar`

### file list

```diff
@@ -1,177 +1,27 @@
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.466576 django-reportbroD-1.1.1/
--rw-r--r--   0 rider     (1000) rider     (1000)      111 2024-02-21 17:30:29.000000 django-reportbroD-1.1.1/MANIFEST.in
--rw-r--r--   0 rider     (1000) rider     (1000)     2630 2024-04-11 17:08:37.466576 django-reportbroD-1.1.1/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     1686 2024-04-09 19:59:30.000000 django-reportbroD-1.1.1/README.md
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.349901 django-reportbroD-1.1.1/django_reportbroD/
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)      164 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/admin.py
--rw-r--r--   0 rider     (1000) rider     (1000)      190 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/apps.py
--rw-r--r--   0 rider     (1000) rider     (1000)      652 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/forms.py
--rw-r--r--   0 rider     (1000) rider     (1000)      782 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/menus.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.353235 django-reportbroD-1.1.1/django_reportbroD/migrations/
--rw-r--r--   0 rider     (1000) rider     (1000)     1738 2024-04-11 16:35:52.000000 django-reportbroD-1.1.1/django_reportbroD/migrations/0001_initial.py
--rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-04-11 16:35:52.000000 django-reportbroD-1.1.1/django_reportbroD/migrations/__init__.py
--rw-r--r--   0 rider     (1000) rider     (1000)     1614 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/models.py
--rw-r--r--   0 rider     (1000) rider     (1000)    14455 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/reportcore.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.343234 django-reportbroD-1.1.1/django_reportbroD/static/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.343234 django-reportbroD-1.1.1/django_reportbroD/static/assets/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.353235 django-reportbroD-1.1.1/django_reportbroD/static/assets/css/
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/css/mCSB_buttons.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1772 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/css/owl.video.play.html
--rw-r--r--   0 rider     (1000) rider     (1000)   509223 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/css/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)   236692 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/css/vendors.css
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.396571 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    24288 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   351196 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    62768 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    31064 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/cryptocurrency-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62984 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/cryptocurrency-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dashicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16604 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dashicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   163862 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dashicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    41636 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dashicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    20528 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dashicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    41808 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dashiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dripicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    99368 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dripicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    40348 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dripicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    26004 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dripicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    40522 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/dripiconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/feather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   213926 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/feather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    61920 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/feather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    29500 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/feather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    62084 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/featherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/font-awesome.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    77159 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/font-awesome.html
--rw-r--r--   0 rider     (1000) rider     (1000)   444379 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/font-awesome.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   165548 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/font-awesome.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    98024 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/font-awesome.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   165742 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/font-awesomed41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/ionicons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    61020 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/ionicons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   400219 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/ionicons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)   143936 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/ionicons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    80356 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/ionicons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)   144114 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/ioniconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/linea-weather.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    48132 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/linea-weather.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    21308 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/linea-weather.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     7936 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/linea-weather.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    21514 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/linea-weatherd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/material-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    38383 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/material-icons.html
--rw-r--r--   0 rider     (1000) rider     (1000)   238287 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/material-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    99212 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/material-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    50312 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/material-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    42495 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/material-iconsd41d.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16746 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/summernotec360.eot
--rw-r--r--   0 rider     (1000) rider     (1000)    16560 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/summernotec360.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    10324 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/summernotec360.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/themify-icons.eot
--rw-r--r--   0 rider     (1000) rider     (1000)   234269 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/themify-icons.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    78584 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/themify-icons.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    56108 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/themify-icons.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    78748 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/fonts/themify-iconsd41d.eot
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.399905 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/
--rw-r--r--   0 rider     (1000) rider     (1000)    39361 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/02.jpg
--rw-r--r--   0 rider     (1000) rider     (1000)    59862 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/base64.png
--rw-r--r--   0 rider     (1000) rider     (1000)    82742 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/dictionario.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.399905 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/export/
--rw-r--r--   0 rider     (1000) rider     (1000)     1876 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/export/csv.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1348 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/export/txt.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     2060 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/export/xlsx.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    48878 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.406572 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/
--rw-r--r--   0 rider     (1000) rider     (1000)     1182 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/ai.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1380 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/css.png
--rw-r--r--   0 rider     (1000) rider     (1000)      948 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/dbf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1383 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/doc.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1215 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/dwg.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1269 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/exe.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1006 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/html.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1364 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/jpg.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1399 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/pdf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1397 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/png.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1430 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/psd.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1005 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/rtf.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1421 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/svg.png
--rw-r--r--   0 rider     (1000) rider     (1000)      974 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/xls.png
--rw-r--r--   0 rider     (1000) rider     (1000)     1332 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/xml.png
--rw-r--r--   0 rider     (1000) rider     (1000)      997 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/file-icon/zip.png
--rw-r--r--   0 rider     (1000) rider     (1000)     7446 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/lista.png
--rw-r--r--   0 rider     (1000) rider     (1000)     4814 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/logo-icon.png
--rw-r--r--   0 rider     (1000) rider     (1000)     2422 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/logo-light.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/logo.png
--rw-r--r--   0 rider     (1000) rider     (1000)    49844 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/img/parametros.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.409906 django-reportbroD-1.1.1/django_reportbroD/static/assets/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   576312 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/js/app.js
--rw-r--r--   0 rider     (1000) rider     (1000)  8320860 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/assets/js/vendors.js
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.446575 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.446575 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.449908 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/iconfonts/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.449908 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)     1633 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.svg
--rw-r--r--   0 rider     (1000) rider     (1000)     1384 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)     1460 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff
--rw-r--r--   0 rider     (1000) rider     (1000)      684 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/iconfonts/fonts/demoapp.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)      855 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/iconfonts/style.css
--rw-r--r--   0 rider     (1000) rider     (1000)     4509 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/css/styles.css
--rw-r--r--   0 rider     (1000) rider     (1000)     2238 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/favicon.ico
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.453242 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/js/
--rw-r--r--   0 rider     (1000) rider     (1000)   288580 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/js/jquery-3.6.0.js
--rw-r--r--   0 rider     (1000) rider     (1000)    89501 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/js/jquery-3.6.0.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)     3121 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/js/jquery.cookie.js
--rw-r--r--   0 rider     (1000) rider     (1000)   318139 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/js/knockout-3.5.1.js
--rw-r--r--   0 rider     (1000) rider     (1000)    68249 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/js/knockout-3.5.1.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)    55398 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/reportbro.css
--rw-r--r--   0 rider     (1000) rider     (1000)    77644 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/reportbro.css.map
--rw-r--r--   0 rider     (1000) rider     (1000)   733475 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/reportbro.js
--rw-r--r--   0 rider     (1000) rider     (1000)      665 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/reportbro.js.LICENSE.txt
--rw-r--r--   0 rider     (1000) rider     (1000)  2440768 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/reportbro.js.map
--rw-r--r--   0 rider     (1000) rider     (1000)   722287 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/reportbro.min.js
--rw-r--r--   0 rider     (1000) rider     (1000)   803864 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/reportbro.min.js.map
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.456575 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/
--rw-r--r--   0 rider     (1000) rider     (1000)    24374 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/ajaxload.gif
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.463243 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    20756 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16748 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-300.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20672 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16756 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-600.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20664 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16696 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-800.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    20712 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff
--rw-r--r--   0 rider     (1000) rider     (1000)    16740 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/fonts/open-sans-v34-latin-regular.woff2
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.463243 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/iconfonts/
--rw-r--r--   0 rider     (1000) rider     (1000)    37788 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.svg
--rw-r--r--   0 rider     (1000) rider     (1000)    12676 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.ttf
--rw-r--r--   0 rider     (1000) rider     (1000)    12752 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff
--rw-r--r--   0 rider     (1000) rider     (1000)     4460 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/iconfonts/reportbro.woff2
--rw-r--r--   0 rider     (1000) rider     (1000)    12924 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/rb_logo_dark.png
--rw-r--r--   0 rider     (1000) rider     (1000)    13606 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/static/reportlib/src/rb_logo_white.png
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.466576 django-reportbroD-1.1.1/django_reportbroD/templates/
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.466576 django-reportbroD-1.1.1/django_reportbroD/templates/bases/
--rw-r--r--   0 rider     (1000) rider     (1000)     1776 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/bases/base.html
--rw-r--r--   0 rider     (1000) rider     (1000)      346 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/bases/footer.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1969 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/bases/header.html
--rw-r--r--   0 rider     (1000) rider     (1000)      653 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/bases/navigator.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1890 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/create.html
--rw-r--r--   0 rider     (1000) rider     (1000)    20741 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/document.html
--rw-r--r--   0 rider     (1000) rider     (1000)     2116 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/edit.html
--rw-r--r--   0 rider     (1000) rider     (1000)     6189 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/especif.html
--rw-r--r--   0 rider     (1000) rider     (1000)     1128 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/formulario.html
--rw-r--r--   0 rider     (1000) rider     (1000)     8226 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/index.html
--rw-r--r--   0 rider     (1000) rider     (1000)     3102 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/templates/report.html
--rw-r--r--   0 rider     (1000) rider     (1000)       63 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/tests.py
--rw-r--r--   0 rider     (1000) rider     (1000)     1618 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/urls.py
--rw-r--r--   0 rider     (1000) rider     (1000)     2727 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/utils.py
--rw-r--r--   0 rider     (1000) rider     (1000)     1831 2024-04-11 13:25:44.000000 django-reportbroD-1.1.1/django_reportbroD/views.py
-drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-11 17:08:37.349901 django-reportbroD-1.1.1/django_reportbroD.egg-info/
--rw-r--r--   0 rider     (1000) rider     (1000)     2630 2024-04-11 17:08:37.000000 django-reportbroD-1.1.1/django_reportbroD.egg-info/PKG-INFO
--rw-r--r--   0 rider     (1000) rider     (1000)     7910 2024-04-11 17:08:37.000000 django-reportbroD-1.1.1/django_reportbroD.egg-info/SOURCES.txt
--rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-04-11 17:08:37.000000 django-reportbroD-1.1.1/django_reportbroD.egg-info/dependency_links.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-04-11 17:08:37.000000 django-reportbroD-1.1.1/django_reportbroD.egg-info/requires.txt
--rw-r--r--   0 rider     (1000) rider     (1000)       18 2024-04-11 17:08:37.000000 django-reportbroD-1.1.1/django_reportbroD.egg-info/top_level.txt
--rw-r--r--   0 rider     (1000) rider     (1000)     1063 2024-04-11 17:08:37.466576 django-reportbroD-1.1.1/setup.cfg
--rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django-reportbroD-1.1.1/setup.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:24:16.307563 django-reportbroD-1.2/
+-rw-r--r--   0 rider     (1000) rider     (1000)      111 2024-02-21 17:30:29.000000 django-reportbroD-1.2/MANIFEST.in
+-rw-r--r--   0 rider     (1000) rider     (1000)     2628 2024-04-24 11:24:16.307563 django-reportbroD-1.2/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)     1686 2024-04-09 19:59:30.000000 django-reportbroD-1.2/README.md
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:24:16.300896 django-reportbroD-1.2/django_reportbroD.egg-info/
+-rw-r--r--   0 rider     (1000) rider     (1000)     2628 2024-04-24 11:24:16.000000 django-reportbroD-1.2/django_reportbroD.egg-info/PKG-INFO
+-rw-r--r--   0 rider     (1000) rider     (1000)      543 2024-04-24 11:24:16.000000 django-reportbroD-1.2/django_reportbroD.egg-info/SOURCES.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)        1 2024-04-24 11:24:16.000000 django-reportbroD-1.2/django_reportbroD.egg-info/dependency_links.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       33 2024-04-24 11:24:16.000000 django-reportbroD-1.2/django_reportbroD.egg-info/requires.txt
+-rw-r--r--   0 rider     (1000) rider     (1000)       11 2024-04-24 11:24:16.000000 django-reportbroD-1.2/django_reportbroD.egg-info/top_level.txt
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:24:16.304230 django-reportbroD-1.2/reportbroD/
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-1.2/reportbroD/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      164 2024-04-22 20:05:48.000000 django-reportbroD-1.2/reportbroD/admin.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      192 2024-04-24 11:15:09.000000 django-reportbroD-1.2/reportbroD/apps.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      832 2024-04-22 20:05:48.000000 django-reportbroD-1.2/reportbroD/forms.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      801 2024-04-22 20:05:48.000000 django-reportbroD-1.2/reportbroD/menus.py
+drwxr-xr-x   0 rider     (1000) rider     (1000)        0 2024-04-24 11:24:16.304230 django-reportbroD-1.2/reportbroD/migrations/
+-rw-r--r--   0 rider     (1000) rider     (1000)     1738 2024-04-11 16:32:42.000000 django-reportbroD-1.2/reportbroD/migrations/0001_initial.py
+-rw-r--r--   0 rider     (1000) rider     (1000)        0 2024-02-16 20:55:14.000000 django-reportbroD-1.2/reportbroD/migrations/__init__.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     1864 2024-04-22 20:05:48.000000 django-reportbroD-1.2/reportbroD/models.py
+-rw-r--r--   0 rider     (1000) rider     (1000)    14448 2024-04-22 20:05:48.000000 django-reportbroD-1.2/reportbroD/reportcore.py
+-rw-r--r--   0 rider     (1000) rider     (1000)       63 2024-04-22 20:05:48.000000 django-reportbroD-1.2/reportbroD/tests.py
+-rw-r--r--   0 rider     (1000) rider     (1000)      743 2024-04-24 10:41:26.000000 django-reportbroD-1.2/reportbroD/urls.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     2702 2024-04-24 10:48:33.000000 django-reportbroD-1.2/reportbroD/utils.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     3221 2024-04-24 10:41:58.000000 django-reportbroD-1.2/reportbroD/views.py
+-rw-r--r--   0 rider     (1000) rider     (1000)     1061 2024-04-24 11:24:16.307563 django-reportbroD-1.2/setup.cfg
+-rw-r--r--   0 rider     (1000) rider     (1000)       37 2024-02-21 17:28:39.000000 django-reportbroD-1.2/setup.py
```

### Comparing `django-reportbroD-1.1.1/PKG-INFO` & `django-reportbroD-1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reportbroD
-Version: 1.1.1
+Version: 1.2
 Summary: A Django app to create and use ReportBro reports with a sample admin
 Author: Rider Raul Espinosa Perez
 Author-email: riderraule@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
```

### Comparing `django-reportbroD-1.1.1/README.md` & `django-reportbroD-1.2/README.md`

 * *Files identical despite different names*

### Comparing `django-reportbroD-1.1.1/django_reportbroD/forms.py` & `django-reportbroD-1.2/reportbroD/forms.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,8 +16,16 @@
         widgets={
            'name':forms.TextInput(attrs={"class":"form-control", "id":"nombre" , "placeholder":"Entre el nombre del reporte"}),
             'remark':forms.Textarea(attrs={"class":"form-control", "rows":"3" ,"id":"desc" ,"placeholder":"Provee una reseña sobre la función del reporte"}),
             
             }  
 
 
+
+class ReportImpForm(forms.Form):
+
+    template= forms.FileField(label="Plantilla",widget=forms.FileInput(attrs={"class":"form-control-file","id":"filetemplate"}))
+
+    
+
+
```

### Comparing `django-reportbroD-1.1.1/django_reportbroD/menus.py` & `django-reportbroD-1.2/reportbroD/menus.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 from django.urls import reverse
 
 
 def get_menu_items(request):
     """Returns application menu items with special class for active menu item."""
     return {
-      "active_page":"",
+      "active_page":"reportlist",
       "menu": ( {'url': reverse('reportbroD:list'), 'label': "ReportBro Designer",
         'icon': "nav-icon ti ti-pencil-alt",  'id':'reportlist' },
         
         {'url': reverse('reportbroD:docs'), 'label': "Designer Documentación",
         'icon': "nav-icon ti ti-comment-alt",  'id':  'reportdocs' },
         
          {'url': reverse('admin:index'), 'label': "Administración del Sitio",
-        'icon': "nav-icon fa fa-users",  'id': '' },
+        'icon': "nav-icon fa fa-users",  'id': 'admin' },
         
          {'url': '/', 'label': "Inicio",
-        'icon': "nav-icon ti ti-rocket",  'id': ''}
+        'icon': "nav-icon ti ti-rocket",  'id': 'home'}
          )
          }
```

### Comparing `django-reportbroD-1.1.1/django_reportbroD/migrations/0001_initial.py` & `django-reportbroD-1.2/reportbroD/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-reportbroD-1.1.1/django_reportbroD/models.py` & `django-reportbroD-1.2/reportbroD/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -40,8 +40,17 @@
         verbose_name='Reporte'
         verbose_name_plural='Reportes'
         
 
     def __str__(self):
         
         return self.name
+    
+    def to_dict(self):
+        return {
+            "report_definition":self.report_definition,
+            "name":self.name,
+            "remark":self.remark,
+            "last_modified_at":self.last_modified_at.isoformat()
+
+        }
```

### Comparing `django-reportbroD-1.1.1/django_reportbroD/reportcore.py` & `django-reportbroD-1.2/reportbroD/reportcore.py`

 * *Files 0% similar despite different names*

```diff
@@ -298,10 +298,8 @@
         
         response = HttpResponse(bytes(pdf_report), content_type='application/xlsx')
         response['Content-Disposition'] = 'inline; filename="{filename}"'.format(filename=f"{file}.xlsx")
         return response
     except ReportBroError as ex:
         return HttpResponseServerError('report error: ' + str(ex.error))
     except Exception as ex:
-        return HttpResponseServerError('report exception: ' + str(ex))
-    
-
+        return HttpResponseServerError('report exception: ' + str(ex))
```

### Comparing `django-reportbroD-1.1.1/django_reportbroD/utils.py` & `django-reportbroD-1.2/reportbroD/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import datetime
 import decimal
 import json
-import os
 from django.conf import settings
 from django.urls import reverse
 from django.utils.translation import gettext as _
 from .models import ReportDefinition
 from django.db import models
 from itertools import chain
 
@@ -50,15 +49,14 @@
             if f.value_from_object(instance) is not None:
                 formato= f.value_from_object(instance).url.split(".")[-1]
                 data[f.name] = convert_to_base64(f.value_from_object(instance).url, formato)
             else:
                 data[f.name] = None
         else:
             data[f.name] = f.value_from_object(instance)
-            
     return data
 
 
 def convert_list_to_dict(listado):
     """Convierte una query o lista de elementos de la clase Model en un 
     diccionario entendible para ReportBro"""
 
@@ -66,15 +64,15 @@
     return lista
 
 
 def convert_to_base64(path, format_image):
     """
     Nota: path se refiere a la ruta de la imagen y  format_image se refiere al fomato de la imagen (jpg, png, jpeg, etc)
     Este método permite convertir una imagen jpg o png a una imagen en base 64 
-      para que ReportBro pueda renderizarla como parte de sus parámetros  """
+    para que ReportBro pueda renderizarla como parte de sus parámetros  """
     import base64
     from django.conf import settings
     print(str(settings.BASE_DIR)+path)
     
     with open(str(settings.BASE_DIR)+path, "rb") as image_file:
         return f"data:image/{format_image};base64,{base64.b64encode(image_file.read()).decode('utf-8')}"
```

### Comparing `django-reportbroD-1.1.1/django_reportbroD/views.py` & `django-reportbroD-1.2/reportbroD/views.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from typing import Any
 from django.shortcuts import render, get_object_or_404, redirect
 from .models import ReportDefinition
 from django.views.generic import ListView, CreateView, UpdateView
-from .forms import ReportForm
+from .forms import ReportForm, ReportImpForm
 from django.urls import reverse_lazy
 from datetime import datetime
+from django.http import HttpResponse
+import json
+
 
 
 # Create your views here.
 
 def indexreport(request):
     return render (request, 'index.html')
 
@@ -20,17 +23,16 @@
     ordering= ('-last_modified_at', 'name')
 
     def get_context_data(self, **kwargs: Any) -> dict[str, Any]:
         context = super().get_context_data(**kwargs)
         context['active_page']="reportlist"
         
         return context
-
-
-
+    
+    
 def deletereport(request, id):
     reporte=get_object_or_404(ReportDefinition, pk=id)
     reporte.delete()
     return redirect("reportbroD:list")
 
 class CreateReport(CreateView):
     model=ReportDefinition
@@ -42,17 +44,14 @@
     model=ReportDefinition
     template_name="edit.html"
     form_class=ReportForm
     success_url=reverse_lazy("reportbroD:list")
     context_object_name="reporte"
 
 
-    
-
-
 def docs_view(request):
     context={}
     context['active_page']="reportdocs"
     return render(request, "document.html", context) 
 
 
 
@@ -61,8 +60,46 @@
     now = datetime.now()
     ReportDefinition.objects.create(
             name=reporte.name+" "+now.isoformat(),
             report_definition=reporte.report_definition,
             remark=reporte.remark,  
             last_modified_at=now )
     
-    return redirect("reportbroD:list")
+    return redirect("reportbroD:list")
+
+
+def exportreport(request, id):
+    reporte=get_object_or_404(ReportDefinition, pk=id)
+
+    exportation = json.dumps(reporte.to_dict())
+    response=HttpResponse(exportation,  content_type='application/force-download')
+    response['Content-Disposition'] = f'attachment; filename={reporte.name}.json'
+    return response
+
+
+def importreport(request):
+    
+    if request.method=="POST":
+        form=ReportImpForm(request.POST, request.FILES)
+
+        if form.is_valid():
+            cd = request.FILES ['template']
+            actual=datetime.now()
+            
+            try:
+                file=json.load(cd)
+                namereport= file["name"] if ReportDefinition.objects.filter(name=file["name"]).first() is None else file["name"]+" "+actual.isoformat()
+                ReportDefinition.objects.create(
+                 name=namereport,
+                 report_definition=file["report_definition"],
+                 remark=file ["remark"],  
+                 last_modified_at=actual )
+            except :
+                return render(request,"import.html",{"form":ReportImpForm(), "error":"El archivo no posee el formato adecuado."} )
+
+
+            return redirect("reportbroD:list")
+        
+    
+    return render(request,"import.html",{"form":ReportImpForm()} )
+    
+
```

### Comparing `django-reportbroD-1.1.1/django_reportbroD.egg-info/PKG-INFO` & `django-reportbroD-1.2/django_reportbroD.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-reportbroD
-Version: 1.1.1
+Version: 1.2
 Summary: A Django app to create and use ReportBro reports with a sample admin
 Author: Rider Raul Espinosa Perez
 Author-email: riderraule@gmail.com
 License: MIT
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Framework :: Django :: 5.0
```

### Comparing `django-reportbroD-1.1.1/setup.cfg` & `django-reportbroD-1.2/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = django-reportbroD
-version = 1.1.1
+version = 1.2
 description = A Django app to create and use ReportBro reports with a sample admin
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Rider Raul Espinosa Perez
 author_email = riderraule@gmail.com
 license = MIT
 classifiers =
```

