# Comparing `tmp/schedula-1.5.7.tar.gz` & `tmp/schedula-1.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schedula-1.5.7.tar", last modified: Fri Apr 19 10:48:53 2024, max compression
+gzip compressed data, was "schedula-1.5.8.tar", last modified: Fri Apr 19 12:08:09 2024, max compression
```

## Comparing `schedula-1.5.7.tar` & `schedula-1.5.8.tar`

### file list

```diff
@@ -1,291 +1,387 @@
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.879416 schedula-1.5.7/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2024-04-12 16:17:27.000000 schedula-1.5.7/AUTHORS.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2024-04-12 16:17:27.000000 schedula-1.5.7/LICENSE.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14759 2024-04-19 10:48:53.879261 schedula-1.5.7/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-19 10:36:00.000000 schedula-1.5.7/README.rst
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.832148 schedula-1.5.7/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4309 2024-04-17 14:10:45.000000 schedula-1.5.7/schedula/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-19 10:36:00.000000 schedula-1.5.7/schedula/_version.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1267 2024-04-17 14:10:45.000000 schedula-1.5.7/schedula/cli.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/dispatcher.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.833144 schedula-1.5.7/schedula/ext/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      450 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10745 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/autosummary.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.833565 schedula-1.5.7/schedula/ext/dispatcher/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      715 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/dispatcher/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12020 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/dispatcher/documenter.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3162 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/ext/dispatcher/graphviz.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.836198 schedula-1.5.7/schedula/utils/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/__init__.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/alg.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.836636 schedula-1.5.7/schedula/utils/asy/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/asy/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/asy/executors.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/asy/factory.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16000 2024-04-17 16:28:10.000000 schedula-1.5.7/schedula/utils/base.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/blue.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/cst.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.836757 schedula-1.5.7/schedula/utils/des/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6766 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/des/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.837103 schedula-1.5.7/schedula/utils/drw/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    64721 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.829721 schedula-1.5.7/schedula/utils/drw/index/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.838232 schedula-1.5.7/schedula/utils/drw/index/css/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   155758 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   625953 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css.map
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18280 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/icon.css
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3340 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/css/index.css
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.839412 schedula-1.5.7/schedula/utils/drw/index/js/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15950 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/bootstrap-treeview.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    58072 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   190253 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js.map
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16226 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/d3-scale.v3.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88144 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/jquery-3.4.1.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6341 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/jquery.fullscreen.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    67320 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/index/js/sunburst-chart.min.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1839 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/nodes.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.839737 schedula-1.5.7/schedula/utils/drw/templates/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18102 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/templates/index.html
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11626 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/templates/render.html
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.839894 schedula-1.5.7/schedula/utils/drw/viz/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)  2396719 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/drw/viz/viz.js
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/dsp.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/exc.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.842544 schedula-1.5.7/schedula/utils/form/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11497 2024-04-18 07:55:31.000000 schedula-1.5.7/schedula/utils/form/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6065 2024-04-19 10:04:16.000000 schedula-1.5.7/schedula/utils/form/cli.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5433 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/config.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1986 2024-04-18 10:08:20.000000 schedula-1.5.7/schedula/utils/form/gapp.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1541 2024-04-18 07:56:48.000000 schedula-1.5.7/schedula/utils/form/json_secrets.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1928 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/mail.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13359 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/server.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.830036 schedula-1.5.7/schedula/utils/form/static/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.830413 schedula-1.5.7/schedula/utils/form/static/schedula/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.845370 schedula-1.5.7/schedula/utils/form/static/schedula/css/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2151 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      280 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      837 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2164 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      137 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      139 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      185 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/4337.588bea5b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      234 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/4452.70b7e4bb.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      346 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/4459.a24c0b46.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/5255.de163d1c.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      314 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/5836.0a2c9e70.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/6753.de163d1c.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      251 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/6836.4de17ac7.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      499 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/7101.8501d8d8.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/7450.1773328b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      494 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      685 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.845641 schedula-1.5.7/schedula/utils/form/static/schedula/forms/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1326 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/static/schedula/forms/index-schema.json
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/forms/index-ui.json
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.870038 schedula-1.5.7/schedula/utils/form/static/schedula/js/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7227 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1064.c8a95e31.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      546 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1224 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1177.87802691.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      364 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4265 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1320.36172a41.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      832 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5084 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13937 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      578 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      298 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3958 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      291 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      601 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      779 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16150 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4504 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      936 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1441 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1748.9293df31.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3519 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/183.b47a21b0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      329 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1831.6e43492c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7430 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      649 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      415 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12856 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2120.8c0a0809.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1281 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    36347 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3771 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2256.b2d17449.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4863 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2286.c7768ada.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432061 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      324 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6016 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6928 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      388 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      281 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4570 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/268.dcd7a1fb.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2749 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      744 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2723.fe690409.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4363 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   468331 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      718 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8687 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    20917 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10227 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3070.687d86ba.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      498 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4704 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1622 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      655 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      465 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    19245 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      279 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      268 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3636 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11271 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/368.faa82a4c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1405 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      496 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10536 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4048.3d808f93.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11849 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4818 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5839 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/414.1d21b2ba.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      282 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6642 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4279.0095aff5.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      976 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5055 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4438.4a7723bc.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3470 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4452.ae121668.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      463 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5746 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3344 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4596.e723b7c7.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1499 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7075 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4673.a90e4863.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1777 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      297 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1422 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4218 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16181 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5025.7d25a45a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      283 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3728 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5097.cd4fde21.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4011 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28348 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2750 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1672 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5652.07f8f3c6.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5672.70cda519.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2752 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      278 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1960 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5836.fd1f9bd1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      734 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      284 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     9308 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4893 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11587 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/608.9032add2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      306 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4645 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6474.54e0a295.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      608 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7293 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6753.b68db48b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      426 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3700 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6836.a7cf7081.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1430 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      334 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1421 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4333 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2161 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2949 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4366 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6023 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8087 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7435.1a8a10a2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      275 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3130 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27276 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3731 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7565.764a83fd.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2984 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5252 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    37414 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/796.565e7a29.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   266738 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4005 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14837 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1367 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8859 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8148.354b6264.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1014 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8191.b709ea11.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8259.923684c0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3289 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8428.5b191797.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28904 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13457 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      339 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/853.904196e2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11594 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8531.d5720770.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12185 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8583.6d996cdc.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7427 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8698.c7f6106a.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8133 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3512 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      273 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4064 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9009.86c17596.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3720 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9196.45380a31.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6097 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2955 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4148 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2613 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6409 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      264 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      917 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9622.ef0af135.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      604 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    25595 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      486 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432389 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/js/main.fda4aa49.js.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873127 schedula-1.5.7/schedula/utils/form/static/schedula/media/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89335 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    97121 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88989 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95155 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    94641 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88308 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95760 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89222 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    96312 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88471 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    86875 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    93771 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      229 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/getFetch.40f37ddea2378391108f.cjs.gz
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      515 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.830564 schedula-1.5.7/schedula/utils/form/templates/
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873380 schedula-1.5.7/schedula/utils/form/templates/schedula/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3610 2024-04-19 10:27:45.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/base.html
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873777 schedula-1.5.7/schedula/utils/form/templates/schedula/email/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      238 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/email/contact-body-en.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      250 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/email/contact-body-it.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       57 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/email/contact-subject.rst
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       34 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/form/templates/schedula/index.html
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/gen.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/graph.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/imp.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.873909 schedula-1.5.7/schedula/utils/io/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6380 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/io/__init__.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/sol.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/utl.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.874037 schedula-1.5.7/schedula/utils/web/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7053 2024-04-12 16:17:27.000000 schedula-1.5.7/schedula/utils/web/__init__.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.875069 schedula-1.5.7/schedula.egg-info/
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14759 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/PKG-INFO
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15005 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/SOURCES.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/dependency_links.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       46 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/entry_points.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1083 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/requires.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-19 10:48:53.000000 schedula-1.5.7/schedula.egg-info/top_level.txt
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-19 10:48:53.879706 schedula-1.5.7/setup.cfg
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7344 2024-04-19 10:12:23.000000 schedula-1.5.7/setup.py
-drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 10:48:53.874710 schedula-1.5.7/tests/
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_dispatcher.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_import.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_micropython.py
--rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_readme.py
--rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-04-12 16:17:27.000000 schedula-1.5.7/tests/test_setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.340441 schedula-1.5.8/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       67 2024-04-12 16:17:27.000000 schedula-1.5.8/AUTHORS.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13141 2024-04-12 16:17:27.000000 schedula-1.5.8/LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14759 2024-04-19 12:08:09.340279 schedula-1.5.8/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    21979 2024-04-19 12:06:22.000000 schedula-1.5.8/README.rst
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.239559 schedula-1.5.8/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4309 2024-04-17 14:10:45.000000 schedula-1.5.8/schedula/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      777 2024-04-19 12:06:22.000000 schedula-1.5.8/schedula/_version.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1267 2024-04-17 14:10:45.000000 schedula-1.5.8/schedula/cli.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    68892 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/dispatcher.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.241634 schedula-1.5.8/schedula/ext/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      450 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/ext/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10745 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/ext/autosummary.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.242557 schedula-1.5.8/schedula/ext/dispatcher/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      715 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/ext/dispatcher/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12020 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/ext/dispatcher/documenter.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3162 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/ext/dispatcher/graphviz.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.246411 schedula-1.5.8/schedula/utils/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1446 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/__init__.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    13251 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/alg.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.247369 schedula-1.5.8/schedula/utils/asy/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11064 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/asy/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8126 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/asy/executors.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3284 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/asy/factory.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16000 2024-04-17 16:28:10.000000 schedula-1.5.8/schedula/utils/base.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24001 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/blue.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2009 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/cst.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.247589 schedula-1.5.8/schedula/utils/des/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6766 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/des/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.248475 schedula-1.5.8/schedula/utils/drw/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    64721 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.233071 schedula-1.5.8/schedula/utils/drw/index/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.249741 schedula-1.5.8/schedula/utils/drw/index/css/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   155758 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/css/bootstrap.min.css
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   625953 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/css/bootstrap.min.css.map
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18280 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/css/icon.css
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3340 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/css/index.css
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.251039 schedula-1.5.8/schedula/utils/drw/index/js/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    15950 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/js/bootstrap-treeview.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    58072 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/js/bootstrap.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   190253 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/js/bootstrap.min.js.map
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16226 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/js/d3-scale.v3.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88144 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/js/jquery-3.4.1.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6341 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/js/jquery.fullscreen.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    67320 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/index/js/sunburst-chart.min.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1839 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/nodes.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.254176 schedula-1.5.8/schedula/utils/drw/templates/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    18102 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/templates/index.html
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11626 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/templates/render.html
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.254368 schedula-1.5.8/schedula/utils/drw/viz/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)  2396719 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/drw/viz/viz.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    56461 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/dsp.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     1392 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/exc.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.259468 schedula-1.5.8/schedula/utils/form/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11497 2024-04-18 07:55:31.000000 schedula-1.5.8/schedula/utils/form/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6065 2024-04-19 10:04:16.000000 schedula-1.5.8/schedula/utils/form/cli.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5433 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/config.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1986 2024-04-18 10:08:20.000000 schedula-1.5.8/schedula/utils/form/gapp.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1541 2024-04-18 07:56:48.000000 schedula-1.5.8/schedula/utils/form/json_secrets.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1928 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/mail.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.260869 schedula-1.5.8/schedula/utils/form/sample/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      625 2024-04-18 16:02:47.000000 schedula-1.5.8/schedula/utils/form/sample/.babelrc
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      256 2024-04-17 15:20:03.000000 schedula-1.5.8/schedula/utils/form/sample/app.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1866 2024-04-19 10:04:16.000000 schedula-1.5.8/schedula/utils/form/sample/package.json
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.233513 schedula-1.5.8/schedula/utils/form/sample/src/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.262474 schedula-1.5.8/schedula/utils/form/sample/src/index/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      113 2024-04-17 16:48:50.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/editOnChange.js
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.262769 schedula-1.5.8/schedula/utils/form/sample/src/index/fields/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       17 2024-04-17 16:28:10.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/fields/index.js
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.263540 schedula-1.5.8/schedula/utils/form/sample/src/index/formContext/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.263823 schedula-1.5.8/schedula/utils/form/sample/src/index/formContext/components/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       17 2024-04-17 16:28:10.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/formContext/components/index.js
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.264107 schedula-1.5.8/schedula/utils/form/sample/src/index/formContext/domains/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       17 2024-04-17 16:28:10.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/formContext/domains/index.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      107 2024-04-18 06:14:25.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/formContext/index.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      315 2024-04-18 16:22:07.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/index.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      108 2024-04-17 16:28:10.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/postSubmit.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      102 2024-04-17 16:28:10.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/preSubmit.js
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.264380 schedula-1.5.8/schedula/utils/form/sample/src/index/widgets/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       17 2024-04-17 16:28:10.000000 schedula-1.5.8/schedula/utils/form/sample/src/index/widgets/index.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    19654 2024-04-19 10:04:16.000000 schedula-1.5.8/schedula/utils/form/sample/webpack.config.js
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13359 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/server.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.233990 schedula-1.5.8/schedula/utils/form/static/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.234271 schedula-1.5.8/schedula/utils/form/static/schedula/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.268339 schedula-1.5.8/schedula/utils/form/static/schedula/css/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2151 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      280 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      837 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2164 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      137 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      139 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      185 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/4337.588bea5b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      234 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/4452.70b7e4bb.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      346 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/4459.a24c0b46.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/5255.de163d1c.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      314 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/5836.0a2c9e70.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      135 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/6753.de163d1c.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      251 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/6836.4de17ac7.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      499 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/7101.8501d8d8.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/7450.1773328b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      494 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/8428.03ea8396.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      685 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      147 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/9665.80050c43.chunk.css.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/css/main.539ebc22.css.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.268732 schedula-1.5.8/schedula/utils/form/static/schedula/forms/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1326 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/static/schedula/forms/index-schema.json
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/forms/index-ui.json
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.315173 schedula-1.5.8/schedula/utils/form/static/schedula/js/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7227 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1064.c8a95e31.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      546 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1224 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1177.87802691.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      364 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/132.a4de6573.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4265 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1320.36172a41.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      832 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5084 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13937 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      578 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1476.d0e9ba73.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      298 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1511.d20fbe21.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3958 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      291 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/159.42f57d98.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      601 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      779 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16150 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4504 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      936 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1441 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1748.9293df31.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3519 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/183.b47a21b0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      329 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1831.6e43492c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       99 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7430 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      649 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      415 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12856 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2120.8c0a0809.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1281 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       70 2024-04-18 21:33:38.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    36347 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3771 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2256.b2d17449.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4863 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2286.c7768ada.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       78 2024-04-18 21:33:38.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432061 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      324 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6016 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6928 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      388 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      281 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4570 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/268.dcd7a1fb.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2749 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      744 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3768 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2723.fe690409.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4363 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      811 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   468331 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      718 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8687 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    20917 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10227 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3070.687d86ba.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      498 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4704 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1622 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      655 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      465 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3368.b732d88e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    19245 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      279 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3509.62544ca4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      268 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3565.b1e72cb6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      272 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3667.19631032.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3636 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11271 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/368.faa82a4c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1405 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      496 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/3963.54debd2a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    10536 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4048.3d808f93.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11849 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4818 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5839 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/414.1d21b2ba.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      282 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4164.9cdf0caa.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6642 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4279.0095aff5.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      976 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4390.3c3f840c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5055 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4438.4a7723bc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3470 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4452.ae121668.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1781 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      463 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4569.9990e2a1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5746 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3344 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4596.e723b7c7.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1499 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7075 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4673.a90e4863.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1777 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      297 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4842.17363063.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1422 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4218 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    16181 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5025.7d25a45a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      276 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5029.09813ba3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      283 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5051.955a4b55.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3728 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5097.cd4fde21.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4011 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28348 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2750 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2155 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5522.772b12da.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1672 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5652.07f8f3c6.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5672.70cda519.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2752 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      278 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5827.1e26cd85.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1960 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5836.fd1f9bd1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      734 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      284 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5954.df1a43db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     9308 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4893 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11587 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/608.9032add2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      306 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6302.996dbe65.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4645 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6474.54e0a295.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      608 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7293 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6753.b68db48b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      426 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6801.62068c84.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3700 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6836.a7cf7081.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1430 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      334 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6907.0fe74465.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1421 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4333 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2161 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2949 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4366 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6023 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8087 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7435.1a8a10a2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      275 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3130 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       41 2024-04-18 21:33:38.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27276 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3731 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7565.764a83fd.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2984 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     5252 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    37414 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/796.565e7a29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      271 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   266738 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      246 2024-04-18 21:33:38.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4005 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1297 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14837 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1367 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8859 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8148.354b6264.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1014 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8191.b709ea11.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3730 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8259.923684c0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3289 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8428.5b191797.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       81 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28904 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       75 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    13457 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      339 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/853.904196e2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    11594 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8531.d5720770.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12185 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8583.6d996cdc.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     7427 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8698.c7f6106a.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      188 2024-04-18 21:33:38.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     8133 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3512 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      269 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      273 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      425 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4064 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9009.86c17596.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      270 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3720 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9196.45380a31.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6097 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2955 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4148 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2613 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     6409 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      264 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      917 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9622.ef0af135.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      604 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    25595 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      486 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     2218 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/main.fda4aa49.js.LICENSE.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)   432389 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/js/main.fda4aa49.js.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.324992 schedula-1.5.8/schedula/utils/form/static/schedula/media/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89335 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    97121 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88989 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95155 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    94641 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88308 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    95760 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    89222 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    96312 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    88471 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    86875 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    93771 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      229 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/getFetch.40f37ddea2378391108f.cjs.gz
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      515 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.234403 schedula-1.5.8/schedula/utils/form/templates/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.325538 schedula-1.5.8/schedula/utils/form/templates/schedula/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     3610 2024-04-19 10:27:45.000000 schedula-1.5.8/schedula/utils/form/templates/schedula/base.html
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.326395 schedula-1.5.8/schedula/utils/form/templates/schedula/email/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      238 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/templates/schedula/email/contact-body-en.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      250 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/templates/schedula/email/contact-body-it.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       57 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/templates/schedula/email/contact-subject.rst
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       34 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/templates/schedula/index.html
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.237202 schedula-1.5.8/schedula/utils/form/translations/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.234670 schedula-1.5.8/schedula/utils/form/translations/af_ZA/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.326556 schedula-1.5.8/schedula/utils/form/translations/af_ZA/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27931 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/af_ZA/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.234795 schedula-1.5.8/schedula/utils/form/translations/ca_ES/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.327091 schedula-1.5.8/schedula/utils/form/translations/ca_ES/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27418 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/ca_ES/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.234926 schedula-1.5.8/schedula/utils/form/translations/da_DK/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.327994 schedula-1.5.8/schedula/utils/form/translations/da_DK/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    26537 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/da_DK/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235056 schedula-1.5.8/schedula/utils/form/translations/de_DE/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.328383 schedula-1.5.8/schedula/utils/form/translations/de_DE/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27565 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/de_DE/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235181 schedula-1.5.8/schedula/utils/form/translations/en_US/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.328657 schedula-1.5.8/schedula/utils/form/translations/en_US/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    22850 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/en_US/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235303 schedula-1.5.8/schedula/utils/form/translations/es_ES/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.328950 schedula-1.5.8/schedula/utils/form/translations/es_ES/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27478 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/es_ES/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235427 schedula-1.5.8/schedula/utils/form/translations/eu_ES/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.329217 schedula-1.5.8/schedula/utils/form/translations/eu_ES/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27136 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/eu_ES/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235555 schedula-1.5.8/schedula/utils/form/translations/fr_FR/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.329446 schedula-1.5.8/schedula/utils/form/translations/fr_FR/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28935 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/fr_FR/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235685 schedula-1.5.8/schedula/utils/form/translations/hu_HU/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.329681 schedula-1.5.8/schedula/utils/form/translations/hu_HU/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28296 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/hu_HU/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235806 schedula-1.5.8/schedula/utils/form/translations/hy_AM/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.329896 schedula-1.5.8/schedula/utils/form/translations/hy_AM/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    32154 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/hy_AM/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.235936 schedula-1.5.8/schedula/utils/form/translations/is_IS/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.330143 schedula-1.5.8/schedula/utils/form/translations/is_IS/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27667 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/is_IS/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.236070 schedula-1.5.8/schedula/utils/form/translations/it_IT/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.330984 schedula-1.5.8/schedula/utils/form/translations/it_IT/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    24359 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/it_IT/LC_MESSAGES/antd.po
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    12590 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/it_IT/LC_MESSAGES/flask_security.mo
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    19544 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/it_IT/LC_MESSAGES/flask_security.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.236207 schedula-1.5.8/schedula/utils/form/translations/ja_JP/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.331256 schedula-1.5.8/schedula/utils/form/translations/ja_JP/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    28930 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/ja_JP/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.236328 schedula-1.5.8/schedula/utils/form/translations/nl_NL/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.331803 schedula-1.5.8/schedula/utils/form/translations/nl_NL/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    26330 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/nl_NL/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.236443 schedula-1.5.8/schedula/utils/form/translations/pl_PL/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.332040 schedula-1.5.8/schedula/utils/form/translations/pl_PL/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    27176 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/pl_PL/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.236568 schedula-1.5.8/schedula/utils/form/translations/pt_BR/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.332273 schedula-1.5.8/schedula/utils/form/translations/pt_BR/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    26832 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/pt_BR/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.236692 schedula-1.5.8/schedula/utils/form/translations/pt_PT/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.332500 schedula-1.5.8/schedula/utils/form/translations/pt_PT/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    26725 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/pt_PT/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.236903 schedula-1.5.8/schedula/utils/form/translations/ru_RU/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.332713 schedula-1.5.8/schedula/utils/form/translations/ru_RU/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    32462 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/ru_RU/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.237115 schedula-1.5.8/schedula/utils/form/translations/tr_TR/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.333069 schedula-1.5.8/schedula/utils/form/translations/tr_TR/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    26511 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/tr_TR/LC_MESSAGES/antd.po
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.237265 schedula-1.5.8/schedula/utils/form/translations/zh_Hans_CN/
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.333535 schedula-1.5.8/schedula/utils/form/translations/zh_Hans_CN/LC_MESSAGES/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    25640 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/form/translations/zh_Hans_CN/LC_MESSAGES/antd.po
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     2194 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/gen.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     4332 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/graph.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      692 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/imp.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.333736 schedula-1.5.8/schedula/utils/io/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     6380 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/io/__init__.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    40509 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/sol.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1630 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/utl.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.334003 schedula-1.5.8/schedula/utils/web/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7053 2024-04-12 16:17:27.000000 schedula-1.5.8/schedula/utils/web/__init__.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.336008 schedula-1.5.8/schedula.egg-info/
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    14759 2024-04-19 12:08:09.000000 schedula-1.5.8/schedula.egg-info/PKG-INFO
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)    17862 2024-04-19 12:08:09.000000 schedula-1.5.8/schedula.egg-info/SOURCES.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        1 2024-04-19 12:08:09.000000 schedula-1.5.8/schedula.egg-info/dependency_links.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)       46 2024-04-19 12:08:09.000000 schedula-1.5.8/schedula.egg-info/entry_points.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1083 2024-04-19 12:08:09.000000 schedula-1.5.8/schedula.egg-info/requires.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)        9 2024-04-19 12:08:09.000000 schedula-1.5.8/schedula.egg-info/top_level.txt
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)      162 2024-04-19 12:08:09.340740 schedula-1.5.8/setup.cfg
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)     7360 2024-04-19 12:06:22.000000 schedula-1.5.8/setup.py
+drwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)        0 2024-04-19 12:08:09.335623 schedula-1.5.8/tests/
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)    89504 2024-04-12 16:17:27.000000 schedula-1.5.8/tests/test_dispatcher.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1020 2024-04-12 16:17:27.000000 schedula-1.5.8/tests/test_import.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1164 2024-04-12 16:17:27.000000 schedula-1.5.8/tests/test_micropython.py
+-rwxr-xr-x   0 vincenzoarcidiacono   (503) staff       (20)      872 2024-04-12 16:17:27.000000 schedula-1.5.8/tests/test_readme.py
+-rw-r--r--   0 vincenzoarcidiacono   (503) staff       (20)     1028 2024-04-12 16:17:27.000000 schedula-1.5.8/tests/test_setup.py
```

### Comparing `schedula-1.5.7/LICENSE.txt` & `schedula-1.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/PKG-INFO` & `schedula-1.5.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula
-Version: 1.5.7
+Version: 1.5.8
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.8
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-1.5.7/README.rst` & `schedula-1.5.8/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 
 #######################################################################
 schedula: A smart function scheduler for dynamic flow-based programming
 #######################################################################
 |pypi_ver| |test_status| |cover_status| |docs_status| |downloads|
 |month_downloads| |github_issues| |python_ver| |proj_license| |binder|
 
-:release:       1.5.7
-:date:          2024-04-19 12:30:00
+:release:       1.5.8
+:date:          2024-04-20 00:00:00
 :repository:    https://github.com/vinci1it2000/schedula
 :pypi-repo:     https://pypi.org/project/schedula/
 :docs:          https://schedula.readthedocs.io/
 :wiki:          https://github.com/vinci1it2000/schedula/wiki/
 :download:      https://github.com/vinci1it2000/schedula/releases/
 :keywords:      flow-based programming, dataflow, parallel, async, scheduling,
                 dispatch, functional programming, dataflow programming
```

### Comparing `schedula-1.5.7/schedula/__init__.py` & `schedula-1.5.8/schedula/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/_version.py` & `schedula-1.5.8/schedula/_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,19 +5,19 @@
 # You may not use this work except in compliance with the Licence.
 # You may obtain a copy of the Licence at: http://ec.europa.eu/idabc/eupl
 
 __all__ = ['__version__', '__updated__', '__title__', '__author__',
            '__license__', '__copyright__']
 
 #: Authoritative project's PEP 440 version.
-__version__ = version = "1.5.7"  # Also update README.rst
+__version__ = version = "1.5.8"  # Also update README.rst
 
 # Please UPDATE TIMESTAMP WHEN BUMPING VERSIONS AND BEFORE RELEASE.
 #: Release date.
-__updated__ = "2024-04-19 12:30:00"
+__updated__ = "2024-04-20 00:00:00"
 
 __title__ = 'schedula'
 
 __author__ = 'Vincenzo Arcidiacono <vinci1it2000@gmail.com>'
 
 __license__ = 'EUPL, see LICENSE.txt'
```

### Comparing `schedula-1.5.7/schedula/cli.py` & `schedula-1.5.8/schedula/cli.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/dispatcher.py` & `schedula-1.5.8/schedula/dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/ext/autosummary.py` & `schedula-1.5.8/schedula/ext/autosummary.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/ext/dispatcher/__init__.py` & `schedula-1.5.8/schedula/ext/dispatcher/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/ext/dispatcher/documenter.py` & `schedula-1.5.8/schedula/ext/dispatcher/documenter.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/ext/dispatcher/graphviz.py` & `schedula-1.5.8/schedula/ext/dispatcher/graphviz.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/__init__.py` & `schedula-1.5.8/schedula/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/alg.py` & `schedula-1.5.8/schedula/utils/alg.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/asy/__init__.py` & `schedula-1.5.8/schedula/utils/asy/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/asy/executors.py` & `schedula-1.5.8/schedula/utils/asy/executors.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/asy/factory.py` & `schedula-1.5.8/schedula/utils/asy/factory.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/base.py` & `schedula-1.5.8/schedula/utils/base.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/blue.py` & `schedula-1.5.8/schedula/utils/blue.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/cst.py` & `schedula-1.5.8/schedula/utils/cst.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/des/__init__.py` & `schedula-1.5.8/schedula/utils/des/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/__init__.py` & `schedula-1.5.8/schedula/utils/drw/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css` & `schedula-1.5.8/schedula/utils/drw/index/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/css/bootstrap.min.css.map` & `schedula-1.5.8/schedula/utils/drw/index/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/css/icon.css` & `schedula-1.5.8/schedula/utils/drw/index/css/icon.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/css/index.css` & `schedula-1.5.8/schedula/utils/drw/index/css/index.css`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/js/bootstrap-treeview.min.js` & `schedula-1.5.8/schedula/utils/drw/index/js/bootstrap-treeview.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js` & `schedula-1.5.8/schedula/utils/drw/index/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/js/bootstrap.min.js.map` & `schedula-1.5.8/schedula/utils/drw/index/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/js/d3-scale.v3.min.js` & `schedula-1.5.8/schedula/utils/drw/index/js/d3-scale.v3.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/js/jquery-3.4.1.min.js` & `schedula-1.5.8/schedula/utils/drw/index/js/jquery-3.4.1.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/js/jquery.fullscreen.min.js` & `schedula-1.5.8/schedula/utils/drw/index/js/jquery.fullscreen.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/index/js/sunburst-chart.min.js` & `schedula-1.5.8/schedula/utils/drw/index/js/sunburst-chart.min.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/nodes.py` & `schedula-1.5.8/schedula/utils/drw/nodes.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/templates/index.html` & `schedula-1.5.8/schedula/utils/drw/templates/index.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/templates/render.html` & `schedula-1.5.8/schedula/utils/drw/templates/render.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/drw/viz/viz.js` & `schedula-1.5.8/schedula/utils/drw/viz/viz.js`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/dsp.py` & `schedula-1.5.8/schedula/utils/dsp.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/exc.py` & `schedula-1.5.8/schedula/utils/exc.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/__init__.py` & `schedula-1.5.8/schedula/utils/form/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/cli.py` & `schedula-1.5.8/schedula/utils/form/cli.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/config.py` & `schedula-1.5.8/schedula/utils/form/config.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/gapp.py` & `schedula-1.5.8/schedula/utils/form/gapp.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/json_secrets.py` & `schedula-1.5.8/schedula/utils/form/json_secrets.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/mail.py` & `schedula-1.5.8/schedula/utils/form/mail.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/server.py` & `schedula-1.5.8/schedula/utils/form/server.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/css/9003.d2d6266b.chunk.css.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/forms/index-schema.json` & `schedula-1.5.8/schedula/utils/form/static/schedula/forms/index-schema.json`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/forms/index-ui.json` & `schedula-1.5.8/schedula/utils/form/static/schedula/forms/index-ui.json`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1064.c8a95e31.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1064.c8a95e31.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1165.ff804d16.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1177.87802691.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1177.87802691.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1320.36172a41.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1320.36172a41.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1362.0594020f.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1431.780747e9.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1432.f3b34f42.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1465.edd9ba38.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1583.fbdd1527.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1641.cc9646e9.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1642.5186d671.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1748.9293df31.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1748.9293df31.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/183.b47a21b0.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/183.b47a21b0.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2120.8c0a0809.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2120.8c0a0809.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2256.b2d17449.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2256.b2d17449.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2286.c7768ada.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2286.c7768ada.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/268.dcd7a1fb.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/268.dcd7a1fb.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2723.fe690409.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2723.fe690409.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3070.687d86ba.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3070.687d86ba.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3281.a4f1ba69.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3327.f5840c2f.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3333.3da6381e.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3457.a6f7a355.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3642.27ee29bf.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3676.1ee61f29.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/368.faa82a4c.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/368.faa82a4c.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/3850.689e0ff9.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4048.3d808f93.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4048.3d808f93.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4093.1b358dc3.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4095.87cc9b62.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/414.1d21b2ba.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/414.1d21b2ba.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4279.0095aff5.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4279.0095aff5.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4337.8da858ce.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4438.4a7723bc.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4438.4a7723bc.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4452.ae121668.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4452.ae121668.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4459.6704ca6e.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4587.5ff7f02e.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4596.e723b7c7.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4596.e723b7c7.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4672.f1f003ed.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4673.a90e4863.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4673.a90e4863.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4786.f0dbe7a4.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4906.d6a6dad2.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/4925.6cb145d6.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5025.7d25a45a.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5025.7d25a45a.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5097.cd4fde21.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5097.cd4fde21.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5255.baba9ad1.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5349.d6abdf80.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5415.96511657.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5459.ab6195a8.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5652.07f8f3c6.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5652.07f8f3c6.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5672.70cda519.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5672.70cda519.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5784.aa6dfd10.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5836.fd1f9bd1.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5836.fd1f9bd1.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5880.5ad7e40e.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/5959.d5ebe3fe.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6043.6bea23a4.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/608.9032add2.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/608.9032add2.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6474.54e0a295.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6474.54e0a295.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/654.98d33eb8.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6753.b68db48b.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6753.b68db48b.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6836.a7cf7081.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6836.a7cf7081.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6855.c4d51fc1.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6925.228697fa.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6938.c8986bc2.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7435.1a8a10a2.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7435.1a8a10a2.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7565.764a83fd.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7565.764a83fd.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/796.565e7a29.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/796.565e7a29.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8148.354b6264.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8148.354b6264.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8191.b709ea11.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8191.b709ea11.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8259.923684c0.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8259.923684c0.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8428.5b191797.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8428.5b191797.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8531.d5720770.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8531.d5720770.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8583.6d996cdc.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8583.6d996cdc.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8698.c7f6106a.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8698.c7f6106a.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9009.86c17596.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9009.86c17596.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9196.45380a31.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9196.45380a31.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9235.b2714593.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9238.8ae8b0d0.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9367.127331a0.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9622.ef0af135.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9622.ef0af135.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/js/main.fda4aa49.js.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/js/main.fda4aa49.js.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-LightItalic.c590382422f2742d788b.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Medium.7c8d04cd831df3033c8a.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-MediumItalic.82736aaa11c64709055f.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Regular.fc2b5060f7accec5cf74.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-Thin.a732a12eb07742232407.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/Roboto-ThinItalic.9d2ca34eae96e77c6eef.ttf.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz` & `schedula-1.5.8/schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/form/templates/schedula/base.html` & `schedula-1.5.8/schedula/utils/form/templates/schedula/base.html`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/gen.py` & `schedula-1.5.8/schedula/utils/gen.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/graph.py` & `schedula-1.5.8/schedula/utils/graph.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/imp.py` & `schedula-1.5.8/schedula/utils/imp.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/io/__init__.py` & `schedula-1.5.8/schedula/utils/io/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/sol.py` & `schedula-1.5.8/schedula/utils/sol.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/utl.py` & `schedula-1.5.8/schedula/utils/utl.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula/utils/web/__init__.py` & `schedula-1.5.8/schedula/utils/web/__init__.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/schedula.egg-info/PKG-INFO` & `schedula-1.5.8/schedula.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: schedula
-Version: 1.5.7
+Version: 1.5.8
 Summary: Produce a plan that dispatches calls based on a graph of functions, satisfying data dependencies.
 Home-page: https://github.com/vinci1it2000/schedula
-Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.7
+Download-URL: https://github.com/vinci1it2000/schedula/tarball/v1.5.8
 Author: Vincenzo Arcidiacono
 Author-email: vinci1it2000@gmail.com
 License: EUPL 1.1+
 Project-URL: Documentation, https://schedula.readthedocs.io
 Project-URL: Issue tracker, https://github.com/vinci1it2000/schedula/issues
 Keywords: flow-based programming,dataflow,parallel,asynchronous,async,scheduling,dispatch,functional programming,dataflow programming
 Classifier: Programming Language :: Python
```

### Comparing `schedula-1.5.7/schedula.egg-info/SOURCES.txt` & `schedula-1.5.8/schedula.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -53,14 +53,27 @@
 schedula/utils/form/__init__.py
 schedula/utils/form/cli.py
 schedula/utils/form/config.py
 schedula/utils/form/gapp.py
 schedula/utils/form/json_secrets.py
 schedula/utils/form/mail.py
 schedula/utils/form/server.py
+schedula/utils/form/sample/.babelrc
+schedula/utils/form/sample/app.py
+schedula/utils/form/sample/package.json
+schedula/utils/form/sample/webpack.config.js
+schedula/utils/form/sample/src/index/editOnChange.js
+schedula/utils/form/sample/src/index/index.js
+schedula/utils/form/sample/src/index/postSubmit.js
+schedula/utils/form/sample/src/index/preSubmit.js
+schedula/utils/form/sample/src/index/fields/index.js
+schedula/utils/form/sample/src/index/formContext/index.js
+schedula/utils/form/sample/src/index/formContext/components/index.js
+schedula/utils/form/sample/src/index/formContext/domains/index.js
+schedula/utils/form/sample/src/index/widgets/index.js
 schedula/utils/form/static/schedula/css/1362.038687f8.chunk.css.gz
 schedula/utils/form/static/schedula/css/1724.5fbb5eb3.chunk.css.gz
 schedula/utils/form/static/schedula/css/1737.87abdd03.chunk.css.gz
 schedula/utils/form/static/schedula/css/2286.6e5fc492.chunk.css.gz
 schedula/utils/form/static/schedula/css/2706.83c2b1be.chunk.css.gz
 schedula/utils/form/static/schedula/css/3667.3d691932.chunk.css.gz
 schedula/utils/form/static/schedula/css/414.4a9f9388.chunk.css.gz
@@ -97,33 +110,37 @@
 schedula/utils/form/static/schedula/js/1656.c5fbd8dc.chunk.js.gz
 schedula/utils/form/static/schedula/js/1678.b278cefb.chunk.js.gz
 schedula/utils/form/static/schedula/js/1724.d97efc34.chunk.js.gz
 schedula/utils/form/static/schedula/js/1737.13089dbe.chunk.js.gz
 schedula/utils/form/static/schedula/js/1748.9293df31.chunk.js.gz
 schedula/utils/form/static/schedula/js/183.b47a21b0.chunk.js.gz
 schedula/utils/form/static/schedula/js/1831.6e43492c.chunk.js.gz
+schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/1973.f98049be.chunk.js.gz
 schedula/utils/form/static/schedula/js/2055.204f9b8c.chunk.js.gz
 schedula/utils/form/static/schedula/js/2085.3afcba83.chunk.js.gz
 schedula/utils/form/static/schedula/js/2120.8c0a0809.chunk.js.gz
 schedula/utils/form/static/schedula/js/2128.9a07d096.chunk.js.gz
+schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/218.37c2a3e8.chunk.js.gz
 schedula/utils/form/static/schedula/js/2256.b2d17449.chunk.js.gz
 schedula/utils/form/static/schedula/js/2286.c7768ada.chunk.js.gz
+schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/24.5f2a5395.chunk.js.gz
 schedula/utils/form/static/schedula/js/2452.288238f6.chunk.js.gz
 schedula/utils/form/static/schedula/js/2506.47c8c058.chunk.js.gz
 schedula/utils/form/static/schedula/js/2556.ab2f7391.chunk.js.gz
 schedula/utils/form/static/schedula/js/2604.46d4f061.chunk.js.gz
 schedula/utils/form/static/schedula/js/2638.b7999325.chunk.js.gz
 schedula/utils/form/static/schedula/js/268.dcd7a1fb.chunk.js.gz
 schedula/utils/form/static/schedula/js/2698.09529134.chunk.js.gz
 schedula/utils/form/static/schedula/js/2706.a995f39e.chunk.js.gz
 schedula/utils/form/static/schedula/js/2723.fe690409.chunk.js.gz
 schedula/utils/form/static/schedula/js/2742.e2a045d8.chunk.js.gz
+schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/2768.200f44b2.chunk.js.gz
 schedula/utils/form/static/schedula/js/287.053696ba.chunk.js.gz
 schedula/utils/form/static/schedula/js/2894.d8c25e8b.chunk.js.gz
 schedula/utils/form/static/schedula/js/3052.40fbeb2c.chunk.js.gz
 schedula/utils/form/static/schedula/js/3070.687d86ba.chunk.js.gz
 schedula/utils/form/static/schedula/js/3099.e186daed.chunk.js.gz
 schedula/utils/form/static/schedula/js/3101.c13d903f.chunk.js.gz
@@ -192,34 +209,41 @@
 schedula/utils/form/static/schedula/js/6984.ab1ec70c.chunk.js.gz
 schedula/utils/form/static/schedula/js/7035.5a8c5d98.chunk.js.gz
 schedula/utils/form/static/schedula/js/7101.48b6eb7a.chunk.js.gz
 schedula/utils/form/static/schedula/js/7106.0babb553.chunk.js.gz
 schedula/utils/form/static/schedula/js/7435.1a8a10a2.chunk.js.gz
 schedula/utils/form/static/schedula/js/744.c1913bc4.chunk.js.gz
 schedula/utils/form/static/schedula/js/7450.d618087b.chunk.js.gz
+schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/7522.bc15dd2d.chunk.js.gz
 schedula/utils/form/static/schedula/js/7565.764a83fd.chunk.js.gz
 schedula/utils/form/static/schedula/js/78.d0c28d0b.chunk.js.gz
 schedula/utils/form/static/schedula/js/7828.8fdd74db.chunk.js.gz
 schedula/utils/form/static/schedula/js/796.565e7a29.chunk.js.gz
+schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/7974.f3ea029b.chunk.js.gz
+schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/8007.cbee9608.chunk.js.gz
+schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/8047.6dae9f00.chunk.js.gz
 schedula/utils/form/static/schedula/js/8119.038d4e91.chunk.js.gz
 schedula/utils/form/static/schedula/js/8148.354b6264.chunk.js.gz
 schedula/utils/form/static/schedula/js/8191.b709ea11.chunk.js.gz
 schedula/utils/form/static/schedula/js/8259.923684c0.chunk.js.gz
 schedula/utils/form/static/schedula/js/8384.733495df.chunk.js.gz
 schedula/utils/form/static/schedula/js/8428.5b191797.chunk.js.gz
+schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/8497.83aecf6b.chunk.js.gz
+schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/8516.103cbc32.chunk.js.gz
 schedula/utils/form/static/schedula/js/853.904196e2.chunk.js.gz
 schedula/utils/form/static/schedula/js/8531.d5720770.chunk.js.gz
 schedula/utils/form/static/schedula/js/8583.6d996cdc.chunk.js.gz
 schedula/utils/form/static/schedula/js/8698.c7f6106a.chunk.js.gz
+schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/8703.743baf71.chunk.js.gz
 schedula/utils/form/static/schedula/js/875.2593b9db.chunk.js.gz
 schedula/utils/form/static/schedula/js/8797.9e3c01c2.chunk.js.gz
 schedula/utils/form/static/schedula/js/8916.4a5d5d2c.chunk.js.gz
 schedula/utils/form/static/schedula/js/9003.b108ee29.chunk.js.gz
 schedula/utils/form/static/schedula/js/9009.86c17596.chunk.js.gz
 schedula/utils/form/static/schedula/js/9079.476a64c2.chunk.js.gz
@@ -230,14 +254,15 @@
 schedula/utils/form/static/schedula/js/9419.1497cff3.chunk.js.gz
 schedula/utils/form/static/schedula/js/9517.d6983e61.chunk.js.gz
 schedula/utils/form/static/schedula/js/9559.52882117.chunk.js.gz
 schedula/utils/form/static/schedula/js/9622.ef0af135.chunk.js.gz
 schedula/utils/form/static/schedula/js/9665.8425fb6b.chunk.js.gz
 schedula/utils/form/static/schedula/js/9919.f339f893.chunk.js.gz
 schedula/utils/form/static/schedula/js/9925.cc714497.chunk.js.gz
+schedula/utils/form/static/schedula/js/main.fda4aa49.js.LICENSE.txt
 schedula/utils/form/static/schedula/js/main.fda4aa49.js.gz
 schedula/utils/form/static/schedula/media/Roboto-Black.cf56c1b149d0a5e8d7c6.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-BlackItalic.fd62a10743bd89a3d97c.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Bold.f80816a5455d171f948d.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-BoldItalic.87d61cea6fe1d235d4a8.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Italic.87f3afe16a8c3c370634.ttf.gz
 schedula/utils/form/static/schedula/media/Roboto-Light.333da16a3f3cc391d087.ttf.gz
@@ -250,14 +275,36 @@
 schedula/utils/form/static/schedula/media/getFetch.40f37ddea2378391108f.cjs.gz
 schedula/utils/form/static/schedula/media/index.42119833dddefe38a9fa.cjs.gz
 schedula/utils/form/templates/schedula/base.html
 schedula/utils/form/templates/schedula/index.html
 schedula/utils/form/templates/schedula/email/contact-body-en.rst
 schedula/utils/form/templates/schedula/email/contact-body-it.rst
 schedula/utils/form/templates/schedula/email/contact-subject.rst
+schedula/utils/form/translations/af_ZA/LC_MESSAGES/antd.po
+schedula/utils/form/translations/ca_ES/LC_MESSAGES/antd.po
+schedula/utils/form/translations/da_DK/LC_MESSAGES/antd.po
+schedula/utils/form/translations/de_DE/LC_MESSAGES/antd.po
+schedula/utils/form/translations/en_US/LC_MESSAGES/antd.po
+schedula/utils/form/translations/es_ES/LC_MESSAGES/antd.po
+schedula/utils/form/translations/eu_ES/LC_MESSAGES/antd.po
+schedula/utils/form/translations/fr_FR/LC_MESSAGES/antd.po
+schedula/utils/form/translations/hu_HU/LC_MESSAGES/antd.po
+schedula/utils/form/translations/hy_AM/LC_MESSAGES/antd.po
+schedula/utils/form/translations/is_IS/LC_MESSAGES/antd.po
+schedula/utils/form/translations/it_IT/LC_MESSAGES/antd.po
+schedula/utils/form/translations/it_IT/LC_MESSAGES/flask_security.mo
+schedula/utils/form/translations/it_IT/LC_MESSAGES/flask_security.po
+schedula/utils/form/translations/ja_JP/LC_MESSAGES/antd.po
+schedula/utils/form/translations/nl_NL/LC_MESSAGES/antd.po
+schedula/utils/form/translations/pl_PL/LC_MESSAGES/antd.po
+schedula/utils/form/translations/pt_BR/LC_MESSAGES/antd.po
+schedula/utils/form/translations/pt_PT/LC_MESSAGES/antd.po
+schedula/utils/form/translations/ru_RU/LC_MESSAGES/antd.po
+schedula/utils/form/translations/tr_TR/LC_MESSAGES/antd.po
+schedula/utils/form/translations/zh_Hans_CN/LC_MESSAGES/antd.po
 schedula/utils/io/__init__.py
 schedula/utils/web/__init__.py
 tests/test_dispatcher.py
 tests/test_import.py
 tests/test_micropython.py
 tests/test_readme.py
 tests/test_setup.py
```

### Comparing `schedula-1.5.7/schedula.egg-info/requires.txt` & `schedula-1.5.8/schedula.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/setup.py` & `schedula-1.5.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -180,17 +180,19 @@
         extras_require=extras,
         tests_require=['requests', 'cryptography', 'ddt'],
         package_data={
             'schedula.utils.drw': [
                 'templates/*', 'index/js/*', 'index/css/*', 'viz/*'
             ],
             'schedula.utils.form': [
-                'templates/schedula/*', 'static/schedula/js/*.js.gz',
-                'static/schedula/css/*.css.gz',
-                'static/schedula/media/*.gz',
                 'static/schedula/forms/*',
-                'templates/schedula/*',
-                'templates/schedula/email/*'
+                'static/schedula/**/*.gz',
+                'static/schedula/**/*.LICENSE.txt',
+                'templates/**/*',
+                'sample/.babelrc',
+                'sample/*.*',
+                'sample/src/**/*',
+                'translations/**/*'
             ]
         },
         **kw
     )
```

### Comparing `schedula-1.5.7/tests/test_dispatcher.py` & `schedula-1.5.8/tests/test_dispatcher.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/tests/test_import.py` & `schedula-1.5.8/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/tests/test_micropython.py` & `schedula-1.5.8/tests/test_micropython.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/tests/test_readme.py` & `schedula-1.5.8/tests/test_readme.py`

 * *Files identical despite different names*

### Comparing `schedula-1.5.7/tests/test_setup.py` & `schedula-1.5.8/tests/test_setup.py`

 * *Files identical despite different names*

