# Comparing `tmp/open-cravat-2.5.0.tar.gz` & `tmp/open-cravat-2.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open-cravat-2.5.0.tar", last modified: Mon Feb 26 16:08:07 2024, max compression
+gzip compressed data, was "open-cravat-2.6.0.tar", last modified: Wed Apr 24 13:29:53 2024, max compression
```

## Comparing `open-cravat-2.5.0.tar` & `open-cravat-2.6.0.tar`

### file list

```diff
@@ -1,340 +1,338 @@
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.490916 open-cravat-2.5.0/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1067 2024-02-26 16:08:07.000000 open-cravat-2.5.0/LICENSE
--rw-r--r--   0 kyle      (1000) kyle      (1000)      971 2024-02-26 16:08:07.489916 open-cravat-2.5.0/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)      661 2024-02-26 16:08:07.000000 open-cravat-2.5.0/README.rst
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.447916 open-cravat-2.5.0/cravat/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6364 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    60556 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/admin_util.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19600 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/aggregator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2990 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/annotator_options.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.448917 open-cravat-2.5.0/cravat/annotator_template/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      178 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/annotator_template/annotator_template.md
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2326 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/annotator_template/annotator_template.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1460 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/annotator_template/annotator_template.yml
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.448917 open-cravat-2.5.0/cravat/annotator_template/data/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/annotator_template/data/annotator_template.sqlite
--rw-r--r--   0 kyle      (1000) kyle      (1000)    28521 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/base_annotator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2074 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/base_commonmodule.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1259 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/base_converter.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    17199 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/base_mapper.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12209 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/base_postaggregator.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20758 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/base_summarizer.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5266 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/config_loader.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12114 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/constants.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      475 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat-system.template.yml
--rw-r--r--   0 kyle      (1000) kyle      (1000)       80 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat.yml
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32368 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_admin.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    85512 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_class.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    31453 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_convert.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    38094 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_filter.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6424 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_metrics.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1969 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_pack.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    51336 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_report.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32133 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_test.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    56209 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_util.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20271 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/cravat_web.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     9941 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/example_input
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1245 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/exceptions.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19368 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/inout.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.449916 open-cravat-2.5.0/cravat/liftover/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   931825 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/liftover/hg18ToHg38.over.chain
--rw-r--r--   0 kyle      (1000) kyle      (1000)   606773 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/liftover/hg19ToHg38.over.chain
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3165 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/mp_runners.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/oc.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      295 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/runcravat.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10553 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/store_utils.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10935 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/util.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.451917 open-cravat-2.5.0/cravat/webresult/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16774 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/cravat_view.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.451917 open-cravat-2.5.0/cravat/webresult/css/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2389 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/css/pqselect.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/favicon.ico
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/favicon.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.452916 open-cravat-2.5.0/cravat/webresult/fonts/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26456 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/roboto-bold-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19508 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/roboto-bold-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25692 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/roboto-light-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18980 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/roboto-light-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26312 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/roboto-medium-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    19416 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/roboto-medium-webfont.woff2
--rw-r--r--   0 kyle      (1000) kyle      (1000)    33072 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25740 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.460916 open-cravat-2.5.0/cravat/webresult/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      350 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-90deg-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      326 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-down-right-circle-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      379 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-down-right-circle.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-down-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      311 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-left.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      312 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      815 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-spinner-static.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6792 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-spinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)      309 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrow-up.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      706 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/arrows-move.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12538 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/back_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)   264317 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/bigSpinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2302 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/camera.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2140 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/camera.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      291 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/caret-down.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      289 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/caret-right.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      916 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/close-button.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3125 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/close.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2390 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/close.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1160 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/close_icon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      722 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/download-material-black.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7432 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/download-material-blue.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      263 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/download.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2066 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/download.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      378 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/download12.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      485 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/grip-vertical.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      591 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/help_16x16.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7061 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/help_icon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32137 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/loading-gif-animation.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2056 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/mail.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1211 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/menu.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      200 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/minus.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1568 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/openNewTab.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5131 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/package.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1703 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/pencil.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      805 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/pin-2.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      698 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/pin.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2219 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/pin.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2243 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/plus-circle-dotted.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/plus-circle-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      217 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/plus.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3324 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13026 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/resize.jpg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3498 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/save.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1408 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/save_new.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25171 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/search.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4645 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/sorry.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    55605 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/spinCircle.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)    25333 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/spinner.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1106 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/triangle-down.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1112 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/triangle-right.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      733 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/upload-material-black.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7573 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/upload-material-blue.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/x-lg.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      332 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/images/x.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6007 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/index.html
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.463916 open-cravat-2.5.0/cravat/webresult/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   398184 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/Chart.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     9279 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/dom-to-image.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6000 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/download.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)   954164 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/graphics.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86659 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-3.2.1.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.466916 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12660 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1817 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.439916 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.466916 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
--rw-r--r--   0 kyle      (1000) kyle      (1000)   293430 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.467916 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6992 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6988 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6999 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4549 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6299 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    32588 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    35997 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   520714 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    30747 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   253668 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18705 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    15548 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    17342 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13847 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1340 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13171 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery.tools.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5451 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/jquery.url.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    84772 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/packery.pkgd.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.470916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    11951 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)   103213 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.471916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      230 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      210 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      771 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1668 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       51 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)       76 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)      216 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      201 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.471916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1169 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)    76985 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.473916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      755 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      774 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      794 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      826 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      837 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      830 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      661 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      796 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      808 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      847 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      797 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)      700 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.474916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1153 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      613 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)      541 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2973 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    27759 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2383 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12585 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2408 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2034 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16186 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   481365 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12765 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)   242939 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1646 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1286 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)      587 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/readme.txt
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.441917 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.474916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.474916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/brown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.474916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.475916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.475916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.475916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/gray/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.475916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.475916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/office/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.475916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/purple/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.475916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/red/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.476916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.476916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.476916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.476916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/tan/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.476916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/violet/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4392 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.477916 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1071 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1190 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2677 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3716 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1847 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12591 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/pqselect.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    92225 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/js/raphael-min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1530 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/jsonreporter.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.477916 open-cravat-2.5.0/cravat/webresult/nocache/
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.477916 open-cravat-2.5.0/cravat/webresult/nocache/css/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1714 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/css/singlevariantpage.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    21047 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/css/style.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2920 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/css/widget.css
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.479916 open-cravat-2.5.0/cravat/webresult/nocache/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    26685 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/filter.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12851 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/infomgr.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    44175 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/main.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    99826 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/setup.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     7986 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/showvariant.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    35998 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/singlevariantpage.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    31708 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/util.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1688 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/variables.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    20474 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/js/widgethelper.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     5535 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/nocache/variant.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    29719 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/webresult.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      173 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webresult/webviewer.yml
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.480916 open-cravat-2.5.0/cravat/webstore/
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1365 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/cravat_store.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/favicon.ico
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.482916 open-cravat-2.5.0/cravat/webstore/images/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      446 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/chat-dots-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      740 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/chat-dots.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      396 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/chat-left-text-fill.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)      545 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/chat-left-text.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    22268 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/done.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2226 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/empty.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/favicon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1763 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/folder.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    38197 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/genericmodulelogo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4766 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/hamburger.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1194 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/left_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    67804 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/logo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3524 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/new.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1214 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/right_arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      340 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/images/x-lg.svg
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/jquery-3.3.1.min.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.483916 open-cravat-2.5.0/cravat/webstore/js/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    75673 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/js/showdown-1.9.1.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    91924 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/js/showdown.min.js.map
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.483916 open-cravat-2.5.0/cravat/webstore/nocache/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    15015 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/nocache/webstore.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86292 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/nocache/webstore.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2342 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/sse.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1700 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/store_handlers.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)    16522 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/webstore.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      283 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/ws.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)      720 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/webstore/ws.js
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.487916 open-cravat-2.5.0/cravat/websubmit/
--rw-r--r--   0 kyle      (1000) kyle      (1000)       11 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/.gitignore
--rw-r--r--   0 kyle      (1000) kyle      (1000)   210024 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/Chart.bundle.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/__init__.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)      719 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/arrow.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2291 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/down.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     4948 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/email.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1224 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/favicon.ico
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1351 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/favicon.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      108 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/googleAnalytics.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1052 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/help.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      716 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/house-solid.svg
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.487916 open-cravat-2.5.0/cravat/websubmit/input-examples/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     9941 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/input-examples/cravat.hg38.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)    21369 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/input-examples/vcf.hg38.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)    86927 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/jquery-3.3.1.min.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    53784 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/logo.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    56098 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/logo_transparent.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      225 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/menu.png
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.488916 open-cravat-2.5.0/cravat/websubmit/nocache/
--rw-r--r--   0 kyle      (1000) kyle      (1000)    13800 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/broken_wheel.gif
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6103 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/core.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     8077 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/header.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    18239 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/index.html
--rw-r--r--   0 kyle      (1000) kyle      (1000)      343 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/main.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)     8595 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/moduleinfo.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    17405 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/websubmit.css
--rw-r--r--   0 kyle      (1000) kyle      (1000)    78774 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nocache/websubmit.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    11488 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/nointernet.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    27869 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/pqselect.dev.customforsubmit.js
--rw-r--r--   0 kyle      (1000) kyle      (1000)    10263 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/question.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2167 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/refresh.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)     1972 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/setting.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)      280 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/threedots.png
--rw-r--r--   0 kyle      (1000) kyle      (1000)    48884 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/websubmit/websubmit.py
--rw-r--r--   0 kyle      (1000) kyle      (1000)     3724 2024-02-26 16:08:07.000000 open-cravat-2.5.0/cravat/wincravat.pyw
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.489916 open-cravat-2.5.0/open_cravat.egg-info/
--rw-r--r--   0 kyle      (1000) kyle      (1000)      971 2024-02-26 16:08:07.000000 open-cravat-2.5.0/open_cravat.egg-info/PKG-INFO
--rw-r--r--   0 kyle      (1000) kyle      (1000)    12303 2024-02-26 16:08:07.000000 open-cravat-2.5.0/open_cravat.egg-info/SOURCES.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)        1 2024-02-26 16:08:07.000000 open-cravat-2.5.0/open_cravat.egg-info/dependency_links.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2024-02-26 16:08:07.000000 open-cravat-2.5.0/open_cravat.egg-info/entry_points.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)      190 2024-02-26 16:08:07.000000 open-cravat-2.5.0/open_cravat.egg-info/requires.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)        7 2024-02-26 16:08:07.000000 open-cravat-2.5.0/open_cravat.egg-info/top_level.txt
--rw-r--r--   0 kyle      (1000) kyle      (1000)       38 2024-02-26 16:08:07.490916 open-cravat-2.5.0/setup.cfg
--rw-r--r--   0 kyle      (1000) kyle      (1000)     2907 2024-02-26 16:08:07.000000 open-cravat-2.5.0/setup.py
-drwxr-xr-x   0 kyle      (1000) kyle      (1000)        0 2024-02-26 16:08:07.489916 open-cravat-2.5.0/tests/
--rw-r--r--   0 kyle      (1000) kyle      (1000)     6183 2024-02-26 16:08:07.000000 open-cravat-2.5.0/tests/test_admin_util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.338945 open-cravat-2.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-04-24 13:29:51.000000 open-cravat-2.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-24 13:29:53.338945 open-cravat-2.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 13:29:51.000000 open-cravat-2.6.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.290944 open-cravat-2.6.0/cravat/
+-rw-r--r--   0 runner    (1001) docker     (127)     6364 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60556 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/admin_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19600 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/aggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.290944 open-cravat-2.6.0/cravat/annotator_template/
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/annotator_template.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/annotator_template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/annotator_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.290944 open-cravat-2.6.0/cravat/annotator_template/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/annotator_template/data/annotator_template.sqlite
+-rw-r--r--   0 runner    (1001) docker     (127)    28521 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_annotator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_commonmodule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17199 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_mapper.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12209 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_postaggregator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20758 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/base_summarizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12114 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat-system.template.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    32368 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_admin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85512 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31514 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42490 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6575 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_pack.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51476 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32133 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56209 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20260 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/cravat_web.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/example_input
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19608 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/inout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.294944 open-cravat-2.6.0/cravat/liftover/
+-rw-r--r--   0 runner    (1001) docker     (127)   931825 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/liftover/hg18ToHg38.over.chain
+-rw-r--r--   0 runner    (1001) docker     (127)   606773 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/liftover/hg19ToHg38.over.chain
+-rw-r--r--   0 runner    (1001) docker     (127)     3165 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/mp_runners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8110 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/oc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/runcravat.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10553 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/store_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10935 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18622 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/vcfanno.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.294944 open-cravat-2.6.0/cravat/webresult/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.294944 open-cravat-2.6.0/cravat/webresult/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     2389 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/css/pqselect.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/email.png
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/favicon.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.298944 open-cravat-2.6.0/cravat/webresult/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    26456 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19508 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    25692 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18980 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    26312 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19416 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    33072 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    25740 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.306944 open-cravat-2.6.0/cravat/webresult/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-90deg-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down-right-circle-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down-right-circle.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-left.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-spinner-static.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6792 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-spinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrow-up.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/arrows-move.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12538 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/back_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)   264317 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/bigSpinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2302 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/camera.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/camera.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/caret-down.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/caret-right.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      916 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close-button.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3125 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2390 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/close_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download-material-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download-material-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2066 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/download12.png
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/grip-vertical.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      591 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/help_16x16.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     7061 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/help_icon.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32137 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/loading-gif-animation.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     2056 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/mail.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1211 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/menu.png
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/minus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/openNewTab.png
+-rw-r--r--   0 runner    (1001) docker     (127)     5131 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/package.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1703 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pencil.png
+-rw-r--r--   0 runner    (1001) docker     (127)      805 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pin-2.png
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pin.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/pin.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/plus-circle-dotted.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/plus-circle-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/plus.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3324 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)    13026 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/resize.jpg
+-rw-r--r--   0 runner    (1001) docker     (127)     3498 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/save.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/save_new.png
+-rw-r--r--   0 runner    (1001) docker     (127)    25171 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/search.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4645 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/sorry.png
+-rw-r--r--   0 runner    (1001) docker     (127)    55605 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/spinCircle.gif
+-rw-r--r--   0 runner    (1001) docker     (127)    25333 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/spinner.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/triangle-down.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1112 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/triangle-right.png
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/upload-material-black.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7573 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/upload-material-blue.png
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/x-lg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/images/x.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.310944 open-cravat-2.6.0/cravat/webresult/js/
+-rw-r--r--   0 runner    (1001) docker     (127)   398184 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/Chart.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/dom-to-image.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6000 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/download.js
+-rw-r--r--   0 runner    (1001) docker     (127)   954164 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/graphics.js
+-rw-r--r--   0 runner    (1001) docker     (127)    86659 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-3.2.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.310944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.282944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.310944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/
+-rw-r--r--   0 runner    (1001) docker     (127)   293430 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.314944 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/
+-rw-r--r--   0 runner    (1001) docker     (127)     6992 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6988 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4549 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32588 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)    35997 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css
+-rw-r--r--   0 runner    (1001) docker     (127)   520714 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30747 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   253668 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18705 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css
+-rw-r--r--   0 runner    (1001) docker     (127)    15548 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    17342 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css
+-rw-r--r--   0 runner    (1001) docker     (127)    13847 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13171 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery.tools.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5451 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/jquery.url.js
+-rw-r--r--   0 runner    (1001) docker     (127)    84772 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/packery.pkgd.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/
+-rw-r--r--   0 runner    (1001) docker     (127)    11951 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   103213 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      230 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/horiz-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/horiz-slider-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     1668 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square-blue-tr.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square-red-rb.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square-red-tr.gif
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/square_dirty.gif
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/vert-bg.png
+-rw-r--r--   0 runner    (1001) docker     (127)      201 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/vert-slider-bg.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    76985 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.318945 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js
+-rw-r--r--   0 runner    (1001) docker     (127)      661 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      808 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js
+-rw-r--r--   0 runner    (1001) docker     (127)      847 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js
+-rw-r--r--   0 runner    (1001) docker     (127)      797 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)    27759 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2383 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    12585 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2408 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)    16186 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)   481365 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12765 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   242939 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/readme.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.286944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/brown/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/gray/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/office/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/purple/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/red/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/tan/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/violet/
+-rw-r--r--   0 runner    (1001) docker     (127)     4392 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2677 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3716 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12591 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/pqselect.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    92225 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/js/raphael-min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/jsonreporter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.322944 open-cravat-2.6.0/cravat/webresult/nocache/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.326944 open-cravat-2.6.0/cravat/webresult/nocache/css/
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/css/singlevariantpage.css
+-rw-r--r--   0 runner    (1001) docker     (127)    21047 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/css/style.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2920 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/css/widget.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.326944 open-cravat-2.6.0/cravat/webresult/nocache/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    27149 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/filter.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12851 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/infomgr.js
+-rw-r--r--   0 runner    (1001) docker     (127)    44130 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)   102552 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/setup.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7986 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/showvariant.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35998 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/singlevariantpage.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31708 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/util.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/variables.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20474 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/js/widgethelper.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/nocache/variant.html
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)    30198 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/webresult.py
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webresult/webviewer.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.326944 open-cravat-2.6.0/cravat/webstore/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1365 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/cravat_store.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.330944 open-cravat-2.6.0/cravat/webstore/images/
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-dots-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-dots.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-left-text-fill.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/chat-left-text.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    22268 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/done.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/email.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/empty.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/folder.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38197 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/genericmodulelogo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4766 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/hamburger.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/left_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)    67804 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3524 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/new.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/right_arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/images/x-lg.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/jquery-3.3.1.min.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.330944 open-cravat-2.6.0/cravat/webstore/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    75673 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/js/showdown-1.9.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    91924 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/js/showdown.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.330944 open-cravat-2.6.0/cravat/webstore/nocache/
+-rw-r--r--   0 runner    (1001) docker     (127)    15015 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/nocache/webstore.css
+-rw-r--r--   0 runner    (1001) docker     (127)    86167 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/nocache/webstore.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/sse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/store_handlers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16522 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/webstore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/ws.html
+-rw-r--r--   0 runner    (1001) docker     (127)      720 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/webstore/ws.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.334945 open-cravat-2.6.0/cravat/websubmit/
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)   210024 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/Chart.bundle.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/arrow.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/down.png
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/email.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1224 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/favicon.png
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/googleAnalytics.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/help.png
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/house-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.334945 open-cravat-2.6.0/cravat/websubmit/input-examples/
+-rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/input-examples/cravat.hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    21369 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/input-examples/vcf.hg38.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    86927 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/jquery-3.3.1.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    53784 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/logo.png
+-rw-r--r--   0 runner    (1001) docker     (127)    56098 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/logo_transparent.png
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/menu.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.334945 open-cravat-2.6.0/cravat/websubmit/nocache/
+-rw-r--r--   0 runner    (1001) docker     (127)    13800 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/broken_wheel.gif
+-rw-r--r--   0 runner    (1001) docker     (127)     6157 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/core.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8077 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/header.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18218 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/main.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8595 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/moduleinfo.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17348 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.css
+-rw-r--r--   0 runner    (1001) docker     (127)    79780 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11488 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/nointernet.png
+-rw-r--r--   0 runner    (1001) docker     (127)    27869 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/pqselect.dev.customforsubmit.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10263 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/question.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/refresh.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/setting.png
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/threedots.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49732 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/websubmit/websubmit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-24 13:29:51.000000 open-cravat-2.6.0/cravat/wincravat.pyw
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 13:29:53.338945 open-cravat-2.6.0/open_cravat.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12264 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 13:29:53.000000 open-cravat-2.6.0/open_cravat.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 13:29:53.338945 open-cravat-2.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-24 13:29:51.000000 open-cravat-2.6.0/setup.py
```

### Comparing `open-cravat-2.5.0/LICENSE` & `open-cravat-2.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/PKG-INFO` & `open-cravat-2.6.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.5.0
+Version: 2.6.0
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: Kyle Moad, Kyle Anderson, Madison Larsen, Jeltje van Baren, and Rachel Karchin
 Author-email: support@opencravat.org
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Open-CRAVAT is a python package that performs genomic variant interpretation including variant impact, annotation, and scoring. 
 It has a modular architecture with a wide variety of analysis modules that are developed both by 
 the CRAVAT team and the broader variant analysis community. Open-CRAVAT is a product of the `Karchin Lab`_ 
 at Johns Hopkins University with funding provided by the National 
@@ -16,7 +18,9 @@
 
 .. _Karchin Lab: http://karchinlab.org
 .. _ITCR: https://itcr.cancer.gov
 
 Please see: `Open-CRAVAT Docs`_ for installation instructions and software documentation.
 
 .. _Open-CRAVAT Docs: https://open-cravat.readthedocs.io
+
+
```

### Comparing `open-cravat-2.5.0/README.rst` & `open-cravat-2.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/__init__.py` & `open-cravat-2.6.0/cravat/__init__.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/admin_util.py` & `open-cravat-2.6.0/cravat/admin_util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/aggregator.py` & `open-cravat-2.6.0/cravat/aggregator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/annotator_options.py` & `open-cravat-2.6.0/cravat/annotator_options.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/annotator_template/annotator_template.py` & `open-cravat-2.6.0/cravat/annotator_template/annotator_template.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/annotator_template/annotator_template.yml` & `open-cravat-2.6.0/cravat/annotator_template/annotator_template.yml`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/base_annotator.py` & `open-cravat-2.6.0/cravat/base_annotator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/base_commonmodule.py` & `open-cravat-2.6.0/cravat/base_commonmodule.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/base_converter.py` & `open-cravat-2.6.0/cravat/base_converter.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+from cravat.config_loader import ConfigLoader
+
+
 class BaseConverter(object):
     IGNORE = "converter_ignore"
 
     def __init__(self):
         self.format_name = None
         self.output_dir = None
         self.run_name = None
         self.input_assembly = None
+        self.module_name = self.__class__.__module__
+        config_loader = ConfigLoader()
+        self.conf = config_loader.get_module_conf(self.module_name)
 
     def check_format(self, *args, **kwargs):
         err_msg = (
             "Converter for %s format has no method check_format" % self.format_name
         )
         raise NotImplementedError(err_msg)
```

### Comparing `open-cravat-2.5.0/cravat/base_mapper.py` & `open-cravat-2.6.0/cravat/base_mapper.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/base_postaggregator.py` & `open-cravat-2.6.0/cravat/base_postaggregator.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/base_summarizer.py` & `open-cravat-2.6.0/cravat/base_summarizer.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/config_loader.py` & `open-cravat-2.6.0/cravat/config_loader.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/constants.py` & `open-cravat-2.6.0/cravat/constants.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/cravat_admin.py` & `open-cravat-2.6.0/cravat/cravat_admin.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/cravat_class.py` & `open-cravat-2.6.0/cravat/cravat_class.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/cravat_convert.py` & `open-cravat-2.6.0/cravat/cravat_convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -256,14 +256,15 @@
             # path based import from https://docs.python.org/3/library/importlib.html#importing-a-source-file-directly
             spec = importlib.util.spec_from_file_location(
                 module_info.name, module_info.script_path
             )
             module = importlib.util.module_from_spec(spec)
             spec.loader.exec_module(module)
             converter = module.CravatConverter()
+            converter.input_assembly = self.input_assembly
             if converter.format_name not in self.converters:
                 self.converters[converter.format_name] = converter
             else:
                 err_msg = (
                     "Cannot load two converters for format %s" % converter.format_name
                 )
                 raise ExpectedException(err_msg)
@@ -446,15 +447,15 @@
                                 if not chrom.startswith("chr"):
                                     chrom = "chr" + chrom
                                 if not self.do_liftover:
                                     if chrom.lower() == "chrmt":
                                         chrom = "chrM"
                                 wdict["chrom"] = self.chromdict.get(chrom, chrom)
                                 if multiple_files:
-                                    if wdict["sample_id"]:
+                                    if "sample_id" in wdict:
                                         wdict["sample_id"] = "__".join(
                                             [samp_prefix, wdict["sample_id"]]
                                         )
                                     else:
                                         wdict["sample_id"] = samp_prefix
                                 if "ref_base" not in wdict or wdict["ref_base"] == "":
                                     wdict["ref_base"] = self.wgsreader.get_bases(
```

### Comparing `open-cravat-2.5.0/cravat/cravat_filter.py` & `open-cravat-2.6.0/cravat/cravat_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -560,18 +560,15 @@
         bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
         level = "variant"
         await self.exec_db(self.make_filtered_uid_table)
         if bypassfilter:
             ftable = level
         else:
             ftable = level + "_filtered"
-        q = "select count(*) from " + ftable
-        await cursor.execute(q)
-        for row in await cursor.fetchone():
-            n = row
+        n = await self.exec_db(self.get_filtered_count, level=level)
         if self.stdout == True:
             print("#" + level)
             print(str(n))
         return n
 
     def getvariantrows(self):
         loop = asyncio.get_event_loop()
@@ -641,16 +638,118 @@
             + level
             + exclude_where
         )
         await cursor.execute(sql)
         it = await cursor.fetchall()
         return it
 
+    @staticmethod
+    def reaggregate_column(base_alias, meta):
+        column = meta['name']
+        function = meta.get('filter_reagg_function', None)
+        reagg_args = meta.get('filter_reagg_function_args', [])
+        reagg_source = meta.get('filter_reagg_source_column', None)
+
+        if not function:
+            return "{}.{}".format(base_alias, column)
+
+        reagg_template = "{}({}{}) OVER (PARTITION BY {}.base__uid ORDER BY sample.base__sample_id ROWS BETWEEN UNBOUNDED PRECEDING and UNBOUNDED FOLLOWING) {}"
+        quoted_args = ["'{}'".format(x) for x in reagg_args]
+        formatted_args = ",{}".format(",".join(quoted_args)) if reagg_args else ""
+        return reagg_template.format(function, reagg_source, formatted_args, base_alias, column)
+
+    @staticmethod
+    async def level_column_definitions(cursor, level):
+        await cursor.execute("select col_name, col_def from {}_header".format(level))
+        return {k: json.loads(v) for k, v in await cursor.fetchall()}
+
+    async def make_sample_filter_group(self, cursor, sample_filter):
+        sample_columns = await self.level_column_definitions(cursor, 'sample')
+        prefixes = {k: 'sample' for k in sample_columns.keys()}
+        filter_group = FilterGroup(sample_filter)
+        filter_group.add_prefixes(prefixes)
+        return filter_group
+
     async def get_filtered_iterator(self, level="variant", conn=None, cursor=None):
-        bypassfilter = not(self.filter or self.filtersql or self.includesample or self.excludesample)
+        sql = await self.build_base_sql(cursor, level)
+
+        if level == 'variant' and self.filter and 'samplefilter' in self.filter and len(self.filter['samplefilter']['rules']) > 0:
+            sample_filter = self.filter['samplefilter']
+            variant_columns = await self.level_column_definitions(cursor, 'variant')
+
+            reaggregated_columns = [self.reaggregate_column('v', meta) for col, meta in variant_columns.items()]
+            sample_filters = self.build_sample_exclusions()
+            filter_group = await self.make_sample_filter_group(cursor, sample_filter)
+
+            sql = """
+                with base_variant as ({}),
+                scoped_sample as (
+                    select * 
+                    from sample 
+                    where 1=1
+                    {}
+                )
+                select distinct {}
+                from base_variant v
+                join scoped_sample sample on sample.base__uid = v.base__uid
+                where {}
+            """.format(sql, sample_filters, ",".join(reaggregated_columns), filter_group.get_sql())
+
+        await cursor.execute(sql)
+        cols = [v[0] for v in cursor.description]
+        rows = await cursor.fetchall()
+
+        return cols, rows
+    
+    async def get_filtered_count(self, level="variant", conn=None, cursor=None):
+
+        if level == 'variant' and self.filter and 'samplefilter' in self.filter and len(self.filter['samplefilter']['rules']) > 0:
+            sql = await self.build_base_sql(cursor, level)
+            sample_filter = self.filter['samplefilter']
+            variant_columns = await self.level_column_definitions(cursor, 'variant')
+
+            reaggregated_columns = [self.reaggregate_column('v', meta) for col, meta in variant_columns.items()]
+            sample_filters = self.build_sample_exclusions()
+            filter_group = await self.make_sample_filter_group(cursor, sample_filter)
+
+            sql = """
+                with base_variant as ({}),
+                scoped_sample as (
+                    select * 
+                    from sample 
+                    where 1=1
+                    {}
+                )
+                select count(distinct v.base__uid)
+                from base_variant v
+                join scoped_sample sample on sample.base__uid = v.base__uid
+                where {}
+            """.format(sql, sample_filters, filter_group.get_sql())
+        else:
+            sql = await self.build_base_sql(cursor, level, count=True)
+        await cursor.execute(sql)
+        rows = await cursor.fetchall()
+
+        return rows[0][0]
+
+    def build_sample_exclusions(self):
+        # this is needed because joining back to the sample table causes
+        # re-inclusion of sample data that was excluded at the variant level.
+        sample_filters = ""
+        req, rej = self.required_and_rejected_samples()
+        if req:
+            sample_filters += "and base__sample_id in ({})".format(
+                ", ".join(["'{}'".format(sid) for sid in req]))
+        if rej:
+            sample_filters += "and base__sample_id not in ({})".format(
+                ", ".join(["'{}'".format(sid) for sid in rej]))
+        return sample_filters
+
+    async def build_base_sql(self, cursor, level, count=False):
+        bypassfilter = not (self.filter or self.filtersql or self.includesample or self.excludesample)
         if level == "variant":
             kcol = "base__uid"
             if bypassfilter:
                 ftable = "variant"
             else:
                 ftable = "variant_filtered"
         elif level == "gene":
@@ -678,37 +777,28 @@
                 await cursor.execute(sql)
                 rs = await cursor.fetchall()
                 colnames = ["gene." + r[1] for r in rs if r[1] != "base__hugo"]
                 sql = "select distinct variant.base__hugo, {} from variant inner join gene on variant.base__hugo==gene.base__hugo".format(
                     ", ".join(colnames)
                 )
             else:
-                sql = "select v.* from " + table + " as v"
+                if not count:
+                    sql = "select v.* from " + table + " as v"
+                else:
+                    sql = "select count(v.base__uid) from " + table + " as v"
                 if bypassfilter == False:
                     sql += " inner join " + ftable + " as f on v." + kcol + "=f." + kcol
-        await cursor.execute(sql)
-        cols = [v[0] for v in cursor.description]
-        rows = await cursor.fetchall()
-        return cols, rows
+
+        return sql
 
     async def make_filtered_sample_table(self, conn=None, cursor=None):
         q = "drop table if exists fsample"
         await cursor.execute(q)
         await conn.commit()
-        req = []
-        rej = []
-        if "sample" in self.filter:
-            if "require" in self.filter["sample"]:
-                req = self.filter["sample"]["require"]
-            if "reject" in self.filter["sample"]:
-                rej = self.filter["sample"]["reject"]
-        if self.includesample is not None:
-            req = self.includesample
-        if self.excludesample is not None:
-            rej = self.excludesample
+        req, rej = self.required_and_rejected_samples()
         if len(req) > 0 or len(rej) > 0:
             q = "create table fsample as select distinct base__uid from sample"
             if req:
                 q += " where base__sample_id in ({})".format(
                     ", ".join(['"{}"'.format(sid) for sid in req])
                 )
             for s in rej:
@@ -717,14 +807,21 @@
                 )
             await cursor.execute(q)
             await conn.commit()
             return True
         else:
             return False
 
+    def required_and_rejected_samples(self):
+        sample = self.filter.get("sample", {})
+        req = sample.get("require", self.includesample or [])
+        rej = sample.get("reject",  self.excludesample or [])
+
+        return req, rej
+
     async def make_filter_where(self, conn=None, cursor=None):
         q = ""
         if len(self.filter) == 0:
             if self.includesample is not None or self.excludesample is not None:
                 fsample_made = await self.exec_db(self.make_filtered_sample_table)
             else:
                 fsample_made = False
```

### Comparing `open-cravat-2.5.0/cravat/cravat_metrics.py` & `open-cravat-2.6.0/cravat/cravat_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,19 @@
         self.machinedata['OSVersion'] = platform.release()
         self.machinedata['totalMemory'] = psutil.virtual_memory().total
         self.machinedata['availableMemory'] = psutil.virtual_memory().available
         self.machinedata['freeMemory'] = psutil.virtual_memory().free
         self.machinedata['amountRAM'] = psutil.virtual_memory().total
         self.machinedata['swapMemory'] = psutil.swap_memory().total
         self.machinedata['numCPU'] = os.cpu_count()
-        self.machinedata['fileSystem'] = psutil.disk_partitions()[0].fstype
+        partitions = psutil.disk_partitions()
+        if len(partitions) > 0:
+            self.machinedata['fileSystem'] = psutil.disk_partitions()[0].fstype
+        else:
+            self.machinedata['fileSystem'] = 'unknown'
         self.machinedata['machineId'] = hex(uuid.getnode())
         self.machinedata['pythonVersion'] = platform.python_version()
 
     def set_job_data(self,param,value):
         self.jobdata[param] = value
 
     def set_job_converter(self,param,value):
```

### Comparing `open-cravat-2.5.0/cravat/cravat_pack.py` & `open-cravat-2.6.0/cravat/cravat_pack.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/cravat_report.py` & `open-cravat-2.6.0/cravat/cravat_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -611,14 +611,17 @@
         self.setup()
         level = "variant"
         if await self.exec_db(self.table_exists, level):
             await self.exec_db(self.make_col_info, level)
         level = "gene"
         if await self.exec_db(self.table_exists, level):
             await self.exec_db(self.make_col_info, level)
+        level = "sample"
+        if await self.exec_db(self.table_exists, level):
+            await self.exec_db(self.make_col_info, level)
         return self.colinfo
 
     def setup(self):
         pass
 
     def end(self):
         pass
```

### Comparing `open-cravat-2.5.0/cravat/cravat_test.py` & `open-cravat-2.6.0/cravat/cravat_test.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/cravat_util.py` & `open-cravat-2.6.0/cravat/cravat_util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/cravat_web.py` & `open-cravat-2.6.0/cravat/cravat_web.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,14 @@
 import os
 import webbrowser
 import multiprocessing
 import urllib.parse
 import json
 import sys
 import argparse
-import imp
 import oyaml as yaml
 import re
 from cravat import admin_util as au
 from cravat.webresult import webresult as wr
 from cravat.webstore import webstore as ws
 from cravat.websubmit import websubmit as wu
 import websockets
```

### Comparing `open-cravat-2.5.0/cravat/example_input` & `open-cravat-2.6.0/cravat/example_input`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/exceptions.py` & `open-cravat-2.6.0/cravat/exceptions.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/inout.py` & `open-cravat-2.6.0/cravat/inout.py`

 * *Files 1% similar despite different names*

```diff
@@ -539,14 +539,17 @@
         self.width = d.get("width")
         self.desc = d.get("desc")
         self.hidden = bool(d.get("hidden", False))
         self.category = d.get("category")
         self.filterable = bool(d.get("filterable", True))
         self.link_format = d.get("link_format")
         self.genesummary = d.get("genesummary", False)
+        self.filter_reagg_function = d.get("filter_reagg_function", None)
+        self.filter_reagg_function_args = d.get("filter_reagg_function_args", [])
+        self.filter_reagg_source_column = d.get("filter_reagg_source_column", None)
         self.table = d.get("table", False)
 
     def from_row(self, row, order=None):
         if order is None:
             order = self.db_order
         d = {self.sql_map[column]: value for column, value in zip(order, row)}
         self._load_dict(d)
```

### Comparing `open-cravat-2.5.0/cravat/liftover/hg18ToHg38.over.chain` & `open-cravat-2.6.0/cravat/liftover/hg18ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/liftover/hg19ToHg38.over.chain` & `open-cravat-2.6.0/cravat/liftover/hg19ToHg38.over.chain`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/mp_runners.py` & `open-cravat-2.6.0/cravat/mp_runners.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/oc.py` & `open-cravat-2.6.0/cravat/oc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import argparse
 from cravat import cravat_admin, cravat_util
 from cravat.cravat_class import cravat_cmd_parser
 from cravat.cravat_test import parser as test_parser
 from cravat.cravat_web import parser as gui_parser
 from cravat.cravat_report import parser as report_parser
+from cravat.vcfanno import vcfanno
 import sys
+import pathlib
 
 root_p = argparse.ArgumentParser(
     description="Open-CRAVAT genomic variant interpreter. https://github.com/KarchinLab/open-cravat"
 )
 root_sp = root_p.add_subparsers(title="Commands")
 
 # run
@@ -221,14 +223,38 @@
 feedback_p = root_sp.add_parser(
     "feedback",
     parents=[cravat_admin.parser_report_issue],
     add_help=False,
     help="Send feedback to the developers",
 )
 
+# vcfanno
+vcfanno_p = root_sp.add_parser(
+    'vcfanno',
+    help = 'annotate a vcf',
+)
+vcfanno_p.add_argument('input_path')
+vcfanno_p.add_argument('-a','--annotators',
+					   nargs = '*',
+)
+vcfanno_p.add_argument('-t','--threads',
+                       type = int,
+                       help = 'Number of CPU threads to use')
+vcfanno_p.add_argument('--temp-dir',
+                       type = pathlib.Path,
+                       default = pathlib.Path('temp-vcfanno'),
+                       help = 'Temporary directory for working files')
+vcfanno_p.add_argument('-o','--output-path',
+                       type = pathlib.Path,
+                       help = 'Output vcf path (gzipped). Defaults to input_path.oc.vcf.gz')
+vcfanno_p.add_argument('--chunk-size',
+                       type = int,
+                       default = 10**4,
+                       help = 'Number of lines to annotate in each thread before syncing to disk. Affects performance.')
+vcfanno_p.set_defaults(func=vcfanno)
 
 def main():
     try:
         # Global parser silently consumes the --debug option
         # --debug is used below in case of exceptions
         global_parser = argparse.ArgumentParser(add_help=False)
         global_parser.add_argument('--debug', action='store_true')
```

### Comparing `open-cravat-2.5.0/cravat/store_utils.py` & `open-cravat-2.6.0/cravat/store_utils.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/util.py` & `open-cravat-2.6.0/cravat/util.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/css/pqselect.min.css` & `open-cravat-2.6.0/cravat/webresult/css/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/email.png` & `open-cravat-2.6.0/cravat/webresult/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/favicon.ico` & `open-cravat-2.6.0/cravat/webresult/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/favicon.png` & `open-cravat-2.6.0/cravat/webresult/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/roboto-bold-webfont.woff` & `open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/roboto-bold-webfont.woff2` & `open-cravat-2.6.0/cravat/webresult/fonts/roboto-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/roboto-light-webfont.woff` & `open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/roboto-light-webfont.woff2` & `open-cravat-2.6.0/cravat/webresult/fonts/roboto-light-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/roboto-medium-webfont.woff` & `open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/roboto-medium-webfont.woff2` & `open-cravat-2.6.0/cravat/webresult/fonts/roboto-medium-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff` & `open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2` & `open-cravat-2.6.0/cravat/webresult/fonts/sourcesanspro-bold-webfont.woff2`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/arrow-spinner-static.gif` & `open-cravat-2.6.0/cravat/webresult/images/arrow-spinner-static.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/arrow-spinner.gif` & `open-cravat-2.6.0/cravat/webresult/images/arrow-spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/arrows-move.svg` & `open-cravat-2.6.0/cravat/webresult/images/arrows-move.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/back_arrow.png` & `open-cravat-2.6.0/cravat/webresult/images/back_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/bigSpinner.gif` & `open-cravat-2.6.0/cravat/webresult/images/bigSpinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/camera.png` & `open-cravat-2.6.0/cravat/webresult/images/camera.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/camera.svg` & `open-cravat-2.6.0/cravat/webresult/images/camera.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/close-button.png` & `open-cravat-2.6.0/cravat/webresult/images/close-button.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/close.png` & `open-cravat-2.6.0/cravat/webresult/images/close.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/close.svg` & `open-cravat-2.6.0/cravat/webresult/images/close.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/close_icon.png` & `open-cravat-2.6.0/cravat/webresult/images/close_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/download-material-black.png` & `open-cravat-2.6.0/cravat/webresult/images/download-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/download-material-blue.png` & `open-cravat-2.6.0/cravat/webresult/images/download-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/download.svg` & `open-cravat-2.6.0/cravat/webresult/images/download.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/help_16x16.gif` & `open-cravat-2.6.0/cravat/webresult/images/help_16x16.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/help_icon.png` & `open-cravat-2.6.0/cravat/webresult/images/help_icon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/loading-gif-animation.gif` & `open-cravat-2.6.0/cravat/webresult/images/loading-gif-animation.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/mail.png` & `open-cravat-2.6.0/cravat/webresult/images/mail.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/menu.png` & `open-cravat-2.6.0/cravat/webresult/images/menu.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/openNewTab.png` & `open-cravat-2.6.0/cravat/webresult/images/openNewTab.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/package.png` & `open-cravat-2.6.0/cravat/webresult/images/package.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/pencil.png` & `open-cravat-2.6.0/cravat/webresult/images/pencil.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/pin-2.png` & `open-cravat-2.6.0/cravat/webresult/images/pin-2.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/pin.png` & `open-cravat-2.6.0/cravat/webresult/images/pin.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/pin.svg` & `open-cravat-2.6.0/cravat/webresult/images/pin.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/plus-circle-dotted.svg` & `open-cravat-2.6.0/cravat/webresult/images/plus-circle-dotted.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/question.png` & `open-cravat-2.6.0/cravat/webresult/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/resize.jpg` & `open-cravat-2.6.0/cravat/webresult/images/resize.jpg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/save.png` & `open-cravat-2.6.0/cravat/webresult/images/save.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/save_new.png` & `open-cravat-2.6.0/cravat/webresult/images/save_new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/search.png` & `open-cravat-2.6.0/cravat/webresult/images/search.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/sorry.png` & `open-cravat-2.6.0/cravat/webresult/images/sorry.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/spinCircle.gif` & `open-cravat-2.6.0/cravat/webresult/images/spinCircle.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/spinner.gif` & `open-cravat-2.6.0/cravat/webresult/images/spinner.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/triangle-down.png` & `open-cravat-2.6.0/cravat/webresult/images/triangle-down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/triangle-right.png` & `open-cravat-2.6.0/cravat/webresult/images/triangle-right.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/upload-material-black.png` & `open-cravat-2.6.0/cravat/webresult/images/upload-material-black.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/images/upload-material-blue.png` & `open-cravat-2.6.0/cravat/webresult/images/upload-material-blue.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/index.html` & `open-cravat-2.6.0/cravat/webresult/index.html`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         <button id='tabledetailmaxbutton' class='butn' onclick='onClickTableDetailMinMaxButton();'>View table</button>
     </div>
     <div style='position: absolute; top: 0px; right: 0px; display:flex;'>
         <div><a href='https://opencravat.org' target='_blank'><img src='/submit/house-solid.svg' alt='Open Cravat Home' class='house-icon' /></a></div>
         <div><a href='https://open-cravat.readthedocs.io/en/latest/index.html' target='_blank' title='Help Wiki'><img src='/result/images/question.png' class='question-icon' /></a></div>
         <div><a href='mailto:support@opencravat.org?Subject=open-cravat%20feedback'><img src='/result/images/mail.png' title='Email for support' class='email-icon' onclick='mailto:support@opencravat.org' /></a></div>
         <input type='image' onclick='invokePackage();' src='images/package.png' title='Save job as Package' style='width: 21px; padding: 2px;' id="save-pkg-btn" />    
-        <input type='image' onclick='quicksave();' src='images/save_new.png' title='Quick save' style='width: 21px; padding: 2px;' />
+        <input type='image' onclick='quicksave();' src='images/save_new.png' title='Save current filters and layout as default' style='width: 21px; padding: 2px;' />
      </div>
     <div id='packageSubmit' style="position: absolute; top: 2px; right: 0px;width: 305px;background-color:white;display:none">
 	    <label for="packageName" style='font-size: 14px;'><b>Package Name:</b></label>
     	<input id='packageName' type="text" style='width: 200px;height: 18px;'><br>
         <button id='packageSubmitBtn' class='butn' onclick='saveAndPackage();' style='float: right;'>Submit</button>
         <button id='packageCancelBtn' class='butn' onclick='cancelPackage();' style='float: right;'>Cancel</button>
     </div>
```

### Comparing `open-cravat-2.5.0/cravat/webresult/js/Chart.js` & `open-cravat-2.6.0/cravat/webresult/js/Chart.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/dom-to-image.min.js` & `open-cravat-2.6.0/cravat/webresult/js/dom-to-image.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/download.js` & `open-cravat-2.6.0/cravat/webresult/js/download.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/graphics.js` & `open-cravat-2.6.0/cravat/webresult/js/graphics.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-3.2.1.min.js` & `open-cravat-2.6.0/cravat/webresult/js/jquery-3.2.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/AUTHORS.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/external/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_444444_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_555555_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777620_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_777777_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_cc0000_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/images/ui-icons_ffffff_256x240.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/index.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.structure.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/jquery-ui.theme.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json` & `open-cravat-2.6.0/cravat/webresult/js/jquery-ui-1.12.1.custom/package.json`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery.tools.min.js` & `open-cravat-2.6.0/cravat/webresult/js/jquery.tools.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/jquery.url.js` & `open-cravat-2.6.0/cravat/webresult/js/jquery.url.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/packery.pkgd.js` & `open-cravat-2.6.0/cravat/webresult/js/packery.pkgd.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/EULA.pdf`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/loading.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/images/sprite.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/MIT-License.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/jsZip-2.5.0/jszip.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-de.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-en.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-es.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-fr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-hu.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-it.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-ja.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-nl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pl.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-pt.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-tr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/localize/pq-localize-zh.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqSelect/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.dev.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/pqgrid.ui.min.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/readme.txt` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/readme.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/bootstrap/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/brown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/chocolate/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/cocoa/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/crimson/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/gray/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/indigo/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/office/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/purple/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/red/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/rosybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/sandybrown/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/steelblue/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/tan/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/themes/violet/pqgrid.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/ChangeLog.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/MIT-LICENSE.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/README.md`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.dev.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js` & `open-cravat-2.6.0/cravat/webresult/js/paramquery-pro-3/touch-punch/touch-punch.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/pqselect.min.js` & `open-cravat-2.6.0/cravat/webresult/js/pqselect.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/js/raphael-min.js` & `open-cravat-2.6.0/cravat/webresult/js/raphael-min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/jsonreporter.py` & `open-cravat-2.6.0/cravat/webresult/jsonreporter.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/css/singlevariantpage.css` & `open-cravat-2.6.0/cravat/webresult/nocache/css/singlevariantpage.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/css/style.css` & `open-cravat-2.6.0/cravat/webresult/nocache/css/style.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/css/widget.css` & `open-cravat-2.6.0/cravat/webresult/nocache/css/widget.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/filter.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/filter.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -94,31 +94,38 @@
     var moveImg = getEl('img')
     moveImg.setAttribute('src', '/result/images/grip-vertical.svg')
     moveImg.classList.add('passthrough')
     addEl(moveDiv, moveImg)
     return moveDiv
 }
 
-const makeFilterColDiv = (filter) => {
+const makeFilterColDiv = (filter, sampfilt) => {
     const colDiv = $(getEl('div'))
         .addClass('filter-column-div')
         .addClass('filter-element-div');
     addHoverControlEventListener(colDiv[0])
     addEl(colDiv[0], makeDragHandle())
     // Annotator select
     const groupSel = $(getEl('select'))
         .addClass('filter-annotator-selector')
         .change(filterGroupChangeHandler);
     colDiv.append(groupSel);
     for (let i = 0; i < filterCols.length; i++) {
         var colGroup = filterCols[i];
-        let groupOpt = $(getEl('option'))
-            .val(colGroup.title)
-            .append(colGroup.title);
-        groupSel.append(groupOpt);
+        if (sampfilt === true && colGroup.name === 'vcfinfo') {
+            let groupOpt = $(getEl('option'))
+                .val(colGroup.title)
+                .append(colGroup.title);
+            groupSel.append(groupOpt);
+        } else if (sampfilt !== true && colGroup.name !== 'vcfinfo') {
+            let groupOpt = $(getEl('option'))
+                .val(colGroup.title)
+                .append(colGroup.title);
+            groupSel.append(groupOpt);
+        }
     };
     // Column select
     const colSel = $(getEl('select'))
         .addClass('filter-column-selector')
         .on('change', onFilterColumnSelectorChange);
     colDiv.append(colSel);
     // Not toggle
@@ -415,15 +422,15 @@
     filterRootGroupDiv[0].id = name;
     filterRootGroupDiv.css('margin-left', '0px');
     filterRootGroupDiv.children('.filter-element-remove').attr('hidden', 'true');
     const rootElemsDiv = filterRootGroupDiv.children('.filter-group-div').children('.filter-group-elements-div');
     return filterRootGroupDiv;
 }
 
-const makeFilterGroupDiv = (filter) => {
+const makeFilterGroupDiv = (filter, sampfilt) => {
     // Group div
     const groupDiv = $(getEl('div'))
         .addClass('filter-group-div')
         .addClass('filter-element-div');
     addHoverControlEventListener(groupDiv[0])
     addEl(groupDiv[0], makeDragHandle())
     // Elements div
@@ -455,26 +462,26 @@
     const addRuleBtn = $(getEl('button'))
         .text('+')
         .addClass('filter-control-button')
         .addClass('butn')
         .addClass('addrule')
         .addClass('hovercontrol')
         .click(function(evt) {
-            addFilterRuleHandler(evt);
+            addFilterRuleHandler(evt, sampfilt);
         })
         .attr('title', 'Add rule');
     groupDiv.append(addRuleBtn);
     const addGroupBtn = $(getEl('button'))
         .text('( )')
         .addClass('filter-control-button')
         .addClass('butn')
         .addClass('addgroup')
         .addClass('hovercontrol')
         .click(function(evt) {
-            addFilterGroupHandler(evt);
+            addFilterGroupHandler(evt), sampfilt;
         })
         .attr('title', 'Add group');
     groupDiv.append(addGroupBtn);
     // Populate from filter
     if (filter !== undefined && !$.isEmptyObject(filter)) {
         if (filter.operator != undefined) {
             // Assign operator
@@ -483,26 +490,26 @@
             if (joinOperators.length > 0) {
                 $(joinOperators[0]).click();
             }*/
             // Add rules
             for (let i = 0; i < filter.rules.length; i++) {
                 let rule = filter.rules[i];
                 if (rule.hasOwnProperty('operator')) {
-                    addFilterElement($(elemsDiv), 'group', rule, undefined);
+                    addFilterElement($(elemsDiv), 'group', rule, undefined, sampfilt);
                 } else {
-                    addFilterElement($(elemsDiv), 'rule', rule, undefined);
+                    addFilterElement($(elemsDiv), 'rule', rule, undefined, sampfilt);
                 }
             }
             // Check negate
             if (filter.negate) {
                 notToggle.click();
             }
         }
     } else {
-        addFilterElement($(elemsDiv), 'rule', undefined);
+        addFilterElement($(elemsDiv), 'rule', undefined, sampfilt);
     }
     return groupDiv;
 }
 
 const filterGroupRemoveHandler = (event) => {
     const filterElemDiv = $(event.target.closest(".filter-element-div"))
     removeFilterElem(filterElemDiv);
@@ -521,24 +528,24 @@
     } else {
         elemDiv.next('.filter-join-operator-div').remove();
     }
     // Remove element
     elemDiv.remove();
 }
 
-const addFilterRuleHandler = (event) => {
+const addFilterRuleHandler = (event, sampfilt) => {
     const button = event.target
     const elemsDiv = $(button.closest('.filter-group-div').querySelector('div.filter-group-elements-div'))
-    addFilterElement(elemsDiv, 'rule', undefined);
+    addFilterElement(elemsDiv, 'rule', undefined, sampfilt);
 }
 
-const addFilterGroupHandler = (event) => {
+const addFilterGroupHandler = (event, sampfilt) => {
     const button = event.target
     const elemsDiv = $(button.closest('.filter-group-div').querySelector('div.filter-group-elements-div'))
-    addFilterElement(elemsDiv, 'group', undefined);
+    addFilterElement(elemsDiv, 'group', undefined, sampfilt);
 }
 
 const makeJoinOperatorDiv = function(operator) {
     const joinOpDiv = $(getEl('div'))
         .addClass('filter-join-operator-div')
         .addClass('filter-drop-target')
     joinOpDiv.click(groupOperatorClickHandler);
@@ -576,20 +583,20 @@
             el.classList.remove('dragenter')
         })
         evt.preventDefault()
     })
     return joinOpDiv
 }
 
-const addFilterElement = (allElemsDiv, elementType, filter) => {
+const addFilterElement = (allElemsDiv, elementType, filter, sampfilt) => {
     let elemDiv;
     if (elementType === 'group') {
-        elemDiv = makeFilterGroupDiv(filter);
+        elemDiv = makeFilterGroupDiv(filter, sampfilt);
     } else if (elementType === 'rule') {
-        elemDiv = makeFilterColDiv(filter);
+        elemDiv = makeFilterColDiv(filter, sampfilt);
     }
     elemDiv[0].id = 'filter-element-' + filterElemCount
     filterElemCount += 1
     elemDiv[0].setAttribute('draggable', true)
     elemDiv[0].addEventListener('dragstart', function(evt) {
         evt.dataTransfer.setData('text/plain', evt.target.id)
         evt.dataTransfer.dropEffect = 'move'
```

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/infomgr.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/infomgr.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/main.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/main.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1127,32 +1127,29 @@
     $.get('/result/service/variantcols', {
         job_id: jobId,
         username: username,
         dbpath: dbPath,
         confpath: confPath,
         filter: JSON.stringify(filterJson)
     }).done(function(jsonResponseData) {
-        allVarCols = JSON.parse(JSON.stringify(jsonResponseData['columns']['variant']));
-        filterCols = [];
-        for (let colGroup of allVarCols) {
+        filterCols = JSON.parse(JSON.stringify(jsonResponseData['columns']['variant']));
+        let vcfInfoTypes = {}
+        for (let colGroup of jsonResponseData['columns']['sample']) {
+            for (let col of colGroup.colModel) {
+                vcfInfoTypes[col.col] = col.type;
+            }
+        }
+        for (let colGroup of filterCols) {
             if (colGroup.name === 'vcfinfo') {
-                let filterableCols = [];
                 for (let col of colGroup.colModel) {
-                    if (col.filterable) {
-                        filterableCols.push(col);
-                    }
-                }
-                if (filterableCols.length > 0) {
-                    filterCols.push(colGroup);
-                    filterCols.slice(-1)[0].colModel = filterableCols;
+                    colNameToks = col.col.split('__');
+                    baseColName = `base__${colNameToks[1]}`
+                    col.type = vcfInfoTypes[baseColName];
                 }
-            } else {
-                filterCols.push(colGroup)
             }
-
         }
         usedAnnotators = {};
         var cols = jsonResponseData['columns']['variant'];
         usedAnnotators['variant'] = [];
         usedAnnotators['info'] = [];
         for (var i = 0; i < cols.length; i++) {
             var col = cols[i];
```

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/setup.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/setup.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -82,15 +82,15 @@
 
 class FilterManager {
 
     constructor() {
         this.sampleContId = 'filter-cont-sample';
         this.geneContId = 'filter-cont-gene';
         this.variantContId = 'filter-cont-variant'
-
+        this.sampFiltContId = 'filter-cont-sampfilt';
         this.sampleControlClass = 'sample-control'
         this.sampleFilterId = 'sample-select-filt';
         this.sampleFileId = 'sample-list-file';
         this.sampleFileDisplayId = 'sample-list-file-display';
         this.sampleFileClearId = 'sample-list-file-clear';
         this.sampleSelectId = 'sample-select-cont';
         this.sampleReqCountId = 'sample-req-count';
@@ -100,15 +100,16 @@
         this.sampleShownCount = 'sample-shown-count';
         this.sampleInteractedSpan = 'sample-interacted-cont';
         this.geneTextId = 'gene-list-text';
         this.geneFileId = 'gene-list-file';
         this.vpropSelectId = 'vprop-sel';
         this.vpropSfId = 'vprop-sf';
         this.vpropQbId = 'vprop-qb';
-        this.qbRootId = 'qb-root';
+        this.qbVarRootId = 'qb-root';
+        this.qbSampRootId = 'qb-samp-root';
         this.qbBannedColumns = [
             //'base__numsample',
             'base__samples',
         ];
         this.allSamples = [];
         this.requireSamples = new Set();
         this.rejectSamples = new Set();
@@ -531,14 +532,64 @@
         this.addGeneSelect(geneSelect, filter);
         let geneHeader = geneSelect.closest('.filter-body').siblings('.filter-header');
         if (filter.genes.length > 0) {
             geneHeader.removeClass('inactive');
         }
     }
 
+    addSPropUI(sPropCont, filter) {
+        filter = new CravatFilter(filter);
+        sPropCont.attr('id', this.sampFiltContId);
+        // sPropCont.append($(getEl('div'))
+        // 	.text('Select variants by applying filters or building a query'))
+        // let fTypeDiv = $(getEl('div'));
+        // sPropCont.append(fTypeDiv);
+        // let vPropSel = $(getEl('select'))
+        // 	.attr('id', this.vpropSelectId)
+        // 	.append($(getEl('option')).val('sf').text('sf'))
+        // 	.append($(getEl('option')).val('qb').text('qb'))
+        // 	.css('display','none')
+        // 	.change(this.vPropSelectChange.bind(this));
+        // fTypeDiv.append(vPropSel);
+        // let sfHeader = $(getEl('span'))
+        // 	.addClass('vprop-option')
+        // 	.text('Smart Filters')
+        // 	.addClass('title')
+        // 	.click(this.vPropOptionClick)
+        // 	.attr('value','sf');
+        // fTypeDiv.append(sfHeader);
+        // let qbHeader = $(getEl('span'))
+        // 	.addClass('vprop-option')
+        // 	.text('Query Builder')
+        // 	.addClass('title')
+        // 	.click(this.vPropOptionClick)
+        // 	.attr('value','qb');
+        // fTypeDiv.append(qbHeader);
+        // let sfContent = $(getEl('div'))
+        // 	.attr('id', this.vpropSfId);
+        // sPropCont.append(sfContent);
+        // this.addSfUI(sfContent, filter);
+        // let qbContent = $(getEl('div'))
+        // 	.attr('id', this.vpropQbId);
+        // sPropCont.append(qbContent);
+        this.addQbUI(sPropCont, filter, 'sample');
+
+        // Activate the correct vProp type
+        // let sfValued = Object.keys(filter.smartfilter).length !== 0;
+        // let qbValued = filter.variant.rules!==undefined && filter.variant.rules.length>0;
+        // if (sfValued || !qbValued) {
+        // 	vPropSel.val('sf');
+        // 	sfHeader.addClass('active');
+        // } else {
+        // 	vPropSel.val('qb');
+        // 	qbHeader.addClass('active');
+        // }
+        // vPropSel.change();
+    }
+
     addVpropUI(vPropCont, filter) {
         filter = new CravatFilter(filter);
         vPropCont.attr('id', this.variantContId);
         vPropCont.append($(getEl('div'))
             .text('Select variants by applying filters or building a query'))
         let fTypeDiv = $(getEl('div'));
         vPropCont.append(fTypeDiv);
@@ -611,25 +662,30 @@
                 let sfDiv = sf.getDiv();
                 sfDiv.attr('full-name', sfSource + '.' + sfName);
                 outerDiv.append(sfDiv);
             }
         }
     }
 
-    addQbUI(outerDiv, filter) {
+    addQbUI(outerDiv, filter, QbType) {
         filter = new CravatFilter(filter);
-        outerDiv.append($(getEl('div')).text('Use the query builder to create a set of filter rules'));
-        let qbDiv = makeFilterGroupDiv(filter.variant);
+        if (QbType === 'sample') {
+            outerDiv.append($(getEl('div')).text('Variants are returned if any sample matches the criteria'));
+            var qbDiv = makeFilterGroupDiv(filter.samplefilter, true);
+        } else {
+            outerDiv.append($(getEl('div')).text('Use the query builder to create a set of filter rules'));
+            var qbDiv = makeFilterGroupDiv(filter.variant);
+        }
         qbDiv.children('.filter-element-control-div').remove()
         qbDiv[0].querySelector('.addrule').style.visibility = 'visible'
         qbDiv[0].querySelector('.addgroup').style.visibility = 'visible'
         qbDiv[0].querySelector('.passthrough').remove()
-        qbDiv.attr('id', this.qbRootId);
+        let divId = QbType === 'sample' ? this.qbSampRootId : this.qbVarRootId
+        qbDiv.attr('id', divId);
         outerDiv.append(qbDiv);
-        //addFilterElement(qbDiv, 'rule', undefined)
     }
 
     updateVpropUI(filter) {
         filter = new CravatFilter(filter);
         let vPropCont = $('#' + this.variantContId);
         vPropCont.empty()
         this.addVpropUI(vPropCont, filter);
@@ -681,14 +737,18 @@
         };
         this.smartfilter = f.smartfilter !== undefined ? f.smartfilter : {};
         this.genes = f.genes !== undefined ? f.genes : [];
         this.sample = f.sample !== undefined ? f.sample : {
             require: [],
             reject: []
         };
+        this.samplefilter = f.samplefilter !== undefined ? f.samplefilter : {
+            operator: 'and',
+            rules: []
+        }
     }
 }
 
 class SmartFilter {
     constructor(sfDef, value) {
         this.sfDef = sfDef;
         this.valProvided = value !== undefined;
@@ -964,14 +1024,20 @@
 
     // Gene selector
     let geneSection = filterMgr.getFilterSection('Genes', false);
     rightPanel.append(geneSection);
     let geneContent = geneSection.find('.filter-content');
     filterMgr.addGeneSelect(geneContent);
 
+    // Sample properties
+    let sPropSection = filterMgr.getFilterSection('Sample Properties', false);
+    rightPanel.append(sPropSection);
+    let sPropContent = sPropSection.find('.filter-content');
+    filterMgr.addSPropUI(sPropContent);
+
     // Smartfilters
     let vPropSection = filterMgr.getFilterSection('Variant Properties', true);
     rightPanel.append(vPropSection);
     let vPropContent = vPropSection.find('.filter-content');
     filterMgr.addVpropUI(vPropContent);
 
     // Load controls
@@ -1129,15 +1195,15 @@
     // Gene list
     let geneListString = $('#' + filterMgr.geneTextId).val();
     let geneList = geneListString.split('\n')
         .map(s => s.trim())
         .map(s => s.toUpperCase())
         .filter(s => s);
     fjs.genes = geneList;
-    // Variant Properties
+    // Variant properties
     let activeVprop = $('#' + filterMgr.vpropSelectId).val();
     if (activeVprop === 'sf') {
         let sfWrapDiv = $('#' + filterMgr.vpropSfId);
         let sfDivs = sfWrapDiv.children('div');
         let fullSf = {
             operator: 'and',
             rules: []
@@ -1159,18 +1225,26 @@
                 sfState[sfSource] = {};
             }
             sfState[sfSource][sfName] = val;
         }
         fjs.variant = fullSf;
         fjs.smartfilter = sfState;
     } else if (activeVprop === 'qb') {
-        let qbRoot = $('#' + filterMgr.qbRootId);
+        let qbRoot = $('#' + filterMgr.qbVarRootId);
         fjs.variant = makeGroupFilter(qbRoot);
         fjs.smartfilter = {};
     }
+    // Sample filter
+    let spropRoot = $('#' + filterMgr.qbSampRootId);
+    fjs.samplefilter = makeGroupFilter(spropRoot);
+    for (let rule of fjs.samplefilter.rules) {
+        rule.column = rule.column.replace('vcfinfo__', 'base__')
+    }
+
+    // Set global
     filterJson = fjs;
 }
 
 function addSfValue(topRule, value) {
     topRule = JSON.parse(JSON.stringify(topRule));
     if (topRule.hasOwnProperty('rules')) {
         for (let i = 0; i < topRule.rules.length; i++) {
```

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/showvariant.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/showvariant.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/singlevariantpage.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/singlevariantpage.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/util.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/util.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/variables.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/variables.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/js/widgethelper.js` & `open-cravat-2.6.0/cravat/webresult/nocache/js/widgethelper.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/nocache/variant.html` & `open-cravat-2.6.0/cravat/webresult/nocache/variant.html`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/question.png` & `open-cravat-2.6.0/cravat/webresult/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webresult/webresult.py` & `open-cravat-2.6.0/cravat/webresult/webresult.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import aiosqlite
 import sqlite3
 import json
 import sys
-import imp
+import importlib
+from importlib import util as importlib_util
 from cravat import admin_util as au
 from cravat import CravatFilter
 from cravat.constants import base_smartfilters
 from aiohttp import web
 import time
 try:
     import cravat_multiuser
@@ -326,18 +327,18 @@
     else:
         filterstring = None
     if 'confpath' in queries:
         confpath = queries['confpath']
     else:
         confpath = None
     reporter_name = 'jsonreporter'
-    f, fn, d = imp.find_module(
-        reporter_name, 
-        [os.path.join(os.path.dirname(__file__),)])
-    m = imp.load_module(reporter_name, f, fn, d)
+    fp = os.path.join(os.path.dirname(__file__), f'{reporter_name}.py')
+    spec = importlib_util.spec_from_file_location(reporter_name, fp)
+    m = importlib_util.module_from_spec(spec)
+    spec.loader.exec_module(m)
     arg_dict = {'dbpath': dbpath, 'module_name': reporter_name}
     if confpath != None:
         arg_dict['confpath'] = confpath
     if filterstring != None:
         arg_dict['filterstring'] = filterstring
     arg_dict['nogenelevelonvariantlevel'] = True
     if 'separatesample' in queries:
@@ -441,14 +442,16 @@
     data['status'] = {}
     colinfo = await get_colinfo(dbpath, confpath, filterstring)
     data['columns'] = {}
     if 'variant' in colinfo:
         data['columns']['variant'] = get_colmodel('variant', colinfo)
     if 'gene' in colinfo:
         data['columns']['gene'] = get_colmodel('gene', colinfo)
+    if 'sample' in colinfo:
+        data['columns']['sample'] = get_colmodel('sample', colinfo)
     content = data
     return web.json_response(content)
 
 def get_summary_widget_names (request):
     queries = request.rel_url.query
     runid = queries['jobid'][0]
 
@@ -542,18 +545,18 @@
         if genesummary_present:
             columngroupdef['genesummary'] = True
         colModel.append(columngroupdef)
     return colModel
 
 async def get_colinfo (dbpath, confpath, filterstring):
     reporter_name = 'jsonreporter'
-    f, fn, d = imp.find_module(
-        reporter_name, 
-        [os.path.join(os.path.dirname(__file__),)])
-    m = imp.load_module(reporter_name, f, fn, d)
+    fp = os.path.join(os.path.dirname(__file__), f'{reporter_name}.py')
+    spec = importlib_util.spec_from_file_location(reporter_name, fp)
+    m = importlib_util.module_from_spec(spec)
+    spec.loader.exec_module(m)
     arg_dict = {'dbpath': dbpath, 'module_name': reporter_name}
     if confpath != None:
         arg_dict['confpath'] = confpath
     if filterstring != None:
         arg_dict['filterstring'] = filterstring
     arg_dict['reporttypes'] = ['text']
     reporter = m.Reporter(arg_dict)
@@ -599,38 +602,39 @@
     if ('dbpath' not in queries or queries['dbpath'] == '') and dbpath is not None:
         new_queries = {}
         new_queries['dbpath'] = dbpath
         for key in queries:
             if key != 'dbpath':
                 new_queries[key] = queries[key]
         queries = new_queries
-    f, fn, d = imp.find_module(path, 
-        [os.path.join(au.get_modules_dir(), 
-                      'webviewerwidgets', path)])
-    m = imp.load_module(path, f, fn, d)
+    info = au.get_local_module_info(path)
+    spec = importlib_util.spec_from_file_location(path, info.script_path)
+    m = importlib_util.module_from_spec(spec)
+    spec.loader.exec_module(m)
     content = await m.get_data(queries)
     return web.json_response(content)
 
 async def serve_webapp_runwidget (request):
     module_name = request.match_info['module']
     widget_name = request.match_info['widget']
     queries = request.rel_url.query
     tmp_queries = {}
     for key in queries:
         tmp_queries[key] = queries[key]
     queries = tmp_queries
-    f, fn, d = imp.find_module(
-        'wg' + widget_name,
-        [os.path.join(au.get_modules_dir(), 'webapps', module_name, 'widgets', 'wg' + widget_name)]
-    )
-    m = imp.load_module(widget_name, f, fn, d)
+    name = f'wg{widget_name}'
+    widget_path = os.path.join(au.get_modules_dir(), 'webapps', module_name, 'widgets', name, f'{name}.py')
+    spec = importlib_util.spec_from_file_location(name, widget_path)
+    m = importlib_util.module_from_spec(spec)
+    spec.loader.exec_module(m)
     content = await m.get_data(queries)
     return web.json_response(content)
 
 async def serve_runwidget_post (request):
+    # NOTE: This method seems to not be called either in the OpenCravat or OpenCravat modules code
     path = 'wg' + request.match_info['module']
     job_id, dbpath = await get_jobid_dbpath(request)
     queries = await request.post()
     new_queries = {}
     for k in queries:
         val = queries[k]
         if val == '':
@@ -649,18 +653,18 @@
     if ('dbpath' not in queries or queries['dbpath'] == '') and dbpath is not None:
         new_queries = {}
         new_queries['dbpath'] = dbpath
         for key in queries:
             if key != 'dbpath':
                 new_queries[key] = queries[key]
         queries = new_queries
-    f, fn, d = imp.find_module(path, 
-        [os.path.join(au.get_modules_dir(), 
-                      'webviewerwidgets', path)])
-    m = imp.load_module(path, f, fn, d)
+    info = au.get_local_module_info(path)
+    spec = importlib_util.spec_from_file_location(path, info.script_path)
+    m = importlib_util.module_from_spec(spec)
+    spec.loader.exec_module(m)
     content = await m.get_data(queries)
     return web.json_response(content)
 
 async def get_modules_info (request):
     queries = request.rel_url.query
     job_id, dbpath = await get_jobid_dbpath(request)
     conn = await get_db_conn(dbpath)
```

### Comparing `open-cravat-2.5.0/cravat/webstore/cravat_store.css` & `open-cravat-2.6.0/cravat/webstore/cravat_store.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/favicon.ico` & `open-cravat-2.6.0/cravat/webstore/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/chat-dots.svg` & `open-cravat-2.6.0/cravat/webstore/images/chat-dots.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/chat-left-text.svg` & `open-cravat-2.6.0/cravat/webstore/images/chat-left-text.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/done.png` & `open-cravat-2.6.0/cravat/webstore/images/done.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/email.png` & `open-cravat-2.6.0/cravat/webstore/images/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/empty.png` & `open-cravat-2.6.0/cravat/webstore/images/empty.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/favicon.png` & `open-cravat-2.6.0/cravat/webstore/images/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/folder.png` & `open-cravat-2.6.0/cravat/webstore/images/folder.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/genericmodulelogo.png` & `open-cravat-2.6.0/cravat/webstore/images/genericmodulelogo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/hamburger.png` & `open-cravat-2.6.0/cravat/webstore/images/hamburger.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/left_arrow.png` & `open-cravat-2.6.0/cravat/webstore/images/left_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/logo.png` & `open-cravat-2.6.0/cravat/webstore/images/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/new.png` & `open-cravat-2.6.0/cravat/webstore/images/new.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/question.png` & `open-cravat-2.6.0/cravat/webstore/images/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/images/right_arrow.png` & `open-cravat-2.6.0/cravat/webstore/images/right_arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/jquery-3.3.1.min.js` & `open-cravat-2.6.0/cravat/webstore/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/js/showdown-1.9.1.min.js` & `open-cravat-2.6.0/cravat/webstore/js/showdown-1.9.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/js/showdown.min.js.map` & `open-cravat-2.6.0/cravat/webstore/js/showdown.min.js.map`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/nocache/webstore.css` & `open-cravat-2.6.0/cravat/webstore/nocache/webstore.css`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/nocache/webstore.js` & `open-cravat-2.6.0/cravat/webstore/nocache/webstore.js`

 * *Files 0% similar despite different names*

#### js-beautify {}

```diff
@@ -2349,17 +2349,15 @@
             }
             OC.mediator.publish('showyesnodialog', div, yescallback, noSpace);
         },
     });
 }
 
 function announceStoreUpdatingAll() {
-    var span = document.getElementById('store-update-all-span');
     var button = document.getElementById('store-update-all-button');
-    span.textContent = 'Updating all available modules...';
     button.style.display = 'none';
 }
 
 function announceStoreUpdateAllAvailable() {
     //var span = document.getElementById('store-update-all-span');
     //span.textContent = 'Updates to your installed modules are available!';
     var button = document.getElementById('store-update-all-button');
```

### Comparing `open-cravat-2.5.0/cravat/webstore/sse.py` & `open-cravat-2.6.0/cravat/webstore/sse.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/store_handlers.py` & `open-cravat-2.6.0/cravat/webstore/store_handlers.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/webstore.py` & `open-cravat-2.6.0/cravat/webstore/webstore.py`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/webstore/ws.js` & `open-cravat-2.6.0/cravat/webstore/ws.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/Chart.bundle.min.js` & `open-cravat-2.6.0/cravat/websubmit/Chart.bundle.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/arrow.png` & `open-cravat-2.6.0/cravat/websubmit/arrow.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/down.png` & `open-cravat-2.6.0/cravat/websubmit/down.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/email.png` & `open-cravat-2.6.0/cravat/websubmit/email.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/favicon.ico` & `open-cravat-2.6.0/cravat/websubmit/favicon.ico`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/favicon.png` & `open-cravat-2.6.0/cravat/websubmit/favicon.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/help.png` & `open-cravat-2.6.0/cravat/websubmit/help.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/house-solid.svg` & `open-cravat-2.6.0/cravat/websubmit/house-solid.svg`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/input-examples/cravat.hg38.txt` & `open-cravat-2.6.0/cravat/websubmit/input-examples/cravat.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/input-examples/vcf.hg38.txt` & `open-cravat-2.6.0/cravat/websubmit/input-examples/vcf.hg38.txt`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/jquery-3.3.1.min.js` & `open-cravat-2.6.0/cravat/websubmit/jquery-3.3.1.min.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/logo.png` & `open-cravat-2.6.0/cravat/websubmit/logo.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/logo_transparent.png` & `open-cravat-2.6.0/cravat/websubmit/logo_transparent.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/nocache/broken_wheel.gif` & `open-cravat-2.6.0/cravat/websubmit/nocache/broken_wheel.gif`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/nocache/core.js` & `open-cravat-2.6.0/cravat/websubmit/nocache/core.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -20,25 +20,27 @@
 function changePage(selectedPageId) {
     const pageSelect = document.getElementById('pageselect');
     const pageIdDivs = pageSelect.children;
     for (let i = 0; i < pageIdDivs.length; i++) {
         const pageIdDiv = pageIdDivs[i];
         const pageId = pageIdDiv.getAttribute('value');
         const page = document.getElementById(pageId);
-        if (page.id === selectedPageId) {
+        if (page && page.id === selectedPageId) {
             page.style.display = 'block';
             pageIdDiv.setAttribute('selval', 't');
             if (selectedPageId === 'storediv') {
                 OC.currentTab = 'store';
             } else if (selectedPageId === 'submitdiv') {
                 OC.currentTab = 'submit';
             }
         } else {
-            page.style.display = 'none';
-            pageIdDiv.setAttribute('selval', 'f');
+            if (page) {
+                page.style.display = 'none';
+                pageIdDiv.setAttribute('selval', 'f');
+            }
         }
     }
 }
 
 /************** Mediator / PubSub ****************/
 /***
  * PubSub is a simple publish / subscribe mediator pattern module to facilitate cross-module communication within the app.
```

### Comparing `open-cravat-2.5.0/cravat/websubmit/nocache/header.js` & `open-cravat-2.6.0/cravat/websubmit/nocache/header.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/nocache/index.html` & `open-cravat-2.6.0/cravat/websubmit/nocache/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 <div id='pageselect'>
     <div id='submitdiv_tabhead' class='tabhead' selval='t' value='submitdiv'>
         JOBS
     </div>
     <div id='storediv_tabhead' class='tabhead' value='storediv' disabled='t'>
         STORE
     </div>
-    <a target="_blank" href="/webapps/variantreport/index.html">
+    <a target="_blank" id='singlevar-link'>
     <div id='singlevar_tabhead' class='tabhead' value='singlevardiv' disabled='t' style="background-color: #94d1eb;">
         SINGLE VARIANT
     </div>
     </a>
     <div id='admindiv_tabhead' class='tabhead' value='admindiv' disabled='t' style='display: none;'>
         ADMIN
     </div>
```

#### html2text {}

```diff
@@ -1,10 +1,10 @@
 JOBS
 STORE
-_S_I_N_G_L_E_ _V_A_R_I_A_N_T
+SINGLE VARIANT
 ADMIN
 System update available Update
 Version:
 [Open Cravat Logo]
 _[_/_s_u_b_m_i_t_/_h_o_u_s_e_-_s_o_l_i_d_._s_v_g_]_[_/_r_e_s_u_l_t_/_i_m_a_g_e_s_/_q_u_e_s_t_i_o_n_._p_n_g_]_[_/_r_e_s_u_l_t_/_i_m_a_g_e_s_/_m_a_i_l_._p_n_g_]
 [/submit/setting.png]
 [/submit/nointernet.png]
```

### Comparing `open-cravat-2.5.0/cravat/websubmit/nocache/moduleinfo.js` & `open-cravat-2.6.0/cravat/websubmit/nocache/moduleinfo.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/nocache/websubmit.css` & `open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.css`

 * *Files 1% similar despite different names*

```diff
@@ -556,23 +556,21 @@
     content: ' ' url('/result/images/download12.png');
 }
 */
 
 .inactive-download-button {
   background-color: white;
   color: #c5af8d;
-  background-color: white;
   border: 1px solid #c5af8d;
   position: relative;
 }
 
 .inactive-download-button:hover {
-    background-color: #6e593a;
-    border: 1px solid #6e593a;
-    color: white;
+    background-color: white;
+    cursor: default;
 }
 
 .checkbox-container {
   display: block;
   position: relative;
   padding-left: 21px;
   margin-bottom: 2px;
```

### Comparing `open-cravat-2.5.0/cravat/websubmit/nocache/websubmit.js` & `open-cravat-2.6.0/cravat/websubmit/nocache/websubmit.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -582,21 +582,38 @@
         }
     }
     // Log
     var logLink = getEl('a');
     logLink.setAttribute('href', '/submit/jobs/' + job.id + '/log');
     logLink.setAttribute('target', '_blank');
     logLink.setAttribute('title', 'Click to download.');
-    var button = getEl('button');
-    button.classList.add('butn');
-    button.classList.add('active-download-button');
-    addEl(button, getTn('Log'));
-    addEl(logLink, button);
+    var logButton = getEl('button');
+    logButton.classList.add('butn');
+    logButton.classList.add('active-download-button');
+    addEl(logButton, getTn('Log'));
+    addEl(logLink, logButton);
     addEl(dbTd, logLink);
     addEl(jobTr, dbTd);
+    // Err
+    var errLink = getEl('a');
+    addEl(dbTd, errLink);
+    var errButton = getEl('button');
+    addEl(errLink, errButton);
+    errButton.classList.add('butn');
+    if (job.num_error_input > 0) {
+        errButton.classList.add('active-download-button');
+        errLink.setAttribute('href', '/submit/jobs/' + job.id + '/err');
+        errLink.setAttribute('target', '_blank');
+        errLink.setAttribute('title', 'View per-variant errors.');
+    } else {
+        errButton.classList.add('inactive-download-button');
+        errLink.setAttribute('title', 'No errors.');
+    }
+    addEl(errButton, getTn('Errors'));
+    addEl(jobTr, dbTd);
     // + button
     var btn = getEl('button');
     btn.classList.add('butn');
     btn.setAttribute('jobid', job.id);
     addEl(btn, getTn('+'));
     btn.classList.add('inactive-download-button');
     btn.addEventListener('click', function(evt) {
@@ -1977,16 +1994,25 @@
     });
 }
 
 function addMediatorListeners() {
     OC.mediator.subscribe('navigate', changePage);
     OC.mediator.subscribe('populateJobs', populateJobs);
     OC.mediator.subscribe('moduleinfo.annotators', buildAnnotatorsSelector);
-
     OC.mediator.subscribe('setupJobs', handleSetupJobsTab);
+    OC.mediator.subscribe('moduleinfo.local', setVariantReportURL)
+}
+
+function setVariantReportURL() {
+    let url = '/webapps/variantreport/index.html'
+    if (!('variantreport' in OC.localModuleInfo)) {
+        url = 'https://run.opencravat.org' + url
+    }
+    let anchor = document.querySelector('#singlevar-link');
+    anchor.href = url;
 }
 
 function setLastAssembly() {
     let sel = document.getElementById('assembly-select');
     if (!OC.servermode) {
         $.ajax({
             url: '/submit/lastassembly',
```

### Comparing `open-cravat-2.5.0/cravat/websubmit/nointernet.png` & `open-cravat-2.6.0/cravat/websubmit/nointernet.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/pqselect.dev.customforsubmit.js` & `open-cravat-2.6.0/cravat/websubmit/pqselect.dev.customforsubmit.js`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/question.png` & `open-cravat-2.6.0/cravat/websubmit/question.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/refresh.png` & `open-cravat-2.6.0/cravat/websubmit/refresh.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/setting.png` & `open-cravat-2.6.0/cravat/websubmit/setting.png`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/cravat/websubmit/websubmit.py` & `open-cravat-2.6.0/cravat/websubmit/websubmit.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,14 +205,24 @@
         if run_path is not None:
             log_path = run_path + '.log'
             if os.path.exists(log_path) == False:
                 log_path = None
         else:
             log_path = None
         return log_path
+    
+    async def job_err (self, request, job_id):
+        run_path = await self.job_run_path(request, job_id)
+        if run_path is not None:
+            err_path = run_path + '.err'
+            if os.path.exists(err_path) == False:
+                err_path = None
+        else:
+            err_path = None
+        return err_path
 
 class WebJob(object):
     def __init__(self, job_dir, job_status_fpath):
         self.info = {}
         self.info['orig_input_fname'] = ''
         self.info['assembly'] = ''
         self.info['note'] = ''
@@ -701,14 +711,27 @@
     log_path = await filerouter.job_log(request, job_id)
     if log_path is not None:
         with open(log_path) as f:
             return web.Response(text=f.read())
     else:
         return web.Response(text='log file does not exist.')
 
+async def get_job_err (request):
+    global filerouter
+    job_id = request.match_info['job_id']
+    err_path = await filerouter.job_err(request, job_id)
+    if err_path is not None:
+        if os.stat(err_path).st_size == 0:
+            return web.Response(text='No errors')
+        else:
+            with open(err_path) as f:
+                return web.Response(text=f.read())
+    else:
+        return web.Response(text='log file does not exist.')
+
 def get_valid_report_types():
     global valid_report_types
     if valid_report_types is not None:
         return valid_report_types
     reporter_infos = au.get_local_module_infos(types=['reporter'])
     valid_report_types = [x.name.split('reporter')[0] for x in reporter_infos]
     valid_report_types = [v for v in valid_report_types if not v in ['text', 'pandas', 'stdout', 'example']]
@@ -1274,14 +1297,15 @@
 routes.append(['DELETE','/submit/jobs/{job_id}',delete_job])
 routes.append(['GET','/submit/jobs/{job_id}/db', download_db])
 routes.append(['GET','/submit/reports',get_report_types])
 routes.append(['GET','/submit/jobs/{job_id}/reports', get_available_report_types])
 routes.append(['POST','/submit/jobs/{job_id}/reports/{report_type}',generate_report])
 routes.append(['GET','/submit/jobs/{job_id}/reports/{report_type}',download_report])
 routes.append(['GET','/submit/jobs/{job_id}/log',get_job_log])
+routes.append(['GET','/submit/jobs/{job_id}/err',get_job_err])
 routes.append(['GET', '/submit/getjobsdir', get_jobs_dir])
 routes.append(['GET', '/submit/setjobsdir', set_jobs_dir])
 routes.append(['GET', '/submit/getsystemconfinfo', get_system_conf_info])
 routes.append(['GET', '/submit/updatesystemconf', update_system_conf])
 routes.append(['GET', '/submit/resetsystemconf', reset_system_conf])
 routes.append(['GET', '/submit/servermode', get_servermode])
 routes.append(['GET', '/submit/packageversions', get_package_versions])
```

### Comparing `open-cravat-2.5.0/cravat/wincravat.pyw` & `open-cravat-2.6.0/cravat/wincravat.pyw`

 * *Files identical despite different names*

### Comparing `open-cravat-2.5.0/open_cravat.egg-info/PKG-INFO` & `open-cravat-2.6.0/open_cravat.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: open-cravat
-Version: 2.5.0
+Version: 2.6.0
 Summary: OpenCRAVAT - variant analysis toolkit
 Home-page: https://www.opencravat.org
 Author: Kyle Moad, Kyle Anderson, Madison Larsen, Jeltje van Baren, and Rachel Karchin
 Author-email: support@opencravat.org
+License: UNKNOWN
+Platform: UNKNOWN
 Requires-Python: >=3.8
 License-File: LICENSE
 
 Open-CRAVAT is a python package that performs genomic variant interpretation including variant impact, annotation, and scoring. 
 It has a modular architecture with a wide variety of analysis modules that are developed both by 
 the CRAVAT team and the broader variant analysis community. Open-CRAVAT is a product of the `Karchin Lab`_ 
 at Johns Hopkins University with funding provided by the National 
@@ -16,7 +18,9 @@
 
 .. _Karchin Lab: http://karchinlab.org
 .. _ITCR: https://itcr.cancer.gov
 
 Please see: `Open-CRAVAT Docs`_ for installation instructions and software documentation.
 
 .. _Open-CRAVAT Docs: https://open-cravat.readthedocs.io
+
+
```

### Comparing `open-cravat-2.5.0/open_cravat.egg-info/SOURCES.txt` & `open-cravat-2.6.0/open_cravat.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -29,23 +29,23 @@
 cravat/exceptions.py
 cravat/inout.py
 cravat/mp_runners.py
 cravat/oc.py
 cravat/runcravat.py
 cravat/store_utils.py
 cravat/util.py
+cravat/vcfanno.py
 cravat/wincravat.pyw
 cravat/annotator_template/annotator_template.md
 cravat/annotator_template/annotator_template.py
 cravat/annotator_template/annotator_template.yml
 cravat/annotator_template/data/annotator_template.sqlite
 cravat/liftover/hg18ToHg38.over.chain
 cravat/liftover/hg19ToHg38.over.chain
 cravat/webresult/__init__.py
-cravat/webresult/cravat_view.py
 cravat/webresult/email.png
 cravat/webresult/favicon.ico
 cravat/webresult/favicon.png
 cravat/webresult/index.html
 cravat/webresult/jsonreporter.py
 cravat/webresult/question.png
 cravat/webresult/webresult.py
@@ -282,9 +282,8 @@
 cravat/websubmit/nocache/websubmit.css
 cravat/websubmit/nocache/websubmit.js
 open_cravat.egg-info/PKG-INFO
 open_cravat.egg-info/SOURCES.txt
 open_cravat.egg-info/dependency_links.txt
 open_cravat.egg-info/entry_points.txt
 open_cravat.egg-info/requires.txt
-open_cravat.egg-info/top_level.txt
-tests/test_admin_util.py
+open_cravat.egg-info/top_level.txt
```

### Comparing `open-cravat-2.5.0/setup.py` & `open-cravat-2.6.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 for root, dirs, files in os.walk(os.path.join('cravat', 'websubmit')):
     root_files = [os.path.join('..', root, f) for f in files]
     data_files.extend(root_files)
 
 setup(
     name='open-cravat',
     packages=['cravat'],
-    version='2.5.0',
+    version='2.6.0',
     description='OpenCRAVAT - variant analysis toolkit',
     long_description=readme(),
     author='Kyle Moad, Kyle Anderson, Madison Larsen, Jeltje van Baren, and Rachel Karchin',
     author_email='support@opencravat.org',
     url='https://www.opencravat.org',
     license='',
     package_data={
```

