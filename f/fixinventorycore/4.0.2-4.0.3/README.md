# Comparing `tmp/fixinventorycore-4.0.2.tar.gz` & `tmp/fixinventorycore-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventorycore-4.0.2.tar", last modified: Fri Apr 12 12:17:10 2024, max compression
+gzip compressed data, was "fixinventorycore-4.0.3.tar", last modified: Wed Apr 24 10:33:00 2024, max compression
```

## Comparing `fixinventorycore-4.0.2.tar` & `fixinventorycore-4.0.3.tar`

### file list

```diff
@@ -1,754 +1,754 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.373278 fixinventorycore-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-12 12:17:10.373278 fixinventorycore-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.257278 fixinventorycore-4.0.2/fixcore/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.257278 fixinventorycore-4.0.2/fixcore/action_handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/action_handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/action_handlers/merge_outer_edge_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.257278 fixinventorycore-4.0.2/fixcore/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/analytics/posthog.py
--rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/analytics/recurrent_events.py
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/async_extensions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.257278 fixinventorycore-4.0.2/fixcore/cli/
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    31738 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/cli/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)   276516 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/cli/command.py
--rw-r--r--   0 runner    (1001) docker     (127)    29181 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/cli/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/cli/tip_of_the_day.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/compat.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.257278 fixinventorycore-4.0.2/fixcore/config/
--rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13420 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/config/config_handler_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/config/config_override_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/config/core_config_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/console_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    35525 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/core_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.261278 fixinventorycore-4.0.2/fixcore/db/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    45739 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/arango_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/arangodb_extensions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/arangodb_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/async_arangodb.py
--rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/configdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    31907 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/db_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/deferredouteredgedb.py
--rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (127)    87214 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/graphdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/jobdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/model.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/modeldb.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/packagedb.py
--rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/reportdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/runningtaskdb.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/system_data_db.py
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/templatedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    13535 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/timeseriesdb.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/db/usagedb.py
--rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.261278 fixinventorycore-4.0.2/fixcore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/graph_manager/graph_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/ids.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.261278 fixinventorycore-4.0.2/fixcore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/infra_apps/local_runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/infra_apps/manifest.py
--rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/infra_apps/package_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/infra_apps/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.265278 fixinventorycore-4.0.2/fixcore/jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.245278 fixinventorycore-4.0.2/fixcore/jupyterlite/api/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.265278 fixinventorycore-4.0.2/fixcore/jupyterlite/api/contents/
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-12 12:17:08.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/api/contents/all.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.265278 fixinventorycore-4.0.2/fixcore/jupyterlite/api/translations/
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-12 12:17:08.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/api/translations/all.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-12 12:17:08.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/api/translations/en.json
--rw-r--r--   0 runner    (1001) docker     (127)     3223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/bootstrap.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.325278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/
--rw-r--r--   0 runner    (1001) docker     (127)    40339 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1053.7a56130.js
--rw-r--r--   0 runner    (1001) docker     (127)     4145 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1088.33c6076.js
--rw-r--r--   0 runner    (1001) docker     (127)     9193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1091.1cf35e6.js
--rw-r--r--   0 runner    (1001) docker     (127)     5021 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1122.d86c258.js
--rw-r--r--   0 runner    (1001) docker     (127)     1079 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/114.1c04540.js
--rw-r--r--   0 runner    (1001) docker     (127)     4133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1169.4cf2d13.js
--rw-r--r--   0 runner    (1001) docker     (127)     2128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/125.4c6ac03.js
--rw-r--r--   0 runner    (1001) docker     (127)    45561 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1261.3da9a56.js
--rw-r--r--   0 runner    (1001) docker     (127)    17387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/131.5b6a7ab.js
--rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1385.707019c.js
--rw-r--r--   0 runner    (1001) docker     (127)     9183 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1388.0f22ef8.js
--rw-r--r--   0 runner    (1001) docker     (127)     2081 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1418.d9431d8.js
--rw-r--r--   0 runner    (1001) docker     (127)   412668 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/142.6e89fb8.js
--rw-r--r--   0 runner    (1001) docker     (127)   457855 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1495.671bdd4.js
--rw-r--r--   0 runner    (1001) docker     (127)      493 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1495.671bdd4.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   133253 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1542.22098a5.js
--rw-r--r--   0 runner    (1001) docker     (127)      483 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1542.22098a5.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2053 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1558.548303d.js
--rw-r--r--   0 runner    (1001) docker     (127)    35637 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1584.d919fce.js
--rw-r--r--   0 runner    (1001) docker     (127)     4181 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1618.983fc32.js
--rw-r--r--   0 runner    (1001) docker     (127)    18800 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1715.ebbb93b.js
--rw-r--r--   0 runner    (1001) docker     (127)     6293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1769.10c2b5d.js
--rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1815.2af66e5.js
--rw-r--r--   0 runner    (1001) docker     (127)     5509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1837.622ebbe.js
--rw-r--r--   0 runner    (1001) docker     (127)     4941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1846.ed084ce.js
--rw-r--r--   0 runner    (1001) docker     (127)      612 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1869.86f5778.js
--rw-r--r--   0 runner    (1001) docker     (127)    74760 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1871.7fed383.js
--rw-r--r--   0 runner    (1001) docker     (127)      945 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/1941.79180b2.js
--rw-r--r--   0 runner    (1001) docker     (127)   119985 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2065.410c3bc.js
--rw-r--r--   0 runner    (1001) docker     (127)    20937 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/214.300dbf1.js
--rw-r--r--   0 runner    (1001) docker     (127)     3072 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2188.9676797.js
--rw-r--r--   0 runner    (1001) docker     (127)     2185 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/221.59c0059.js
--rw-r--r--   0 runner    (1001) docker     (127)    16250 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2213.b58cab4.js
--rw-r--r--   0 runner    (1001) docker     (127)    82064 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2241.91c6cce.js
--rw-r--r--   0 runner    (1001) docker     (127)    47604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2323.7e4d795.js
--rw-r--r--   0 runner    (1001) docker     (127)  1481212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2324.aff3939.js
--rw-r--r--   0 runner    (1001) docker     (127)     4331 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2343.3cf0fe8.js
--rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2349.9acb0b1.js
--rw-r--r--   0 runner    (1001) docker     (127)     2129 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2363.6aa6a7f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2405 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2386.5f8e2da.js
--rw-r--r--   0 runner    (1001) docker     (127)    29147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2520.5c65366.js
--rw-r--r--   0 runner    (1001) docker     (127)    54845 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2552.6c5224e.js
--rw-r--r--   0 runner    (1001) docker     (127)    37964 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/261.431b309.js
--rw-r--r--   0 runner    (1001) docker     (127)     2784 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2622.3d61d64.js
--rw-r--r--   0 runner    (1001) docker     (127)    12742 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2666.6cce729.js
--rw-r--r--   0 runner    (1001) docker     (127)     1216 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2682.0c612a1.js
--rw-r--r--   0 runner    (1001) docker     (127)    30032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2692.f2b8d53.js
--rw-r--r--   0 runner    (1001) docker     (127)     7589 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/270.9675bfe.js
--rw-r--r--   0 runner    (1001) docker     (127)      745 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2702.0e1a6ff.js
--rw-r--r--   0 runner    (1001) docker     (127)    55572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/28.9f8dd00.js
--rw-r--r--   0 runner    (1001) docker     (127)     6706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2871.e1a64a6.js
--rw-r--r--   0 runner    (1001) docker     (127)   128665 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2913.25c5e72.js
--rw-r--r--   0 runner    (1001) docker     (127)      559 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   256757 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2930.896decd.js
--rw-r--r--   0 runner    (1001) docker     (127)   169282 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/2955.c8d0773.js
--rw-r--r--   0 runner    (1001) docker     (127)    74307 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/306.b568c30.js
--rw-r--r--   0 runner    (1001) docker     (127)    35812 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3079.18e3c32.js
--rw-r--r--   0 runner    (1001) docker     (127)     3294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/311.76f79fc.js
--rw-r--r--   0 runner    (1001) docker     (127)     4341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3111.8de2d0a.js
--rw-r--r--   0 runner    (1001) docker     (127)     4545 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3154.5d8f80d.js
--rw-r--r--   0 runner    (1001) docker     (127)     4274 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3211.aa42b4a.js
--rw-r--r--   0 runner    (1001) docker     (127)     5817 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3218.758a794.js
--rw-r--r--   0 runner    (1001) docker     (127)       99 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3218.758a794.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     6827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3230.2c849ff.js
--rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3245.c48f805.js
--rw-r--r--   0 runner    (1001) docker     (127)     9703 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3322.428e385.js
--rw-r--r--   0 runner    (1001) docker     (127)     2505 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3336.3d4780f.js
--rw-r--r--   0 runner    (1001) docker     (127)     2502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3370.b5d78cd.js
--rw-r--r--   0 runner    (1001) docker     (127)     5287 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3420.418f467.js
--rw-r--r--   0 runner    (1001) docker     (127)     4032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3449.4a13bea.js
--rw-r--r--   0 runner    (1001) docker     (127)    39449 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3488.9d14a3e.js
--rw-r--r--   0 runner    (1001) docker     (127)    22236 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/35.26a4324.js
--rw-r--r--   0 runner    (1001) docker     (127)     3879 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3501.a0b897f.js
--rw-r--r--   0 runner    (1001) docker     (127)     4774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3562.77d1e3d.js
--rw-r--r--   0 runner    (1001) docker     (127)    20774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3604.9c8b7b0.js
--rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3694.3437882.js
--rw-r--r--   0 runner    (1001) docker     (127)     1837 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3700.ab2c843.js
--rw-r--r--   0 runner    (1001) docker     (127)      170 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3752.8735345.js
--rw-r--r--   0 runner    (1001) docker     (127)     6789 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3797.2bb532c.js
--rw-r--r--   0 runner    (1001) docker     (127)    15060 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/383.0385e5e.js
--rw-r--r--   0 runner    (1001) docker     (127)    31562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3864.acf045c.js
--rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/3992.5a17c7b.js
--rw-r--r--   0 runner    (1001) docker     (127)    10989 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4002.d2530f2.js
--rw-r--r--   0 runner    (1001) docker     (127)     4576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/403.ea946dc.js
--rw-r--r--   0 runner    (1001) docker     (127)     6923 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4030.8963386.js
--rw-r--r--   0 runner    (1001) docker     (127)    22224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4035.88e3670.js
--rw-r--r--   0 runner    (1001) docker     (127)     2326 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4038.bb0e593.js
--rw-r--r--   0 runner    (1001) docker     (127)     7912 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4039.2635132.js
--rw-r--r--   0 runner    (1001) docker     (127)    12480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4105.05362d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     2689 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4148.0cb7e6d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2841 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/431.f294aa7.js
--rw-r--r--   0 runner    (1001) docker     (127)    62818 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4324.992bd2c.js
--rw-r--r--   0 runner    (1001) docker     (127)   205182 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4333.fdaab90.js
--rw-r--r--   0 runner    (1001) docker     (127)     3743 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4387.f2b950d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2215 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4434.547c185.js
--rw-r--r--   0 runner    (1001) docker     (127)    65652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4478.8778446.js
--rw-r--r--   0 runner    (1001) docker     (127)     4446 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4498.fced3e4.js
--rw-r--r--   0 runner    (1001) docker     (127)    73801 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4499.7b7aa96.js
--rw-r--r--   0 runner    (1001) docker     (127)     2226 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4521.c2278f6.js
--rw-r--r--   0 runner    (1001) docker     (127)    12658 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4588.66d005c.js
--rw-r--r--   0 runner    (1001) docker     (127)   232363 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4630.32049fe.js
--rw-r--r--   0 runner    (1001) docker     (127)      366 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4630.32049fe.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2653 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4670.72adecb.js
--rw-r--r--   0 runner    (1001) docker     (127)    58986 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4780.f7ebd53.js
--rw-r--r--   0 runner    (1001) docker     (127)     2671 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4810.fdb4bef.js
--rw-r--r--   0 runner    (1001) docker     (127)     9509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4825.0f290ff.js
--rw-r--r--   0 runner    (1001) docker     (127)     3737 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4843.96ed13d.js
--rw-r--r--   0 runner    (1001) docker     (127)   189502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4926.3619db2.js
--rw-r--r--   0 runner    (1001) docker     (127)      160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4926.3619db2.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4954.ac85606.js
--rw-r--r--   0 runner    (1001) docker     (127)     1574 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4965.9c0bd12.js
--rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/4971.ba52a81.js
--rw-r--r--   0 runner    (1001) docker     (127)     1827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/500.b866efa.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5008.7707efe.js
--rw-r--r--   0 runner    (1001) docker     (127)    13539 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5013.5ff10dd.js
--rw-r--r--   0 runner    (1001) docker     (127)    27124 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5019.fe7898c.js
--rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5051.baecc00.js
--rw-r--r--   0 runner    (1001) docker     (127)     5283 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5061.d662bbf.js
--rw-r--r--   0 runner    (1001) docker     (127)    55045 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5115.c11e8fa.js
--rw-r--r--   0 runner    (1001) docker     (127)     6292 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/514.1c1b052.js
--rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5233.96f1668.js
--rw-r--r--   0 runner    (1001) docker     (127)     3708 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5249.847f856.js
--rw-r--r--   0 runner    (1001) docker     (127)    22174 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5261.2a76287.js
--rw-r--r--   0 runner    (1001) docker     (127)    17171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5276.069ed0f.js
--rw-r--r--   0 runner    (1001) docker     (127)     5308 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5299.4fe47ed.js
--rw-r--r--   0 runner    (1001) docker     (127)    25735 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5343.c65eb48.js
--rw-r--r--   0 runner    (1001) docker     (127)     3346 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5425.ff5465e.js
--rw-r--r--   0 runner    (1001) docker     (127)    17359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5464.7c73ae4.js
--rw-r--r--   0 runner    (1001) docker     (127)       55 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5464.7c73ae4.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5494.db2521b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5597.2470f52.js
--rw-r--r--   0 runner    (1001) docker     (127)     2456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/563.7fd8ced.js
--rw-r--r--   0 runner    (1001) docker     (127)     2378 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5691.16de5f4.js
--rw-r--r--   0 runner    (1001) docker     (127)     1927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5698.7febbe1.js
--rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5765.72d36d2.js
--rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5777.c1c07e5.js
--rw-r--r--   0 runner    (1001) docker     (127)     8379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5822.7e14b54.js
--rw-r--r--   0 runner    (1001) docker     (127)    25560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5828.e1ab6ce.js
--rw-r--r--   0 runner    (1001) docker     (127)     4057 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5834.ba430d2.js
--rw-r--r--   0 runner    (1001) docker     (127)    77942 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5850.9fd6e53.js
--rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5945.4a06217.js
--rw-r--r--   0 runner    (1001) docker     (127)     4724 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5972.aa32cae.js
--rw-r--r--   0 runner    (1001) docker     (127)     5952 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/5996.8503bba.js
--rw-r--r--   0 runner    (1001) docker     (127)     2227 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6139.0c4aaeb.js
--rw-r--r--   0 runner    (1001) docker     (127)   122842 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6236.5f93bea.js
--rw-r--r--   0 runner    (1001) docker     (127)       95 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6236.5f93bea.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    40991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6271.c4952fd.js
--rw-r--r--   0 runner    (1001) docker     (127)    11869 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6281.f763d40.js
--rw-r--r--   0 runner    (1001) docker     (127)     3030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/632.200fdf3.js
--rw-r--r--   0 runner    (1001) docker     (127)    10676 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6417.bebf125.js
--rw-r--r--   0 runner    (1001) docker     (127)    11489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6433.a6cfc6e.js
--rw-r--r--   0 runner    (1001) docker     (127)    77133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/644.0a629ee.js
--rw-r--r--   0 runner    (1001) docker     (127)      212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/644.0a629ee.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/647.8cecbd3.js
--rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6473.a97af61.js
--rw-r--r--   0 runner    (1001) docker     (127)     5819 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/653.7dd3d36.js
--rw-r--r--   0 runner    (1001) docker     (127)     9121 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6553.a73f98d.js
--rw-r--r--   0 runner    (1001) docker     (127)   243122 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6607.4ee069b.js
--rw-r--r--   0 runner    (1001) docker     (127)    16747 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/661.477cacc.js
--rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6640.bf24711.js
--rw-r--r--   0 runner    (1001) docker     (127)    13477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6667.60cb1d2.js
--rw-r--r--   0 runner    (1001) docker     (127)     7469 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/67.3672096.js
--rw-r--r--   0 runner    (1001) docker     (127)    25966 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6739.d19f4c2.js
--rw-r--r--   0 runner    (1001) docker     (127)     3497 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/677.493cb60.js
--rw-r--r--   0 runner    (1001) docker     (127)     2967 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6788.4fb5bb9.js
--rw-r--r--   0 runner    (1001) docker     (127)     1318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/69.fc53c91.js
--rw-r--r--   0 runner    (1001) docker     (127)     8125 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6941.7241556.js
--rw-r--r--   0 runner    (1001) docker     (127)     4275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6942.bcc3a2f.js
--rw-r--r--   0 runner    (1001) docker     (127)    71168 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/6972.930242c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7005.de1d9f9.js
--rw-r--r--   0 runner    (1001) docker     (127)    37281 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7010.979a827.js
--rw-r--r--   0 runner    (1001) docker     (127)     5011 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7022.6d0ffc3.js
--rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7036.d0dae7d.js
--rw-r--r--   0 runner    (1001) docker     (127)     2980 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7054.de34848.js
--rw-r--r--   0 runner    (1001) docker     (127)     1828 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7061.30f7cf6.js
--rw-r--r--   0 runner    (1001) docker     (127)    24171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7097.d4214d0.js
--rw-r--r--   0 runner    (1001) docker     (127)     2649 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7125.4a0562f.js
--rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7153.135087f.js
--rw-r--r--   0 runner    (1001) docker     (127)    79078 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7154.804d332.js
--rw-r--r--   0 runner    (1001) docker     (127)     2725 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7170.7bba13a.js
--rw-r--r--   0 runner    (1001) docker     (127)     9092 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7179.af46233.js
--rw-r--r--   0 runner    (1001) docker     (127)    50998 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7259.6d595ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     1971 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7264.0ec5936.js
--rw-r--r--   0 runner    (1001) docker     (127)     4269 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7360.7b1e065.js
--rw-r--r--   0 runner    (1001) docker     (127)   210697 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7369.a12e276.js
--rw-r--r--   0 runner    (1001) docker     (127)     6663 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7378.b4f5497.js
--rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7378.b4f5497.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    68002 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7427.368a8bc.js
--rw-r--r--   0 runner    (1001) docker     (127)     1807 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/745.83ff9e4.js
--rw-r--r--   0 runner    (1001) docker     (127)    26652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7450.d5ee0a9.js
--rw-r--r--   0 runner    (1001) docker     (127)    38991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7471.30d9d48.js
--rw-r--r--   0 runner    (1001) docker     (127)    28319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7495.3c478a0.js
--rw-r--r--   0 runner    (1001) docker     (127)     4149 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7534.a755d75.js
--rw-r--r--   0 runner    (1001) docker     (127)    13033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/755.6424780.js
--rw-r--r--   0 runner    (1001) docker     (127)    18136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7557.bd5cd49.js
--rw-r--r--   0 runner    (1001) docker     (127)    15293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7582.7350cc5.js
--rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7634.7befbe5.js
--rw-r--r--   0 runner    (1001) docker     (127)   101829 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7674.93d7410.js
--rw-r--r--   0 runner    (1001) docker     (127)      849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7803.45d27da.js
--rw-r--r--   0 runner    (1001) docker     (127)    11315 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7811.bd10193.js
--rw-r--r--   0 runner    (1001) docker     (127)      249 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7811.bd10193.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2730 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7817.6a39acf.js
--rw-r--r--   0 runner    (1001) docker     (127)    28662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7866.e7f89f6.js
--rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7892.c46785d.js
--rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7918.506a625.js
--rw-r--r--   0 runner    (1001) docker     (127)    14437 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/792.f22b43b.js
--rw-r--r--   0 runner    (1001) docker     (127)    60194 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7969.f8f9146.js
--rw-r--r--   0 runner    (1001) docker     (127)    62260 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7995.e40b57d.js
--rw-r--r--   0 runner    (1001) docker     (127)      240 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7995.e40b57d.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    26076 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/7997.46ee9b7.js
--rw-r--r--   0 runner    (1001) docker     (127)    95179 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8010.dbb2b65.js
--rw-r--r--   0 runner    (1001) docker     (127)    12379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8103.25c6881.js
--rw-r--r--   0 runner    (1001) docker     (127)    14035 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8178.6647b58.js
--rw-r--r--   0 runner    (1001) docker     (127)    15318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8285.46eba3a.js
--rw-r--r--   0 runner    (1001) docker     (127)     7917 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8378.d951634.js
--rw-r--r--   0 runner    (1001) docker     (127)     2679 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8381.4b39fc5.js
--rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8387.c2a5ccb.js
--rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8427.379d337.js
--rw-r--r--   0 runner    (1001) docker     (127)     1150 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8433.c26711e.js
--rw-r--r--   0 runner    (1001) docker     (127)    31538 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8443.32841be.js
--rw-r--r--   0 runner    (1001) docker     (127)     2520 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8446.d952b7d.js
--rw-r--r--   0 runner    (1001) docker     (127)    37231 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8479.7ad07d9.js
--rw-r--r--   0 runner    (1001) docker     (127)     1001 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/85.eb26499.js
--rw-r--r--   0 runner    (1001) docker     (127)    31624 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/850.16f7c82.js
--rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8579.7c15dcd.js
--rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8701.9ba3e4c.js
--rw-r--r--   0 runner    (1001) docker     (127)    37514 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8734.0965980.js
--rw-r--r--   0 runner    (1001) docker     (127)     8576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8768.cd685a6.js
--rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8800.5b7449b.js
--rw-r--r--   0 runner    (1001) docker     (127)    17638 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8801.7946caf.js
--rw-r--r--   0 runner    (1001) docker     (127)     8107 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/883.7552b75.js
--rw-r--r--   0 runner    (1001) docker     (127)   197120 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8845.3412b3f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1144 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)    12870 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8927.b773418.js
--rw-r--r--   0 runner    (1001) docker     (127)   122785 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8929.0b66a95.js
--rw-r--r--   0 runner    (1001) docker     (127)     6103 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8937.6c8605f.js
--rw-r--r--   0 runner    (1001) docker     (127)     6360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8979.2760112.js
--rw-r--r--   0 runner    (1001) docker     (127)      949 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/8983.5db65ea.js
--rw-r--r--   0 runner    (1001) docker     (127)     6530 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/899.dd8da16.js
--rw-r--r--   0 runner    (1001) docker     (127)     2941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9022.85c8176.js
--rw-r--r--   0 runner    (1001) docker     (127)     4058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9037.6397c79.js
--rw-r--r--   0 runner    (1001) docker     (127)    10341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/906.f6a46ca.js
--rw-r--r--   0 runner    (1001) docker     (127)     1032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9060.9fe49c6.js
--rw-r--r--   0 runner    (1001) docker     (127)     8533 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9073.fadf4d8.js
--rw-r--r--   0 runner    (1001) docker     (127)      492 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9116.656701b.js
--rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9166.d072a52.js
--rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9208.10ca99e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1731 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9233.b14ca62.js
--rw-r--r--   0 runner    (1001) docker     (127)     2184 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9234.488a70b.js
--rw-r--r--   0 runner    (1001) docker     (127)    22474 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9239.13871ef.js
--rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9244.a95e8aa.js
--rw-r--r--   0 runner    (1001) docker     (127)    11877 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9250.43c7d24.js
--rw-r--r--   0 runner    (1001) docker     (127)    29186 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/927.399dde7.js
--rw-r--r--   0 runner    (1001) docker     (127)      163 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/927.399dde7.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9282.eb25fa6.js
--rw-r--r--   0 runner    (1001) docker     (127)     4219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9331.415f707.js
--rw-r--r--   0 runner    (1001) docker     (127)    24754 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9334.9101b2f.js
--rw-r--r--   0 runner    (1001) docker     (127)     1342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9372.65a2507.js
--rw-r--r--   0 runner    (1001) docker     (127)    22275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9425.d103ed5.js
--rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9531.5517c40.js
--rw-r--r--   0 runner    (1001) docker     (127)     2795 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9558.09c3851.js
--rw-r--r--   0 runner    (1001) docker     (127)    13560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9565.66944bd.js
--rw-r--r--   0 runner    (1001) docker     (127)    12802 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9597.9d6c989.js
--rw-r--r--   0 runner    (1001) docker     (127)     2123 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9604.c2c5590.js
--rw-r--r--   0 runner    (1001) docker     (127)    82415 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9643.4b4e30e.js
--rw-r--r--   0 runner    (1001) docker     (127)     1562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9676.f7b737a.js
--rw-r--r--   0 runner    (1001) docker     (127)    41456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9799.ecf3e29.js
--rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9847.20223dd.js
--rw-r--r--   0 runner    (1001) docker     (127)    35515 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9866.ea3fe7f.js
--rw-r--r--   0 runner    (1001) docker     (127)    36793 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9879.951cc05.js
--rw-r--r--   0 runner    (1001) docker     (127)   246342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/9903.633a36a.js
--rw-r--r--   0 runner    (1001) docker     (127)    40808 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9908 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)     9600 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    22340 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    21480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    34464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Main-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    20832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Main-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    34160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Main-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19776 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    19360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Math-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    15944 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)    14628 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff
--rw-r--r--   0 runner    (1001) docker     (127)    12660 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    11852 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Script-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5792 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     5148 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    17604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1116 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Zero.woff
--rw-r--r--   0 runner    (1001) docker     (127)   134294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   747927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)   133988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    89988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    76736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    34034 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.eot
--rw-r--r--   0 runner    (1001) docker     (127)   144714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.svg
--rw-r--r--   0 runner    (1001) docker     (127)    33736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    16276 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.woff
--rw-r--r--   0 runner    (1001) docker     (127)    13224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.woff2
--rw-r--r--   0 runner    (1001) docker     (127)   203030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.eot
--rw-r--r--   0 runner    (1001) docker     (127)   918991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.svg
--rw-r--r--   0 runner    (1001) docker     (127)   202744 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   101648 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.woff
--rw-r--r--   0 runner    (1001) docker     (127)    78268 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.woff2
--rw-r--r--   0 runner    (1001) docker     (127)  2437261 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/jlab_core.b96c356.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.325278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/lab/
--rw-r--r--   0 runner    (1001) docker     (127)    63254 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/lab/bundle.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.325278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.245278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1805 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json
--rw-r--r--   0 runner    (1001) docker     (127)      473 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/pages.json
--rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (127)      223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/title.json
--rw-r--r--   0 runner    (1001) docker     (127)      832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json
--rw-r--r--   0 runner    (1001) docker     (127)      386 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/zen.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      472 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/open.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      256 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
--rw-r--r--   0 runner    (1001) docker     (127)      560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
--rw-r--r--   0 runner    (1001) docker     (127)      517 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      557 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json
--rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     8478 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
--rw-r--r--   0 runner    (1001) docker     (127)     3219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
--rw-r--r--   0 runner    (1001) docker     (127)      543 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json
--rw-r--r--   0 runner    (1001) docker     (127)     3036 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
--rw-r--r--   0 runner    (1001) docker     (127)     2151 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json
--rw-r--r--   0 runner    (1001) docker     (127)      936 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
--rw-r--r--   0 runner    (1001) docker     (127)      563 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
--rw-r--r--   0 runner    (1001) docker     (127)      677 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json
--rw-r--r--   0 runner    (1001) docker     (127)     4575 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
--rw-r--r--   0 runner    (1001) docker     (127)      694 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json
--rw-r--r--   0 runner    (1001) docker     (127)      457 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      444 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.329278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json
--rw-r--r--   0 runner    (1001) docker     (127)     1445 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      343 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/completer.json
--rw-r--r--   0 runner    (1001) docker     (127)      365 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
--rw-r--r--   0 runner    (1001) docker     (127)     3674 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
--rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (127)     3935 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2233 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     6714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
--rw-r--r--   0 runner    (1001) docker     (127)      513 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
--rw-r--r--   0 runner    (1001) docker     (127)      385 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
--rw-r--r--   0 runner    (1001) docker     (127)      477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
--rw-r--r--   0 runner    (1001) docker     (127)     3147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      336 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/completer.json
--rw-r--r--   0 runner    (1001) docker     (127)     6617 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      422 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
--rw-r--r--   0 runner    (1001) docker     (127)      456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
--rw-r--r--   0 runner    (1001) docker     (127)      364 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      332 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (127)      782 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
--rw-r--r--   0 runner    (1001) docker     (127)      319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1102 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
--rw-r--r--   0 runner    (1001) docker     (127)    10058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.333278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2325 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      756 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      348 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/completer.json
--rw-r--r--   0 runner    (1001) docker     (127)      672 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
--rw-r--r--   0 runner    (1001) docker     (127)     3267 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
--rw-r--r--   0 runner    (1001) docker     (127)     3605 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json
--rw-r--r--   0 runner    (1001) docker     (127)    24926 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1487 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      389 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
--rw-r--r--   0 runner    (1001) docker     (127)      440 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1152 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      848 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     2050 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      551 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
--rw-r--r--   0 runner    (1001) docker     (127)      402 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
--rw-r--r--   0 runner    (1001) docker     (127)      572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
--rw-r--r--   0 runner    (1001) docker     (127)     1394 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/
--rw-r--r--   0 runner    (1001) docker     (127)      359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/share-file.json
--rw-r--r--   0 runner    (1001) docker     (127)   105099 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/all.json
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-12 12:17:08.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/all_federated.json
--rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
--rw-r--r--   0 runner    (1001) docker     (127)    17882 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
--rw-r--r--   0 runner    (1001) docker     (127)    16550 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
--rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
--rw-r--r--   0 runner    (1001) docker     (127)   415751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/build/third-party-licenses.json
--rw-r--r--   0 runner    (1001) docker     (127)     7193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/config-utils.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/doc/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/doc/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/doc/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/doc/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)      295 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/doc/workspaces/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.337278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
--rw-rw-rw-   0 runner    (1001) docker     (127)      219 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/install.json
--rw-rw-rw-   0 runner    (1001) docker     (127)     2343 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.341278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
--rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js
--rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)    14992 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js
--rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)    16598 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png
--rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js
--rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)      598 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     4254 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png
--rw-rw-rw-   0 runner    (1001) docker     (127)     7359 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (127)    13107 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.341278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/
--rw-rw-rw-   0 runner    (1001) docker     (127)     2732 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.345278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/
--rw-rw-rw-   0 runner    (1001) docker     (127)     2643 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     8311 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js
--rw-rw-rw-   0 runner    (1001) docker     (127)  3598363 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     1110 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)    70520 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      336 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
--rw-rw-rw-   0 runner    (1001) docker     (127)     2360 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js
--rw-rw-rw-   0 runner    (1001) docker     (127)    14766 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     7706 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     5802 2024-04-12 12:16:55.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.345278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/
--rw-rw-rw-   0 runner    (1001) docker     (127)      199 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/install.json
--rw-rw-rw-   0 runner    (1001) docker     (127)     5919 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.349278 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/
--rw-rw-rw-   0 runner    (1001) docker     (127)      224 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     8351 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     3925 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js
--rw-rw-rw-   0 runner    (1001) docker     (127)      162 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
--rw-rw-rw-   0 runner    (1001) docker     (127)     2452 2024-04-12 12:17:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.349278 fixinventorycore-4.0.2/fixcore/jupyterlite/files/
--rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/files/example.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     4609 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/icon-120x120.png
--rw-r--r--   0 runner    (1001) docker     (127)    20954 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/icon-512x512.png
--rw-r--r--   0 runner    (1001) docker     (127)     2516 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-12 12:17:08.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (127)    11526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/jupyterlite.schema.v0.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.349278 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/
--rw-r--r--   0 runner    (1001) docker     (127)   324251 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/jupyter-lite.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      166 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/jupyter-lite.json
--rw-r--r--   0 runner    (1001) docker     (127)    12425 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.349278 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/tree/
--rw-r--r--   0 runner    (1001) docker     (127)      290 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/tree/index.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.349278 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)      288 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/lab/workspaces/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      690 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/manifest.webmanifest
--rw-r--r--   0 runner    (1001) docker     (127)     1088 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/package.json
--rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/service-worker.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.249278 fixinventorycore-4.0.2/fixcore/jupyterlite/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.349278 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-12 12:17:03.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-12 12:17:03.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-12 12:17:03.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-12 12:17:03.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-file.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-12 12:17:03.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-notebook.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-12 12:17:03.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-terminal.ico
--rw-rw-rw-   0 runner    (1001) docker     (127)    32038 2024-04-12 12:17:03.000000 fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/message_bus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.353278 fixinventorycore-4.0.2/fixcore/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/adjust_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/db_updater.py
--rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/exportable_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    30006 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/graph_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/json_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)    69697 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/model_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/resolve_in_graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/transform_kind_convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/model/typed_model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.353278 fixinventorycore-4.0.2/fixcore/query/
--rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51739 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/query/model.py
--rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/query/query_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/query/template_expander.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/query/template_expander_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.353278 fixinventorycore-4.0.2/fixcore/report/
--rw-r--r--   0 runner    (1001) docker     (127)    18529 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6266 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/report/benchmark_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)    25655 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/report/inspector_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/report/report_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.353278 fixinventorycore-4.0.2/fixcore/static/
--rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/static/api-doc.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/static/ck-unicode-truecolor.ans
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/static/fix.css
--rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/static/fixinventory_logo_and_text.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/system_start.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.357278 fixinventorycore-4.0.2/fixcore/task/
--rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/job_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/start_workflow_on_first_subscriber.py
--rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/subscribers.py
--rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/task_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)    33482 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/task_description.py
--rw-r--r--   0 runner    (1001) docker     (127)    30250 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/task/task_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.357278 fixinventorycore-4.0.2/fixcore/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/templates/create_first_user.html
--rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/templates/home.html
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/templates/login.html
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.357278 fixinventorycore-4.0.2/fixcore/user/
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/user/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/user/user_management.py
--rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.357278 fixinventorycore-4.0.2/fixcore/web/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/accesslog.py
--rw-r--r--   0 runner    (1001) docker     (127)    80702 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/certificate_handler.py
--rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/content_renderer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/directives.py
--rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/web/tsdb.py
--rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/fixcore/worker_task_queue.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.369278 fixinventorycore-4.0.2/fixinventorycore.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-12 12:17:10.000000 fixinventorycore-4.0.2/fixinventorycore.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    30702 2024-04-12 12:17:10.000000 fixinventorycore-4.0.2/fixinventorycore.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:17:10.000000 fixinventorycore-4.0.2/fixinventorycore.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-12 12:17:10.000000 fixinventorycore-4.0.2/fixinventorycore.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:17:09.000000 fixinventorycore-4.0.2/fixinventorycore.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-12 12:17:10.000000 fixinventorycore-4.0.2/fixinventorycore.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-12 12:17:10.000000 fixinventorycore-4.0.2/fixinventorycore.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-12 12:17:10.373278 fixinventorycore-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.357278 fixinventorycore-4.0.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.361278 fixinventorycore-4.0.2/tests/fixcore/
--rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.361278 fixinventorycore-4.0.2/tests/fixcore/analytics/
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/analytics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/analytics/posthog_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/analytics/recurrent_events_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.361278 fixinventorycore-4.0.2/tests/fixcore/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13675 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/cli/cli_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    65736 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/cli/command_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/cli/model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.361278 fixinventorycore-4.0.2/tests/fixcore/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/config/config_handler_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/config/config_override_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/config/core_config_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    31104 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/console_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/core_config_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.365278 fixinventorycore-4.0.2/tests/fixcore/db/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    19137 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/arango_query_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/arangodb_functions_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/async_arangodb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/configdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/db_access_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/deferredouteredgedb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/entitydb.py
--rw-r--r--   0 runner    (1001) docker     (127)    42015 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/graphdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/jobdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/modeldb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/reportdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/runningtaskdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/system_data_db_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/templatedb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     7627 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/db/timeseriesdb_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/dependencies_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.365278 fixinventorycore-4.0.2/tests/fixcore/graph_manager/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/graph_manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/graph_manager/graph_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/hypothesis_extension.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.365278 fixinventorycore-4.0.2/tests/fixcore/infra_apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/infra_apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/infra_apps/local_runtime_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/infra_apps/package_manager_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/message_bus_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.365278 fixinventorycore-4.0.2/tests/fixcore/model/
--rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/adjust_node_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/db_updater_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/exportable_model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/graph_access_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/json_schema_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/model_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    28515 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/resolve_in_graph_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/model/typed_model_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.369278 fixinventorycore-4.0.2/tests/fixcore/query/
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/query/model_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/query/query_parser_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/query/template_expander_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.369278 fixinventorycore-4.0.2/tests/fixcore/report/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/report/benchmark_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     9259 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/report/inspector_service_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.369278 fixinventorycore-4.0.2/tests/fixcore/task/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/task/job_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/task/start_workflow_on_first_subscriber_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/task/subscribers_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/task/task_description_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/task/task_handler_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.369278 fixinventorycore-4.0.2/tests/fixcore/user/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/user/user_management_service_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/util_test.py
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/validator_test.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:10.369278 fixinventorycore-4.0.2/tests/fixcore/web/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/web/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    24373 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/web/api_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/web/auth_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/web/certificate_handler_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/web/content_renderer_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/web/permission_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-12 12:13:44.000000 fixinventorycore-4.0.2/tests/fixcore/worker_task_queue_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.449605 fixinventorycore-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-24 10:33:00.449605 fixinventorycore-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3841 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.317603 fixinventorycore-4.0.3/fixcore/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.317603 fixinventorycore-4.0.3/fixcore/action_handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/action_handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5467 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/action_handlers/merge_outer_edge_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.317603 fixinventorycore-4.0.3/fixcore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/analytics/posthog.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1917 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/analytics/recurrent_events.py
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/async_extensions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.321603 fixinventorycore-4.0.3/fixcore/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31738 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/cli/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)   276866 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/cli/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29181 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/cli/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7391 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/cli/tip_of_the_day.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/compat.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.321603 fixinventorycore-4.0.3/fixcore/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     6218 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13420 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/config/config_handler_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7293 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/config/config_override_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12670 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/config/core_config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4197 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/console_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35525 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/core_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.325603 fixinventorycore-4.0.3/fixcore/db/
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46365 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/arango_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/arangodb_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2499 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/arangodb_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21571 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/async_arangodb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      896 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/configdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31907 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/db_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/deferredouteredgedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5787 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87214 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/graphdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/jobdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/modeldb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/packagedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      685 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/reportdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11718 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/runningtaskdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3069 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/system_data_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/templatedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13753 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/timeseriesdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/db/usagedb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19730 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2831 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.325603 fixinventorycore-4.0.3/fixcore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4475 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/graph_manager/graph_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/ids.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.325603 fixinventorycore-4.0.3/fixcore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4698 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/infra_apps/local_runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2351 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/infra_apps/manifest.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13696 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/infra_apps/package_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/infra_apps/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.329603 fixinventorycore-4.0.3/fixcore/jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.305603 fixinventorycore-4.0.3/fixcore/jupyterlite/api/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.329603 fixinventorycore-4.0.3/fixcore/jupyterlite/api/contents/
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-24 10:32:58.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/api/contents/all.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.329603 fixinventorycore-4.0.3/fixcore/jupyterlite/api/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 10:32:58.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/api/translations/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 10:32:58.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/api/translations/en.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/bootstrap.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.397604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/
+-rw-r--r--   0 runner    (1001) docker     (127)    40339 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1053.7a56130.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4145 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1088.33c6076.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1091.1cf35e6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5021 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1122.d86c258.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/114.1c04540.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1169.4cf2d13.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/125.4c6ac03.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45561 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1261.3da9a56.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/131.5b6a7ab.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1385.707019c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9183 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1388.0f22ef8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2081 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1418.d9431d8.js
+-rw-r--r--   0 runner    (1001) docker     (127)   412668 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/142.6e89fb8.js
+-rw-r--r--   0 runner    (1001) docker     (127)   457855 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1495.671bdd4.js
+-rw-r--r--   0 runner    (1001) docker     (127)      493 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1495.671bdd4.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   133253 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1542.22098a5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      483 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1542.22098a5.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1558.548303d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35637 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1584.d919fce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4181 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1618.983fc32.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18800 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1715.ebbb93b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1769.10c2b5d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1815.2af66e5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1837.622ebbe.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1846.ed084ce.js
+-rw-r--r--   0 runner    (1001) docker     (127)      612 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1869.86f5778.js
+-rw-r--r--   0 runner    (1001) docker     (127)    74760 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1871.7fed383.js
+-rw-r--r--   0 runner    (1001) docker     (127)      945 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/1941.79180b2.js
+-rw-r--r--   0 runner    (1001) docker     (127)   119985 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2065.410c3bc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20937 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/214.300dbf1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3072 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2188.9676797.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/221.59c0059.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16250 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2213.b58cab4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    82064 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2241.91c6cce.js
+-rw-r--r--   0 runner    (1001) docker     (127)    47604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2323.7e4d795.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1481212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2324.aff3939.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4331 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2343.3cf0fe8.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2349.9acb0b1.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2129 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2363.6aa6a7f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2386.5f8e2da.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2520.5c65366.js
+-rw-r--r--   0 runner    (1001) docker     (127)    54845 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2552.6c5224e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37964 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/261.431b309.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2784 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2622.3d61d64.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12742 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2666.6cce729.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2682.0c612a1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    30032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2692.f2b8d53.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7589 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/270.9675bfe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      745 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2702.0e1a6ff.js
+-rw-r--r--   0 runner    (1001) docker     (127)    55572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/28.9f8dd00.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2871.e1a64a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)   128665 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2913.25c5e72.js
+-rw-r--r--   0 runner    (1001) docker     (127)      559 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   256757 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2930.896decd.js
+-rw-r--r--   0 runner    (1001) docker     (127)   169282 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/2955.c8d0773.js
+-rw-r--r--   0 runner    (1001) docker     (127)    74307 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/306.b568c30.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35812 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3079.18e3c32.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/311.76f79fc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3111.8de2d0a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4545 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3154.5d8f80d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4274 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3211.aa42b4a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5817 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3218.758a794.js
+-rw-r--r--   0 runner    (1001) docker     (127)       99 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3218.758a794.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3230.2c849ff.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3245.c48f805.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3322.428e385.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2505 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3336.3d4780f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3370.b5d78cd.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5287 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3420.418f467.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3449.4a13bea.js
+-rw-r--r--   0 runner    (1001) docker     (127)    39449 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3488.9d14a3e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22236 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/35.26a4324.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3501.a0b897f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3562.77d1e3d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    20774 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3604.9c8b7b0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3694.3437882.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3700.ab2c843.js
+-rw-r--r--   0 runner    (1001) docker     (127)      170 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3752.8735345.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6789 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3797.2bb532c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15060 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/383.0385e5e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3864.acf045c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/3992.5a17c7b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4002.d2530f2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/403.ea946dc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6923 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4030.8963386.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4035.88e3670.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2326 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4038.bb0e593.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7912 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4039.2635132.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4105.05362d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4148.0cb7e6d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2841 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/431.f294aa7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62818 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4324.992bd2c.js
+-rw-r--r--   0 runner    (1001) docker     (127)   205182 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4333.fdaab90.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3743 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4387.f2b950d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4434.547c185.js
+-rw-r--r--   0 runner    (1001) docker     (127)    65652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4478.8778446.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4446 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4498.fced3e4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    73801 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4499.7b7aa96.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4521.c2278f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12658 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4588.66d005c.js
+-rw-r--r--   0 runner    (1001) docker     (127)   232363 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4630.32049fe.js
+-rw-r--r--   0 runner    (1001) docker     (127)      366 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4630.32049fe.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2653 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4670.72adecb.js
+-rw-r--r--   0 runner    (1001) docker     (127)    58986 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4780.f7ebd53.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4810.fdb4bef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9509 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4825.0f290ff.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3737 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4843.96ed13d.js
+-rw-r--r--   0 runner    (1001) docker     (127)   189502 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4926.3619db2.js
+-rw-r--r--   0 runner    (1001) docker     (127)      160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4926.3619db2.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     4128 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4954.ac85606.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1574 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4965.9c0bd12.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/4971.ba52a81.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/500.b866efa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5008.7707efe.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5013.5ff10dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    27124 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5019.fe7898c.js
+-rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5051.baecc00.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5283 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5061.d662bbf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    55045 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5115.c11e8fa.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6292 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/514.1c1b052.js
+-rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5233.96f1668.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3708 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5249.847f856.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22174 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5261.2a76287.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5276.069ed0f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5308 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5299.4fe47ed.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25735 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5343.c65eb48.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3346 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5425.ff5465e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5464.7c73ae4.js
+-rw-r--r--   0 runner    (1001) docker     (127)       55 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5464.7c73ae4.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5494.db2521b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5597.2470f52.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/563.7fd8ced.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2378 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5691.16de5f4.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5698.7febbe1.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5765.72d36d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16498 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5777.c1c07e5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5822.7e14b54.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5828.e1ab6ce.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5834.ba430d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77942 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5850.9fd6e53.js
+-rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5945.4a06217.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5972.aa32cae.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5952 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/5996.8503bba.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6139.0c4aaeb.js
+-rw-r--r--   0 runner    (1001) docker     (127)   122842 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6236.5f93bea.js
+-rw-r--r--   0 runner    (1001) docker     (127)       95 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6236.5f93bea.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    40991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6271.c4952fd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11869 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6281.f763d40.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/632.200fdf3.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10676 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6417.bebf125.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6433.a6cfc6e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    77133 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/644.0a629ee.js
+-rw-r--r--   0 runner    (1001) docker     (127)      212 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/644.0a629ee.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/647.8cecbd3.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6473.a97af61.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5819 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/653.7dd3d36.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9121 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6553.a73f98d.js
+-rw-r--r--   0 runner    (1001) docker     (127)   243122 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6607.4ee069b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    16747 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/661.477cacc.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6640.bf24711.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6667.60cb1d2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7469 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/67.3672096.js
+-rw-r--r--   0 runner    (1001) docker     (127)    25966 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6739.d19f4c2.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3497 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/677.493cb60.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2967 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6788.4fb5bb9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/69.fc53c91.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8125 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6941.7241556.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6942.bcc3a2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    71168 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/6972.930242c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7005.de1d9f9.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37281 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7010.979a827.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5011 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7022.6d0ffc3.js
+-rw-r--r--   0 runner    (1001) docker     (127)      488 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7036.d0dae7d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7054.de34848.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7061.30f7cf6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24171 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7097.d4214d0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7125.4a0562f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10601 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7153.135087f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    79078 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7154.804d332.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7170.7bba13a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9092 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7179.af46233.js
+-rw-r--r--   0 runner    (1001) docker     (127)    50998 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7259.6d595ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7264.0ec5936.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4269 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7360.7b1e065.js
+-rw-r--r--   0 runner    (1001) docker     (127)   210697 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7369.a12e276.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6663 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7378.b4f5497.js
+-rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7378.b4f5497.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    68002 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7427.368a8bc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1807 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/745.83ff9e4.js
+-rw-r--r--   0 runner    (1001) docker     (127)    26652 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7450.d5ee0a9.js
+-rw-r--r--   0 runner    (1001) docker     (127)    38991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7471.30d9d48.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7495.3c478a0.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7534.a755d75.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/755.6424780.js
+-rw-r--r--   0 runner    (1001) docker     (127)    18136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7557.bd5cd49.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7582.7350cc5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7634.7befbe5.js
+-rw-r--r--   0 runner    (1001) docker     (127)   101829 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7674.93d7410.js
+-rw-r--r--   0 runner    (1001) docker     (127)      849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7803.45d27da.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11315 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7811.bd10193.js
+-rw-r--r--   0 runner    (1001) docker     (127)      249 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7811.bd10193.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7817.6a39acf.js
+-rw-r--r--   0 runner    (1001) docker     (127)    28662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7866.e7f89f6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7892.c46785d.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7918.506a625.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14437 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/792.f22b43b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    60194 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7969.f8f9146.js
+-rw-r--r--   0 runner    (1001) docker     (127)    62260 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7995.e40b57d.js
+-rw-r--r--   0 runner    (1001) docker     (127)      240 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7995.e40b57d.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    26076 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/7997.46ee9b7.js
+-rw-r--r--   0 runner    (1001) docker     (127)    95179 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8010.dbb2b65.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8103.25c6881.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14035 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8178.6647b58.js
+-rw-r--r--   0 runner    (1001) docker     (127)    15318 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8285.46eba3a.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7917 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8378.d951634.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2679 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8381.4b39fc5.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8387.c2a5ccb.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8427.379d337.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8433.c26711e.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31538 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8443.32841be.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8446.d952b7d.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37231 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8479.7ad07d9.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/85.eb26499.js
+-rw-r--r--   0 runner    (1001) docker     (127)    31624 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/850.16f7c82.js
+-rw-r--r--   0 runner    (1001) docker     (127)     7383 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8579.7c15dcd.js
+-rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8701.9ba3e4c.js
+-rw-r--r--   0 runner    (1001) docker     (127)    37514 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8734.0965980.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8576 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8768.cd685a6.js
+-rw-r--r--   0 runner    (1001) docker     (127)      857 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8800.5b7449b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    17638 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8801.7946caf.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8107 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/883.7552b75.js
+-rw-r--r--   0 runner    (1001) docker     (127)   197120 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8845.3412b3f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    12870 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8927.b773418.js
+-rw-r--r--   0 runner    (1001) docker     (127)   122785 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8929.0b66a95.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8937.6c8605f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8979.2760112.js
+-rw-r--r--   0 runner    (1001) docker     (127)      949 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/8983.5db65ea.js
+-rw-r--r--   0 runner    (1001) docker     (127)     6530 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/899.dd8da16.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9022.85c8176.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9037.6397c79.js
+-rw-r--r--   0 runner    (1001) docker     (127)    10341 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/906.f6a46ca.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1032 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9060.9fe49c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8533 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9073.fadf4d8.js
+-rw-r--r--   0 runner    (1001) docker     (127)      492 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9116.656701b.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9166.d072a52.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9208.10ca99e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9233.b14ca62.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2184 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9234.488a70b.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22474 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9239.13871ef.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9244.a95e8aa.js
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9250.43c7d24.js
+-rw-r--r--   0 runner    (1001) docker     (127)    29186 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/927.399dde7.js
+-rw-r--r--   0 runner    (1001) docker     (127)      163 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/927.399dde7.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9282.eb25fa6.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9331.415f707.js
+-rw-r--r--   0 runner    (1001) docker     (127)    24754 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9334.9101b2f.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9372.65a2507.js
+-rw-r--r--   0 runner    (1001) docker     (127)    22275 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9425.d103ed5.js
+-rw-r--r--   0 runner    (1001) docker     (127)      232 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9531.5517c40.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9558.09c3851.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9565.66944bd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    12802 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9597.9d6c989.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9604.c2c5590.js
+-rw-r--r--   0 runner    (1001) docker     (127)    82415 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9643.4b4e30e.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1562 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9676.f7b737a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    41456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9799.ecf3e29.js
+-rw-r--r--   0 runner    (1001) docker     (127)     8960 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9847.20223dd.js
+-rw-r--r--   0 runner    (1001) docker     (127)    35515 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9866.ea3fe7f.js
+-rw-r--r--   0 runner    (1001) docker     (127)    36793 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9879.951cc05.js
+-rw-r--r--   0 runner    (1001) docker     (127)   246342 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/9903.633a36a.js
+-rw-r--r--   0 runner    (1001) docker     (127)    40808 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9908 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     9600 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    22340 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    21480 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    34464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Main-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    20832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Main-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    34160 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Main-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19776 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    19360 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Math-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    15944 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    14628 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    12660 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    11852 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Script-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5792 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5464 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     3244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     5148 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    17604 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1116 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Zero.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   134294 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   747927 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   133988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    89988 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    76736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    34034 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   144714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    33736 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    16276 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    13224 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)   203030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   918991 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   202744 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   101648 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    78268 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)  2437261 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/jlab_core.b96c356.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.397604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)    63254 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/lab/bundle.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.397604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.305603 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.397604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json
+-rw-r--r--   0 runner    (1001) docker     (127)      473 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/pages.json
+-rw-r--r--   0 runner    (1001) docker     (127)      864 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (127)      223 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/title.json
+-rw-r--r--   0 runner    (1001) docker     (127)      832 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json
+-rw-r--r--   0 runner    (1001) docker     (127)      386 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/zen.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.397604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      472 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/help-extension/open.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.397604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      256 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/checkpoints.json
+-rw-r--r--   0 runner    (1001) docker     (127)      560 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)      237 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/kernel-logo.json
+-rw-r--r--   0 runner    (1001) docker     (127)      517 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.397604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      557 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     8478 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3219 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json
+-rw-r--r--   0 runner    (1001) docker     (127)      543 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1379 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json
+-rw-r--r--   0 runner    (1001) docker     (127)      936 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json
+-rw-r--r--   0 runner    (1001) docker     (127)      563 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json
+-rw-r--r--   0 runner    (1001) docker     (127)      677 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json
+-rw-r--r--   0 runner    (1001) docker     (127)      694 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json
+-rw-r--r--   0 runner    (1001) docker     (127)      457 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/workspaces.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      444 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/codemirror-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1849 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      365 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/foreign.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3674 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.401604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3935 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2233 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     6714 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json
+-rw-r--r--   0 runner    (1001) docker     (127)      513 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json
+-rw-r--r--   0 runner    (1001) docker     (127)      385 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-browser-tab.json
+-rw-r--r--   0 runner    (1001) docker     (127)      477 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/open-with.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3147 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      336 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6617 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      422 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/about.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/jupyter-forum.json
+-rw-r--r--   0 runner    (1001) docker     (127)      364 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/help-extension/launch-classic.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      332 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (127)      782 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json
+-rw-r--r--   0 runner    (1001) docker     (127)      319 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      662 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2293 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    10058 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2325 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      756 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.405604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2387 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/completer.json
+-rw-r--r--   0 runner    (1001) docker     (127)      672 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3267 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3605 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json
+-rw-r--r--   0 runner    (1001) docker     (127)    24926 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      389 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/form-ui.json
+-rw-r--r--   0 runner    (1001) docker     (127)      440 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/settingeditor-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1152 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     2050 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      551 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json
+-rw-r--r--   0 runner    (1001) docker     (127)      402 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/files.json
+-rw-r--r--   0 runner    (1001) docker     (127)      572 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)      359 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlite/application-extension/share-file.json
+-rw-r--r--   0 runner    (1001) docker     (127)   105099 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/all.json
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-24 10:32:58.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/all_federated.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    17882 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/
+-rw-r--r--   0 runner    (1001) docker     (127)    16550 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)        0 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)   415751 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/build/third-party-licenses.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7193 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/config-utils.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/doc/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/doc/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      303 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/doc/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.409604 fixinventorycore-4.0.3/fixcore/jupyterlite/doc/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      295 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/doc/workspaces/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.413604 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      219 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2343 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.413604 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)    14992 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)    16598 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png
+-rw-rw-rw-   0 runner    (1001) docker     (127)     6950 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)       88 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)      598 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     4254 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png
+-rw-rw-rw-   0 runner    (1001) docker     (127)     7359 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)    13107 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.413604 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2732 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.421604 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2643 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     8311 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)  3598363 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1110 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)    70520 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      336 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js.LICENSE.txt
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2360 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)    14766 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     7706 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      118 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5802 2024-04-24 10:32:45.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.421604 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      199 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/install.json
+-rw-rw-rw-   0 runner    (1001) docker     (127)     5919 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.421604 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/
+-rw-rw-rw-   0 runner    (1001) docker     (127)      224 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/568.1e2faa2ba0bbe59c4780.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     8351 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     3925 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)      162 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/style.js
+-rw-rw-rw-   0 runner    (1001) docker     (127)     2452 2024-04-24 10:32:50.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.421604 fixinventorycore-4.0.3/fixcore/jupyterlite/files/
+-rw-r--r--   0 runner    (1001) docker     (127)     7578 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/files/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     4609 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/icon-120x120.png
+-rw-r--r--   0 runner    (1001) docker     (127)    20954 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/icon-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     6308 2024-04-24 10:32:58.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (127)    11526 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/jupyterlite.schema.v0.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.421604 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/
+-rw-r--r--   0 runner    (1001) docker     (127)   324251 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/jupyter-lite.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      166 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/jupyter-lite.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12425 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.421604 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/tree/
+-rw-r--r--   0 runner    (1001) docker     (127)      290 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/tree/index.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.421604 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)      288 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/lab/workspaces/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      690 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/manifest.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/package.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1626 1985-10-26 08:15:00.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/service-worker.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.309603 fixinventorycore-4.0.3/fixcore/jupyterlite/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.425604 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 10:32:53.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 10:32:53.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 10:32:53.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 10:32:53.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-file.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 10:32:53.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-notebook.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)     1150 2024-04-24 10:32:53.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-terminal.ico
+-rw-rw-rw-   0 runner    (1001) docker     (127)    32038 2024-04-24 10:32:53.000000 fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)    11967 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/message_bus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.425604 fixinventorycore-4.0.3/fixcore/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/adjust_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16822 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/db_updater.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3027 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/exportable_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30006 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/graph_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5799 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/json_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69697 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11128 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/model_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/resolve_in_graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/transform_kind_convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/model/typed_model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.429604 fixinventorycore-4.0.3/fixcore/query/
+-rw-r--r--   0 runner    (1001) docker     (127)      973 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51739 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/query/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15449 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/query/query_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/query/template_expander.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/query/template_expander_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.429604 fixinventorycore-4.0.3/fixcore/report/
+-rw-r--r--   0 runner    (1001) docker     (127)    19667 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6264 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/report/benchmark_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26776 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/report/inspector_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6471 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/report/report_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.429604 fixinventorycore-4.0.3/fixcore/static/
+-rw-r--r--   0 runner    (1001) docker     (127)   141248 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/static/api-doc.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3931 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/static/ck-unicode-truecolor.ans
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/static/fix.css
+-rw-r--r--   0 runner    (1001) docker     (127)    14617 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/static/fixinventory_logo_and_text.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12500 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/system_start.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.429604 fixinventorycore-4.0.3/fixcore/task/
+-rw-r--r--   0 runner    (1001) docker     (127)     1616 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/job_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1579 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2999 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/start_workflow_on_first_subscriber.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8059 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/subscribers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/task_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33482 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/task_description.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30250 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/task/task_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.429604 fixinventorycore-4.0.3/fixcore/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3345 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/templates/create_first_user.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3410 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/templates/home.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/templates/login.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.433604 fixinventorycore-4.0.3/fixcore/user/
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/user/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/user/user_management.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15809 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.433604 fixinventorycore-4.0.3/fixcore/web/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      519 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/accesslog.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80914 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10187 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13060 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/certificate_handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8726 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/content_renderer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6786 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/directives.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5280 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/web/tsdb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10475 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/fixcore/worker_task_queue.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.445604 fixinventorycore-4.0.3/fixinventorycore.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6017 2024-04-24 10:33:00.000000 fixinventorycore-4.0.3/fixinventorycore.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    30702 2024-04-24 10:33:00.000000 fixinventorycore-4.0.3/fixinventorycore.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:33:00.000000 fixinventorycore-4.0.3/fixinventorycore.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 10:33:00.000000 fixinventorycore-4.0.3/fixinventorycore.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:33:00.000000 fixinventorycore-4.0.3/fixinventorycore.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 10:33:00.000000 fixinventorycore-4.0.3/fixinventorycore.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 10:33:00.000000 fixinventorycore-4.0.3/fixinventorycore.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1971 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 10:33:00.449605 fixinventorycore-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.433604 fixinventorycore-4.0.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.437604 fixinventorycore-4.0.3/tests/fixcore/
+-rw-r--r--   0 runner    (1001) docker     (127)     1924 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.437604 fixinventorycore-4.0.3/tests/fixcore/analytics/
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/analytics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1001 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/analytics/posthog_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/analytics/recurrent_events_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.437604 fixinventorycore-4.0.3/tests/fixcore/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13659 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/cli/cli_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65515 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/cli/command_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4904 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/cli/model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.437604 fixinventorycore-4.0.3/tests/fixcore/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12726 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/config/config_handler_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6605 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/config/config_override_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4798 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/config/core_config_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31093 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/console_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9003 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/core_config_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.441604 fixinventorycore-4.0.3/tests/fixcore/db/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19729 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/arango_query_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/arangodb_functions_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/async_arangodb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/configdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/db_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2394 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/deferredouteredgedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/entitydb.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41807 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/graphdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2792 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/jobdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3513 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/modeldb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/reportdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6042 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/runningtaskdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/system_data_db_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2706 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/templatedb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7587 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/db/timeseriesdb_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6327 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/dependencies_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.441604 fixinventorycore-4.0.3/tests/fixcore/graph_manager/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/graph_manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7310 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/graph_manager/graph_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/hypothesis_extension.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.441604 fixinventorycore-4.0.3/tests/fixcore/infra_apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/infra_apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4632 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/infra_apps/local_runtime_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4642 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/infra_apps/package_manager_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/message_bus_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.445604 fixinventorycore-4.0.3/tests/fixcore/model/
+-rw-r--r--   0 runner    (1001) docker     (127)     1266 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/adjust_node_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3523 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/db_updater_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/exportable_model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16753 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/graph_access_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/json_schema_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/model_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28507 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/resolve_in_graph_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/model/typed_model_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.445604 fixinventorycore-4.0.3/tests/fixcore/query/
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15213 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/query/model_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18737 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/query/query_parser_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8095 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/query/template_expander_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.445604 fixinventorycore-4.0.3/tests/fixcore/report/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/report/benchmark_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9621 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/report/inspector_service_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.445604 fixinventorycore-4.0.3/tests/fixcore/task/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/task/job_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/task/start_workflow_on_first_subscriber_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3613 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/task/subscribers_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11073 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/task/task_description_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11113 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/task/task_handler_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.445604 fixinventorycore-4.0.3/tests/fixcore/user/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/user/user_management_service_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6082 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/util_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/validator_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:33:00.445604 fixinventorycore-4.0.3/tests/fixcore/web/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15974 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/web/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24351 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/web/api_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/web/auth_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4697 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/web/certificate_handler_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/web/content_renderer_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/web/permission_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-24 10:29:25.000000 fixinventorycore-4.0.3/tests/fixcore/worker_task_queue_test.py
```

### Comparing `fixinventorycore-4.0.2/PKG-INFO` & `fixinventorycore-4.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorycore
-Version: 4.0.2
+Version: 4.0.3
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Homepage, https://inventory.fix.security
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `fixinventorycore-4.0.2/README.md` & `fixinventorycore-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/__main__.py` & `fixinventorycore-4.0.3/fixcore/__main__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/action_handlers/merge_outer_edge_handler.py` & `fixinventorycore-4.0.3/fixcore/action_handlers/merge_outer_edge_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/analytics/__init__.py` & `fixinventorycore-4.0.3/fixcore/analytics/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/analytics/posthog.py` & `fixinventorycore-4.0.3/fixcore/analytics/posthog.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/analytics/recurrent_events.py` & `fixinventorycore-4.0.3/fixcore/analytics/recurrent_events.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/async_extensions.py` & `fixinventorycore-4.0.3/fixcore/async_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/cli/__init__.py` & `fixinventorycore-4.0.3/fixcore/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/cli/cli.py` & `fixinventorycore-4.0.3/fixcore/cli/cli.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/cli/command.py` & `fixinventorycore-4.0.3/fixcore/cli/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -6238,14 +6238,15 @@
             "get": [
                 ArgInfo("--name", expects_value=True, help_text="<time series>"),
                 ArgInfo("--start", expects_value=True, value_hint="datetime", help_text="<time series>"),
                 ArgInfo("--end", expects_value=True, value_hint="datetime", help_text="<time series>"),
                 ArgInfo("--group", expects_value=True, can_occur_multiple_times=True, help_text="<group>"),
                 ArgInfo("--filter", expects_value=True, can_occur_multiple_times=True, help_text="<var><op><value>"),
                 ArgInfo("--granularity", expects_value=True, help_text="<duration|integer>"),
+                ArgInfo("--aggregation", expects_value=True, possible_values=["avg", "sum", "min", "max"]),
             ],
             "downsample": [],
         }
 
     def parse(self, arg: Optional[str] = None, ctx: CLIContext = EmptyContext, **kwargs: Any) -> CLIAction:
         async def snapshot_time_series(part: str) -> AsyncIterator[str]:
             parser = NoExitArgumentParser()
@@ -6269,18 +6270,26 @@
             parser = NoExitArgumentParser()
             parser.add_argument("--name", type=str, required=True)
             parser.add_argument("--start", type=parse_time_or_delta, required=True)
             parser.add_argument("--end", type=parse_time_or_delta, required=True)
             parser.add_argument("--group", type=str, nargs="*", default=None)
             parser.add_argument("--filter", type=predicate_term.parse, nargs="*", default=None)
             parser.add_argument("--granularity", type=parse_duration_or_int, default=5)
+            parser.add_argument("--aggregation", choices=["avg", "sum", "min", "max"], default="avg")
             p = parser.parse_args(args_parts_unquoted_parser.parse(part))
             timeout = if_set(ctx.env.get("search_timeout"), duration)
             cursor = await self.dependencies.db_access.time_series_db.load_time_series(
-                p.name, p.start, p.end, group_by=p.group, filter_by=p.filter, granularity=p.granularity, timeout=timeout
+                p.name,
+                p.start,
+                p.end,
+                group_by=p.group,
+                filter_by=p.filter,
+                granularity=p.granularity,
+                timeout=timeout,
+                aggregation=p.aggregation,
             )
             return CLISourceContext(cursor.count(), cursor.full_count()), cursor
 
         async def list_ts() -> Tuple[int, JsGen]:
             ts = await self.dependencies.db_access.time_series_db.list_time_series()
             return len(ts), stream.iterate([to_js(a) for a in ts])
```

### Comparing `fixinventorycore-4.0.2/fixcore/cli/model.py` & `fixinventorycore-4.0.3/fixcore/cli/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/cli/tip_of_the_day.py` & `fixinventorycore-4.0.3/fixcore/cli/tip_of_the_day.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/config/__init__.py` & `fixinventorycore-4.0.3/fixcore/config/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/config/config_handler_service.py` & `fixinventorycore-4.0.3/fixcore/config/config_handler_service.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/config/config_override_service.py` & `fixinventorycore-4.0.3/fixcore/config/config_override_service.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/config/core_config_handler.py` & `fixinventorycore-4.0.3/fixcore/config/core_config_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/console_renderer.py` & `fixinventorycore-4.0.3/fixcore/console_renderer.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/constants.py` & `fixinventorycore-4.0.3/fixcore/constants.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/core_config.py` & `fixinventorycore-4.0.3/fixcore/core_config.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/__init__.py` & `fixinventorycore-4.0.3/fixcore/db/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/arango_query.py` & `fixinventorycore-4.0.3/fixcore/db/arango_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -871,14 +871,15 @@
 
 def load_time_series(
     time_series_collection: str,
     time_series: str,
     start: datetime,
     end: datetime,
     granularity: timedelta,
+    group_aggregation: Literal["avg", "sum", "min", "max"] = "avg",
     group_by: Optional[Collection[str]] = None,
     group_filter: Optional[List[Predicate]] = None,
 ) -> Tuple[str, Json]:
     ctx = ArangoQueryContext()
     bv_name = ctx.add_bind_var(time_series)
     bv_start = ctx.add_bind_var(int(start.timestamp()))
     bv_end = ctx.add_bind_var(int(end.timestamp()))
@@ -890,32 +891,44 @@
             bv = ctx.add_bind_var(f.value)
             parts.append(f"d.group.{f.name}{f.op}@{bv}")
         query += f" FILTER {' AND '.join(parts)}"
     time_slot = ctx.next_crs()
     slotter = int(granularity.total_seconds())
     gran = ctx.add_bind_var(slotter)
     offset = start.timestamp() - ((start.timestamp() // slotter) * slotter)
+    # slot the time by averaging each single group
     query += f" LET {time_slot} = (FLOOR(d.at / @{gran}) * @{gran}) + @{ctx.add_bind_var(offset)}"
+    query += f" COLLECT group_slot={time_slot}, complete_group=d.group"
+    query += " AGGREGATE slot_avg = AVG(d.v)"
+    query += " RETURN {at: group_slot, group: complete_group, v: slot_avg}"
+
+    # short circuit: no additional grouping and aggregation is avg
+    if group_by is None and group_aggregation == "avg":
+        return query, ctx.bind_vars  # already the correct query
+
     # create the groups to collect
-    collect = [f"group_slot={time_slot}"]
+    slotted = ctx.next_crs()
+    collect = ["group_slot=d.at"]
     group = ""
     if group_by is None:
         collect.append("complete_group=d.group")
         group = "group: complete_group,"
     elif len(group_by) == 0:
         pass  # no other groups
     else:
         parts = []
         for g in group_by:
             collect.append(f"group_{g}=d.group.{g}")
             parts.append(f"{g}: group_{g}")
         group = f"group: {{ {', '.join(parts)} }},"
 
-    query += f" COLLECT {', '.join(collect)} INTO group"
-    query += f" SORT group_slot RETURN {{at: group_slot, {group} v: AVG(group[*].d.v)}}"
+    query = f"LET {slotted} = ( {query} )\n"
+    query += f" FOR d in {slotted} COLLECT {', '.join(collect)}"
+    query += f" AGGREGATE agg_val={group_aggregation}(d.v)"
+    query += f" SORT group_slot RETURN {{at: group_slot,{group} v: agg_val}}"
     return query, ctx.bind_vars
 
 
 async def query_cost(graph_db: Any, model: QueryModel, with_edges: bool) -> EstimatedSearchCost:
     q_string, bind = to_query(graph_db, model, with_edges=with_edges)
     nr_nodes = await graph_db.db.count(graph_db.vertex_name)
     plan = await graph_db.db.explain(query=q_string, bind_vars=bind)
```

### Comparing `fixinventorycore-4.0.2/fixcore/db/arangodb_extensions.py` & `fixinventorycore-4.0.3/fixcore/db/arangodb_extensions.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/arangodb_functions.py` & `fixinventorycore-4.0.3/fixcore/db/arangodb_functions.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/async_arangodb.py` & `fixinventorycore-4.0.3/fixcore/db/async_arangodb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/configdb.py` & `fixinventorycore-4.0.3/fixcore/db/configdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/db_access.py` & `fixinventorycore-4.0.3/fixcore/db/db_access.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/deferredouteredgedb.py` & `fixinventorycore-4.0.3/fixcore/db/deferredouteredgedb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/entitydb.py` & `fixinventorycore-4.0.3/fixcore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/graphdb.py` & `fixinventorycore-4.0.3/fixcore/db/graphdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/model.py` & `fixinventorycore-4.0.3/fixcore/db/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/packagedb.py` & `fixinventorycore-4.0.3/fixcore/db/packagedb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/reportdb.py` & `fixinventorycore-4.0.3/fixcore/db/reportdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/runningtaskdb.py` & `fixinventorycore-4.0.3/fixcore/db/runningtaskdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/system_data_db.py` & `fixinventorycore-4.0.3/fixcore/db/system_data_db.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/db/timeseriesdb.py` & `fixinventorycore-4.0.3/fixcore/db/timeseriesdb.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import logging
 import time
 from collections import defaultdict
 from contextlib import asynccontextmanager
 from datetime import timedelta, datetime, timezone
 from functools import partial
 from numbers import Number
-from typing import Optional, List, Set, Union, cast, Callable, Dict, AsyncIterator
+from typing import Optional, List, Set, Union, cast, Callable, Dict, AsyncIterator, Literal
 
 from attr import evolve, define
 from fixcore.core_config import CoreConfig
 from fixcore.db import arango_query
 from fixcore.db.async_arangodb import AsyncArangoDB, AsyncCursor, AsyncArangoTransactionDB
 from fixcore.db.graphdb import GraphDB
 from fixcore.db.model import QueryModel
@@ -111,28 +111,30 @@
         *,
         group_by: Optional[Set[str]] = None,
         filter_by: Optional[List[Predicate]] = None,
         granularity: Optional[Union[timedelta, int]] = None,
         trafo: Optional[Callable[[Json], Json]] = None,
         batch_size: Optional[int] = None,
         timeout: Optional[timedelta] = None,
+        aggregation: Literal["avg", "sum", "min", "max"] = "avg",
     ) -> AsyncCursor:
         """
         Load time series data.
         :param name: The name of the time series.
         :param start: Filter data after this time.
         :param end: Filter data before this time.
         :param group_by: Combine defined group properties. Only existing group properties can be used.
         :param filter_by: Filter specific group properties by predicate.
         :param granularity: Optional timedelta to retrieve data in a specific granularity.
                The minimum granularity is one hour.
                In case this number is an integer, it is interpreted as the number of steps between start and end.
         :param trafo: Optional transformation function to apply to each result.
         :param batch_size: Optional batch size for the query.
         :param timeout: Timeout for the query to run.
+        :param aggregation: The aggregation function to use.
         :return: A cursor to iterate over the time series data.
         """
         assert start < end, "start must be before end"
         assert name, "name must not be empty"
         duration = end - start
 
         # compute effective granularity
@@ -141,15 +143,17 @@
         elif isinstance(granularity, timedelta):
             grl = granularity
         else:
             grl = duration / 20  # default to 20 datapoints if nothing is specified
 
         grl = max(grl, timedelta(hours=1))
 
-        qs, bv = arango_query.load_time_series(self.collection_name, name, start, end, grl, group_by, filter_by)
+        qs, bv = arango_query.load_time_series(
+            self.collection_name, name, start, end, grl, aggregation, group_by, filter_by
+        )
 
         def result_trafo(js: Json) -> Json:
             js["at"] = utc_str(datetime.fromtimestamp(js["at"], timezone.utc))
             return js
 
         ttl = cast(Number, int(timeout.total_seconds())) if timeout else None
         async with await self.db.aql_cursor(
@@ -188,14 +192,15 @@
                             ts.name,
                             c_start,
                             c_end,
                             granularity=bucket.resolution,
                             trafo=partial(ts_format, ts.name),
                             batch_size=100_000,  # The values are tiny. Use a large batch size.
                             timeout=timedelta(seconds=60),
+                            aggregation="avg",
                         )
                     ]:
                         log.info(f"Compact {ts.name} bucket {bucket} to {len(ts_data)} entries (last={ts_bucket_last})")
                         result[ts.name].append(
                             {
                                 "bucket": str(bucket),
                                 "start": utc_str(c_start),
```

### Comparing `fixinventorycore-4.0.2/fixcore/db/usagedb.py` & `fixinventorycore-4.0.3/fixcore/db/usagedb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/dependencies.py` & `fixinventorycore-4.0.3/fixcore/dependencies.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/error.py` & `fixinventorycore-4.0.3/fixcore/error.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/graph_manager/graph_manager.py` & `fixinventorycore-4.0.3/fixcore/graph_manager/graph_manager.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/ids.py` & `fixinventorycore-4.0.3/fixcore/ids.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/infra_apps/local_runtime.py` & `fixinventorycore-4.0.3/fixcore/infra_apps/local_runtime.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/infra_apps/manifest.py` & `fixinventorycore-4.0.3/fixcore/infra_apps/manifest.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/infra_apps/package_manager.py` & `fixinventorycore-4.0.3/fixcore/infra_apps/package_manager.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/infra_apps/runtime.py` & `fixinventorycore-4.0.3/fixcore/infra_apps/runtime.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/api/contents/all.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/api/contents/all.json`

 * *Files 21% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9131944444444443%*

 * *Differences: {"'content'": "{0: {'created': '2024-04-24T10:32:58.033576Z', 'last_modified': "*

 * *              "'2024-04-24T10:29:25.664898Z'}}",*

 * * "'created'": "'2024-04-24T10:32:58.033576Z'",*

 * * "'last_modified'": "'2024-04-24T10:32:58.033576Z'"}*

```diff
@@ -1,29 +1,29 @@
 {
     "content": [
         {
             "content": null,
-            "created": "2024-04-12T12:17:08.169280Z",
+            "created": "2024-04-24T10:32:58.033576Z",
             "format": null,
             "hash": null,
             "hash_algorithm": null,
-            "last_modified": "2024-04-12T12:13:44.701395Z",
+            "last_modified": "2024-04-24T10:29:25.664898Z",
             "mimetype": null,
             "name": "example.ipynb",
             "path": "example.ipynb",
             "size": 7578,
             "type": "notebook",
             "writable": true
         }
     ],
-    "created": "2024-04-12T12:17:08.169280Z",
+    "created": "2024-04-24T10:32:58.033576Z",
     "format": "json",
     "hash": null,
     "hash_algorithm": null,
-    "last_modified": "2024-04-12T12:17:08.169280Z",
+    "last_modified": "2024-04-24T10:32:58.033576Z",
     "mimetype": null,
     "name": "",
     "path": "",
     "size": null,
     "type": "directory",
     "writable": true
 }
```

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/bootstrap.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/bootstrap.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1053.7a56130.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1053.7a56130.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1088.33c6076.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1088.33c6076.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1091.1cf35e6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1091.1cf35e6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1122.d86c258.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1122.d86c258.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/114.1c04540.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/114.1c04540.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1169.4cf2d13.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1169.4cf2d13.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/125.4c6ac03.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/125.4c6ac03.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1261.3da9a56.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1261.3da9a56.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/131.5b6a7ab.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/131.5b6a7ab.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1385.707019c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1385.707019c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1388.0f22ef8.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1388.0f22ef8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1418.d9431d8.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1418.d9431d8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/142.6e89fb8.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/142.6e89fb8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1495.671bdd4.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1495.671bdd4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1542.22098a5.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1542.22098a5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1558.548303d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1558.548303d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1584.d919fce.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1584.d919fce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1618.983fc32.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1618.983fc32.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1715.ebbb93b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1715.ebbb93b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1769.10c2b5d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1769.10c2b5d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1815.2af66e5.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1815.2af66e5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1837.622ebbe.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1837.622ebbe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1846.ed084ce.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1846.ed084ce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1869.86f5778.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1869.86f5778.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1871.7fed383.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1871.7fed383.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/1941.79180b2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/1941.79180b2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2065.410c3bc.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2065.410c3bc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/214.300dbf1.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/214.300dbf1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2188.9676797.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2188.9676797.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/221.59c0059.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/221.59c0059.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2213.b58cab4.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2213.b58cab4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2241.91c6cce.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2241.91c6cce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2323.7e4d795.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2323.7e4d795.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2324.aff3939.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2324.aff3939.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2343.3cf0fe8.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2343.3cf0fe8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2349.9acb0b1.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2349.9acb0b1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2363.6aa6a7f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2363.6aa6a7f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2386.5f8e2da.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2386.5f8e2da.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2520.5c65366.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2520.5c65366.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2552.6c5224e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2552.6c5224e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/261.431b309.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/261.431b309.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2622.3d61d64.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2622.3d61d64.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2666.6cce729.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2666.6cce729.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2682.0c612a1.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2682.0c612a1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2692.f2b8d53.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2692.f2b8d53.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/270.9675bfe.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/270.9675bfe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2702.0e1a6ff.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2702.0e1a6ff.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/28.9f8dd00.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/28.9f8dd00.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2871.e1a64a6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2871.e1a64a6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2913.25c5e72.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2913.25c5e72.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2913.25c5e72.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2930.896decd.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2930.896decd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/2955.c8d0773.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/2955.c8d0773.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/306.b568c30.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/306.b568c30.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3079.18e3c32.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3079.18e3c32.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/311.76f79fc.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/311.76f79fc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3111.8de2d0a.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3111.8de2d0a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3154.5d8f80d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3154.5d8f80d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3211.aa42b4a.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3211.aa42b4a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3218.758a794.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3218.758a794.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3230.2c849ff.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3230.2c849ff.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3245.c48f805.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3245.c48f805.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3322.428e385.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3322.428e385.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3336.3d4780f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3336.3d4780f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3370.b5d78cd.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3370.b5d78cd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3420.418f467.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3420.418f467.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3449.4a13bea.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3449.4a13bea.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3488.9d14a3e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3488.9d14a3e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/35.26a4324.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/35.26a4324.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3501.a0b897f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3501.a0b897f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3562.77d1e3d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3562.77d1e3d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3604.9c8b7b0.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3604.9c8b7b0.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3694.3437882.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3694.3437882.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3700.ab2c843.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3700.ab2c843.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3797.2bb532c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3797.2bb532c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/383.0385e5e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/383.0385e5e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3864.acf045c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3864.acf045c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/3992.5a17c7b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/3992.5a17c7b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4002.d2530f2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4002.d2530f2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/403.ea946dc.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/403.ea946dc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4030.8963386.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4030.8963386.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4035.88e3670.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4035.88e3670.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4038.bb0e593.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4038.bb0e593.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4039.2635132.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4039.2635132.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4105.05362d2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4105.05362d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4148.0cb7e6d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4148.0cb7e6d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/431.f294aa7.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/431.f294aa7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4324.992bd2c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4324.992bd2c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4333.fdaab90.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4333.fdaab90.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4387.f2b950d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4387.f2b950d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4434.547c185.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4434.547c185.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4478.8778446.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4478.8778446.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4498.fced3e4.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4498.fced3e4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4499.7b7aa96.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4499.7b7aa96.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4521.c2278f6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4521.c2278f6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4588.66d005c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4588.66d005c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4630.32049fe.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4630.32049fe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4670.72adecb.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4670.72adecb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4780.f7ebd53.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4780.f7ebd53.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4810.fdb4bef.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4810.fdb4bef.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4825.0f290ff.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4825.0f290ff.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4843.96ed13d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4843.96ed13d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4926.3619db2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4926.3619db2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4954.ac85606.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4954.ac85606.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4965.9c0bd12.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4965.9c0bd12.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/4971.ba52a81.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/4971.ba52a81.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/500.b866efa.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/500.b866efa.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5008.7707efe.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5008.7707efe.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5013.5ff10dd.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5013.5ff10dd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5019.fe7898c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5019.fe7898c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5061.d662bbf.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5061.d662bbf.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5115.c11e8fa.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5115.c11e8fa.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/514.1c1b052.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/514.1c1b052.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5233.96f1668.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5233.96f1668.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5249.847f856.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5249.847f856.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5261.2a76287.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5261.2a76287.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5276.069ed0f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5276.069ed0f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5299.4fe47ed.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5299.4fe47ed.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5343.c65eb48.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5343.c65eb48.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5425.ff5465e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5425.ff5465e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5464.7c73ae4.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5464.7c73ae4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5494.db2521b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5494.db2521b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5597.2470f52.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5597.2470f52.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/563.7fd8ced.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/563.7fd8ced.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5691.16de5f4.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5691.16de5f4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5698.7febbe1.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5698.7febbe1.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5765.72d36d2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5765.72d36d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5777.c1c07e5.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5777.c1c07e5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5822.7e14b54.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5822.7e14b54.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5828.e1ab6ce.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5828.e1ab6ce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5834.ba430d2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5834.ba430d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5850.9fd6e53.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5850.9fd6e53.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5945.4a06217.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5945.4a06217.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5972.aa32cae.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5972.aa32cae.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/5996.8503bba.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/5996.8503bba.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6139.0c4aaeb.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6139.0c4aaeb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6236.5f93bea.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6236.5f93bea.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6271.c4952fd.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6271.c4952fd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6281.f763d40.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6281.f763d40.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/632.200fdf3.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/632.200fdf3.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6417.bebf125.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6417.bebf125.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6433.a6cfc6e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6433.a6cfc6e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/644.0a629ee.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/644.0a629ee.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/647.8cecbd3.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/647.8cecbd3.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6473.a97af61.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6473.a97af61.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/653.7dd3d36.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/653.7dd3d36.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6553.a73f98d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6553.a73f98d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6607.4ee069b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6607.4ee069b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/661.477cacc.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/661.477cacc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6640.bf24711.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6640.bf24711.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6667.60cb1d2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6667.60cb1d2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/67.3672096.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/67.3672096.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6739.d19f4c2.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6739.d19f4c2.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/677.493cb60.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/677.493cb60.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6788.4fb5bb9.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6788.4fb5bb9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/69.fc53c91.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/69.fc53c91.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6941.7241556.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6941.7241556.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6942.bcc3a2f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6942.bcc3a2f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/6972.930242c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/6972.930242c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7005.de1d9f9.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7005.de1d9f9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7010.979a827.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7010.979a827.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7022.6d0ffc3.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7022.6d0ffc3.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7054.de34848.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7054.de34848.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7061.30f7cf6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7061.30f7cf6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7097.d4214d0.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7097.d4214d0.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7125.4a0562f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7125.4a0562f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7153.135087f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7153.135087f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7154.804d332.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7154.804d332.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7170.7bba13a.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7170.7bba13a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7179.af46233.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7179.af46233.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7259.6d595ca.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7259.6d595ca.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7264.0ec5936.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7264.0ec5936.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7360.7b1e065.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7360.7b1e065.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7369.a12e276.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7369.a12e276.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7378.b4f5497.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7378.b4f5497.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7427.368a8bc.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7427.368a8bc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/745.83ff9e4.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/745.83ff9e4.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7450.d5ee0a9.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7450.d5ee0a9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7471.30d9d48.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7471.30d9d48.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7495.3c478a0.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7495.3c478a0.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7534.a755d75.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7534.a755d75.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/755.6424780.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/755.6424780.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7557.bd5cd49.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7557.bd5cd49.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7582.7350cc5.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7582.7350cc5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7674.93d7410.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7674.93d7410.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7803.45d27da.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7803.45d27da.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7811.bd10193.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7811.bd10193.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7817.6a39acf.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7817.6a39acf.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7866.e7f89f6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7866.e7f89f6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7892.c46785d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7892.c46785d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7918.506a625.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7918.506a625.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/792.f22b43b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/792.f22b43b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7969.f8f9146.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7969.f8f9146.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7995.e40b57d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7995.e40b57d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/7997.46ee9b7.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/7997.46ee9b7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8010.dbb2b65.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8010.dbb2b65.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8103.25c6881.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8103.25c6881.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8178.6647b58.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8178.6647b58.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8285.46eba3a.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8285.46eba3a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8378.d951634.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8378.d951634.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8381.4b39fc5.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8381.4b39fc5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8387.c2a5ccb.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8387.c2a5ccb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8427.379d337.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8427.379d337.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8433.c26711e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8433.c26711e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8443.32841be.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8443.32841be.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8446.d952b7d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8446.d952b7d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8479.7ad07d9.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8479.7ad07d9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/85.eb26499.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/85.eb26499.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/850.16f7c82.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/850.16f7c82.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8579.7c15dcd.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8579.7c15dcd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8734.0965980.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8734.0965980.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8768.cd685a6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8768.cd685a6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8800.5b7449b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8800.5b7449b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8801.7946caf.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8801.7946caf.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/883.7552b75.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/883.7552b75.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8845.3412b3f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8845.3412b3f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8845.3412b3f.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8927.b773418.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8927.b773418.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8929.0b66a95.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8929.0b66a95.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8937.6c8605f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8937.6c8605f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8979.2760112.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8979.2760112.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/8983.5db65ea.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/8983.5db65ea.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/899.dd8da16.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/899.dd8da16.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9022.85c8176.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9022.85c8176.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9037.6397c79.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9037.6397c79.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/906.f6a46ca.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/906.f6a46ca.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9060.9fe49c6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9060.9fe49c6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9073.fadf4d8.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9073.fadf4d8.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9166.d072a52.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9166.d072a52.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9208.10ca99e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9208.10ca99e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9233.b14ca62.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9233.b14ca62.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9234.488a70b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9234.488a70b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9239.13871ef.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9239.13871ef.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9244.a95e8aa.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9244.a95e8aa.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9250.43c7d24.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9250.43c7d24.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/927.399dde7.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/927.399dde7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9282.eb25fa6.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9282.eb25fa6.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9331.415f707.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9331.415f707.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9334.9101b2f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9334.9101b2f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9372.65a2507.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9372.65a2507.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9425.d103ed5.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9425.d103ed5.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9558.09c3851.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9558.09c3851.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9565.66944bd.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9565.66944bd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9597.9d6c989.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9597.9d6c989.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9604.c2c5590.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9604.c2c5590.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9643.4b4e30e.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9643.4b4e30e.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9676.f7b737a.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9676.f7b737a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9799.ecf3e29.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9799.ecf3e29.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9847.20223dd.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9847.20223dd.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9866.ea3fe7f.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9866.ea3fe7f.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9879.951cc05.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9879.951cc05.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/9903.633a36a.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/9903.633a36a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_AMS-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Calligraphic-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Calligraphic-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Fraktur-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Fraktur-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Main-Bold.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Main-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Main-Italic.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Main-Italic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Main-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Main-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Math-BoldItalic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Math-Italic.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Math-Italic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_SansSerif-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_SansSerif-Italic.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_SansSerif-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Script-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Script-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size1-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size2-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size3-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Size4-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Typewriter-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Vector-Bold.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Vector-Regular.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/MathJax_Zero.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/MathJax_Zero.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.eot` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.svg` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.ttf` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-brands-400.woff2` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.eot` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.svg` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.ttf` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-regular-400.woff2` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.eot` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.svg` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.ttf` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.woff` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/fa-solid-900.woff2` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/jlab_core.b96c356.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/jlab_core.b96c356.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/lab/bundle.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/lab/bundle.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/menus.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/application-extension/top.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/edit-notebook-metadata.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/notebook-extension/scroll-output.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/file-actions.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyter-notebook/tree-extension/widget.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/commands.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/context-menu.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/property-inspector.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/shell.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/application-extension/top-bar.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/notification.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/palette.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/print.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/sanitizer.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/themes.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/apputils-extension/utilityCommands.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/cell-toolbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/celltags-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/inline-completer.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/completer-extension/manager.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/console-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/csv.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/csvviewer-extension/tsv.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/docmanager-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/documentsearch-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/browser.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/download.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/filebrowser-extension/widget.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/fileeditor-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/htmlviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/imageviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/inspector-extension/inspector.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/launcher-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/logconsole-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/lsp-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/mainmenu-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/markdownviewer-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/mathjax-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/metadataform-extension/metadataforms.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/export.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/panel.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tools.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/notebook-extension/tracker.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/running-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/shortcuts-extension/shortcuts.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/statusbar-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/toc-extension/registry.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/consoles.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/tooltip-extension/notebooks.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/@jupyterlab/translation-extension/plugin.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/schemas/all.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/schemas/all.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/service-worker.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/service-worker.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-dark-extension/index.css`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/themes/@jupyterlab/theme-light-extension/index.css`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/build/third-party-licenses.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/build/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/config-utils.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/config-utils.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/312.749011b8237164f040ce.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/584.7e49152bd31ca0f8291b.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/5e8d6f34d83488f083fd.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/692.c1aeb4d97f766d3b4515.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/804.fb6a8eda889cf61eea27.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/b1c098fa349a030dacbe.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/remoteEntry.6014628263d9ee9ca44a.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/@jupyterlite/javascript-kernel-extension/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/133.7957020c5e8bc5703dbc.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/423.d0d3e2912c33c7566484.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/478.b48f45da3d88616ad3f9.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/486.6450efe6168c2f8caddb.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/657.15db1deb504caf7dbc6d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/855.323c80e7298812d692e7.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/remoteEntry.70a4f7e7a0383740860d.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab-plotly/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/747.67662283a5707eeb4d4c.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/remoteEntry.5cbb9d2323598fbda535.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/extensions/jupyterlab_pygments/static/third-party-licenses.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/files/example.ipynb` & `fixinventorycore-4.0.3/fixcore/jupyterlite/files/example.ipynb`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/icon-120x120.png` & `fixinventorycore-4.0.3/fixcore/jupyterlite/icon-120x120.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/icon-512x512.png` & `fixinventorycore-4.0.3/fixcore/jupyterlite/icon-512x512.png`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/index.html` & `fixinventorycore-4.0.3/fixcore/jupyterlite/index.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/jupyter-lite.ipynb` & `fixinventorycore-4.0.3/fixcore/jupyterlite/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/jupyter-lite.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/jupyter-lite.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/jupyterlite.schema.v0.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/jupyterlite.schema.v0.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/lab/favicon.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/lab/favicon.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/lab/index.html` & `fixinventorycore-4.0.3/fixcore/jupyterlite/lab/index.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/lab/jupyter-lite.ipynb` & `fixinventorycore-4.0.3/fixcore/jupyterlite/lab/jupyter-lite.ipynb`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/lab/package.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/lab/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/manifest.webmanifest` & `fixinventorycore-4.0.3/fixcore/jupyterlite/manifest.webmanifest`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/package.json` & `fixinventorycore-4.0.3/fixcore/jupyterlite/package.json`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/service-worker.js` & `fixinventorycore-4.0.3/fixcore/jupyterlite/service-worker.js`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-busy-1.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-busy-2.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-busy-3.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-file.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-file.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-notebook.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-notebook.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon-terminal.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon-terminal.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/jupyterlite/static/favicons/favicon.ico` & `fixinventorycore-4.0.3/fixcore/jupyterlite/static/favicons/favicon.ico`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/message_bus.py` & `fixinventorycore-4.0.3/fixcore/message_bus.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/metrics.py` & `fixinventorycore-4.0.3/fixcore/metrics.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/adjust_node.py` & `fixinventorycore-4.0.3/fixcore/model/adjust_node.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/db_updater.py` & `fixinventorycore-4.0.3/fixcore/model/db_updater.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/exportable_model.py` & `fixinventorycore-4.0.3/fixcore/model/exportable_model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/graph_access.py` & `fixinventorycore-4.0.3/fixcore/model/graph_access.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/json_schema.py` & `fixinventorycore-4.0.3/fixcore/model/json_schema.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/model.py` & `fixinventorycore-4.0.3/fixcore/model/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/model_handler.py` & `fixinventorycore-4.0.3/fixcore/model/model_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/resolve_in_graph.py` & `fixinventorycore-4.0.3/fixcore/model/resolve_in_graph.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/transform_kind_convert.py` & `fixinventorycore-4.0.3/fixcore/model/transform_kind_convert.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/model/typed_model.py` & `fixinventorycore-4.0.3/fixcore/model/typed_model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/query/__init__.py` & `fixinventorycore-4.0.3/fixcore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/query/model.py` & `fixinventorycore-4.0.3/fixcore/query/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/query/query_parser.py` & `fixinventorycore-4.0.3/fixcore/query/query_parser.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/query/template_expander.py` & `fixinventorycore-4.0.3/fixcore/query/template_expander.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/query/template_expander_service.py` & `fixinventorycore-4.0.3/fixcore/query/template_expander_service.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/report/__init__.py` & `fixinventorycore-4.0.3/fixcore/report/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from __future__ import annotations
 
 import logging
 from abc import ABC, abstractmethod
+from collections import defaultdict
 from enum import Enum
 from functools import reduce, total_ordering
 from typing import List, Optional, Dict, ClassVar, AsyncIterator, cast, Set, Tuple, Any
 
 from attr import define, field, evolve
 
 from fixcore.ids import ConfigId, GraphName
@@ -23,31 +24,37 @@
 # config keys and prefixes
 CheckConfigRoot = "report_check"
 BenchmarkConfigRoot = "report_benchmark"
 ReportConfigRoot = "report_config"
 
 
 _ReportSeverityPriority: Dict[str, int] = {"info": 0, "low": 1, "medium": 2, "high": 3, "critical": 4}
+_ReportSeverityScore: Dict[str, int] = {"info": 0, "low": 1, "medium": 2, "high": 3, "critical": 4}
 
 
 @total_ordering
 class ReportSeverity(Enum):
     kind: ClassVar[str] = "fix_core_report_check_severity"
     info = "info"
     low = "low"
     medium = "medium"
     high = "high"
     critical = "critical"
 
+    @property
     def prio(self) -> int:
         return _ReportSeverityPriority[self.value]
 
+    @property
+    def score(self) -> int:
+        return _ReportSeverityScore[self.value]
+
     def __lt__(self, other: Any) -> bool:
         if isinstance(other, ReportSeverity):
-            return self.prio() < other.prio()
+            return self.prio < other.prio
         return NotImplemented
 
     @staticmethod
     def from_name(name: str) -> ReportSeverity:
         return ReportSeverity[name]
 
 
@@ -355,14 +362,32 @@
                     result.append(
                         {"from": collection.node_id, "to": child.node_id, "type": "edge", "edge_type": "default"}
                     )
 
         visit_check_collection(self)
         return result
 
+    def score_for(self, account: str) -> int:
+        failing: Dict[ReportSeverity, int] = defaultdict(int)
+        available: Dict[ReportSeverity, int] = defaultdict(int)
+
+        def available_failing(check: CheckCollectionResult) -> None:
+            for result in check.checks:
+                available[result.check.severity] += 1
+                failing[result.check.severity] += (
+                    1 if result.number_of_resources_failing_by_account.get(account, 0) else 0
+                )
+            for child in check.children:
+                available_failing(child)
+
+        available_failing(self)  # walk the benchmark hierarchy
+        missing = sum(severity.score * count for severity, count in failing.items())
+        total = sum(severity.score * count for severity, count in available.items())
+        return int((max(0, total - missing) * 100) // total) if total > 0 else 100
+
 
 class Inspector(ABC):
     """
     The inspector is able to perform benchmarks or a set of checks.
     Benchmarks and checks are maintained via the configuration registry.
     A complete graph can be checked against either a pre-defined benchmark or from a selected set of checks.
     """
```

### Comparing `fixinventorycore-4.0.2/fixcore/report/benchmark_renderer.py` & `fixinventorycore-4.0.3/fixcore/report/benchmark_renderer.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 def render_benchmark_summary(benchmark: CheckCollectionResult, account: str) -> str:
     passing, failing = benchmark.passing_failing_checks_for_account(account)
 
     def render_result_list(name: str, icon: str, checks: List[CheckResult]) -> str:
         if checks:
             lr = f"## {name} \n\n"
-            for check in sorted(checks, key=lambda x: -x.check.severity.prio()):
+            for check in sorted(checks, key=lambda x: -x.check.severity.prio):
                 lr += f"- {icon} {check.check.severity.name}: {check.check.title}\n"
             return lr
         else:
             return ""
 
     result = render_result_list("Passed Checks", check_mark, passing)
     result += render_result_list("Failed Checks", cross_mark, failing)
```

### Comparing `fixinventorycore-4.0.2/fixcore/report/inspector_service.py` & `fixinventorycore-4.0.3/fixcore/report/inspector_service.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,15 +58,15 @@
     def severities_including(self, severity: ReportSeverity) -> List[ReportSeverity]:
         return [s for s in ReportSeverity if self.includes_severity(severity)]
 
     def includes_severity(self, severity: ReportSeverity) -> bool:
         if self.severity is None:
             return True
         else:
-            return self.severity.prio() <= severity.prio()
+            return self.severity.prio <= severity.prio
 
     def override_values(self) -> Optional[Json]:
         return self.config.override_values
 
     def filtered_accounts(self) -> Optional[List[str]]:
         if (accounts := self.accounts) and (ignore := self.config.ignore_accounts):
             return list(set(accounts) - set(ignore))
@@ -237,32 +237,47 @@
         accounts: Optional[List[str]] = None,
         severity: Optional[ReportSeverity] = None,
         only_failing: bool = False,
         sync_security_section: bool = False,
         report_run_id: Optional[str] = None,
     ) -> Dict[str, BenchmarkResult]:
         config = await self.report_config()
-        context = CheckContext(accounts=accounts, severity=severity, only_failed=only_failing, config=config)
         benchmarks = await self.__benchmarks(benchmark_names)
+        clouds = {c for b in benchmarks.values() for c in b.clouds or []}
+        cloud_accounts = accounts or await self.__list_accounts(list(clouds), graph)
+        context = CheckContext(accounts=cloud_accounts, severity=severity, only_failed=only_failing, config=config)
         # collect all checks
         check_ids = {check for b in benchmarks.values() for check in b.nested_checks() if config.check_allowed(check)}
         checks = await self.list_checks(check_ids=list(check_ids), context=context)
         check_lookup = {check.id: check for check in checks}
         # create benchmark results
         results = await self.__perform_checks(graph, checks, context)
         result = {
             name: self.__to_result(benchmark, check_lookup, results, context) for name, benchmark in benchmarks.items()
         }
         if sync_security_section:
             model = await self.model_handler.load_model(graph)
             # In case no run_id is provided, we invent a report run id here.
             run_id = report_run_id or uuid_str()
-            await self.db_access.get_graph_db(graph).update_security_section(
-                run_id, self.__benchmarks_to_security_iterator(result), model, accounts
-            )
+            db = self.db_access.get_graph_db(graph)
+            await db.update_security_section(run_id, self.__benchmarks_to_security_iterator(result), model, accounts)
+            # store the security score of an account
+            if account_ids := context.accounts:
+                async with await db.search_list(  # lookup node ids for all given accounts
+                    QueryModel(Query.by("account", P("reported.id").is_in(account_ids)), model)
+                ) as crsr:
+                    async for acc in crsr:
+                        if (node_id := value_in_path(acc, NodePath.node_id)) and (
+                            acc_id := value_in_path(acc, NodePath.reported_id)
+                        ):
+                            bench_score = {br.id: br.score_for(acc_id) for br in result.values()}
+                            account_score = sum(bench_score.values()) / len(bench_score) if bench_score else 100
+                            patch = {"score": account_score, "benchmark": bench_score}
+                            async for _ in db.update_nodes_metadata(model, patch, [node_id]):
+                                pass
         return result
 
     async def perform_checks(
         self,
         graph: GraphName,
         *,
         provider: Optional[str] = None,
@@ -299,15 +314,15 @@
             framework="fix",
             version="1.0",
             checks=[c.id for c in checks],
             children=[],
         )
 
         if context.accounts is None:
-            context.accounts = await self.__list_accounts(benchmark, graph)
+            context.accounts = await self.__list_accounts(benchmark.clouds, graph)
 
         checks_to_perform = await self.list_checks(check_ids=benchmark.nested_checks(), context=context)
         check_by_id = {c.id: c for c in checks_to_perform}
         results = await self.__perform_checks(graph, checks_to_perform, context)
         await self.event_sender.core_event(CoreEvent.BenchmarkPerformed, {"benchmark": benchmark.id})
         return self.__to_result(benchmark, check_by_id, results, context)
 
@@ -445,20 +460,20 @@
         resources_by_account = defaultdict(list)
         async for resource in await self.__list_failing_resources(graph, model, inspection, context):
             account_id = value_in_path(resource, NodePath.ancestor_account_id)
             if account_id:
                 resources_by_account[account_id].append(bend(ReportResourceData, resource))
         return resources_by_account
 
-    async def __list_accounts(self, benchmark: Benchmark, graph: GraphName) -> List[str]:
+    async def __list_accounts(self, clouds: Optional[List[str]], graph: GraphName) -> List[str]:
         model = await self.model_handler.load_model(graph)
         gdb = self.db_access.get_graph_db(graph)
         query = Query.by("account")
-        if benchmark.clouds:
-            query = query.combine(Query.by(P.single("ancestors.cloud.reported.id").is_in(benchmark.clouds)))
+        if clouds:
+            query = query.combine(Query.by(P.single("ancestors.cloud.reported.id").is_in(clouds)))
         async with await gdb.search_list(QueryModel(query, model)) as crs:
             ids = [value_in_path(a, NodePath.reported_id) async for a in crs]
             return [aid for aid in ids if aid is not None]
 
     async def validate_benchmark_config(self, cfg_id: ConfigId, json: Json) -> Optional[Json]:
         errors = []
         try:
```

### Comparing `fixinventorycore-4.0.2/fixcore/report/report_config.py` & `fixinventorycore-4.0.3/fixcore/report/report_config.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/static/api-doc.yaml` & `fixinventorycore-4.0.3/fixcore/static/api-doc.yaml`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/static/ck-unicode-truecolor.ans` & `fixinventorycore-4.0.3/fixcore/static/ck-unicode-truecolor.ans`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/static/fixinventory_logo_and_text.svg` & `fixinventorycore-4.0.3/fixcore/static/fixinventory_logo_and_text.svg`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/system_start.py` & `fixinventorycore-4.0.3/fixcore/system_start.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/task/__init__.py` & `fixinventorycore-4.0.3/fixcore/task/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/task/model.py` & `fixinventorycore-4.0.3/fixcore/task/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/task/scheduler.py` & `fixinventorycore-4.0.3/fixcore/task/scheduler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/task/start_workflow_on_first_subscriber.py` & `fixinventorycore-4.0.3/fixcore/task/start_workflow_on_first_subscriber.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/task/subscribers.py` & `fixinventorycore-4.0.3/fixcore/task/subscribers.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/task/task_description.py` & `fixinventorycore-4.0.3/fixcore/task/task_description.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/task/task_handler.py` & `fixinventorycore-4.0.3/fixcore/task/task_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/templates/base.html` & `fixinventorycore-4.0.3/fixcore/templates/base.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/templates/create_first_user.html` & `fixinventorycore-4.0.3/fixcore/templates/create_first_user.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/templates/home.html` & `fixinventorycore-4.0.3/fixcore/templates/home.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/templates/login.html` & `fixinventorycore-4.0.3/fixcore/templates/login.html`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/types.py` & `fixinventorycore-4.0.3/fixcore/types.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/user/__init__.py` & `fixinventorycore-4.0.3/fixcore/user/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/user/model.py` & `fixinventorycore-4.0.3/fixcore/user/model.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/user/user_management.py` & `fixinventorycore-4.0.3/fixcore/user/user_management.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/util.py` & `fixinventorycore-4.0.3/fixcore/util.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/validator.py` & `fixinventorycore-4.0.3/fixcore/validator.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/web/accesslog.py` & `fixinventorycore-4.0.3/fixcore/web/accesslog.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/web/api.py` & `fixinventorycore-4.0.3/fixcore/web/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -768,20 +768,22 @@
                 return int(s)
 
         name = request.match_info["timeseries"]
         body = await request.json() if request.content_length else {}
         start = if_set(body.get("start"), parse_utc, utc() - timedelta(days=7))
         end = if_set(body.get("end"), parse_utc, utc())
         group_by: Optional[Set[str]] = if_set(body.get("group"), set)
+        aggregation: Literal["avg", "sum", "min", "max"] = body.get("aggregation", "avg")
+        assert aggregation in ["avg", "sum", "min", "max"], f"Invalid aggregation {aggregation}"
         filter_by: Optional[List[Predicate]] = if_set(
             body.get("filter"), lambda x: [predicate_term.parse(y) for y in x]  # type: ignore
         )
         granularity: Optional[Union[int, timedelta]] = if_set(body.get("granularity"), parse_duration_or_int)
         cursor = await deps.db_access.time_series_db.load_time_series(
-            name, start, end, group_by=group_by, filter_by=filter_by, granularity=granularity
+            name, start, end, group_by=group_by, filter_by=filter_by, granularity=granularity, aggregation=aggregation
         )
         return await self.stream_response_from_gen(
             request, cursor, count=cursor.count(), total_count=cursor.full_count()
         )
 
     async def handle_events(self, request: Request, deps: TenantDependencies) -> StreamResponse:
         show = request.query["show"].split(",") if "show" in request.query else ["*"]
```

### Comparing `fixinventorycore-4.0.2/fixcore/web/auth.py` & `fixinventorycore-4.0.3/fixcore/web/auth.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/web/certificate_handler.py` & `fixinventorycore-4.0.3/fixcore/web/certificate_handler.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/web/content_renderer.py` & `fixinventorycore-4.0.3/fixcore/web/content_renderer.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/web/directives.py` & `fixinventorycore-4.0.3/fixcore/web/directives.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/web/permission.py` & `fixinventorycore-4.0.3/fixcore/web/permission.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/web/tsdb.py` & `fixinventorycore-4.0.3/fixcore/web/tsdb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixcore/worker_task_queue.py` & `fixinventorycore-4.0.3/fixcore/worker_task_queue.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/fixinventorycore.egg-info/PKG-INFO` & `fixinventorycore-4.0.3/fixinventorycore.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventorycore
-Version: 4.0.2
+Version: 4.0.3
 Summary: Keeps all the things.
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Homepage, https://inventory.fix.security
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `fixinventorycore-4.0.2/fixinventorycore.egg-info/SOURCES.txt` & `fixinventorycore-4.0.3/fixinventorycore.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/pyproject.toml` & `fixinventorycore-4.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fixinventorycore"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{name="Some Engineering Inc."}]
 description = "Keeps all the things."
 license = { text="AGPLv3" }
 urls = {"Homepage" = "https://inventory.fix.security"}
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/__init__.py` & `fixinventorycore-4.0.3/tests/fixcore/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/analytics/posthog_test.py` & `fixinventorycore-4.0.3/tests/fixcore/analytics/posthog_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/analytics/recurrent_events_test.py` & `fixinventorycore-4.0.3/tests/fixcore/analytics/recurrent_events_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/cli/cli_test.py` & `fixinventorycore-4.0.3/tests/fixcore/cli/cli_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -168,22 +168,22 @@
     assert PredecessorsPart.parse_args("--with-origin delete", plain) == (0, EdgeTypes.delete)
     assert PredecessorsPart.parse_args("--with-origin delete", w_delete) == (0, EdgeTypes.delete)
     assert PredecessorsPart.parse_args("delete", w_delete) == (1, EdgeTypes.delete)
 
 
 @pytest.mark.asyncio
 async def test_create_query_parts(cli: CLI) -> None:
-    commands = await cli.evaluate_cli_command('search some_int==0 | search identifier=~"9_" | descendants')
+    commands = await cli.evaluate_cli_command('search some_int==0 | search id=~"9_" | descendants')
     sort = "sort reported.kind asc, reported.name asc, reported.id asc"
     assert len(commands) == 1
     assert len(commands[0].commands) == 2  # list command is added automagically
     assert commands[0].commands[0].name == "execute_search"
     assert (
         commands[0].executable_commands[0].arg
-        == f"'(reported.some_int == 0 and reported.identifier =~ \"9_\") {sort} -default[1:]-> all {sort}'"
+        == f"'(reported.some_int == 0 and reported.id =~ \"9_\") {sort} -default[1:]-> all {sort}'"
     )
     commands = await cli.evaluate_cli_command("search some_int==0 | descendants")
     assert "-default[1:]->" in commands[0].executable_commands[0].arg  # type: ignore
     commands = await cli.evaluate_cli_command("search some_int==0 | ancestors | ancestors")
     assert "<-default[2:]-" in commands[0].executable_commands[0].arg  # type: ignore
     commands = await cli.evaluate_cli_command("search some_int==0 | predecessors | predecessors")
     assert "<-default[2]-" in commands[0].executable_commands[0].arg  # type: ignore
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/cli/command_test.py` & `fixinventorycore-4.0.3/tests/fixcore/cli/command_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,19 +137,17 @@
     assert len(r3[0]) == 11
     r4 = await cli.execute_cli_command("search id(4) | descendants delete", list_sink)
     assert len(r4[0]) == 0
 
 
 @pytest.mark.asyncio
 async def test_search_source(cli: CLIService) -> None:
-    result = await cli.execute_cli_command('search is("foo") and some_int==0 --> identifier=~"9_"', list_sink)
+    result = await cli.execute_cli_command('search is("foo") and some_int==0 --> id=~"9_"', list_sink)
     assert len(result[0]) == 10
-    await cli.dependencies.template_expander.put_template(
-        Template("test", 'is(foo) and some_int==0 --> identifier=~"{{fid}}"')
-    )
+    await cli.dependencies.template_expander.put_template(Template("test", 'is(foo) and some_int==0 --> id=~"{{fid}}"'))
     result2 = await cli.execute_cli_command('search expand(test, fid="9_")', list_sink)
     assert len(result2[0]) == 10
 
     result3 = await cli.execute_cli_command("search --with-edges is(graph_root) -[0:1]->", list_sink)
     # node: graph_root
     # node: collector
     # edge: graph_root -> collector
@@ -498,15 +496,15 @@
     result = await cli.execute_cli_command("kind foo", list_sink)
     assert result[0][0] == {
         "name": "foo",
         "bases": ["base"],
         "properties": {
             "age": "duration",
             "ctime": "datetime",
-            "identifier": "string",
+            "id": "string",
             "kind": "string",
             "name": "string",
             "now_is": "datetime",
             "some_int": "int32",
             "some_string": "string",
         },
         "successors": ["bla"],
@@ -534,50 +532,50 @@
         await cli.execute_cli_command("kind foo bla bar", list_sink)
 
 
 @pytest.mark.asyncio
 async def test_sort_command(cli: CLI) -> None:
     async def identifiers(query: str) -> List[str]:
         result = await cli.execute_cli_command(query + " | dump", list_sink)
-        return [r["reported"]["identifier"] for r in result[0]]
+        return [r["reported"]["id"] for r in result[0]]
 
-    id_wo = await identifiers("search is(bla) | sort identifier")
-    id_asc = await identifiers("search is(bla) | sort identifier asc")
-    id_desc = await identifiers("search is(bla) | sort identifier desc")
-    id_kind = await identifiers("search is(bla) | sort identifier | sort kind")
+    id_wo = await identifiers("search is(bla) | sort id")
+    id_asc = await identifiers("search is(bla) | sort id asc")
+    id_desc = await identifiers("search is(bla) | sort id desc")
+    id_kind = await identifiers("search is(bla) | sort id | sort kind")
     assert id_wo == id_asc
     assert id_wo == id_kind
     assert id_asc == list(reversed(id_desc))
 
 
 @pytest.mark.asyncio
 async def test_limit_command(cli: CLI) -> None:
     async def identifiers(query: str) -> List[str]:
         result = await cli.execute_cli_command(query + " | dump", list_sink)
-        return [r["reported"]["identifier"] for r in result[0]]
+        return [r["reported"]["id"] for r in result[0]]
 
-    assert await identifiers("search is(bla) sort identifier | limit 1") == ["0_0"]
-    assert await identifiers("search is(bla) sort identifier | limit 2") == ["0_0", "0_1"]
-    assert await identifiers("search is(bla) sort identifier | limit 2, 2") == ["0_2", "0_3"]
-    assert await identifiers("search is(bla) sort identifier | limit 10, 2") == ["1_0", "1_1"]
-    assert await identifiers("search is(bla) sort identifier | limit 100, 2") == []
+    assert await identifiers("search is(bla) sort id | limit 1") == ["0_0"]
+    assert await identifiers("search is(bla) sort id | limit 2") == ["0_0", "0_1"]
+    assert await identifiers("search is(bla) sort id | limit 2, 2") == ["0_2", "0_3"]
+    assert await identifiers("search is(bla) sort id | limit 10, 2") == ["1_0", "1_1"]
+    assert await identifiers("search is(bla) sort id | limit 100, 2") == []
 
 
 @pytest.mark.asyncio
 async def test_list_command(cli: CLI) -> None:
-    result = await cli.execute_cli_command('search is (foo) and identifier=="4" sort some_int | list', list_sink)
+    result = await cli.execute_cli_command('search is (foo) and id=="4" sort some_int | list', list_sink)
     assert len(result[0]) == 1
-    assert result[0][0].startswith("kind=foo, identifier=4, some_int=0, age=")
+    assert result[0][0].startswith("kind=foo, id=4, some_int=0, age=")
     list_cmd = "list some_int as si, some_string"
-    result = await cli.execute_cli_command(f'search is (foo) and identifier=="4" | {list_cmd}', list_sink)
+    result = await cli.execute_cli_command(f'search is (foo) and id=="4" | {list_cmd}', list_sink)
     assert result[0] == ["si=0, some_string=hello"]
 
     # list is added automatically when no output renderer is defined and has the same behaviour as if it was given
-    result = await cli.execute_cli_command('search is (foo) and identifier=="4" sort some_int', list_sink)
-    assert result[0][0].startswith("kind=foo, identifier=4, some_int=0, age=")
+    result = await cli.execute_cli_command('search is (foo) and id=="4" sort some_int', list_sink)
+    assert result[0][0].startswith("kind=foo, id=4, some_int=0, age=")
 
     # List is using the correct type
     props = dict(id="test", a="a", b=True, c=False, d=None, e=12, f=1.234, reported={})
     result = await cli.execute_cli_command(f"json {json.dumps(props)} | list a,b,c,d,e,f", list_sink)
     assert result[0] == ["a=a, b=true, c=false, e=12, f=1.234"]
 
     # Queries that use the reported section, also interpret the list format in the reported section
@@ -960,15 +958,15 @@
         "payload": {
             "summary": "test",
             "timestamp": "2023-02-10T15:03:33Z",
             "source": "Fix",
             "severity": "warning",
             "component": "Fix",
             "custom_details": {
-                "collector": {"sub_root": {"no-region": {"0_0": {"id": None, "name": "yes or no", "kind": "bla"}}}}
+                "collector": {"sub_root": {"no-region": {"0_0": {"id": "0_0", "name": "yes or no", "kind": "bla"}}}}
             },
         },
         "routing_key": "123",
         "dedup_key": "234",
         "images": [
             {
                 "src": "https://cdn.some.engineering/assets/fix-illustrations/small/fix-alert.png",
@@ -1431,30 +1429,30 @@
 
     tsdb = cli.dependencies.db_access.time_series_db
     await tsdb.wipe()  # create a clean slate
     now = utc()
     in_one_min = utc_str(now + timedelta(minutes=1))
     one_min_ago = utc_str(now - timedelta(minutes=1))
     # Create a time series based on all foo entries
-    res = await exec("timeseries snapshot --name test 'search aggregate(reported.some_int, reported.identifier: sum(1)): is(foo)'")  # fmt: skip
+    res = await exec("timeseries snapshot --name test 'search aggregate(reported.some_int, reported.id: sum(1)): is(foo)'")  # fmt: skip
     assert res[0] == "10 entries added to time series test."
     # Get the time series combined with each complete group
     res = await exec(f"timeseries get --name test --start {one_min_ago} --end {in_one_min}")
     assert len(res) == 10
     # Get the time series combined over all groups --> only one entry for one timestamp
     res = await exec(f"timeseries get --name test --start {one_min_ago} --end {in_one_min} --group")
     assert len(res) == 1
     # Combine over some_int (which has only one) --> only one entry for one timestamp
     res = await exec(f"timeseries get --name test --start {one_min_ago} --end {in_one_min} --group some_int")
     assert len(res) == 1
-    # Combine over identifier (which is unique for each entry) --> 10 entries for one timestamp
-    res = await exec(f"timeseries get --name test --start {one_min_ago} --end {in_one_min} --group identifier")
+    # Combine over id (which is unique for each entry) --> 10 entries for one timestamp
+    res = await exec(f"timeseries get --name test --start {one_min_ago} --end {in_one_min} --group id")
     assert len(res) == 10
-    # Combine over identifier (which is unique for each entry), filter for identifier==2 --> 1 entry for one timestamp
-    res = await exec(f'timeseries get --name test --start {one_min_ago} --end {in_one_min} --group identifier --filter identifier=="2"')  # fmt: skip
+    # Combine over id (which is unique for each entry), filter for id==2 --> 1 entry for one timestamp
+    res = await exec(f'timeseries get --name test --start {one_min_ago} --end {in_one_min} --group id --filter id=="2"')  # fmt: skip
     assert len(res) == 1
 
 
 @pytest.mark.asyncio
 async def test_refine_resource_data(cli: CLI) -> None:
     from fixcore.cli import command
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/cli/model_test.py` & `fixinventorycore-4.0.3/tests/fixcore/cli/model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/config/config_handler_service_test.py` & `fixinventorycore-4.0.3/tests/fixcore/config/config_handler_service_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/config/config_override_service_test.py` & `fixinventorycore-4.0.3/tests/fixcore/config/config_override_service_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/config/core_config_handler_test.py` & `fixinventorycore-4.0.3/tests/fixcore/config/core_config_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/conftest.py` & `fixinventorycore-4.0.3/tests/fixcore/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -259,15 +259,15 @@
 
 @fixture
 def foo_kinds() -> List[Kind]:
     base = ComplexKind(
         "base",
         [],
         [
-            Property("identifier", "string", required=True),
+            Property("id", "string", required=True),
             Property("kind", "string", required=True),
             Property("ctime", "datetime"),
         ],
         aggregate_root=False,
     )
     foo = ComplexKind(
         "foo",
@@ -324,15 +324,15 @@
 @fixture
 def person_model() -> Model:
     zip = StringKind("zip")
     base = ComplexKind(
         "Base",
         [],
         [
-            Property("id", "string", required=True, description="Some identifier"),
+            Property("id", "string", required=True, description="Some id"),
             Property("kind", "string", required=True, description="Kind of this node."),
             Property("list", "string[]", description="A list of strings."),
             Property("tags", "dictionary[string, string]", description="Key/value pairs."),
             Property("mtime", "datetime", description="Modification time of this node."),
         ],
         metadata={"icon": "icon.svg"},
     )
@@ -588,15 +588,15 @@
 @fixture
 def benchmark() -> Benchmark:
     return Benchmark(
         id="test",
         framework="test",
         documentation="test",
         version="1.5",
-        clouds=["test"],
+        clouds=["collector"],
         title="test_benchmark",
         description="test_benchmark",
         checks=[],
         children=[
             CheckCollection(
                 title="Section 1",
                 description="Some description",
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/console_renderer_test.py` & `fixinventorycore-4.0.3/tests/fixcore/console_renderer_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/core_config_test.py` & `fixinventorycore-4.0.3/tests/fixcore/core_config_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/arango_query_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/arango_query_test.py`

 * *Files 4% similar despite different names*

```diff
@@ -316,47 +316,55 @@
 
 def test_load_time_series() -> None:
     now = datetime.fromtimestamp(1700000000)
     one_hour = timedelta(hours=1)
     # group_by=[] --> no group by any value
     q, bv = load_time_series("ts", "foo", now - (24 * one_hour), now, one_hour, group_by=[])
     assert (
-        q == "FOR d in `ts` FILTER d.ts==@b0 AND d.at>=@b1 AND d.at<@b2 "
+        q == "LET m1 = ( FOR d in `ts` FILTER d.ts==@b0 AND d.at>=@b1 AND d.at<@b2 "
         "LET m0 = (FLOOR(d.at / @b3) * @b3) + @b4 "
-        "COLLECT group_slot=m0 INTO group "
-        "SORT group_slot "
-        "RETURN {at: group_slot,  v: AVG(group[*].d.v)}"
+        "COLLECT group_slot=m0, complete_group=d.group "
+        "AGGREGATE slot_avg = AVG(d.v) "
+        "RETURN {at: group_slot, group: complete_group, v: slot_avg} )\n "
+        "FOR d in m1 COLLECT group_slot=d.at AGGREGATE agg_val=avg(d.v) "
+        "SORT group_slot RETURN {at: group_slot, v: agg_val}"
     )
     assert bv == {"b0": "foo", "b1": 1699913600, "b2": 1700000000, "b3": 3600, "b4": 800}
     # no group by defined --> group by all values
     q, bv = load_time_series("ts", "foo", now - (24 * one_hour), now, one_hour)
     assert (
         q == "FOR d in `ts` FILTER d.ts==@b0 AND d.at>=@b1 AND d.at<@b2 "
         "LET m0 = (FLOOR(d.at / @b3) * @b3) + @b4 "
-        "COLLECT group_slot=m0, complete_group=d.group INTO group "
-        "SORT group_slot "
-        "RETURN {at: group_slot, group: complete_group, v: AVG(group[*].d.v)}"
+        "COLLECT group_slot=m0, complete_group=d.group "
+        "AGGREGATE slot_avg = AVG(d.v) "
+        "RETURN {at: group_slot, group: complete_group, v: slot_avg}"
     )
     assert bv == {"b0": "foo", "b1": 1699913600, "b2": 1700000000, "b3": 3600, "b4": 800}
     # group by specific group variables
     q, bv = load_time_series("ts", "foo", now - (24 * one_hour), now, one_hour, group_by=["a", "b"])
     assert (
-        q == "FOR d in `ts` FILTER d.ts==@b0 AND d.at>=@b1 AND d.at<@b2 "
+        q == "LET m1 = ( FOR d in `ts` FILTER d.ts==@b0 AND d.at>=@b1 AND d.at<@b2 "
         "LET m0 = (FLOOR(d.at / @b3) * @b3) + @b4 "
-        "COLLECT group_slot=m0, group_a=d.group.a, group_b=d.group.b INTO group "
-        "SORT group_slot "
-        "RETURN {at: group_slot, group: { a: group_a, b: group_b }, v: AVG(group[*].d.v)}"
+        "COLLECT group_slot=m0, complete_group=d.group "
+        "AGGREGATE slot_avg = AVG(d.v) "
+        "RETURN {at: group_slot, group: complete_group, v: slot_avg} )\n "
+        "FOR d in m1 "
+        "COLLECT group_slot=d.at, group_a=d.group.a, group_b=d.group.b "
+        "AGGREGATE agg_val=avg(d.v) "
+        "SORT group_slot RETURN {at: group_slot,group: { a: group_a, b: group_b }, v: agg_val}"
     )
     assert bv == {"b0": "foo", "b1": 1699913600, "b2": 1700000000, "b3": 3600, "b4": 800}
     # group by specific group variables and filter by group variables
     q, bv = load_time_series(
         "ts", "foo", now - (24 * one_hour), now, one_hour, group_by=["a", "b"], group_filter=[P("a").eq("a")]
     )
     assert (
-        q == "FOR d in `ts` FILTER d.ts==@b0 AND d.at>=@b1 AND d.at<@b2 "
-        "FILTER d.group.a==@b3 "
+        q == "LET m1 = ( FOR d in `ts` FILTER d.ts==@b0 AND d.at>=@b1 AND d.at<@b2 FILTER d.group.a==@b3 "
         "LET m0 = (FLOOR(d.at / @b4) * @b4) + @b5 "
-        "COLLECT group_slot=m0, group_a=d.group.a, group_b=d.group.b INTO group "
-        "SORT group_slot "
-        "RETURN {at: group_slot, group: { a: group_a, b: group_b }, v: AVG(group[*].d.v)}"
+        "COLLECT group_slot=m0, complete_group=d.group "
+        "AGGREGATE slot_avg = AVG(d.v) RETURN {at: group_slot, group: complete_group, v: slot_avg} )\n "
+        "FOR d in m1 "
+        "COLLECT group_slot=d.at, group_a=d.group.a, group_b=d.group.b "
+        "AGGREGATE agg_val=avg(d.v) "
+        "SORT group_slot RETURN {at: group_slot,group: { a: group_a, b: group_b }, v: agg_val}"
     )
     assert bv == {"b0": "foo", "b1": 1699913600, "b2": 1700000000, "b3": "a", "b4": 3600, "b5": 800}
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/arangodb_functions_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/arangodb_functions_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/async_arangodb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/async_arangodb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/configdb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/configdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/db_access_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/db_access_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/deferredouteredgedb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/deferredouteredgedb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/entitydb.py` & `fixinventorycore-4.0.3/tests/fixcore/db/entitydb.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/graphdb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/graphdb_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,26 +27,26 @@
 from fixcore.util import AccessJson, utc, value_in_path, AccessNone
 from tests.fixcore.utils import eventually
 
 
 class BaseResource(ABC):
     def __init__(
         self,
-        identifier: str,
+        id: str,
     ) -> None:
-        self.identifier = str(identifier)
+        self.id = str(id)
 
     @abstractmethod
     def kind(self) -> str:
         pass
 
 
 @define
 class Foo(BaseResource):
-    identifier: str
+    id: str
     name: Optional[str] = None
     some_int: int = 0
     some_string: str = "hello"
     now_is: datetime = utc()
     ctime: Optional[datetime] = None
 
     def kind(self) -> str:
@@ -57,15 +57,15 @@
 class Inner:
     name: str
     inner: List["Inner"]
 
 
 @define
 class Bla(BaseResource):
-    identifier: str
+    id: str
     name: Optional[str] = None
     now: date = date.today()
     f: int = 23
     g: Optional[List[int]] = None
     h: Optional[Inner] = None
 
     def __attrs_post_init__(self) -> None:
@@ -216,15 +216,15 @@
                         add_edge(parent, child)
                         add_edge(child, parent, EdgeTypes.delete)
 
     return graph
 
 
 async def load_graph(db: GraphDB, model: Model) -> MultiDiGraph:
-    blas = Query.by(P("identifier") == "sub_root").traverse_out(0, Navigation.Max)  # noqa
+    blas = Query.by(P("id") == "sub_root").traverse_out(0, Navigation.Max)  # noqa
     return await db.search_graph(QueryModel(blas.on_section("reported"), model))
 
 
 @mark.asyncio
 async def test_update_merge_batched(graph_db: ArangoGraphDB, foo_model: Model, test_db: StandardDatabase) -> None:
     md = foo_model
     await graph_db.wipe()
@@ -395,15 +395,15 @@
         await db.mark_update(["sub_root"], ["root"], "update under node sub_root", False)
     # clean up for later tests
     await db.db.truncate(db.in_progress)
 
 
 @mark.asyncio
 async def test_query_list(filled_graph_db: ArangoGraphDB, foo_model: Model) -> None:
-    blas = Query.by("foo", P("identifier") == "9").traverse_out().filter("bla", P("f") == 23)  # noqa
+    blas = Query.by("foo", P("id") == "9").traverse_out().filter("bla", P("f") == 23)  # noqa
     async with await filled_graph_db.search_list(QueryModel(blas.on_section("reported"), foo_model)) as gen:
         result = [from_js(x["reported"], Bla) async for x in gen]
         assert len(result) == 10
 
     foos_or_blas = parse_query("is([foo, bla])")
     async with await filled_graph_db.search_list(QueryModel(foos_or_blas.on_section("reported"), foo_model)) as gen:
         result = [x async for x in gen]
@@ -437,15 +437,15 @@
 @mark.asyncio
 async def test_query_graph(filled_graph_db: ArangoGraphDB, foo_model: Model) -> None:
     graph = await load_graph(filled_graph_db, foo_model)
     assert len(graph.edges) == 110
     assert len(graph.nodes.values()) == 111
 
     # filter data and tag result, and then traverse to the end of the graph in both directions
-    around_me = Query.by("foo", P("identifier") == "9").tag("red").traverse_inout(start=0)  # noqa
+    around_me = Query.by("foo", P("id") == "9").tag("red").traverse_inout(start=0)  # noqa
     graph = await filled_graph_db.search_graph(QueryModel(around_me.on_section("reported"), foo_model))
     assert len({x for x in graph.nodes}) == 12
     assert GraphAccess.root_id(graph) == "sub_root"
     assert list(graph.successors("sub_root"))[0] == "9"
     assert set(graph.successors("9")) == {f"9_{x}" for x in range(0, 10)}
     for from_node, to_node, data in graph.edges.data(True):
         assert from_node == "9" or to_node == "9"
@@ -461,22 +461,22 @@
 
     async def assert_result(query: str, nodes: int, edges: int) -> None:
         q = parse_query(query)
         graph = await filled_graph_db.search_graph(QueryModel(q, foo_model))
         assert len(graph.nodes) == nodes
         assert len(graph.edges) == edges
 
-    await assert_result("is(foo) and reported.identifier==9 <-delete[0:]default->", 11, 20)
-    await assert_result("is(foo) and reported.identifier==9 <-default[0:]delete->", 4, 3)
-    await assert_result("is(foo) and reported.identifier==9 <-default[0:]->", 14, 13)
-    await assert_result("is(foo) and reported.identifier==9 <-delete[0:]->", 11, 10)
-    await assert_result("is(foo) and reported.identifier==9 -default[0:]->", 11, 10)
-    await assert_result("is(foo) and reported.identifier==9 <-delete[0:]-", 11, 10)
-    await assert_result("is(foo) and reported.identifier==9 <-default[0:]-", 4, 3)
-    await assert_result("is(foo) and reported.identifier==9 -delete[0:]->", 1, 0)
+    await assert_result("is(foo) and reported.id==9 <-delete[0:]default->", 11, 20)
+    await assert_result("is(foo) and reported.id==9 <-default[0:]delete->", 4, 3)
+    await assert_result("is(foo) and reported.id==9 <-default[0:]->", 14, 13)
+    await assert_result("is(foo) and reported.id==9 <-delete[0:]->", 11, 10)
+    await assert_result("is(foo) and reported.id==9 -default[0:]->", 11, 10)
+    await assert_result("is(foo) and reported.id==9 <-delete[0:]-", 11, 10)
+    await assert_result("is(foo) and reported.id==9 <-default[0:]-", 4, 3)
+    await assert_result("is(foo) and reported.id==9 -delete[0:]->", 1, 0)
 
 
 @mark.asyncio
 async def test_query_nested(filled_graph_db: ArangoGraphDB, foo_model: Model) -> None:
     async def assert_count(query: str, count: int, total_count: Optional[int] = None) -> None:
         q = parse_query(query).on_section("reported")
         async with await filled_graph_db.search_list(QueryModel(q, foo_model), with_count=True) as gen:
@@ -496,20 +496,20 @@
     await assert_count("is(bla) and g[*] none = 2", 0)
     await assert_count("is(bla) limit 1", 1, 100)
     await assert_count("is(bla) limit 10, 10", 10, 100)
 
 
 @mark.asyncio
 async def test_query_aggregate(filled_graph_db: ArangoGraphDB, foo_model: Model) -> None:
-    agg_query = parse_query("aggregate(kind: count(identifier) as instances): is(foo)").on_section("reported")
+    agg_query = parse_query("aggregate(kind: count(id) as instances): is(foo)").on_section("reported")
     async with await filled_graph_db.search_aggregation(QueryModel(agg_query, foo_model)) as gen:
         assert [x async for x in gen] == [{"group": {"kind": "foo"}, "instances": 10}]
 
     agg_combined_var_query = parse_query(
-        'aggregate("test_{kind}_{some_int}_{does_not_exist}" as kind: count(identifier) as instances): is("foo")'
+        'aggregate("test_{kind}_{some_int}_{does_not_exist}" as kind: count(id) as instances): is("foo")'
     ).on_section("reported")
 
     async with await filled_graph_db.search_aggregation(QueryModel(agg_combined_var_query, foo_model)) as g:
         assert [x async for x in g] == [{"group": {"kind": "test_foo_0_"}, "instances": 10}]
 
     agg_multi_fn_same_prop = parse_query('aggregate(sum(f) as a, max(f) as b): is("bla")').on_section("reported")
     async with await filled_graph_db.search_aggregation(QueryModel(agg_multi_fn_same_prop, foo_model)) as g:
@@ -556,20 +556,20 @@
 async def test_query_with_clause(filled_graph_db: ArangoGraphDB, foo_model: Model) -> None:
     async def query(q: str) -> List[Json]:
         agg_query = parse_query(q)
         async with await filled_graph_db.search_list(QueryModel(agg_query.on_section("reported"), foo_model)) as cursor:
             return [bla async for bla in cursor]
 
     assert len(await query("is(bla) with(any, <-- is(foo))")) == 100
-    assert len(await query('is(bla) with(any, <-- is(foo) and identifier=~"1")')) == 10
+    assert len(await query('is(bla) with(any, <-- is(foo) and id=~"1")')) == 10
     assert len(await query("is(bla) with(empty, <-- is(foo))")) == 0
     assert len(await query("is(bla) with(any, <-- is(bla))")) == 0
     assert len(await query("is(bla) with(empty, <-- is(bla))")) == 100
-    assert len(await query('is(bla) with(count==1, <-- is(foo) and identifier=~"1")')) == 10
-    assert len(await query('is(bla) with(count==2, <-- is(foo) and identifier=~"1")')) == 0
+    assert len(await query('is(bla) with(count==1, <-- is(foo) and id=~"1")')) == 10
+    assert len(await query('is(bla) with(count==2, <-- is(foo) and id=~"1")')) == 0
     assert len(await query("is(bla) with(any, <-- with(any, <-- is(foo)))")) == 100
 
 
 @mark.asyncio
 async def test_no_null_if_undefined(graph_db: ArangoGraphDB, foo_model: Model) -> None:
     await graph_db.wipe()
     # imported graph should not have any desired or metadata sections
@@ -610,30 +610,30 @@
 
 @mark.asyncio
 async def test_insert_node(graph_db: ArangoGraphDB, foo_model: Model) -> None:
     await graph_db.wipe()
     json = await graph_db.create_node(
         foo_model, NodeId("some_new_id"), to_json(Foo("some_new_id", "name")), NodeId("root")
     )
-    assert to_foo(json).identifier == "some_new_id"
-    assert to_foo(await graph_db.get_node(foo_model, NodeId("some_new_id"))).identifier == "some_new_id"
+    assert to_foo(json).id == "some_new_id"
+    assert to_foo(await graph_db.get_node(foo_model, NodeId("some_new_id"))).id == "some_new_id"
 
 
 @mark.asyncio
 async def test_update_node(filled_graph_db: ArangoGraphDB, foo_model: Model) -> None:
     nid = NodeId("0")
     # patch
     js = await filled_graph_db.update_node(foo_model, nid, {"name": "bla"}, False, "reported")
     assert to_foo(js).name == "bla"
     assert to_foo(await filled_graph_db.get_node(foo_model, nid)).name == "bla"
     # replace
-    js = await filled_graph_db.update_node(foo_model, nid, {"kind": "bla", "identifier": "123"}, True, "reported")
+    js = await filled_graph_db.update_node(foo_model, nid, {"kind": "bla", "id": "123"}, True, "reported")
     reported = js["reported"]
     reported.pop("ctime")  # ctime is added by the system automatically. remove it
-    assert reported == {"kind": "bla", "identifier": "123"}
+    assert reported == {"kind": "bla", "id": "123"}
     # also make sure that all resolved ancestor props are changed
     nid = NodeId("sub_root")
     # patch
     js = await filled_graph_db.update_node(foo_model, nid, {"name": "bat"}, False, "reported")
     assert js["reported"]["name"] == "bat"
 
     async def elements(history: bool) -> List[Json]:
@@ -794,15 +794,15 @@
 @mark.asyncio
 async def test_list_possible_values(filled_graph_db: ArangoGraphDB, foo_model: Model) -> None:
     async def pv(q: str, path_or_pred: Union[str, Predicate], detail: Literal["attributes", "values"]) -> List[Any]:
         qm = QueryModel(parse_query(q), foo_model)
         async with await filled_graph_db.list_possible_values(qm, path_or_pred, detail) as cursor:
             return [a async for a in cursor]
 
-    props_of_b = ["ctime", "f", "g", "h", "identifier", "kind", "name", "now"]
+    props_of_b = ["ctime", "f", "g", "h", "id", "kind", "name", "now"]
     assert await pv("is(bla)", "reported.f", "values") == [23]
     assert await pv("is(bla)", "reported.h.inner[*].inner[*].name", "values") == ["in_0_0", "in_0_1"]
     assert await pv("is(bla)", "reported.g[*]", "values") == [0, 1, 2, 3, 4]
     assert await pv("is(bla)", "reported", "attributes") == props_of_b
     assert await pv("is(bla)", predicate_term.parse('reported=~"^[fgh]"'), "attributes") == ["f", "g", "h"]
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/jobdb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/jobdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/model_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/modeldb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/modeldb_test.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     string_kind = StringKind("some.string", 0, 3, "\\w+")
     int_kind = NumberKind("some.int", "int32", 0, 100)
     bool_kind = BooleanKind("some.bool")
     base = ComplexKind(
         "base",
         [],
         [
-            Property("identifier", "string", required=True),
+            Property("id", "string", required=True),
             Property("kind", "string", required=True),
         ],
     )
     foo = ComplexKind(
         "foo",
         ["base"],
         [
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/reportdb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/reportdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/runningtaskdb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/runningtaskdb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/system_data_db_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/system_data_db_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/templatedb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/templatedb_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/db/timeseriesdb_test.py` & `fixinventorycore-4.0.3/tests/fixcore/db/timeseriesdb_test.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from fixcore.query.model import P
 from fixcore.query.query_parser import parse_query
 from fixcore.types import Json
 
 
 async def test_create_time_series(timeseries_db: TimeSeriesDB, foo_model: Model, filled_graph_db: GraphDB) -> None:
     await timeseries_db.wipe()  # clean up
-    qm = QueryModel(parse_query("aggregate(reported.some_int, reported.identifier: sum(1)): is(foo)"), foo_model)
+    qm = QueryModel(parse_query("aggregate(reported.some_int, reported.id: sum(1)): is(foo)"), foo_model)
     # create timeseries at 10 different points in time
     for a in range(10):
         await timeseries_db.add_entries("test", qm, filled_graph_db, at=3600 * a)
     begin = datetime.fromtimestamp(0)
     after5h = datetime.fromtimestamp(3600 * 5 - 1)
 
     async def load_ts(**kwargs: Any) -> List[Json]:
@@ -37,27 +37,27 @@
     assert len(await load_ts(name="test", start=begin, end=after5h, granularity=timedelta(hours=2))) == 30
     # first 5 hours with 10 entries each: granularity 5 hours: at 0: 10 entries
     assert len(await load_ts(name="test", start=begin, end=after5h, granularity=timedelta(hours=5))) == 10
 
     ## check group_by is working
     # some_int is the same for all entries: one every hour: 5 entries
     assert len(await load_ts(name="test", start=begin, end=after5h, group_by=["some_int"])) == 5
-    # identifier is different for each entry: 50 entries
-    assert len(await load_ts(name="test", start=begin, end=after5h, group_by=["identifier"])) == 50
+    # id is different for each entry: 50 entries
+    assert len(await load_ts(name="test", start=begin, end=after5h, group_by=["id"])) == 50
     # do not use any groups: 5 entries
     assert len(await load_ts(name="test", start=begin, end=after5h, group_by=[])) == 5
 
     ## check filter_by is working
     # some_int is the same for all entries: one every hour: 5 entries
-    assert len(await load_ts(name="test", start=begin, end=after5h, filter_by=[(P("identifier").eq("1"))])) == 5
+    assert len(await load_ts(name="test", start=begin, end=after5h, filter_by=[(P("id").eq("1"))])) == 5
 
 
 async def test_compact_time_series(timeseries_db: TimeSeriesDB, foo_model: Model, filled_graph_db: GraphDB) -> None:
     await timeseries_db.wipe()  # clean up
-    qm = QueryModel(parse_query("aggregate(reported.some_int, reported.identifier: sum(1)): is(foo)"), foo_model)
+    qm = QueryModel(parse_query("aggregate(reported.some_int, reported.id: sum(1)): is(foo)"), foo_model)
     now = datetime(2023, 12, 1, tzinfo=timezone.utc)
 
     async def create_ts(before_now: timedelta, granularity: timedelta, number_of_entries: int) -> None:
         start = now - before_now
         for a in range(number_of_entries):
             await timeseries_db.add_entries("test", qm, filled_graph_db, at=int((start - a * granularity).timestamp()))
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/dependencies_test.py` & `fixinventorycore-4.0.3/tests/fixcore/dependencies_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/graph_manager/graph_manager_test.py` & `fixinventorycore-4.0.3/tests/fixcore/graph_manager/graph_manager_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/hypothesis_extension.py` & `fixinventorycore-4.0.3/tests/fixcore/hypothesis_extension.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/infra_apps/local_runtime_test.py` & `fixinventorycore-4.0.3/tests/fixcore/infra_apps/local_runtime_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/infra_apps/package_manager_test.py` & `fixinventorycore-4.0.3/tests/fixcore/infra_apps/package_manager_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/message_bus_test.py` & `fixinventorycore-4.0.3/tests/fixcore/message_bus_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/__init__.py` & `fixinventorycore-4.0.3/tests/fixcore/model/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/adjust_node_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/adjust_node_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/db_updater_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/db_updater_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/exportable_model_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/exportable_model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/graph_access_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/graph_access_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/json_schema_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/json_schema_test.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,20 +4,20 @@
 
 def test_schema(foo_model: Model) -> None:
     schema = json_schema(foo_model)
     # The resource is one of the possible 8 types
     assert len(schema["oneOf"]) == 8
 
     # base type - all properties are defined, additional properties are allowed
-    assert schema["$defs"]["base"]["required"] == ["identifier", "kind"]
-    assert schema["$defs"]["base"]["properties"].keys() == {"identifier", "kind", "ctime"}
+    assert schema["$defs"]["base"]["required"] == ["id", "kind"]
+    assert schema["$defs"]["base"]["properties"].keys() == {"id", "kind", "ctime"}
     assert schema["$defs"]["base"]["additionalProperties"] is True
 
     # final resource type - all properties are defined, additional properties are not allowed
     assert schema["$defs"]["some_complex"]["required"] == []
-    expected = {"identifier", "kind", "ctime", "cloud", "account", "parents", "children", "nested"}
+    expected = {"id", "kind", "ctime", "cloud", "account", "parents", "children", "nested"}
     assert schema["$defs"]["some_complex"]["properties"].keys() == expected
     assert schema["$defs"]["some_complex"]["additionalProperties"] is False
 
     # simple types are defined
     assert schema["$defs"]["datetime"]["type"] == "string"
     assert schema["$defs"]["datetime"]["format"] == "date-time"
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/model_handler_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/model_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/model_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/model_test.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,15 @@
         "properties": [
           { "name": "tags", "kind": "dictionary[string, string]", "description": "Tags that describe the resource.", "required": false }
         ]
       },
       { "fqn" :  "test.BaseResource",
         "bases": ["test.Compound", "test.Base"],
         "properties": [
-          { "name": "id", "kind": "string", "description": "The identifier of this resource", "required": true },
+          { "name": "id", "kind": "string", "description": "The id of this resource", "required": true },
           { "name": "name", "kind": "string", "description": "The name of the resource.", "required": true }
         ]
       },
       { "fqn" :  "test.EC2",
         "bases": ["test.BaseResource"],
         "allow_unknown_props": true,
         "properties": [
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/model/typed_model_test.py` & `fixinventorycore-4.0.3/tests/fixcore/model/typed_model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/query/__init__.py` & `fixinventorycore-4.0.3/tests/fixcore/query/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/query/model_test.py` & `fixinventorycore-4.0.3/tests/fixcore/query/model_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/query/query_parser_test.py` & `fixinventorycore-4.0.3/tests/fixcore/query/query_parser_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/query/template_expander_test.py` & `fixinventorycore-4.0.3/tests/fixcore/query/template_expander_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/report/benchmark_renderer_test.py` & `fixinventorycore-4.0.3/tests/fixcore/report/benchmark_renderer_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/report/inspector_service_test.py` & `fixinventorycore-4.0.3/tests/fixcore/report/inspector_service_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,15 @@
     db = inspector_service.db_access.get_graph_db(graph_name)
     model = await inspector_service.model_handler.load_model(graph_name)
     all_vunerable = Query.by(P("security.has_issues") == True)  # noqa
     async with await db.search_list(QueryModel(all_vunerable, model), with_count=True) as cursor:
         return cursor.count()  # type: ignore
 
 
-async def test_perform_benchmark(inspector_service: InspectorService) -> None:
+async def test_perform_benchmark(inspector_service: InspectorService, foo_model: Model) -> None:
     def assert_result(results: Dict[str, BenchmarkResult]) -> None:
         result = results["test"]
         assert result.children[0].checks[0].number_of_resources_failing == 10
         assert result.children[1].checks[0].number_of_resources_failing == 10
         filtered = result.filter_result(filter_failed=True)
         assert filtered.children[0].checks[0].number_of_resources_failing == 10
         assert len(filtered.children[0].checks[0].resources_failing_by_account["sub_root"]) == 10
@@ -97,14 +97,21 @@
 
     assert await count_vulnerable(inspector_service) == 10
 
     # loading the result from the db should give the same information
     loaded = await inspector_service.load_benchmarks(graph_name, ["test"])
     assert_result(loaded)
 
+    # a score is maintained on the account node
+    db = inspector_service.db_access.get_graph_db(graph_name)
+    async with await db.search_list(QueryModel(Query.by("account"), foo_model)) as crsr:
+        async for elem in crsr:
+            assert elem["metadata"]["score"] == 0
+            assert elem["metadata"]["benchmark"]["test"] == 0
+
 
 async def test_perform_benchmark_ignored(
     inspector_service: InspectorService, foo_model: Model, inspection_checks: List[ReportCheck]
 ) -> None:
     check_ids = [c.id for c in inspection_checks]
     first_half = [NodeId(str(a)) for a in range(5)]
     graph_name = GraphName(inspector_service.cli.env["graph"])
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/task/job_handler_test.py` & `fixinventorycore-4.0.3/tests/fixcore/task/job_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/task/start_workflow_on_first_subscriber_test.py` & `fixinventorycore-4.0.3/tests/fixcore/task/start_workflow_on_first_subscriber_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/task/subscribers_test.py` & `fixinventorycore-4.0.3/tests/fixcore/task/subscribers_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/task/task_description_test.py` & `fixinventorycore-4.0.3/tests/fixcore/task/task_description_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/task/task_handler_test.py` & `fixinventorycore-4.0.3/tests/fixcore/task/task_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/user/user_management_service_test.py` & `fixinventorycore-4.0.3/tests/fixcore/user/user_management_service_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/util_test.py` & `fixinventorycore-4.0.3/tests/fixcore/util_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/utils.py` & `fixinventorycore-4.0.3/tests/fixcore/utils.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/validator_test.py` & `fixinventorycore-4.0.3/tests/fixcore/validator_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/web/api_client.py` & `fixinventorycore-4.0.3/tests/fixcore/web/api_client.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/web/api_test.py` & `fixinventorycore-4.0.3/tests/fixcore/web/api_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,17 +200,15 @@
 
     # wipe the data in the graph
     assert await core_client.delete_graph(g, truncate=True) == "Graph truncated."
     assert g in await core_client.list_graphs()
 
     # create a node in the graph
     uid = rnd_str()
-    node = AccessJson(
-        await core_client.create_node("root", uid, {"identifier": uid, "kind": "child", "name": "max"}, g)
-    )
+    node = AccessJson(await core_client.create_node("root", uid, {"id": uid, "kind": "child", "name": "max"}, g))
     assert node.id == uid
     assert node.reported.name == "max"
 
     # update a node in the graph
     node = AccessJson(await core_client.patch_node(uid, {"name": "moritz"}, "reported", g))
     assert node.id == uid
     assert node.reported.name == "moritz"
```

### Comparing `fixinventorycore-4.0.2/tests/fixcore/web/auth_test.py` & `fixinventorycore-4.0.3/tests/fixcore/web/auth_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/web/certificate_handler_test.py` & `fixinventorycore-4.0.3/tests/fixcore/web/certificate_handler_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/web/content_renderer_test.py` & `fixinventorycore-4.0.3/tests/fixcore/web/content_renderer_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/web/permission_test.py` & `fixinventorycore-4.0.3/tests/fixcore/web/permission_test.py`

 * *Files identical despite different names*

### Comparing `fixinventorycore-4.0.2/tests/fixcore/worker_task_queue_test.py` & `fixinventorycore-4.0.3/tests/fixcore/worker_task_queue_test.py`

 * *Files identical despite different names*

