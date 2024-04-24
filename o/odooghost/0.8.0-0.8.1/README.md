# Comparing `tmp/odooghost-0.8.0.tar.gz` & `tmp/odooghost-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "odooghost-0.8.0.tar", max compression
+gzip compressed data, was "odooghost-0.8.1.tar", max compression
```

## Comparing `odooghost-0.8.0.tar` & `odooghost-0.8.1.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1069 2024-04-24 16:07:35.736037 odooghost-0.8.0/LICENSE
--rw-r--r--   0        0        0     1967 2024-04-24 16:07:35.736037 odooghost-0.8.0/README.md
--rw-r--r--   0        0        0      369 2024-04-24 16:08:18.695946 odooghost-0.8.0/odooghost/__init__.py
--rw-r--r--   0        0        0       94 2024-04-24 16:07:35.736037 odooghost-0.8.0/odooghost/__main__.py
--rw-r--r--   0        0        0      127 2024-04-24 16:07:35.736037 odooghost-0.8.0/odooghost/cli/__init__.py
--rw-r--r--   0        0        0      451 2024-04-24 16:07:35.736037 odooghost-0.8.0/odooghost/cli/config.py
--rw-r--r--   0        0        0     1861 2024-04-24 16:07:35.736037 odooghost-0.8.0/odooghost/cli/root.py
--rw-r--r--   0        0        0       42 2024-04-24 16:07:35.736037 odooghost-0.8.0/odooghost/cli/stack/__init__.py
--rw-r--r--   0        0        0      959 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/cli/stack/config.py
--rw-r--r--   0        0        0     9765 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/cli/stack/data.py
--rw-r--r--   0        0        0    13037 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/cli/stack/root.py
--rw-r--r--   0        0        0      271 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/config/__init__.py
--rw-r--r--   0        0        0     4440 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/config/addons.py
--rw-r--r--   0        0        0      267 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/config/app.py
--rw-r--r--   0        0        0     2445 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/config/dependency.py
--rw-r--r--   0        0        0     2082 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/config/service.py
--rw-r--r--   0        0        0     2854 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/config/stack.py
--rw-r--r--   0        0        0      789 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/constant.py
--rw-r--r--   0        0        0     9501 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/container.py
--rw-r--r--   0        0        0     7516 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/context.py
--rw-r--r--   0        0        0     1139 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/exceptions.py
--rw-r--r--   0        0        0      585 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/filters.py
--rw-r--r--   0        0        0     3702 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/git.py
--rw-r--r--   0        0        0     1111 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/logger.py
--rw-r--r--   0        0        0      466 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/renderer.py
--rw-r--r--   0        0        0       63 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/services/__init__.py
--rw-r--r--   0        0        0    14691 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/services/base.py
--rw-r--r--   0        0        0     3972 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/services/db.py
--rw-r--r--   0        0        0      102 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/services/odoo/__init__.py
--rw-r--r--   0        0        0     3756 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/services/odoo/addons.py
--rw-r--r--   0        0        0     4838 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/services/odoo/service.py
--rw-r--r--   0        0        0    10382 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/stack.py
--rw-r--r--   0        0        0     1710 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/templates/Dockerfile.j2
--rw-r--r--   0        0        0      580 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/types.py
--rw-r--r--   0        0        0       93 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/__init__.py
--rw-r--r--   0        0        0      790 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/autocomplete.py
--rw-r--r--   0        0        0      993 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/exec.py
--rw-r--r--   0        0        0     2159 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/misc.py
--rw-r--r--   0        0        0     3914 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/progress_stream.py
--rw-r--r--   0        0        0      884 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/signals.py
--rw-r--r--   0        0        0     2567 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/stream.py
--rw-r--r--   0        0        0     1516 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/utils/sync_to_async.py
--rw-r--r--   0        0        0        0 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/api/query/__init__.py
--rw-r--r--   0        0        0      305 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/api/query/dashboard.py
--rw-r--r--   0        0        0     1156 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/api/query/stack.py
--rw-r--r--   0        0        0      233 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/api/schema.py
--rw-r--r--   0        0        0     2578 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/api/schema_types.py
--rw-r--r--   0        0        0     1551 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/api/subscription.py
--rw-r--r--   0        0        0     1579 2024-04-24 16:07:35.740037 odooghost-0.8.0/odooghost/web/application.py
--rw-r--r--   0        0        0     8986 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/android-chrome-192x192.png
--rw-r--r--   0        0        0    13346 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/android-chrome-512x512.png
--rw-r--r--   0        0        0     8702 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/apple-touch-icon.png
--rw-r--r--   0        0        0      636 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/ContainersView-vBrHvCnL.js
--rw-r--r--   0        0        0     1162 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/DashboardView-QC2AjQPk.js
--rw-r--r--   0        0        0      275 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/SettingsView-BS_D169E.js
--rw-r--r--   0        0        0      286 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/StackItemContainersView-DI931aio.js
--rw-r--r--   0        0        0      611 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/StackItemIndexView-BOSojVnH.js
--rw-r--r--   0        0        0      280 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/StackItemLogsView-Bgz593Fu.js
--rw-r--r--   0        0        0      284 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/StackItemServicesView-XPZCOPql.js
--rw-r--r--   0        0        0     5418 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/StackItemView-ieiARAXz.js
--rw-r--r--   0        0        0     2081 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/StackView-DOsjJPZv.js
--rw-r--r--   0        0        0      272 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/UsageView-CwbrZuiW.js
--rw-r--r--   0        0        0     2082 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/VContainers-AwiqsRRo.js
--rw-r--r--   0        0        0     1206 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/VHeader-B1IUp6LH.js
--rw-r--r--   0        0        0      418 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/VStat-BF-IjV6V.js
--rw-r--r--   0        0        0     1744 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/VWarningAlert-BH59UqxK.js
--rw-r--r--   0        0        0      721 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css
--rw-r--r--   0        0        0      310 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/constant-DWkFHeG6.js
--rw-r--r--   0        0        0    26276 2024-04-24 16:08:16.407951 odooghost-0.8.0/odooghost/web/dist/assets/index-BCu_nn1R.css
--rw-r--r--   0        0        0   345282 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/index-s10VwhOf.js
--rw-r--r--   0        0        0      564 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/assets/stack-C5Mp2ADT.js
--rw-r--r--   0        0        0      575 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/favicon-16x16.png
--rw-r--r--   0        0        0     1199 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/favicon-32x32.png
--rw-r--r--   0        0        0    15406 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/favicon.ico
--rw-r--r--   0        0        0      787 2024-04-24 16:08:16.411951 odooghost-0.8.0/odooghost/web/dist/index.html
--rw-r--r--   0        0        0     3531 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/logo.svg
--rw-r--r--   0        0        0      286 2024-04-24 16:08:16.163952 odooghost-0.8.0/odooghost/web/dist/site.webmanifest
--rw-r--r--   0        0        0     3811 2024-04-24 16:08:18.695946 odooghost-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 odooghost-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-24 16:34:27.036313 odooghost-0.8.1/LICENSE
+-rw-r--r--   0        0        0     1967 2024-04-24 16:34:27.036313 odooghost-0.8.1/README.md
+-rw-r--r--   0        0        0      369 2024-04-24 16:35:18.973046 odooghost-0.8.1/odooghost/__init__.py
+-rw-r--r--   0        0        0       94 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/__main__.py
+-rw-r--r--   0        0        0      127 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/cli/__init__.py
+-rw-r--r--   0        0        0      451 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/cli/config.py
+-rw-r--r--   0        0        0     1861 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/cli/root.py
+-rw-r--r--   0        0        0       42 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/cli/stack/__init__.py
+-rw-r--r--   0        0        0      959 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/cli/stack/config.py
+-rw-r--r--   0        0        0     9765 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/cli/stack/data.py
+-rw-r--r--   0        0        0    13037 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/cli/stack/root.py
+-rw-r--r--   0        0        0      271 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/config/__init__.py
+-rw-r--r--   0        0        0     4440 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/config/addons.py
+-rw-r--r--   0        0        0      267 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/config/app.py
+-rw-r--r--   0        0        0     2445 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/config/dependency.py
+-rw-r--r--   0        0        0     2082 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/config/service.py
+-rw-r--r--   0        0        0     2854 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/config/stack.py
+-rw-r--r--   0        0        0      789 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/constant.py
+-rw-r--r--   0        0        0     9501 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/container.py
+-rw-r--r--   0        0        0     7516 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/context.py
+-rw-r--r--   0        0        0     1139 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/exceptions.py
+-rw-r--r--   0        0        0      585 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/filters.py
+-rw-r--r--   0        0        0     3702 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/git.py
+-rw-r--r--   0        0        0     1111 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/logger.py
+-rw-r--r--   0        0        0      466 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/renderer.py
+-rw-r--r--   0        0        0       63 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/services/__init__.py
+-rw-r--r--   0        0        0    14691 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/services/base.py
+-rw-r--r--   0        0        0     3972 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/services/db.py
+-rw-r--r--   0        0        0      102 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/services/odoo/__init__.py
+-rw-r--r--   0        0        0     3756 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/services/odoo/addons.py
+-rw-r--r--   0        0        0     4838 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/services/odoo/service.py
+-rw-r--r--   0        0        0    10382 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/stack.py
+-rw-r--r--   0        0        0     1710 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/templates/Dockerfile.j2
+-rw-r--r--   0        0        0      580 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/types.py
+-rw-r--r--   0        0        0       93 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/__init__.py
+-rw-r--r--   0        0        0      790 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/autocomplete.py
+-rw-r--r--   0        0        0      993 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/exec.py
+-rw-r--r--   0        0        0     2159 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/misc.py
+-rw-r--r--   0        0        0     3914 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/progress_stream.py
+-rw-r--r--   0        0        0      884 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/signals.py
+-rw-r--r--   0        0        0     2567 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/stream.py
+-rw-r--r--   0        0        0     1516 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/utils/sync_to_async.py
+-rw-r--r--   0        0        0        0 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/web/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/web/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/web/api/query/__init__.py
+-rw-r--r--   0        0        0      305 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/web/api/query/dashboard.py
+-rw-r--r--   0        0        0     1156 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/web/api/query/stack.py
+-rw-r--r--   0        0        0      233 2024-04-24 16:34:27.036313 odooghost-0.8.1/odooghost/web/api/schema.py
+-rw-r--r--   0        0        0     2578 2024-04-24 16:34:27.040314 odooghost-0.8.1/odooghost/web/api/schema_types.py
+-rw-r--r--   0        0        0     1679 2024-04-24 16:34:27.040314 odooghost-0.8.1/odooghost/web/api/subscription.py
+-rw-r--r--   0        0        0     1579 2024-04-24 16:34:27.040314 odooghost-0.8.1/odooghost/web/application.py
+-rw-r--r--   0        0        0     8986 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/android-chrome-192x192.png
+-rw-r--r--   0        0        0    13346 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/android-chrome-512x512.png
+-rw-r--r--   0        0        0     8702 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/apple-touch-icon.png
+-rw-r--r--   0        0        0      636 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/ContainersView-DEOoJDOr.js
+-rw-r--r--   0        0        0     1162 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/DashboardView-9fL2PusH.js
+-rw-r--r--   0        0        0      275 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/SettingsView-CwpsckXe.js
+-rw-r--r--   0        0        0      286 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/StackItemContainersView-DtnjBFd6.js
+-rw-r--r--   0        0        0      611 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/StackItemIndexView-BMo8NmFy.js
+-rw-r--r--   0        0        0      280 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/StackItemLogsView-CToeth34.js
+-rw-r--r--   0        0        0      284 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/StackItemServicesView--A44eQAS.js
+-rw-r--r--   0        0        0     5418 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/StackItemView-NraLa75A.js
+-rw-r--r--   0        0        0     2081 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/StackView-Ce0Va4Vr.js
+-rw-r--r--   0        0        0      272 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/UsageView-DgJ9FyX7.js
+-rw-r--r--   0        0        0     2082 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/VContainers-EH27biMB.js
+-rw-r--r--   0        0        0     1206 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/VHeader-CT5XbojA.js
+-rw-r--r--   0        0        0      418 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/VStat-KUI9Tfce.js
+-rw-r--r--   0        0        0     1744 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/VWarningAlert-B5Y9sf5o.js
+-rw-r--r--   0        0        0      721 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css
+-rw-r--r--   0        0        0      310 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/constant-DWkFHeG6.js
+-rw-r--r--   0        0        0    26276 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/index-BCu_nn1R.css
+-rw-r--r--   0        0        0   345355 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/index-DDQ87HFV.js
+-rw-r--r--   0        0        0      564 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/assets/stack-DYu-LgCo.js
+-rw-r--r--   0        0        0      575 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/favicon-16x16.png
+-rw-r--r--   0        0        0     1199 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/favicon-32x32.png
+-rw-r--r--   0        0        0    15406 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/favicon.ico
+-rw-r--r--   0        0        0      787 2024-04-24 16:35:17.409025 odooghost-0.8.1/odooghost/web/dist/index.html
+-rw-r--r--   0        0        0     3531 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/logo.svg
+-rw-r--r--   0        0        0      286 2024-04-24 16:35:17.153021 odooghost-0.8.1/odooghost/web/dist/site.webmanifest
+-rw-r--r--   0        0        0     3811 2024-04-24 16:35:18.969046 odooghost-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 odooghost-0.8.1/PKG-INFO
```

### Comparing `odooghost-0.8.0/LICENSE` & `odooghost-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/README.md` & `odooghost-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/cli/root.py` & `odooghost-0.8.1/odooghost/cli/root.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/cli/stack/config.py` & `odooghost-0.8.1/odooghost/cli/stack/config.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/cli/stack/data.py` & `odooghost-0.8.1/odooghost/cli/stack/data.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/cli/stack/root.py` & `odooghost-0.8.1/odooghost/cli/stack/root.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/config/addons.py` & `odooghost-0.8.1/odooghost/config/addons.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/config/dependency.py` & `odooghost-0.8.1/odooghost/config/dependency.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/config/service.py` & `odooghost-0.8.1/odooghost/config/service.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/config/stack.py` & `odooghost-0.8.1/odooghost/config/stack.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/constant.py` & `odooghost-0.8.1/odooghost/constant.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/container.py` & `odooghost-0.8.1/odooghost/container.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/context.py` & `odooghost-0.8.1/odooghost/context.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/exceptions.py` & `odooghost-0.8.1/odooghost/exceptions.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/filters.py` & `odooghost-0.8.1/odooghost/filters.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/git.py` & `odooghost-0.8.1/odooghost/git.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/logger.py` & `odooghost-0.8.1/odooghost/logger.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/services/base.py` & `odooghost-0.8.1/odooghost/services/base.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/services/db.py` & `odooghost-0.8.1/odooghost/services/db.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/services/odoo/addons.py` & `odooghost-0.8.1/odooghost/services/odoo/addons.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/services/odoo/service.py` & `odooghost-0.8.1/odooghost/services/odoo/service.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/stack.py` & `odooghost-0.8.1/odooghost/stack.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/templates/Dockerfile.j2` & `odooghost-0.8.1/odooghost/templates/Dockerfile.j2`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/types.py` & `odooghost-0.8.1/odooghost/types.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/utils/autocomplete.py` & `odooghost-0.8.1/odooghost/utils/autocomplete.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/utils/exec.py` & `odooghost-0.8.1/odooghost/utils/exec.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/utils/misc.py` & `odooghost-0.8.1/odooghost/utils/misc.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/utils/progress_stream.py` & `odooghost-0.8.1/odooghost/utils/progress_stream.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/utils/signals.py` & `odooghost-0.8.1/odooghost/utils/signals.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/utils/stream.py` & `odooghost-0.8.1/odooghost/utils/stream.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/utils/sync_to_async.py` & `odooghost-0.8.1/odooghost/utils/sync_to_async.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/api/query/stack.py` & `odooghost-0.8.1/odooghost/web/api/query/stack.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/api/schema_types.py` & `odooghost-0.8.1/odooghost/web/api/schema_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     @strawberry.field
     def network_mode(self) -> str:
         return self.instance._config.network.mode
 
     @strawberry.field
     def state(self) -> StackState:
         containers = self.instance.containers(stopped=True)
-        if all(c.is_running for c in containers):
+        if any(c.is_running for c in containers):
             return StackState.RUNNING
         if all(c.is_paused for c in containers):
             return StackState.PAUSED
         if any(c.is_restarting for c in containers):
             return StackState.RESTARTING
         return StackState.STOPPED
```

### Comparing `odooghost-0.8.0/odooghost/web/api/subscription.py` & `odooghost-0.8.1/odooghost/web/api/subscription.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,17 +38,20 @@
 
 @strawberry.type
 class Subscription:
     @strawberry.subscription
     async def events(self) -> t.AsyncGenerator[Event, None]:
         async for e in stream_events():
             if e.get("Type", False) == "container":
+                action = e.get("Action")
+                if action not in ("die", "start", "kill", "stop"):
+                    continue
                 yield Event(
                     id=e.get("id"),
-                    action=e.get("Action"),
+                    action=action,
                     image_from=e.get("from"),
                     container_id=e.get("Actor").get("ID"),
                     container_name=e.get("Actor").get("Attributes").get("name"),
                     service_name=e.get("Actor")
                     .get("Attributes")
                     .get("odooghost_stack_type"),
                     stack_name=e.get("Actor")
```

### Comparing `odooghost-0.8.0/odooghost/web/application.py` & `odooghost-0.8.1/odooghost/web/application.py`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/android-chrome-192x192.png` & `odooghost-0.8.1/odooghost/web/dist/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/android-chrome-512x512.png` & `odooghost-0.8.1/odooghost/web/dist/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/apple-touch-icon.png` & `odooghost-0.8.1/odooghost/web/dist/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/ContainersView-vBrHvCnL.js` & `odooghost-0.8.1/odooghost/web/dist/assets/ContainersView-DEOoJDOr.js`

 * *Files 23% similar despite different names*

#### js-beautify {}

```diff
@@ -1,27 +1,27 @@
 import {
     b as n
-} from "./stack-C5Mp2ADT.js";
+} from "./stack-DYu-LgCo.js";
 import {
     _ as o,
     a as i
-} from "./VHeader-B1IUp6LH.js";
+} from "./VHeader-CT5XbojA.js";
 import {
     _ as l
-} from "./VContainers-AwiqsRRo.js";
+} from "./VContainers-EH27biMB.js";
 import {
     u as c,
     c as _,
     a as r,
     d as u,
     w as m,
     b as e,
     o as f
-} from "./index-s10VwhOf.js";
-import "./VWarningAlert-BH59UqxK.js";
+} from "./index-DDQ87HFV.js";
+import "./VWarningAlert-B5Y9sf5o.js";
 const B = {
     __name: "ContainersView",
     setup(p) {
         const {
             loading: s,
             result: a,
             error: t
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/DashboardView-QC2AjQPk.js` & `odooghost-0.8.1/odooghost/web/dist/assets/DashboardView-9fL2PusH.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -3,26 +3,26 @@
     u as c,
     c as l,
     a as e,
     w as u,
     b as s,
     o as _,
     d as a
-} from "./index-s10VwhOf.js";
+} from "./index-DDQ87HFV.js";
 import {
     _ as d
-} from "./VContainers-AwiqsRRo.js";
+} from "./VContainers-EH27biMB.js";
 import {
     _ as m,
     a as f
-} from "./VHeader-B1IUp6LH.js";
+} from "./VHeader-CT5XbojA.js";
 import {
     _ as o
-} from "./VStat-BF-IjV6V.js";
-import "./VWarningAlert-BH59UqxK.js";
+} from "./VStat-KUI9Tfce.js";
+import "./VWarningAlert-B5Y9sf5o.js";
 const g = i`
   query getDashboard {
     version
     dockerVersion
     stackCount
     containers(stopped: false) {
       id
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/StackItemIndexView-BOSojVnH.js` & `odooghost-0.8.1/odooghost/web/dist/assets/StackItemIndexView-BMo8NmFy.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -1,21 +1,21 @@
 import {
     _ as a
-} from "./VContainers-AwiqsRRo.js";
+} from "./VContainers-EH27biMB.js";
 import {
     _ as o
-} from "./VStat-BF-IjV6V.js";
+} from "./VStat-KUI9Tfce.js";
 import {
     x as c,
     c as r,
     d as s,
     a as t,
     b as n,
     o as i
-} from "./index-s10VwhOf.js";
+} from "./index-DDQ87HFV.js";
 const l = {
         class: "grid grid-cols-1 gap-4 sm:grid-cols-3"
     },
     _ = s("h3", null, "Containers", -1),
     k = {
         __name: "StackItemIndexView",
         setup(d) {
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/StackItemView-ieiARAXz.js` & `odooghost-0.8.1/odooghost/web/dist/assets/StackItemView-NraLa75A.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     a as w
-} from "./stack-C5Mp2ADT.js";
+} from "./stack-DYu-LgCo.js";
 import {
     V as g,
     _ as b
-} from "./VWarningAlert-BH59UqxK.js";
+} from "./VWarningAlert-B5Y9sf5o.js";
 import {
     o as e,
     c as t,
     d as a,
     h as y,
     r as V,
     a as n,
@@ -28,15 +28,15 @@
     s as I,
     n as z,
     _ as Z,
     V as O,
     f as T,
     v as U,
     R as A
-} from "./index-s10VwhOf.js";
+} from "./index-DDQ87HFV.js";
 import {
     s as k
 } from "./constant-DWkFHeG6.js";
 
 function D(l, s) {
     return e(), t("svg", {
         xmlns: "http://www.w3.org/2000/svg",
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/StackView-DOsjJPZv.js` & `odooghost-0.8.1/odooghost/web/dist/assets/StackView-Ce0Va4Vr.js`

 * *Files 8% similar despite different names*

#### js-beautify {}

```diff
@@ -1,14 +1,14 @@
 import {
     Q as h
-} from "./stack-C5Mp2ADT.js";
+} from "./stack-DYu-LgCo.js";
 import {
     a as p,
     _ as x
-} from "./VHeader-B1IUp6LH.js";
+} from "./VHeader-CT5XbojA.js";
 import {
     s as d
 } from "./constant-DWkFHeG6.js";
 import {
     o,
     c as n,
     d as t,
@@ -18,16 +18,16 @@
     w as l,
     b as s,
     F as v,
     e as w,
     f as k,
     t as a,
     n as y
-} from "./index-s10VwhOf.js";
-import "./VWarningAlert-BH59UqxK.js";
+} from "./index-DDQ87HFV.js";
+import "./VWarningAlert-B5Y9sf5o.js";
 
 function b(u, i) {
     return o(), n("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         viewBox: "0 0 24 24",
         fill: "currentColor",
         "aria-hidden": "true",
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/VContainers-AwiqsRRo.js` & `odooghost-0.8.1/odooghost/web/dist/assets/VContainers-EH27biMB.js`

 * *Files 3% similar despite different names*

#### js-beautify {}

```diff
@@ -4,15 +4,15 @@
     d as e,
     F as d,
     e as _,
     n as r,
     t,
     a as p,
     b as x
-} from "./index-s10VwhOf.js";
+} from "./index-DDQ87HFV.js";
 
 function u(i, o) {
     return n(), a("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         viewBox: "0 0 20 20",
         fill: "currentColor",
         "aria-hidden": "true",
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/VHeader-B1IUp6LH.js` & `odooghost-0.8.1/odooghost/web/dist/assets/VHeader-CT5XbojA.js`

 * *Files 12% similar despite different names*

#### js-beautify {}

```diff
@@ -1,20 +1,20 @@
 import {
     V as d,
     _ as u
-} from "./VWarningAlert-BH59UqxK.js";
+} from "./VWarningAlert-B5Y9sf5o.js";
 import {
     o as s,
     c as a,
     j as o,
     a as l,
     d as c,
     _,
     t as p
-} from "./index-s10VwhOf.js";
+} from "./index-DDQ87HFV.js";
 const m = {
         key: 0,
         class: "py-20"
     },
     h = {
         key: 1
     },
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/VWarningAlert-BH59UqxK.js` & `odooghost-0.8.1/odooghost/web/dist/assets/VWarningAlert-B5Y9sf5o.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -7,15 +7,15 @@
     q as n,
     F as b,
     e as S,
     A as p,
     f as $,
     b as k,
     B
-} from "./index-s10VwhOf.js";
+} from "./index-DDQ87HFV.js";
 
 function C(r, e) {
     return a(), l("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css` & `odooghost-0.8.1/odooghost/web/dist/assets/VWarningAlert-DWujdwvy.css`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/index-BCu_nn1R.css` & `odooghost-0.8.1/odooghost/web/dist/assets/index-BCu_nn1R.css`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/index-s10VwhOf.js` & `odooghost-0.8.1/odooghost/web/dist/assets/index-DDQ87HFV.js`

 * *Files 1% similar despite different names*

#### js-beautify {}

```diff
@@ -1,8 +1,8 @@
-const __vite__fileDeps = ["assets/DashboardView-QC2AjQPk.js", "assets/VContainers-AwiqsRRo.js", "assets/VHeader-B1IUp6LH.js", "assets/VWarningAlert-BH59UqxK.js", "assets/VWarningAlert-DWujdwvy.css", "assets/VStat-BF-IjV6V.js", "assets/StackView-DOsjJPZv.js", "assets/stack-C5Mp2ADT.js", "assets/constant-DWkFHeG6.js", "assets/StackItemView-ieiARAXz.js", "assets/StackItemIndexView-BOSojVnH.js", "assets/ContainersView-vBrHvCnL.js"],
+const __vite__fileDeps = ["assets/DashboardView-9fL2PusH.js", "assets/VContainers-EH27biMB.js", "assets/VHeader-CT5XbojA.js", "assets/VWarningAlert-B5Y9sf5o.js", "assets/VWarningAlert-DWujdwvy.css", "assets/VStat-KUI9Tfce.js", "assets/StackView-Ce0Va4Vr.js", "assets/stack-DYu-LgCo.js", "assets/constant-DWkFHeG6.js", "assets/StackItemView-NraLa75A.js", "assets/StackItemIndexView-BMo8NmFy.js", "assets/ContainersView-DEOoJDOr.js"],
     __vite__mapDeps = i => i.map(i => __vite__fileDeps[i]);
 (function() {
     const t = document.createElement("link").relList;
     if (t && t.supports && t.supports("modulepreload")) return;
     for (const i of document.querySelectorAll('link[rel="modulepreload"]')) r(i);
     new MutationObserver(i => {
         for (const o of i)
@@ -68,15 +68,15 @@
     },
     Uh = /-(\w)/g,
     Pt = so(e => e.replace(Uh, (t, n) => n ? n.toUpperCase() : "")),
     zh = /\B([A-Z])/g,
     mr = so(e => e.replace(zh, "-$1").toLowerCase()),
     ao = so(e => e.charAt(0).toUpperCase() + e.slice(1)),
     Do = so(e => e ? `on${ao(e)}` : ""),
-    pn = (e, t) => !Object.is(e, t),
+    vn = (e, t) => !Object.is(e, t),
     No = (e, t) => {
         for (let n = 0; n < e.length; n++) e[n](t)
     },
     Cc = (e, t, n) => {
         Object.defineProperty(e, t, {
             configurable: !0,
             enumerable: !1,
@@ -133,15 +133,15 @@
 }
 const Xh = "itemscope,allowfullscreen,formnovalidate,ismap,nomodule,novalidate,readonly",
     Zh = ca(Xh);
 
 function Ac(e) {
     return !!e || e === ""
 }
-const Fn = e => je(e) ? e : e == null ? "" : le(e) || De(e) && (e.toString === Oc || !de(e.toString)) ? JSON.stringify(e, Rc, 2) : String(e),
+const cn = e => je(e) ? e : e == null ? "" : le(e) || De(e) && (e.toString === Oc || !de(e.toString)) ? JSON.stringify(e, Rc, 2) : String(e),
     Rc = (e, t) => t && t.__v_isRef ? Rc(e, t.value) : tr(t) ? {
         [`Map(${t.size})`]: [...t.entries()].reduce((n, [r, i], o) => (n[Po(r, o) + " =>"] = i, n), {})
     } : Sc(t) ? {
         [`Set(${t.size})`]: [...t.values()].map(n => Po(n))
     } : qn(t) ? Po(t) : De(t) && !le(t) && !Tc(t) ? String(t) : t,
     Po = (e, t = "") => {
         var n;
@@ -210,34 +210,34 @@
 let Ln;
 class ma {
     constructor(t, n, r, i) {
         this.fn = t, this.trigger = n, this.scheduler = r, this.active = !0, this.deps = [], this._dirtyLevel = 4, this._trackId = 0, this._runnings = 0, this._shouldSchedule = !1, this._depsLength = 0, ep(this, i)
     }
     get dirty() {
         if (this._dirtyLevel === 2 || this._dirtyLevel === 3) {
-            this._dirtyLevel = 1, _n();
+            this._dirtyLevel = 1, wn();
             for (let t = 0; t < this._depsLength; t++) {
                 const n = this.deps[t];
                 if (n.computed && (np(n.computed), this._dirtyLevel >= 4)) break
             }
-            this._dirtyLevel === 1 && (this._dirtyLevel = 0), wn()
+            this._dirtyLevel === 1 && (this._dirtyLevel = 0), Sn()
         }
         return this._dirtyLevel >= 4
     }
     set dirty(t) {
         this._dirtyLevel = t ? 4 : 0
     }
     run() {
         if (this._dirtyLevel = 0, !this.active) return this.fn();
-        let t = fn,
+        let t = dn,
             n = Ln;
         try {
-            return fn = !0, Ln = this, this._runnings++, pl(this), this.fn()
+            return dn = !0, Ln = this, this._runnings++, pl(this), this.fn()
         } finally {
-            vl(this), this._runnings--, Ln = n, fn = t
+            vl(this), this._runnings--, Ln = n, dn = t
         }
     }
     stop() {
         var t;
         this.active && (pl(this), vl(this), (t = this.onStop) == null || t.call(this), this.active = !1)
     }
 }
@@ -257,25 +257,25 @@
     }
 }
 
 function Nc(e, t) {
     const n = e.get(t);
     n !== void 0 && t._trackId !== n && (e.delete(t), e.size === 0 && e.cleanup())
 }
-let fn = !0,
+let dn = !0,
     hs = 0;
 const Pc = [];
 
-function _n() {
-    Pc.push(fn), fn = !1
+function wn() {
+    Pc.push(dn), dn = !1
 }
 
-function wn() {
+function Sn() {
     const e = Pc.pop();
-    fn = e === void 0 ? !0 : e
+    dn = e === void 0 ? !0 : e
 }
 
 function ya() {
     hs++
 }
 
 function ga() {
@@ -304,15 +304,15 @@
         return n.cleanup = e, n.computed = t, n
     },
     Ui = new WeakMap,
     Mn = Symbol(""),
     vs = Symbol("");
 
 function lt(e, t, n) {
-    if (fn && Ln) {
+    if (dn && Ln) {
         let r = Ui.get(e);
         r || Ui.set(e, r = new Map);
         let i = r.get(n);
         i || r.set(n, i = Mc(() => r.delete(n))), Fc(Ln, i)
     }
 }
 
@@ -357,17 +357,17 @@
             const r = be(this);
             for (let o = 0, s = this.length; o < s; o++) lt(r, "get", o + "");
             const i = r[t](...n);
             return i === -1 || i === !1 ? r[t](...n.map(be)) : i
         }
     }), ["push", "pop", "shift", "unshift", "splice"].forEach(t => {
         e[t] = function(...n) {
-            _n(), ya();
+            wn(), ya();
             const r = be(this)[t].apply(this, n);
-            return ga(), wn(), r
+            return ga(), Sn(), r
         }
     }), e
 }
 
 function sp(e) {
     qn(e) || (e = String(e));
     const t = be(this);
@@ -401,15 +401,15 @@
         let o = t[n];
         if (!this._isShallow) {
             const l = Yr(o);
             if (!zi(r) && !Yr(r) && (o = be(o), r = be(r)), !le(t) && Ve(o) && !Ve(r)) return l ? !1 : (o.value = r, !0)
         }
         const s = le(t) && ha(n) ? Number(n) < t.length : ge(t, n),
             a = Reflect.set(t, n, r, i);
-        return t === be(i) && (s ? pn(r, o) && qt(t, "set", n, r) : qt(t, "add", n, r)), a
+        return t === be(i) && (s ? vn(r, o) && qt(t, "set", n, r) : qt(t, "add", n, r)), a
     }
     deleteProperty(t, n) {
         const r = ge(t, n);
         t[n];
         const i = Reflect.deleteProperty(t, n);
         return i && r && qt(t, "delete", n, void 0), i
     }
@@ -438,28 +438,28 @@
 const ba = e => e,
     lo = e => Reflect.getPrototypeOf(e);
 
 function gi(e, t, n = !1, r = !1) {
     e = e.__v_raw;
     const i = be(e),
         o = be(t);
-    n || (pn(t, o) && lt(i, "get", t), lt(i, "get", o));
+    n || (vn(t, o) && lt(i, "get", t), lt(i, "get", o));
     const {
         has: s
     } = lo(i), a = r ? ba : n ? wa : Jr;
     if (s.call(i, t)) return a(e.get(t));
     if (s.call(i, o)) return a(e.get(o));
     e !== i && e.get(t)
 }
 
 function bi(e, t = !1) {
     const n = this.__v_raw,
         r = be(n),
         i = be(e);
-    return t || (pn(e, i) && lt(r, "has", e), lt(r, "has", i)), e === i ? n.has(e) : n.has(e) || n.has(i)
+    return t || (vn(e, i) && lt(r, "has", e), lt(r, "has", i)), e === i ? n.has(e) : n.has(e) || n.has(i)
 }
 
 function Ei(e, t = !1) {
     return e = e.__v_raw, !t && lt(be(e), "iterate", Mn), Reflect.get(e, "size", e)
 }
 
 function yl(e) {
@@ -474,15 +474,15 @@
         {
             has: r,
             get: i
         } = lo(n);
     let o = r.call(n, e);
     o || (e = be(e), o = r.call(n, e));
     const s = i.call(n, e);
-    return n.set(e, t), o ? pn(t, s) && qt(n, "set", e, t) : qt(n, "add", e, t), this
+    return n.set(e, t), o ? vn(t, s) && qt(n, "set", e, t) : qt(n, "add", e, t), this
 }
 
 function bl(e) {
     const t = be(this),
         {
             has: n,
             get: r
@@ -700,15 +700,15 @@
     wa = e => De(e) ? zc(e) : e;
 class Hc {
     constructor(t, n, r, i) {
         this.getter = t, this._setter = n, this.dep = void 0, this.__v_isRef = !0, this.__v_isReadonly = !1, this.effect = new ma(() => t(this._value), () => Ni(this, this.effect._dirtyLevel === 2 ? 2 : 3)), this.effect.computed = this, this.effect.active = this._cacheable = !i, this.__v_isReadonly = r
     }
     get value() {
         const t = be(this);
-        return (!t._cacheable || t.effect.dirty) && pn(t._value, t._value = t.effect.run()) && Ni(t, 4), Gc(t), t.effect._dirtyLevel >= 2 && Ni(t, 2), t._value
+        return (!t._cacheable || t.effect.dirty) && vn(t._value, t._value = t.effect.run()) && Ni(t, 4), Gc(t), t.effect._dirtyLevel >= 2 && Ni(t, 2), t._value
     }
     set value(t) {
         this._setter(t)
     }
     get _dirty() {
         return this.effect.dirty
     }
@@ -721,15 +721,15 @@
     let r, i;
     const o = de(e);
     return o ? (r = e, i = pt) : (r = e.get, i = e.set), new Hc(r, i, o || !i, n)
 }
 
 function Gc(e) {
     var t;
-    fn && Ln && (e = be(e), Fc(Ln, (t = e.dep) != null ? t : e.dep = Mc(() => e.dep = void 0, e instanceof Hc ? e : void 0)))
+    dn && Ln && (e = be(e), Fc(Ln, (t = e.dep) != null ? t : e.dep = Mc(() => e.dep = void 0, e instanceof Hc ? e : void 0)))
 }
 
 function Ni(e, t = 4, n) {
     e = be(e);
     const r = e.dep;
     r && Lc(r, t)
 }
@@ -754,23 +754,23 @@
         this.__v_isShallow = n, this.dep = void 0, this.__v_isRef = !0, this._rawValue = n ? t : be(t), this._value = n ? t : Jr(t)
     }
     get value() {
         return Gc(this), this._value
     }
     set value(t) {
         const n = this.__v_isShallow || zi(t) || Yr(t);
-        t = n ? t : be(t), pn(t, this._rawValue) && (this._rawValue = t, this._value = n ? t : Jr(t), Ni(this, 4))
+        t = n ? t : be(t), vn(t, this._rawValue) && (this._rawValue = t, this._value = n ? t : Jr(t), Ni(this, 4))
     }
 }
 
-function ke(e) {
+function Oe(e) {
     return Ve(e) ? e.value : e
 }
 const xp = {
-    get: (e, t, n) => ke(Reflect.get(e, t, n)),
+    get: (e, t, n) => Oe(Reflect.get(e, t, n)),
     set: (e, t, n, r) => {
         const i = e[t];
         return Ve(i) && !Ve(n) ? (i.value = n, !0) : Reflect.set(e, t, n, r)
     }
 };
 
 function Yc(e) {
@@ -803,25 +803,25 @@
     return Ve(r) ? r : new Tp(e, t, n)
 }
 /**
  * @vue/runtime-core v3.4.25
  * (c) 2018-present Yuxi (Evan) You and Vue contributors
  * @license MIT
  **/
-function dn(e, t, n, r) {
+function hn(e, t, n, r) {
     try {
         return r ? e(...r) : e()
     } catch (i) {
         co(i, t, n)
     }
 }
 
 function vt(e, t, n, r) {
     if (de(e)) {
-        const i = dn(e, t, n, r);
+        const i = hn(e, t, n, r);
         return i && xc(i) && i.catch(o => {
             co(o, t, n)
         }), i
     }
     if (le(e)) {
         const i = [];
         for (let o = 0; o < e.length; o++) i.push(vt(e[o], t, n, r));
@@ -841,15 +841,15 @@
                 for (let c = 0; c < u.length; c++)
                     if (u[c](e, s, a) === !1) return
             }
             o = o.parent
         }
         const l = t.appContext.config.errorHandler;
         if (l) {
-            _n(), dn(l, null, 10, [e, s, a]), wn();
+            wn(), hn(l, null, 10, [e, s, a]), Sn();
             return
         }
     }
     kp(e, n, i, r)
 }
 
 function kp(e, t, n, r = !0) {
@@ -857,15 +857,15 @@
 }
 let Xr = !1,
     ms = !1;
 const tt = [];
 let Nt = 0;
 const nr = [];
 let Zt = null,
-    Rn = 0;
+    In = 0;
 const Jc = Promise.resolve();
 let xa = null;
 
 function $t(e) {
     const t = xa || Jc;
     return e ? t.then(this ? e.bind(this) : e) : t
 }
@@ -892,15 +892,15 @@
 
 function Rp(e) {
     const t = tt.indexOf(e);
     t > Nt && tt.splice(t, 1)
 }
 
 function Ip(e) {
-    le(e) ? nr.push(...e) : (!Zt || !Zt.includes(e, e.allowRecurse ? Rn + 1 : Rn)) && nr.push(e), Xc()
+    le(e) ? nr.push(...e) : (!Zt || !Zt.includes(e, e.allowRecurse ? In + 1 : In)) && nr.push(e), Xc()
 }
 
 function _l(e, t, n = Xr ? Nt + 1 : 0) {
     for (; n < tt.length; n++) {
         const r = tt[n];
         if (r && r.pre) {
             if (e && r.id !== e.uid) continue;
@@ -912,16 +912,16 @@
 function Zc(e) {
     if (nr.length) {
         const t = [...new Set(nr)].sort((n, r) => Zr(n) - Zr(r));
         if (nr.length = 0, Zt) {
             Zt.push(...t);
             return
         }
-        for (Zt = t, Rn = 0; Rn < Zt.length; Rn++) Zt[Rn]();
-        Zt = null, Rn = 0
+        for (Zt = t, In = 0; In < Zt.length; In++) Zt[In]();
+        Zt = null, In = 0
     }
 }
 const Zr = e => e.id == null ? 1 / 0 : e.id,
     Dp = (e, t) => {
         const n = Zr(e) - Zr(t);
         if (n === 0) {
             if (e.pre && !t.pre) return -1;
@@ -931,15 +931,15 @@
     };
 
 function ef(e) {
     ms = !1, Xr = !0, tt.sort(Dp);
     try {
         for (Nt = 0; Nt < tt.length; Nt++) {
             const t = tt[Nt];
-            t && t.active !== !1 && dn(t, null, 14)
+            t && t.active !== !1 && hn(t, null, 14)
         }
     } finally {
         Nt = 0, tt.length = 0, Zc(), Xr = !1, xa = null, (tt.length || nr.length) && ef()
     }
 }
 
 function Np(e, t, ...n) {
@@ -1109,15 +1109,15 @@
         const r = t.subTree;
         if (r.suspense && r.suspense.activeBranch === e && (r.el = e.el), r === e)(e = t.vnode).el = n, t = t.parent;
         else break
     }
 }
 const Ta = "components";
 
-function _1(e, t) {
+function w1(e, t) {
     return of(Ta, e, !0, t) || e
 }
 const rf = Symbol.for("v-ndc");
 
 function ho(e) {
     return je(e) ? of(Ta, e, !1) || e : e || rf
 }
@@ -1172,36 +1172,36 @@
     const l = Je,
         u = O => r === !0 ? O : Gn(O, r === !1 ? 1 : void 0);
     let c, d = !1,
         f = !1;
     if (Ve(e) ? (c = () => e.value, d = zi(e)) : jn(e) ? (c = () => u(e), d = !0) : le(e) ? (f = !0, d = e.some(O => jn(O) || zi(O)), c = () => e.map(O => {
             if (Ve(O)) return O.value;
             if (jn(O)) return u(O);
-            if (de(O)) return dn(O, l, 2)
-        })) : de(e) ? t ? c = () => dn(e, l, 2) : c = () => (h && h(), vt(e, l, 3, [p])) : c = pt, t && r) {
+            if (de(O)) return hn(O, l, 2)
+        })) : de(e) ? t ? c = () => hn(e, l, 2) : c = () => (h && h(), vt(e, l, 3, [p])) : c = pt, t && r) {
         const O = c;
         c = () => Gn(O())
     }
     let h, p = O => {
             h = E.onStop = () => {
-                dn(O, l, 4), h = E.onStop = void 0
+                hn(O, l, 4), h = E.onStop = void 0
             }
         },
         m;
     if (yo)
         if (p = pt, t ? n && vt(t, l, 3, [c(), f ? [] : void 0, p]) : c(), i === "sync") {
             const O = qp();
             m = O.__watcherHandles || (O.__watcherHandles = [])
         } else return pt;
     let b = f ? new Array(e.length).fill(Si) : Si;
     const y = () => {
         if (!(!E.active || !E.dirty))
             if (t) {
                 const O = E.run();
-                (r || d || (f ? O.some((F, A) => pn(F, b[A])) : pn(O, b))) && (h && h(), vt(t, l, 3, [O, b === Si ? void 0 : f && b[0] === Si ? [] : b, p]), b = O)
+                (r || d || (f ? O.some((F, A) => vn(F, b[A])) : vn(O, b))) && (h && h(), vt(t, l, 3, [O, b === Si ? void 0 : f && b[0] === Si ? [] : b, p]), b = O)
             } else E.run()
     };
     y.allowRecurse = !!t;
     let _;
     i === "sync" ? _ = y : i === "post" ? _ = () => st(y, l && l.suspense) : (y.pre = !0, l && (y.id = l.uid), _ = () => Oa(y));
     const E = new ma(c, pt, _),
         S = va(),
@@ -1244,22 +1244,22 @@
         Gn(i, t, n, r)
     });
     else if (Tc(e))
         for (const i in e) Gn(e[i], t, n, r);
     return e
 }
 
-function Sn(e, t, n, r) {
+function xn(e, t, n, r) {
     const i = e.dirs,
         o = t && t.dirs;
     for (let s = 0; s < i.length; s++) {
         const a = i[s];
         o && (a.oldValue = o[s].value);
         let l = a.dir[r];
-        l && (_n(), vt(l, n, 8, [e.el, a, e, t]), wn())
+        l && (wn(), vt(l, n, 8, [e.el, a, e, t]), Sn())
     }
 }
 const en = Symbol("_leaveCb"),
     xi = Symbol("_enterCb");
 
 function Qp() {
     const e = {
@@ -1318,15 +1318,15 @@
                 if (r.isLeaving) return Lo(o);
                 const l = xl(o);
                 if (!l) return Lo(o);
                 const u = ys(l, s, r, n);
                 gs(l, u);
                 const c = n.subTree,
                     d = c && xl(c);
-                if (d && d.type !== mt && !In(l, d)) {
+                if (d && d.type !== mt && !Dn(l, d)) {
                     const f = ys(d, s, r, n);
                     if (gs(d, f), a === "out-in") return r.isLeaving = !0, f.afterLeave = () => {
                         r.isLeaving = !1, n.update.active !== !1 && (n.effect.dirty = !0, n.update())
                     }, Lo(o);
                     a === "in-out" && l.type !== mt && (f.delayLeave = (h, p, m) => {
                         const b = lf(r, d);
                         b[String(d.key)] = d, h[en] = () => {
@@ -1376,15 +1376,15 @@
         beforeEnter(A) {
             let R = a;
             if (!n.isMounted)
                 if (i) R = m || a;
                 else return;
             A[en] && A[en](!0);
             const M = S[E];
-            M && In(e, M) && M.el[en] && M.el[en](), T(R, [A])
+            M && Dn(e, M) && M.el[en] && M.el[en](), T(R, [A])
         },
         enter(A) {
             let R = l,
                 M = u,
                 ne = c;
             if (!n.isMounted)
                 if (i) R = b || l, M = y || u, ne = _ || c;
@@ -1487,18 +1487,18 @@
 }
 
 function vo(e, t, n = Je, r = !1) {
     if (n) {
         const i = n[e] || (n[e] = []),
             o = t.__weh || (t.__weh = (...s) => {
                 if (n.isUnmounted) return;
-                _n();
+                wn();
                 const a = fi(n),
                     l = vt(t, n, e, s);
-                return a(), wn(), l
+                return a(), Sn(), l
             });
         return r ? i.unshift(o) : i.push(o), o
     }
 }
 const zt = e => (t, n = Je) => (!yo || e === "sp") && vo(e, (...r) => t(...r), n),
     Kp = zt("bm"),
     at = zt("m"),
@@ -1536,15 +1536,15 @@
     else i = [];
     return n && (n[r] = i), i
 }
 
 function tv(e, t, n = {}, r, i) {
     if (Ze.isCE || Ze.parent && jr(Ze.parent) && Ze.parent.isCE) return t !== "default" && (n.name = t), me("slot", n, r && r());
     let o = e[t];
-    o && o._c && (o._d = !1), Oe();
+    o && o._c && (o._d = !1), Te();
     const s = o && hf(o(n)),
         a = Tt(Ke, {
             key: n.key || s && s.key || `_${t}`
         }, s || (r ? r() : []), s && e._ === 1 ? 64 : -2);
     return !i && a.scopeId && (a.slotScopeIds = [a.scopeId + "-s"]), o && o._c && (o._d = !0), a
 }
 
@@ -2162,15 +2162,15 @@
         {
             i: a,
             r: l
         } = e,
         u = t && t.r,
         c = a.refs === Pe ? a.refs = {} : a.refs,
         d = a.setupState;
-    if (u != null && u !== l && (je(u) ? (c[u] = null, ge(d, u) && (d[u] = null)) : Ve(u) && (u.value = null)), de(l)) dn(l, a, 12, [s, c]);
+    if (u != null && u !== l && (je(u) ? (c[u] = null, ge(d, u) && (d[u] = null)) : Ve(u) && (u.value = null)), de(l)) hn(l, a, 12, [s, c]);
     else {
         const f = je(l),
             h = Ve(l);
         if (f || h) {
             const p = () => {
                 if (e.f) {
                     const m = f ? ge(d, l) ? d[l] : c[l] : l.value;
@@ -2201,15 +2201,15 @@
         setElementText: c,
         parentNode: d,
         nextSibling: f,
         setScopeId: h = pt,
         insertStaticContent: p
     } = e, m = (v, g, x, P = null, D = null, j = null, z = void 0, q = null, C = !!g.dynamicChildren) => {
         if (v === g) return;
-        v && !In(v, g) && (P = k(v), re(v, D, j, !0), v = null), g.patchFlag === -2 && (C = !1, g.dynamicChildren = null);
+        v && !Dn(v, g) && (P = k(v), re(v, D, j, !0), v = null), g.patchFlag === -2 && (C = !1, g.dynamicChildren = null);
         const {
             type: I,
             ref: B,
             shapeFlag: J
         } = g;
         switch (I) {
             case mo:
@@ -2258,22 +2258,22 @@
         let C, I;
         const {
             props: B,
             shapeFlag: J,
             transition: te,
             dirs: ae
         } = v;
-        if (C = v.el = s(v.type, j, B && B.is, B), J & 8 ? c(C, v.children) : J & 16 && A(v.children, C, null, P, D, jo(v, j), z, q), ae && Sn(v, null, P, "created"), F(C, v, v.scopeId, z, P), B) {
+        if (C = v.el = s(v.type, j, B && B.is, B), J & 8 ? c(C, v.children) : J & 16 && A(v.children, C, null, P, D, jo(v, j), z, q), ae && xn(v, null, P, "created"), F(C, v, v.scopeId, z, P), B) {
             for (const _e in B) _e !== "value" && !Mr(_e) && o(C, _e, null, B[_e], j, v.children, P, D, fe);
             "value" in B && o(C, "value", null, B.value, j), (I = B.onVnodeBeforeMount) && At(I, P, v)
         }
-        ae && Sn(v, null, P, "beforeMount");
+        ae && xn(v, null, P, "beforeMount");
         const se = gv(D, te);
         se && te.beforeEnter(C), r(C, g, x), ((I = B && B.onVnodeMounted) || se || ae) && st(() => {
-            I && At(I, P, v), se && te.enter(C), ae && Sn(v, null, P, "mounted")
+            I && At(I, P, v), se && te.enter(C), ae && xn(v, null, P, "mounted")
         }, D)
     }, F = (v, g, x, P, D) => {
         if (x && h(v, x), P)
             for (let j = 0; j < P.length; j++) h(v, P[j]);
         if (D) {
             let j = D.subTree;
             if (g === j) {
@@ -2293,35 +2293,35 @@
             dynamicChildren: I,
             dirs: B
         } = g;
         C |= v.patchFlag & 16;
         const J = v.props || Pe,
             te = g.props || Pe;
         let ae;
-        if (x && xn(x, !1), (ae = te.onVnodeBeforeUpdate) && At(ae, x, g, v), B && Sn(g, v, x, "beforeUpdate"), x && xn(x, !0), I ? M(v.dynamicChildren, I, q, x, P, jo(g, D), j) : z || U(v, g, q, null, x, P, jo(g, D), j, !1), C > 0) {
+        if (x && On(x, !1), (ae = te.onVnodeBeforeUpdate) && At(ae, x, g, v), B && xn(g, v, x, "beforeUpdate"), x && On(x, !0), I ? M(v.dynamicChildren, I, q, x, P, jo(g, D), j) : z || U(v, g, q, null, x, P, jo(g, D), j, !1), C > 0) {
             if (C & 16) ne(q, g, J, te, x, P, D);
             else if (C & 2 && J.class !== te.class && o(q, "class", null, te.class, D), C & 4 && o(q, "style", J.style, te.style, D), C & 8) {
                 const se = g.dynamicProps;
                 for (let _e = 0; _e < se.length; _e++) {
                     const Ne = se[_e],
                         We = J[Ne],
                         Et = te[Ne];
                     (Et !== We || Ne === "value") && o(q, Ne, We, Et, D, v.children, x, P, fe)
                 }
             }
             C & 1 && v.children !== g.children && c(q, g.children)
         } else !z && I == null && ne(q, g, J, te, x, P, D);
         ((ae = te.onVnodeUpdated) || B) && st(() => {
-            ae && At(ae, x, g, v), B && Sn(g, v, x, "updated")
+            ae && At(ae, x, g, v), B && xn(g, v, x, "updated")
         }, P)
     }, M = (v, g, x, P, D, j, z) => {
         for (let q = 0; q < g.length; q++) {
             const C = v[q],
                 I = g[q],
-                B = C.el && (C.type === Ke || !In(C, I) || C.shapeFlag & 70) ? d(C.el) : x;
+                B = C.el && (C.type === Ke || !Dn(C, I) || C.shapeFlag & 70) ? d(C.el) : x;
             m(C, I, B, null, P, D, j, z, !0)
         }
     }, ne = (v, g, x, P, D, j, z) => {
         if (x !== P) {
             if (x !== Pe)
                 for (const q in x) !Mr(q) && !(q in P) && o(v, q, x[q], null, z, g.children, D, j, fe);
             for (const q in P) {
@@ -2376,29 +2376,29 @@
                                 v.isUnmounted || q()
                             });
                             return
                         }
                     }
                     let _e = B,
                         Ne;
-                    xn(v, !1), B ? (B.el = se.el, $(v, B, z)) : B = se, J && No(J), (Ne = B.props && B.props.onVnodeBeforeUpdate) && At(Ne, ae, B, se), xn(v, !0);
+                    On(v, !1), B ? (B.el = se.el, $(v, B, z)) : B = se, J && No(J), (Ne = B.props && B.props.onVnodeBeforeUpdate) && At(Ne, ae, B, se), On(v, !0);
                     const We = Fo(v),
                         Et = v.subTree;
                     v.subTree = We, m(Et, We, d(Et.el), k(Et), v, D, j), B.el = We.el, _e === null && Mp(v, We.el), te && st(te, D), (Ne = B.props && B.props.onVnodeUpdated) && st(() => At(Ne, ae, B, se), D)
                 } else {
                     let B;
                     const {
                         el: J,
                         props: te
                     } = g, {
                         bm: ae,
                         m: se,
                         parent: _e
                     } = v, Ne = jr(g);
-                    if (xn(v, !1), ae && No(ae), !Ne && (B = te && te.onVnodeBeforeMount) && At(B, _e, g), xn(v, !0), J && Ae) {
+                    if (On(v, !1), ae && No(ae), !Ne && (B = te && te.onVnodeBeforeMount) && At(B, _e, g), On(v, !0), J && Ae) {
                         const We = () => {
                             v.subTree = Fo(v), Ae(J, v.subTree, v, D, null)
                         };
                         Ne ? g.type.__asyncLoader().then(() => !v.isUnmounted && We()) : We()
                     } else {
                         const We = v.subTree = Fo(v);
                         m(null, We, x, P, v, D, j), g.el = We.el
@@ -2409,19 +2409,19 @@
                     }(g.shapeFlag & 256 || _e && jr(_e.vnode) && _e.vnode.shapeFlag & 256) && v.a && st(v.a, D), v.isMounted = !0, g = x = P = null
                 }
             },
             C = v.effect = new ma(q, pt, () => Oa(I), v.scope),
             I = v.update = () => {
                 C.dirty && C.run()
             };
-        I.id = v.uid, xn(v, !0), I()
+        I.id = v.uid, On(v, !0), I()
     }, $ = (v, g, x) => {
         g.component = v;
         const P = v.vnode.props;
-        v.vnode = g, v.next = null, dv(v, g.props, P, x), vv(v, g.children, x), _n(), _l(v), wn()
+        v.vnode = g, v.next = null, dv(v, g.props, P, x), vv(v, g.children, x), wn(), _l(v), Sn()
     }, U = (v, g, x, P, D, j, z, q, C = !1) => {
         const I = v && v.children,
             B = v ? v.shapeFlag : 0,
             J = g.children,
             {
                 patchFlag: te,
                 shapeFlag: ae
@@ -2451,22 +2451,22 @@
         let I = 0;
         const B = g.length;
         let J = v.length - 1,
             te = B - 1;
         for (; I <= J && I <= te;) {
             const ae = v[I],
                 se = g[I] = C ? tn(g[I]) : It(g[I]);
-            if (In(ae, se)) m(ae, se, x, null, D, j, z, q, C);
+            if (Dn(ae, se)) m(ae, se, x, null, D, j, z, q, C);
             else break;
             I++
         }
         for (; I <= J && I <= te;) {
             const ae = v[J],
                 se = g[te] = C ? tn(g[te]) : It(g[te]);
-            if (In(ae, se)) m(ae, se, x, null, D, j, z, q, C);
+            if (Dn(ae, se)) m(ae, se, x, null, D, j, z, q, C);
             else break;
             J--, te--
         }
         if (I > J) {
             if (I <= te) {
                 const ae = te + 1,
                     se = ae < B ? g[ae].el : P;
@@ -2494,15 +2494,15 @@
                     re(ut, D, j, !0);
                     continue
                 }
                 let kt;
                 if (ut.key != null) kt = _e.get(ut.key);
                 else
                     for (Ne = se; Ne <= te; Ne++)
-                        if (Sr[Ne - se] === 0 && In(ut, g[Ne])) {
+                        if (Sr[Ne - se] === 0 && Dn(ut, g[Ne])) {
                             kt = Ne;
                             break
                         } kt === void 0 ? re(ut, D, j, !0) : (Sr[kt - se] = I + 1, kt >= cl ? cl = kt : Qn = !0, m(ut, g[kt], x, null, D, j, z, q, C), We++)
             }
             const fl = Qn ? bv(Sr) : er;
             for (Ne = fl.length - 1, I = Et - 1; I >= 0; I--) {
                 const ut = se + I,
@@ -2576,17 +2576,17 @@
         let _e;
         if (se && (_e = z && z.onVnodeBeforeUnmount) && At(_e, g, v), B & 6) qe(v.component, x, P);
         else {
             if (B & 128) {
                 v.suspense.unmount(x, P);
                 return
             }
-            ae && Sn(v, null, g, "beforeUnmount"), B & 64 ? v.type.remove(v, g, x, D, ee, P) : I && (j !== Ke || J > 0 && J & 64) ? fe(I, g, x, !1, !0) : (j === Ke && J & 384 || !D && B & 16) && fe(C, g, x), P && ve(v)
+            ae && xn(v, null, g, "beforeUnmount"), B & 64 ? v.type.remove(v, g, x, D, ee, P) : I && (j !== Ke || J > 0 && J & 64) ? fe(I, g, x, !1, !0) : (j === Ke && J & 384 || !D && B & 16) && fe(C, g, x), P && ve(v)
         }(se && (_e = z && z.onVnodeUnmounted) || ae) && st(() => {
-            _e && At(_e, g, v), ae && Sn(v, null, g, "unmounted")
+            _e && At(_e, g, v), ae && xn(v, null, g, "unmounted")
         }, x)
     }, ve = v => {
         const {
             type: g,
             el: x,
             anchor: P,
             transition: D
@@ -2654,15 +2654,15 @@
 function jo({
     type: e,
     props: t
 }, n) {
     return n === "svg" && e === "foreignObject" || n === "mathml" && e === "annotation-xml" && t && t.encoding && t.encoding.includes("html") ? void 0 : n
 }
 
-function xn({
+function On({
     effect: e,
     update: t
 }, n) {
     e.allowRecurse = t.allowRecurse = n
 }
 
 function gv(e, t) {
@@ -2841,15 +2841,15 @@
 const Ke = Symbol.for("v-fgt"),
     mo = Symbol.for("v-txt"),
     mt = Symbol.for("v-cmt"),
     Vo = Symbol.for("v-stc"),
     qr = [];
 let St = null;
 
-function Oe(e = !1) {
+function Te(e = !1) {
     qr.push(St = e ? null : [])
 }
 
 function Sv() {
     qr.pop(), St = qr[qr.length - 1] || null
 }
 let ei = 1;
@@ -2870,15 +2870,15 @@
     return Cf(me(e, t, n, r, i, !0))
 }
 
 function Gi(e) {
     return e ? e.__v_isVNode === !0 : !1
 }
 
-function In(e, t) {
+function Dn(e, t) {
     return e.type === t.type && e.key === t.key
 }
 const kf = ({
         key: e
     }) => e ?? null,
     Pi = ({
         ref: e,
@@ -2983,16 +2983,16 @@
     }
 }
 
 function Af(e = " ", t = 0) {
     return me(mo, null, e, t)
 }
 
-function w1(e = "", t = !1) {
-    return t ? (Oe(), Tt(mt, null, e)) : me(mt, null, e)
+function S1(e = "", t = !1) {
+    return t ? (Te(), Tt(mt, null, e)) : me(mt, null, e)
 }
 
 function It(e) {
     return e == null || typeof e == "boolean" ? me(mt) : le(e) ? me(Ke, null, e.slice()) : typeof e == "object" ? tn(e) : me(mo, null, String(e))
 }
 
 function tn(e) {
@@ -3156,17 +3156,17 @@
     e.accessCache = Object.create(null), e.proxy = new Proxy(e.ctx, nv);
     const {
         setup: r
     } = n;
     if (r) {
         const i = e.setupContext = r.length > 1 ? Nv(e) : null,
             o = fi(e);
-        _n();
-        const s = dn(r, e, 0, [e.props, i]);
-        if (wn(), o(), xc(s)) {
+        wn();
+        const s = hn(r, e, 0, [e.props, i]);
+        if (Sn(), o(), xc(s)) {
             if (s.then(Ll, Ll), t) return s.then(a => {
                 Ml(e, a, t)
             }).catch(a => {
                 co(a, e, 0)
             });
             e.asyncDep = s
         } else Ml(e, s, t)
@@ -3196,19 +3196,19 @@
                 }, s), l);
                 r.render = jl(i, u)
             }
         }
         e.render = r.render || pt
     } {
         const i = fi(e);
-        _n();
+        wn();
         try {
             rv(e)
         } finally {
-            wn(), i()
+            Sn(), i()
         }
     }
 }
 const Dv = {
     get(e, t) {
         return lt(e, "get", ""), e[t]
     }
@@ -3328,15 +3328,15 @@
     appearActiveClass: String,
     appearToClass: String,
     leaveFromClass: String,
     leaveActiveClass: String,
     leaveToClass: String
 };
 Na.props = Ue({}, af, Df);
-const On = (e, t = []) => {
+const Tn = (e, t = []) => {
         le(e) ? e.forEach(n => n(...t)) : e && e(...t)
     },
     $l = e => e ? le(e) ? e.some(t => t.length > 1) : e.length > 1 : !1;
 
 function $v(e) {
     const t = {};
     for (const V in e) V in Df || (t[V] = e[V]);
@@ -3360,48 +3360,48 @@
         onEnterCancelled: E,
         onLeave: S,
         onLeaveCancelled: T,
         onBeforeAppear: O = y,
         onAppear: F = _,
         onAppearCancelled: A = E
     } = t, R = (V, Y, he) => {
-        Tn(V, Y ? c : a), Tn(V, Y ? u : s), he && he()
+        Cn(V, Y ? c : a), Cn(V, Y ? u : s), he && he()
     }, M = (V, Y) => {
-        V._isLeaving = !1, Tn(V, d), Tn(V, h), Tn(V, f), Y && Y()
+        V._isLeaving = !1, Cn(V, d), Cn(V, h), Cn(V, f), Y && Y()
     }, ne = V => (Y, he) => {
         const H = V ? F : _,
             L = () => R(Y, V, he);
-        On(H, [Y, L]), ql(() => {
-            Tn(Y, V ? l : o), Kt(Y, V ? c : a), $l(H) || Bl(Y, r, m, L)
+        Tn(H, [Y, L]), ql(() => {
+            Cn(Y, V ? l : o), Kt(Y, V ? c : a), $l(H) || Bl(Y, r, m, L)
         })
     };
     return Ue(t, {
         onBeforeEnter(V) {
-            On(y, [V]), Kt(V, o), Kt(V, s)
+            Tn(y, [V]), Kt(V, o), Kt(V, s)
         },
         onBeforeAppear(V) {
-            On(O, [V]), Kt(V, l), Kt(V, u)
+            Tn(O, [V]), Kt(V, l), Kt(V, u)
         },
         onEnter: ne(!1),
         onAppear: ne(!0),
         onLeave(V, Y) {
             V._isLeaving = !0;
             const he = () => M(V, Y);
             Kt(V, d), Kt(V, f), Uv(), ql(() => {
-                V._isLeaving && (Tn(V, d), Kt(V, h), $l(S) || Bl(V, r, b, he))
-            }), On(S, [V, he])
+                V._isLeaving && (Cn(V, d), Kt(V, h), $l(S) || Bl(V, r, b, he))
+            }), Tn(S, [V, he])
         },
         onEnterCancelled(V) {
-            R(V, !1), On(E, [V])
+            R(V, !1), Tn(E, [V])
         },
         onAppearCancelled(V) {
-            R(V, !0), On(A, [V])
+            R(V, !0), Tn(A, [V])
         },
         onLeaveCancelled(V) {
-            M(V), On(T, [V])
+            M(V), Tn(T, [V])
         }
     })
 }
 
 function qv(e) {
     if (e == null) return null;
     if (De(e)) return [$o(e.enter), $o(e.leave)];
@@ -3415,15 +3415,15 @@
     return Hh(e)
 }
 
 function Kt(e, t) {
     t.split(/\s+/).forEach(n => n && e.classList.add(n)), (e[ti] || (e[ti] = new Set)).add(t)
 }
 
-function Tn(e, t) {
+function Cn(e, t) {
     t.split(/\s+/).forEach(r => r && e.classList.remove(r));
     const n = e[ti];
     n && (n.delete(t), n.size || (e[ti] = void 0))
 }
 
 function ql(e) {
     requestAnimationFrame(() => {
@@ -3753,15 +3753,15 @@
             n = arguments[r];
             for (var o in n) Object.prototype.hasOwnProperty.call(n, o) && (t[o] = n[o])
         }
         return t
     }, w.apply(this, arguments)
 };
 
-function vn(e, t) {
+function mn(e, t) {
     var n = {};
     for (var r in e) Object.prototype.hasOwnProperty.call(e, r) && t.indexOf(r) < 0 && (n[r] = e[r]);
     if (e != null && typeof Object.getOwnPropertySymbols == "function")
         for (var i = 0, r = Object.getOwnPropertySymbols(e); i < r.length; i++) t.indexOf(r[i]) < 0 && Object.prototype.propertyIsEnumerable.call(e, r[i]) && (n[r[i]] = e[r[i]]);
     return n
 }
 
@@ -3891,30 +3891,30 @@
             n === void 0 && (n = Qo);
             var r = e.call(this, typeof n == "number" ? Qo + ": " + n + " (see https://github.com/apollographql/invariant-packages)" : n) || this;
             return r.framesToPop = 1, r.name = Qo, pm(r, t.prototype), r
         }
         return t
     }(Error);
 
-function Dn(e, t) {
+function Nn(e, t) {
     if (!e) throw new Pf(t)
 }
 var Ff = ["debug", "log", "warn", "error", "silent"],
     vm = Ff.indexOf("log");
 
 function Ti(e) {
     return function() {
         if (Ff.indexOf(e) >= vm) {
             var t = console[e] || console.log;
             return t.apply(console, arguments)
         }
     }
 }(function(e) {
     e.debug = Ti("debug"), e.log = Ti("log"), e.warn = Ti("warn"), e.error = Ti("error")
-})(Dn || (Dn = {}));
+})(Nn || (Nn = {}));
 var Fa = "3.10.0";
 
 function wt(e) {
     try {
         return e()
     } catch {}
 }
@@ -3952,20 +3952,20 @@
             t = La(i), t || (t = Ma(i, n), n = [])
         }
         e.apply(void 0, [t].concat(n))
     }
 }
 var ce = Object.assign(function(t, n) {
     for (var r = [], i = 2; i < arguments.length; i++) r[i - 2] = arguments[i];
-    t || Dn(t, La(n, r) || Ma(n, r))
+    t || Nn(t, La(n, r) || Ma(n, r))
 }, {
-    debug: Ci(Dn.debug),
-    log: Ci(Dn.log),
-    warn: Ci(Dn.warn),
-    error: Ci(Dn.error)
+    debug: Ci(Nn.debug),
+    log: Ci(Nn.log),
+    warn: Ci(Nn.warn),
+    error: Ci(Nn.error)
 });
 
 function it(e) {
     for (var t = [], n = 1; n < arguments.length; n++) t[n - 1] = arguments[n];
     return new Pf(La(e, t) || Ma(e, t))
 }
 var tu = Symbol.for("ApolloErrorMessageHandler_" + Fa);
@@ -6147,18 +6147,18 @@
         var n = new Ds(e, t);
         return n.set = function(r, i) {
             return Jf(this), Ds.prototype.set.call(this, r, i)
         }, n
     },
     yy = Symbol.for("apollo.cacheSize"),
     Ut = w({}, Cs[yy]),
-    kn = {};
+    An = {};
 
 function Zf(e, t) {
-    kn[e] = t
+    An[e] = t
 }
 var gy = globalThis.__DEV__ !== !1 ? wy : void 0,
     by = globalThis.__DEV__ !== !1 ? Sy : void 0,
     Ey = globalThis.__DEV__ !== !1 ? ed : void 0;
 
 function _y() {
     var e = {
@@ -6186,17 +6186,17 @@
 
 function wy() {
     var e, t, n, r, i;
     if (globalThis.__DEV__ === !1) throw new Error("only supported in development mode");
     return {
         limits: _y(),
         sizes: w({
-            print: (e = kn.print) === null || e === void 0 ? void 0 : e.call(kn),
-            parser: (t = kn.parser) === null || t === void 0 ? void 0 : t.call(kn),
-            canonicalStringify: (n = kn.canonicalStringify) === null || n === void 0 ? void 0 : n.call(kn),
+            print: (e = An.print) === null || e === void 0 ? void 0 : e.call(An),
+            parser: (t = An.parser) === null || t === void 0 ? void 0 : t.call(An),
+            canonicalStringify: (n = An.canonicalStringify) === null || n === void 0 ? void 0 : n.call(An),
             links: Fs(this.link),
             queryManager: {
                 getDocumentInfo: this.queryManager.transformCache.size,
                 documentTransforms: nd(this.queryManager.documentTransform)
             }
         }, (i = (r = this.cache).getMemoryInternals) === null || i === void 0 ? void 0 : i.call(r))
     }
@@ -6251,26 +6251,26 @@
     return e ? xt(xt([sn(e == null ? void 0 : e.performWork)], Ps(e == null ? void 0 : e.left), !0), Ps(e == null ? void 0 : e.right), !0).filter(td) : []
 }
 
 function Fs(e) {
     var t;
     return e ? xt(xt([(t = e == null ? void 0 : e.getMemoryInternals) === null || t === void 0 ? void 0 : t.call(e)], Fs(e == null ? void 0 : e.left), !0), Fs(e == null ? void 0 : e.right), !0).filter(td) : []
 }
-var hn = Object.assign(function(t) {
+var pn = Object.assign(function(t) {
     return JSON.stringify(t, Oy)
 }, {
     reset: function() {
         Yn = new my(Ut.canonicalStringify || 1e3)
     }
 });
 globalThis.__DEV__ !== !1 && Zf("canonicalStringify", function() {
     return Yn.size
 });
 var Yn;
-hn.reset();
+pn.reset();
 
 function Oy(e, t) {
     if (t && typeof t == "object") {
         var n = Object.getPrototypeOf(t);
         if (n === Object.prototype || n === null) {
             var r = Object.keys(t);
             if (r.every(Ty)) return t;
@@ -6377,15 +6377,15 @@
     return e.arguments && e.arguments.length && (r = {}, e.arguments.forEach(function(i) {
         var o = i.name,
             s = i.value;
         return ur(r, o, s, t)
     })), rd(e.name.value, r, n)
 }
 var jy = ["connection", "include", "skip", "client", "rest", "export", "nonreactive"],
-    Or = hn,
+    Or = pn,
     rd = Object.assign(function(e, t, n) {
         if (t && n && n.connection && n.connection.key)
             if (n.connection.filter && n.connection.filter.length > 0) {
                 var r = n.connection.filter ? n.connection.filter : [];
                 r.sort();
                 var i = {};
                 return r.forEach(function(a) {
@@ -6415,35 +6415,35 @@
                 o = r.value;
             return ur(n, i, o, t)
         }), n
     }
     return null
 }
 
-function mn(e) {
+function yn(e) {
     return e.alias ? e.alias.value : e.name.value
 }
 
 function Ls(e, t, n) {
     for (var r, i = 0, o = t.selections; i < o.length; i++) {
         var s = o[i];
-        if (yn(s)) {
-            if (s.name.value === "__typename") return e[mn(s)]
+        if (gn(s)) {
+            if (s.name.value === "__typename") return e[yn(s)]
         } else r ? r.push(s) : r = [s]
     }
     if (typeof e.__typename == "string") return e.__typename;
     if (r)
         for (var a = 0, l = r; a < l.length; a++) {
             var s = l[a],
                 u = Ls(e, wo(s, n).selectionSet, n);
             if (typeof u == "string") return u
         }
 }
 
-function yn(e) {
+function gn(e) {
     return e.kind === "Field"
 }
 
 function Vy(e) {
     return e.kind === "InlineFragment"
 }
 
@@ -6675,18 +6675,18 @@
     return e.slice(0)
 }
 class To {
     constructor(t) {
         this.fn = t, this.parents = new Set, this.childValues = new Map, this.dirtyChildren = null, this.dirty = !0, this.recomputing = !1, this.value = [], this.deps = null, ++To.count
     }
     peek() {
-        if (this.value.length === 1 && !gn(this)) return hu(this), this.value[0]
+        if (this.value.length === 1 && !bn(this)) return hu(this), this.value[0]
     }
     recompute(t) {
-        return cr(!this.recomputing, "already recomputing"), hu(this), gn(this) ? Yy(this, t) : ad(this.value)
+        return cr(!this.recomputing, "already recomputing"), hu(this), bn(this) ? Yy(this, t) : ad(this.value)
     }
     setDirty() {
         this.dirty || (this.dirty = !0, ud(this), Ji(this))
     }
     dispose() {
         this.setDirty(), pd(this), Ua(this, (t, n) => {
             t.setDirty(), vd(t, this)
@@ -6702,15 +6702,15 @@
         this.deps && (Qa(this.deps).forEach(t => t.delete(this)), this.deps.clear(), ii.push(this.deps), this.deps = null)
     }
 }
 To.count = 0;
 
 function hu(e) {
     const t = Oo.getValue();
-    if (t) return e.parents.add(t), t.childValues.has(e) || t.childValues.set(e, []), gn(e) ? fd(t, e) : dd(t, e), t
+    if (t) return e.parents.add(t), t.childValues.has(e) || t.childValues.set(e, []), bn(e) ? fd(t, e) : dd(t, e), t
 }
 
 function Yy(e, t) {
     return pd(e), Oo.withValue(e, Jy, [e, t]), Zy(e, t) && Xy(e), ad(e.value)
 }
 
 function Jy(e, t) {
@@ -6726,20 +6726,20 @@
         } catch {}
     } catch (i) {
         e.value[1] = i
     }
     e.recomputing = !1
 }
 
-function gn(e) {
+function bn(e) {
     return e.dirty || !!(e.dirtyChildren && e.dirtyChildren.size)
 }
 
 function Xy(e) {
-    e.dirty = !1, !gn(e) && cd(e)
+    e.dirty = !1, !bn(e) && cd(e)
 }
 
 function ud(e) {
     Ua(e, fd)
 }
 
 function cd(e) {
@@ -6751,25 +6751,25 @@
     if (n) {
         const r = Qa(e.parents);
         for (let i = 0; i < n; ++i) t(r[i], e)
     }
 }
 
 function fd(e, t) {
-    cr(e.childValues.has(t)), cr(gn(t));
-    const n = !gn(e);
+    cr(e.childValues.has(t)), cr(bn(t));
+    const n = !bn(e);
     if (!e.dirtyChildren) e.dirtyChildren = ii.pop() || new Set;
     else if (e.dirtyChildren.has(t)) return;
     e.dirtyChildren.add(t), n && ud(e)
 }
 
 function dd(e, t) {
-    cr(e.childValues.has(t)), cr(!gn(t));
+    cr(e.childValues.has(t)), cr(!bn(t));
     const n = e.childValues.get(t);
-    n.length === 0 ? e.childValues.set(t, ld(t.value)) : sd(n, t.value) || e.setDirty(), hd(e, t), !gn(e) && cd(e)
+    n.length === 0 ? e.childValues.set(t, ld(t.value)) : sd(n, t.value) || e.setDirty(), hd(e, t), !bn(e) && cd(e)
 }
 
 function hd(e, t) {
     const n = e.dirtyChildren;
     n && (n.delete(t), n.size === 0 && (ii.length < Ky && ii.push(n), e.dirtyChildren = null))
 }
 
@@ -7102,19 +7102,19 @@
     return Qt(e, {
         SelectionSet: {
             enter: function(t, n, r) {
                 if (!(r && r.kind === X.OPERATION_DEFINITION)) {
                     var i = t.selections;
                     if (i) {
                         var o = i.some(function(a) {
-                            return yn(a) && (a.name.value === "__typename" || a.name.value.lastIndexOf("__", 0) === 0)
+                            return gn(a) && (a.name.value === "__typename" || a.name.value.lastIndexOf("__", 0) === 0)
                         });
                         if (!o) {
                             var s = r;
-                            if (!(yn(s) && s.directives && s.directives.some(function(a) {
+                            if (!(gn(s) && s.directives && s.directives.some(function(a) {
                                     return a.name.value === "export"
                                 }))) return w(w({}, t), {
                                 selections: xt(xt([], i, !0), [vu], !1)
                             })
                         }
                     }
                 }
@@ -7160,21 +7160,21 @@
     return Co(e)
 }
 
 function Co(e) {
     var t = e[0] || {},
         n = e.length;
     if (n > 1)
-        for (var r = new bn, i = 1; i < n; ++i) t = r.merge(t, e[i]);
+        for (var r = new En, i = 1; i < n; ++i) t = r.merge(t, e[i]);
     return t
 }
 var ag = function(e, t, n) {
         return this.merge(e[n], t[n])
     },
-    bn = function() {
+    En = function() {
         function e(t) {
             t === void 0 && (t = ag), this.reconciler = t, this.isObject = Fe, this.pastCopies = new Set
         }
         return e.prototype.merge = function(t, n) {
             for (var r = this, i = [], o = 2; o < arguments.length; o++) i[o - 2] = arguments[o];
             return Fe(n) && Fe(t) ? (Object.keys(n).forEach(function(s) {
                 if (sg.call(t, s)) {
@@ -7258,19 +7258,19 @@
         if (typeof n != "function") throw new TypeError(n + " is not a function");
         return n
     }
 }
 
 function Tr(e) {
     var t = e.constructor;
-    return t !== void 0 && (t = t[_d], t === null && (t = void 0)), t !== void 0 ? t : Ce
+    return t !== void 0 && (t = t[_d], t === null && (t = void 0)), t !== void 0 ? t : ke
 }
 
 function fg(e) {
-    return e instanceof Ce
+    return e instanceof ke
 }
 
 function fr(e) {
     fr.log ? fr.log(e) : setTimeout(function() {
         throw e
     })
 }
@@ -7389,15 +7389,15 @@
         }, Wa(e, [{
             key: "closed",
             get: function() {
                 return this._subscription._state === "closed"
             }
         }]), e
     }(),
-    Ce = function() {
+    ke = function() {
         function e(n) {
             if (!(this instanceof e)) throw new TypeError("Observable cannot be called as a function");
             if (typeof n != "function") throw new TypeError("Observable initializer must be a function");
             this._subscriber = n
         }
         var t = e.prototype;
         return t.subscribe = function(r) {
@@ -7617,15 +7617,15 @@
         }, Wa(e, null, [{
             key: _d,
             get: function() {
                 return this
             }
         }]), e
     }();
-Ha() && Object.defineProperty(Ce, Symbol("extensions"), {
+Ha() && Object.defineProperty(ke, Symbol("extensions"), {
     value: {
         symbol: js,
         hostReportError: fr
     },
     configurable: !0
 });
 
@@ -7641,15 +7641,15 @@
         }
     else t = "@@observable";
     return t
 }
 var zn;
 typeof self < "u" ? zn = self : typeof window < "u" ? zn = window : typeof global < "u" ? zn = global : typeof module < "u" ? zn = module : zn = Function("return this")();
 vg(zn);
-var Eu = Ce.prototype,
+var Eu = ke.prototype,
     _u = "@@observable";
 Eu[_u] || (Eu[_u] = function() {
     return this
 });
 var mg = Object.prototype.toString;
 
 function xd(e) {
@@ -7706,15 +7706,15 @@
         return i[t] && r.push(i)
     }), r.forEach(function(i) {
         return i[t](n)
     })
 }
 
 function Ko(e, t, n) {
-    return new Ce(function(r) {
+    return new ke(function(r) {
         var i = {
             then: function(l) {
                 return new Promise(function(u) {
                     return u(l())
                 })
             }
         };
@@ -7748,15 +7748,15 @@
         }
     })
 }
 
 function Od(e) {
     function t(n) {
         Object.defineProperty(e, n, {
-            value: Ce
+            value: ke
         })
     }
     return Yf && Symbol.species && t(Symbol.species), t("@@species"), e
 }
 
 function wu(e) {
     return e && typeof e.then == "function"
@@ -7795,15 +7795,15 @@
                     }, r.handlers.error) : r.sub = l.subscribe(r.handlers) : (o && setTimeout(function() {
                         return o.unsubscribe()
                     }), r.sub = null, r.latest && r.latest[0] === "next" ? r.resolve(r.latest[1]) : r.resolve(), r.notify("complete"), Qr(r.observers, "complete"))
                 }
             }
         }, r.nextResultListeners = new Set, r.cancel = function(i) {
             r.reject(i), r.sources = [], r.handlers.complete()
-        }, r.promise.catch(function(i) {}), typeof n == "function" && (n = [new Ce(n)]), wu(n) ? n.then(function(i) {
+        }, r.promise.catch(function(i) {}), typeof n == "function" && (n = [new ke(n)]), wu(n) ? n.then(function(i) {
             return r.start(i)
         }, r.handlers.error) : r.start(n), r
     }
     return t.prototype.start = function(n) {
         this.sub === void 0 && (this.sources = Array.from(n), this.handlers.complete())
     }, t.prototype.deliverLastMessage = function(n) {
         if (this.latest) {
@@ -7822,15 +7822,15 @@
         }))
     }, t.prototype.beforeNext = function(n) {
         var r = !1;
         this.nextResultListeners.add(function(i, o) {
             r || (r = !0, n(i, o))
         })
     }, t
-}(Ce);
+}(ke);
 Od(Wn);
 
 function or(e) {
     return "incremental" in e
 }
 
 function bg(e) {
@@ -7843,15 +7843,15 @@
 
 function _g(e) {
     return Fe(e) && "payload" in e
 }
 
 function Td(e, t) {
     var n = e,
-        r = new bn;
+        r = new En;
     return or(t) && Ft(t.incremental) && t.incremental.forEach(function(i) {
         for (var o = i.data, s = i.path, a = s.length - 1; a >= 0; --a) {
             var l = s[a],
                 u = !isNaN(+l),
                 c = u ? [] : {};
             c[l] = o, o = c
         }
@@ -7885,15 +7885,15 @@
 function Yo(e, t) {
     return dr(e, t, t.variables && {
         variables: dr(w(w({}, e && e.variables), t.variables))
     })
 }
 
 function Jo(e) {
-    return new Ce(function(t) {
+    return new ke(function(t) {
         t.error(e)
     })
 }
 var Cd = function(e, t, n) {
     var r = new Error(n);
     throw r.name = "ServerError", r.response = e, r.statusCode = e.status, r.result = t, r
 };
@@ -7942,15 +7942,15 @@
         }
     }), r.forEach(function(i) {
         delete n[i]
     }), n
 }
 
 function Su(e, t) {
-    return t ? t(e) : Ce.of()
+    return t ? t(e) : ke.of()
 }
 
 function Cr(e) {
     return typeof e == "function" ? new Mt(e) : e
 }
 
 function Ai(e) {
@@ -7958,47 +7958,47 @@
 }
 var Mt = function() {
         function e(t) {
             t && (this.request = t)
         }
         return e.empty = function() {
             return new e(function() {
-                return Ce.of()
+                return ke.of()
             })
         }, e.from = function(t) {
             return t.length === 0 ? e.empty() : t.map(Cr).reduce(function(n, r) {
                 return n.concat(r)
             })
         }, e.split = function(t, n, r) {
             var i = Cr(n),
                 o = Cr(r || new e(Su)),
                 s;
             return Ai(i) && Ai(o) ? s = new e(function(a) {
-                return t(a) ? i.request(a) || Ce.of() : o.request(a) || Ce.of()
+                return t(a) ? i.request(a) || ke.of() : o.request(a) || ke.of()
             }) : s = new e(function(a, l) {
-                return t(a) ? i.request(a, l) || Ce.of() : o.request(a, l) || Ce.of()
+                return t(a) ? i.request(a, l) || ke.of() : o.request(a, l) || ke.of()
             }), Object.assign(s, {
                 left: i,
                 right: o
             })
         }, e.execute = function(t, n) {
-            return t.request(Sg(n.context, xg(wg(n)))) || Ce.of()
+            return t.request(Sg(n.context, xg(wg(n)))) || ke.of()
         }, e.concat = function(t, n) {
             var r = Cr(t);
             if (Ai(r)) return globalThis.__DEV__ !== !1 && ce.warn(35, r), r;
             var i = Cr(n),
                 o;
             return Ai(i) ? o = new e(function(s) {
                 return r.request(s, function(a) {
-                    return i.request(a) || Ce.of()
-                }) || Ce.of()
+                    return i.request(a) || ke.of()
+                }) || ke.of()
             }) : o = new e(function(s, a) {
                 return r.request(s, function(l) {
-                    return i.request(l, a) || Ce.of()
-                }) || Ce.of()
+                    return i.request(l, a) || ke.of()
+                }) || ke.of()
             }), Object.assign(o, {
                 left: r,
                 right: i
             })
         }, e.prototype.split = function(t, n, r) {
             return this.concat(e.split(t, n, r || new e(Su)))
         }, e.prototype.concat = function(t) {
@@ -8407,15 +8407,15 @@
             i = e.print,
             o = i === void 0 ? Hg : i,
             s = e.includeExtensions,
             a = e.preserveHeaderCase,
             l = e.useGETForQueries,
             u = e.includeUnusedVariables,
             c = u === void 0 ? !1 : u,
-            d = vn(e, ["uri", "fetch", "print", "includeExtensions", "preserveHeaderCase", "useGETForQueries", "includeUnusedVariables"]);
+            d = mn(e, ["uri", "fetch", "print", "includeExtensions", "preserveHeaderCase", "useGETForQueries", "includeUnusedVariables"]);
         globalThis.__DEV__ !== !1 && Yg(r || Tu);
         var f = {
             http: {
                 includeExtensions: s,
                 preserveHeaderCase: a
             },
             options: d.fetchOptions,
@@ -8470,15 +8470,15 @@
                 if (U) return Jo(U);
                 p = $
             } else try {
                 A.body = Us(R, "Payload")
             } catch (ie) {
                 return Jo(ie)
             }
-            return new Ce(function(ie) {
+            return new ke(function(ie) {
                 var we = r || wt(function() {
                         return fetch
                     }) || Tu,
                     G = ie.next.bind(ie);
                 return we(p, A).then(function(re) {
                         var ve;
                         h.setContext({
@@ -8651,15 +8651,15 @@
             l = {
                 returnPartialData: !0,
                 id: typeof o == "string" ? o : this.identify(o),
                 query: this.getFragmentDoc(r, i),
                 optimistic: a
             },
             u;
-        return new Ce(function(c) {
+        return new ke(function(c) {
             return n.watch(w(w({}, l), {
                 immediate: !0,
                 query: n.getFragmentDoc(r, i),
                 callback: function(d) {
                     if (!Re(d, u)) {
                         var f = {
                             data: d.result,
@@ -8677,25 +8677,25 @@
             query: this.getFragmentDoc(t.fragment, t.fragmentName),
             rootId: t.id,
             optimistic: n
         }))
     }, e.prototype.writeQuery = function(t) {
         var n = t.id,
             r = t.data,
-            i = vn(t, ["id", "data"]);
+            i = mn(t, ["id", "data"]);
         return this.write(Object.assign(i, {
             dataId: n || "ROOT_QUERY",
             result: r
         }))
     }, e.prototype.writeFragment = function(t) {
         var n = t.id,
             r = t.data,
             i = t.fragment,
             o = t.fragmentName,
-            s = vn(t, ["id", "data", "fragment", "fragmentName"]);
+            s = mn(t, ["id", "data", "fragment", "fragmentName"]);
         return this.write(Object.assign(s, {
             query: this.getFragmentDoc(i, o),
             dataId: n,
             result: r
         }))
     }, e.prototype.updateQuery = function(t, n) {
         return this.batch({
@@ -8766,37 +8766,37 @@
 }
 
 function o0(e, t) {
     return Se(t) ? e.get(t.__ref, "__typename") : t && t.__typename
 }
 var Ld = /^[_a-z][_0-9a-z]*/i;
 
-function En(e) {
+function _n(e) {
     var t = e.match(Ld);
     return t ? t[0] : e
 }
 
 function Hs(e, t, n) {
     return Fe(t) ? Me(t) ? t.every(function(r) {
         return Hs(e, r, n)
     }) : e.selections.every(function(r) {
-        if (yn(r) && di(r, n)) {
-            var i = mn(r);
+        if (gn(r) && di(r, n)) {
+            var i = yn(r);
             return He.call(t, i) && (!r.selectionSet || Hs(r.selectionSet, t[i], n))
         }
         return !0
     }) : !1
 }
 
 function Jn(e) {
     return Fe(e) && !Se(e) && !Me(e)
 }
 
 function s0() {
-    return new bn
+    return new En
 }
 
 function Md(e, t) {
     var n = _o(xo(e));
     return {
         fragmentMap: n,
         lookupFragment: function(r) {
@@ -8846,21 +8846,21 @@
             var r = this,
                 i;
             Se(t) && (t = t.__ref), Se(n) && (n = n.__ref);
             var o = typeof t == "string" ? this.lookup(i = t) : t,
                 s = typeof n == "string" ? this.lookup(i = n) : n;
             if (s) {
                 ce(typeof i == "string", 1);
-                var a = new bn(l0).merge(o, s);
+                var a = new En(l0).merge(o, s);
                 if (this.data[i] = a, a !== o && (delete this.refs[i], this.group.caching)) {
                     var l = Object.create(null);
                     o || (l.__exists = 1), Object.keys(s).forEach(function(u) {
                         if (!o || o[u] !== a[u]) {
                             l[u] = 1;
-                            var c = En(u);
+                            var c = _n(u);
                             c !== u && !r.policies.hasKeyArgs(a.__typename, c) && (l[c] = 1), a[u] === void 0 && !(r instanceof Jt) && delete a[u]
                         }
                     }), l.__typename && !(o && o.__typename) && this.policies.rootTypenamesById[i] === a.__typename && delete l.__typename, Object.keys(l).forEach(function(u) {
                         return r.group.dirty(i, u)
                     })
                 }
             }
@@ -8883,15 +8883,15 @@
                                 from: c || ir(t)
                             } : u, {
                                 store: r
                             })
                         }
                     };
                 if (Object.keys(i).forEach(function(u) {
-                        var c = En(u),
+                        var c = _n(u),
                             d = i[u];
                         if (d !== void 0) {
                             var f = typeof n == "function" ? n : n[u] || n[c];
                             if (f) {
                                 var h = f === Xo ? $i : f(qs(d), w(w({}, l), {
                                     fieldName: c,
                                     storeFieldName: u,
@@ -8952,15 +8952,15 @@
             }), n
         }, e.prototype.replace = function(t) {
             var n = this;
             if (Object.keys(this.data).forEach(function(o) {
                     t && He.call(t, o) || n.delete(o)
                 }), t) {
                 var r = t.__META,
-                    i = vn(t, ["__META"]);
+                    i = mn(t, ["__META"]);
                 Object.keys(i).forEach(function(o) {
                     n.merge(o, i[o])
                 }), r && r.extraRootIds.forEach(this.retain, this)
             }
         }, e.prototype.retain = function(t) {
             return this.rootIds[t] = (this.rootIds[t] || 0) + 1
         }, e.prototype.release = function(t) {
@@ -9009,15 +9009,15 @@
             n === void 0 && (n = null), this.caching = t, this.parent = n, this.d = null, this.resetCaching()
         }
         return e.prototype.resetCaching = function() {
             this.d = this.caching ? md() : null, this.keyMaker = new br(Er)
         }, e.prototype.depend = function(t, n) {
             if (this.d) {
                 this.d(Zo(t, n));
-                var r = En(n);
+                var r = _n(n);
                 r !== n && this.d(Zo(t, r)), this.parent && this.parent.depend(t, n)
             }
         }, e.prototype.dirty = function(t, n) {
             this.d && this.d.dirty(Zo(t, n), n === "__exists" ? "forget" : "setDirty")
         }, e
     }();
 
@@ -9226,15 +9226,15 @@
                 objectOrReference: f,
                 enclosingRef: f,
                 context: w({
                     store: n,
                     query: r,
                     policies: d,
                     variables: s,
-                    varString: hn(s),
+                    varString: pn(s),
                     canonizeResults: c
                 }, Md(r, this.config.fragments))
             }),
             p;
         if (h.missing && (p = [new Dd(f0(h.missing), h.missing, r, s)], !l)) throw p[0];
         return {
             result: h.result,
@@ -9258,35 +9258,35 @@
             missing: "Dangling reference to missing ".concat(i.__ref, " object")
         };
         var a = s.variables,
             l = s.policies,
             u = s.store,
             c = u.getFieldValue(i, "__typename"),
             d = [],
-            f, h = new bn;
+            f, h = new En;
         this.config.addTypename && typeof c == "string" && !l.rootIdsByTypename[c] && d.push({
             __typename: c
         });
 
         function p(E, S) {
             var T;
             return E.missing && (f = h.merge(f, (T = {}, T[S] = E.missing, T))), E.result
         }
         var m = new Set(r.selections);
         m.forEach(function(E) {
             var S, T;
             if (di(E, a))
-                if (yn(E)) {
+                if (gn(E)) {
                     var O = l.readField({
                             fieldName: E.name.value,
                             field: E,
                             variables: s.variables,
                             from: i
                         }, s),
-                        F = mn(E);
+                        F = yn(E);
                     O === void 0 ? za.added(E) || (f = h.merge(f, (S = {}, S[F] = "Can't find field '".concat(E.name.value, "' on ").concat(Se(i) ? i.__ref + " object" : "object " + JSON.stringify(i, null, 2)), S))) : Me(O) ? O.length > 0 && (O = p(n.executeSubSelectedArray({
                         field: E,
                         array: O,
                         enclosingRef: o,
                         context: s
                     }), F)) : E.selectionSet ? O != null && (O = p(n.executeSelectionSet({
                         selectionSet: E.selectionSet,
@@ -9309,15 +9309,15 @@
         return _.result && this.knownResults.set(_.result, r), _
     }, e.prototype.execSubSelectedArrayImpl = function(t) {
         var n = this,
             r = t.field,
             i = t.array,
             o = t.enclosingRef,
             s = t.context,
-            a, l = new bn;
+            a, l = new En;
 
         function u(c, d) {
             var f;
             return c.missing && (a = l.merge(a, (f = {}, f[d] = c.missing, f))), c.result
         }
         return r.selectionSet && (i = i.filter(s.store.canRead)), i = i.map(function(c, d) {
             return c === null ? null : Me(c) ? u(n.executeSubSelectedArray({
@@ -9470,15 +9470,15 @@
             }),
             l = JSON.stringify(a);
         return (n || l !== "{}") && (s += ":" + l), s
     })
 }
 
 function Za(e, t) {
-    var n = new bn;
+    var n = new En;
     return Vd(e).reduce(function(r, i) {
         var o, s = t(i);
         if (s !== void 0) {
             for (var a = i.length - 1; a >= 0; --a) s = (o = {}, o[i[a]] = s, o);
             r = n.merge(r, s)
         }
         return r
@@ -9563,15 +9563,15 @@
         }, e.prototype.addTypePolicies = function(t) {
             var n = this;
             Object.keys(t).forEach(function(r) {
                 var i = t[r],
                     o = i.queryType,
                     s = i.mutationType,
                     a = i.subscriptionType,
-                    l = vn(i, ["queryType", "mutationType", "subscriptionType"]);
+                    l = mn(i, ["queryType", "mutationType", "subscriptionType"]);
                 o && n.setRootTypename("Query", r), s && n.setRootTypename("Mutation", r), a && n.setRootTypename("Subscription", r), He.call(n.toBeAdded, r) ? n.toBeAdded[r].push(l) : n.toBeAdded[r] = [l]
             })
         }, e.prototype.updateTypePolicy = function(t, n) {
             var r = this,
                 i = this.getTypePolicy(t),
                 o = n.keyFields,
                 s = n.fields;
@@ -9617,15 +9617,15 @@
                         l && l.forEach(function(u) {
                             return i.add(u)
                         })
                     }
                 })), i && i.size && i.forEach(function(s) {
                     var a = n.getTypePolicy(s),
                         l = a.fields,
-                        u = vn(a, ["fields"]);
+                        u = mn(a, ["fields"]);
                     Object.assign(r, u), Object.assign(r.fields, l)
                 })
             }
             var o = this.toBeAdded[t];
             return o && o.length && o.splice(0).forEach(function(s) {
                 n.updateTypePolicy(t, s)
             }), this.typePolicies[t]
@@ -9674,26 +9674,26 @@
                     var u = s(l, a);
                     if (Me(u)) s = Vu(u);
                     else {
                         o = u || r;
                         break
                     }
                 }
-            return o === void 0 && (o = t.field ? My(t.field, t.variables) : rd(r, Gs(t))), o === !1 ? r : r === En(o) ? o : r + ":" + o
+            return o === void 0 && (o = t.field ? My(t.field, t.variables) : rd(r, Gs(t))), o === !1 ? r : r === _n(o) ? o : r + ":" + o
         }, e.prototype.readField = function(t, n) {
             var r = t.from;
             if (r) {
                 var i = t.field || t.fieldName;
                 if (i) {
                     if (t.typename === void 0) {
                         var o = n.store.getFieldValue(r, "__typename");
                         o && (t.typename = o)
                     }
                     var s = this.getStoreFieldName(t),
-                        a = En(s),
+                        a = _n(s),
                         l = n.store.getFieldValue(r, s),
                         u = this.getFieldPolicy(t.typename, a, !1),
                         c = u && u.read;
                     if (c) {
                         var d = Qu(this, r, t, n, n.store.getStorage(Se(r) ? r.__ref : r, s));
                         return Ja.withValue(this.cache, c, [l, d])
                     }
@@ -9718,15 +9718,15 @@
                 variables: i.variables
             }, i, o || Object.create(null))))
         }, e
     }();
 
 function Qu(e, t, n, r, i) {
     var o = e.getStoreFieldName(n),
-        s = En(o),
+        s = _n(o),
         a = n.variables || r.variables,
         l = r.store,
         u = l.toReference,
         c = l.canRead;
     return {
         args: Gs(n),
         field: n.field || null,
@@ -9797,15 +9797,15 @@
             var d = w(w({
                     store: t,
                     written: Object.create(null),
                     merge: function(h, p) {
                         return c.merge(h, p)
                     },
                     variables: a,
-                    varString: hn(a)
+                    varString: pn(a)
                 }, Md(i, this.fragments)), {
                     overwrite: !!l,
                     incomingById: new Map,
                     clientOnly: !1,
                     deferred: !1,
                     flavors: new Map
                 }),
@@ -9831,15 +9831,15 @@
                 }
                 if (globalThis.__DEV__ !== !1 && !d.overwrite) {
                     var S = Object.create(null);
                     y.forEach(function(F) {
                         F.selectionSet && (S[F.name.value] = !0)
                     });
                     var T = function(F) {
-                            return S[En(F)] === !0
+                            return S[_n(F)] === !0
                         },
                         O = function(F) {
                             var A = b && b.map.get(F);
                             return !!(A && A.info && A.info.merge)
                         };
                     Object.keys(m).forEach(function(F) {
                         T(F) && !O(F) && b0(_, m, F, d.store)
@@ -9869,15 +9869,15 @@
                             if (T !== void 0) return T
                         }
                     }
                     return l.readField(E, s)
                 },
                 f = new Set;
             this.flattenFields(o, i, s, c).forEach(function(E, S) {
-                var T, O = mn(S),
+                var T, O = yn(S),
                     F = i[O];
                 if (f.add(S), F !== void 0) {
                     var A = l.getStoreFieldName({
                             typename: c,
                             fieldName: S.name.value,
                             field: S,
                             variables: E.variables
@@ -9888,15 +9888,15 @@
                     S.selectionSet && (Se(M) || Jn(M)) && (ne = d("__typename", M));
                     var V = l.getMergeFunction(c, S.name.value, ne);
                     V ? R.info = {
                         field: S,
                         typename: c,
                         merge: V
                     } : zu(a, A), u = E.merge(u, (T = {}, T[A] = M, T))
-                } else globalThis.__DEV__ !== !1 && !E.clientOnly && !E.deferred && !za.added(S) && !l.getReadFunction(c, S.name.value) && globalThis.__DEV__ !== !1 && ce.error(12, mn(S), i)
+                } else globalThis.__DEV__ !== !1 && !E.clientOnly && !E.deferred && !za.added(S) && !l.getReadFunction(c, S.name.value) && globalThis.__DEV__ !== !1 && ce.error(12, yn(S), i)
             });
             try {
                 var h = l.identify(i, {
                         typename: c,
                         selectionSet: o,
                         fragmentMap: s.fragmentMap,
                         storeObject: u,
@@ -9946,15 +9946,15 @@
                             p = c.deferred;
                         if (!(h && p) && Ft(f.directives) && f.directives.forEach(function(y) {
                                 var _ = y.name.value;
                                 if (_ === "client" && (h = !0), _ === "defer") {
                                     var E = So(y, r.variables);
                                     (!E || E.if !== !1) && (p = !0)
                                 }
-                            }), yn(f)) {
+                            }), gn(f)) {
                             var m = o.get(f);
                             m && (h = h && m.clientOnly, p = p && m.deferred), o.set(f, es(r, h, p))
                         } else {
                             var b = wo(f, r.lookupFragment);
                             if (!b && f.kind === X.FRAGMENT_SPREAD) throw it(13, f.name.value);
                             b && s.fragmentMatches(b, i, n, r.variables) && l(b.selectionSet, es(r, h, p))
                         }
@@ -10034,15 +10034,15 @@
         o = i(e);
     if (o) {
         var s = i(t);
         if (s && !Se(o) && !Re(o, s) && !Object.keys(o).every(function(d) {
                 return r.getFieldValue(s, d) !== void 0
             })) {
             var a = r.getFieldValue(e, "__typename") || r.getFieldValue(t, "__typename"),
-                l = En(n),
+                l = _n(n),
                 u = "".concat(a, ".").concat(l);
             if (!Wu.has(u)) {
                 Wu.add(u);
                 var c = [];
                 !Me(o) && !Me(s) && [o, s].forEach(function(d) {
                     var f = r.getFieldValue(d, "__typename");
                     typeof f == "string" && !c.includes(f) && c.push(f)
@@ -10087,15 +10087,15 @@
             max: this.config.resultCacheMaxSize || Ut["inMemoryCache.maybeBroadcastWatch"] || 5e3,
             makeCacheKey: function(s) {
                 var a = s.optimistic ? r.optimisticData : r.data;
                 if (Ur(a)) {
                     var l = s.optimistic,
                         u = s.id,
                         c = s.variables;
-                    return a.makeCacheKey(s.query, s.callback, hn({
+                    return a.makeCacheKey(s.query, s.callback, pn({
                         optimistic: l,
                         id: u,
                         variables: c
                     }))
                 }
             }
         }), new Set([this.data.group, this.optimisticData.group]).forEach(function(s) {
@@ -10142,15 +10142,15 @@
         var r = this;
         return this.watches.size || h0(this), this.watches.add(n), n.immediate && this.maybeBroadcastWatch(n),
             function() {
                 r.watches.delete(n) && !r.watches.size && Lu(r), r.maybeBroadcastWatch.forget(n)
             }
     }, t.prototype.gc = function(n) {
         var r;
-        hn.reset(), vi.reset(), this.addTypenameTransform.resetCache(), (r = this.config.fragments) === null || r === void 0 || r.resetCaches();
+        pn.reset(), vi.reset(), this.addTypenameTransform.resetCache(), (r = this.config.fragments) === null || r === void 0 || r.resetCaches();
         var i = this.optimisticData.gc();
         return n && !this.txCount && (n.resetResultCache ? this.resetResultCache(n.resetResultIdentities) : n.resetResultIdentities && this.storeReader.resetCanon()), i
     }, t.prototype.retain = function(n, r) {
         return (r ? this.optimisticData : this.data).retain(n)
     }, t.prototype.release = function(n, r) {
         return (r ? this.optimisticData : this.data).release(n)
     }, t.prototype.identify = function(n) {
@@ -10170,15 +10170,15 @@
         try {
             return ++this.txCount, this.optimisticData.evict(n, this.data)
         } finally {
             !--this.txCount && n.broadcast !== !1 && this.broadcastWatches()
         }
     }, t.prototype.reset = function(n) {
         var r = this;
-        return this.init(), hn.reset(), n && n.discardWatches ? (this.watches.forEach(function(i) {
+        return this.init(), pn.reset(), n && n.discardWatches ? (this.watches.forEach(function(i) {
             return r.maybeBroadcastWatch.forget(i)
         }), this.watches.clear(), Lu(this)) : this.broadcastWatches(), Promise.resolve()
     }, t.prototype.removeOptimistic = function(n) {
         var r = this.optimisticData.removeLayer(n);
         r !== this.optimisticData && (this.optimisticData = r, this.broadcastWatches())
     }, t.prototype.batch = function(n) {
         var r = this,
@@ -10231,41 +10231,41 @@
     }, t.prototype.broadcastWatch = function(n, r) {
         var i = n.lastDiff,
             o = this.diff(n);
         r && (n.optimistic && typeof r.optimistic == "string" && (o.fromOptimisticTransaction = !0), r.onWatchUpdated && r.onWatchUpdated.call(this, n, o, i) === !1) || (!i || !Re(i.result, o.result)) && n.callback(n.lastDiff = o, i)
     }, t
 }(Id);
 globalThis.__DEV__ !== !1 && (Ud.prototype.getMemoryInternals = by);
-var Te;
+var Ce;
 (function(e) {
     e[e.loading = 1] = "loading", e[e.setVariables = 2] = "setVariables", e[e.fetchMore = 3] = "fetchMore", e[e.refetch = 4] = "refetch", e[e.poll = 6] = "poll", e[e.ready = 7] = "ready", e[e.error = 8] = "error"
-})(Te || (Te = {}));
+})(Ce || (Ce = {}));
 
 function ai(e) {
     return e ? e < 7 : !1
 }
 
 function E0(e, t, n, r) {
     var i = t.data,
-        o = vn(t, ["data"]),
+        o = mn(t, ["data"]),
         s = n.data,
-        a = vn(n, ["data"]);
+        a = mn(n, ["data"]);
     return Re(o, a) && qi(_r(e).selectionSet, i, s, {
         fragmentMap: _o(xo(e)),
         variables: r
     })
 }
 
 function qi(e, t, n, r) {
     if (t === n) return !0;
     var i = new Set;
     return e.selections.every(function(o) {
         if (i.has(o) || (i.add(o), !di(o, r.variables)) || Hu(o)) return !0;
-        if (yn(o)) {
-            var s = mn(o),
+        if (gn(o)) {
+            var s = yn(o),
                 a = t && t[s],
                 l = n && n[s],
                 u = o.selectionSet;
             if (!u) return Re(a, l);
             var c = Array.isArray(a),
                 d = Array.isArray(l);
             if (c !== d) return !1;
@@ -10355,26 +10355,26 @@
                     s = n.subscribe(o)
             })
         }, t.prototype.resetDiff = function() {
             this.queryInfo.resetDiff()
         }, t.prototype.getCurrentResult = function(n) {
             n === void 0 && (n = !0);
             var r = this.getLastResult(!0),
-                i = this.queryInfo.networkStatus || r && r.networkStatus || Te.ready,
+                i = this.queryInfo.networkStatus || r && r.networkStatus || Ce.ready,
                 o = w(w({}, r), {
                     loading: ai(i),
                     networkStatus: i
                 }),
                 s = this.options.fetchPolicy,
                 a = s === void 0 ? "cache-first" : s;
             if (!(ts(a) || this.queryManager.getDocumentInfo(this.query).hasForcedResolvers))
                 if (this.waitForOwnResult) this.queryInfo.updateWatch();
                 else {
                     var l = this.queryInfo.getDiff();
-                    (l.complete || this.options.returnPartialData) && (o.data = l.result), Re(o.data, {}) && (o.data = void 0), l.complete ? (delete o.partial, l.complete && o.networkStatus === Te.loading && (a === "cache-first" || a === "cache-only") && (o.networkStatus = Te.ready, o.loading = !1)) : o.partial = !0, globalThis.__DEV__ !== !1 && !l.complete && !this.options.partialRefetch && !o.loading && !o.data && !o.error && Wd(l.missing)
+                    (l.complete || this.options.returnPartialData) && (o.data = l.result), Re(o.data, {}) && (o.data = void 0), l.complete ? (delete o.partial, l.complete && o.networkStatus === Ce.loading && (a === "cache-first" || a === "cache-only") && (o.networkStatus = Ce.ready, o.loading = !1)) : o.partial = !0, globalThis.__DEV__ !== !1 && !l.complete && !this.options.partialRefetch && !o.loading && !o.data && !o.error && Wd(l.missing)
                 } return n && this.updateLastResult(o), o
         }, t.prototype.isDifferentFromLastResult = function(n, r) {
             if (!this.last) return !0;
             var i = this.queryManager.getDocumentInfo(this.query).hasNonreactiveDirective ? !E0(this.query, this.last.result, n, this.variables) : !Re(this.last.result, n);
             return i || r && !Re(this.last.variables, r)
         }, t.prototype.getLast = function(n, r) {
             var i = this.last;
@@ -10395,33 +10395,33 @@
             if (o === "cache-and-network" ? i.fetchPolicy = o : o === "no-cache" ? i.fetchPolicy = "no-cache" : i.fetchPolicy = "network-only", globalThis.__DEV__ !== !1 && n && w0.call(n, "variables")) {
                 var s = id(this.query),
                     a = s.variableDefinitions;
                 (!a || !a.some(function(l) {
                     return l.variable.name.value === "variables"
                 })) && globalThis.__DEV__ !== !1 && ce.warn(20, n, ((r = s.name) === null || r === void 0 ? void 0 : r.value) || s)
             }
-            return n && !Re(this.options.variables, n) && (i.variables = this.options.variables = w(w({}, this.options.variables), n)), this.queryInfo.resetLastWrite(), this.reobserve(i, Te.refetch)
+            return n && !Re(this.options.variables, n) && (i.variables = this.options.variables = w(w({}, this.options.variables), n)), this.queryInfo.resetLastWrite(), this.reobserve(i, Ce.refetch)
         }, t.prototype.fetchMore = function(n) {
             var r = this,
                 i = w(w({}, n.query ? n : w(w(w(w({}, this.options), {
                     query: this.options.query
                 }), n), {
                     variables: w(w({}, this.options.variables), n.variables)
                 })), {
                     fetchPolicy: "no-cache"
                 });
             i.query = this.transformDocument(i.query);
             var o = this.queryManager.generateQueryId();
             this.lastQuery = n.query ? this.transformDocument(this.options.query) : i.query;
             var s = this.queryInfo,
                 a = s.networkStatus;
-            s.networkStatus = Te.fetchMore, i.notifyOnNetworkStatusChange && this.observe();
+            s.networkStatus = Ce.fetchMore, i.notifyOnNetworkStatusChange && this.observe();
             var l = new Set;
-            return this.queryManager.fetchQuery(o, i, Te.fetchMore).then(function(u) {
-                return r.queryManager.removeQuery(o), s.networkStatus === Te.fetchMore && (s.networkStatus = a), r.queryManager.cache.batch({
+            return this.queryManager.fetchQuery(o, i, Ce.fetchMore).then(function(u) {
+                return r.queryManager.removeQuery(o), s.networkStatus === Ce.fetchMore && (s.networkStatus = a), r.queryManager.cache.batch({
                     update: function(c) {
                         var d = n.updateQuery;
                         d ? c.updateQuery({
                             query: r.query,
                             variables: r.variables,
                             returnPartialData: !0,
                             optimistic: !1
@@ -10477,15 +10477,15 @@
         }, t.prototype.silentSetOptions = function(n) {
             var r = dr(this.options, n || {});
             Gu(this.options, r)
         }, t.prototype.setVariables = function(n) {
             return Re(this.variables, n) ? this.observers.size ? this.result() : Promise.resolve() : (this.options.variables = n, this.observers.size ? this.reobserve({
                 fetchPolicy: this.options.initialFetchPolicy,
                 variables: n
-            }, Te.setVariables) : Promise.resolve())
+            }, Ce.setVariables) : Promise.resolve())
         }, t.prototype.updateQuery = function(n) {
             var r = this.queryManager,
                 i = r.cache.diff({
                     query: this.options.query,
                     variables: this.variables,
                     returnPartialData: !0,
                     optimistic: !1
@@ -10532,15 +10532,15 @@
                     ce(o, 22);
                     var s = i || (this.pollingInfo = {});
                     s.interval = o;
                     var a = function() {
                             var u, c;
                             n.pollingInfo && (!ai(n.queryInfo.networkStatus) && !(!((c = (u = n.options).skipPollAttempt) === null || c === void 0) && c.call(u)) ? n.reobserve({
                                 fetchPolicy: n.options.initialFetchPolicy === "no-cache" ? "no-cache" : "network-only"
-                            }, Te.poll).then(l, l) : l())
+                            }, Ce.poll).then(l, l) : l())
                         },
                         l = function() {
                             var u = n.pollingInfo;
                             u && (clearTimeout(u.timeout), u.timeout = setTimeout(a, u.interval))
                         };
                     l()
                 }
@@ -10553,21 +10553,21 @@
                 variables: r
             }, i ? {
                 error: i
             } : null)
         }, t.prototype.reobserveAsConcast = function(n, r) {
             var i = this;
             this.isTornDown = !1;
-            var o = r === Te.refetch || r === Te.fetchMore || r === Te.poll,
+            var o = r === Ce.refetch || r === Ce.fetchMore || r === Ce.poll,
                 s = this.options.variables,
                 a = this.options.fetchPolicy,
                 l = dr(this.options, n || {}),
                 u = o ? l : Gu(this.options, l),
                 c = this.transformDocument(u.query);
-            this.lastQuery = c, o || (this.updatePolling(), n && n.variables && !Re(n.variables, s) && u.fetchPolicy !== "standby" && u.fetchPolicy === a && (this.applyNextFetchPolicy("variables-changed", u), r === void 0 && (r = Te.setVariables))), this.waitForOwnResult && (this.waitForOwnResult = ts(u.fetchPolicy));
+            this.lastQuery = c, o || (this.updatePolling(), n && n.variables && !Re(n.variables, s) && u.fetchPolicy !== "standby" && u.fetchPolicy === a && (this.applyNextFetchPolicy("variables-changed", u), r === void 0 && (r = Ce.setVariables))), this.waitForOwnResult && (this.waitForOwnResult = ts(u.fetchPolicy));
             var d = function() {
                     i.concast === p && (i.waitForOwnResult = !1)
                 },
                 f = u.variables && w({}, u.variables),
                 h = this.fetch(u, r, c),
                 p = h.concast,
                 m = h.fromLink,
@@ -10594,28 +10594,28 @@
             var i = this.getLastError(),
                 o = this.isDifferentFromLastResult(n, r);
             (i || !n.partial || this.options.returnPartialData) && this.updateLastResult(n, r), (i || o) && Qr(this.observers, "next", n)
         }, t.prototype.reportError = function(n, r) {
             var i = w(w({}, this.getLastResult()), {
                 error: n,
                 errors: n.graphQLErrors,
-                networkStatus: Te.error,
+                networkStatus: Ce.error,
                 loading: !1
             });
             this.updateLastResult(i, r), Qr(this.observers, "error", this.last.error = n)
         }, t.prototype.hasObservers = function() {
             return this.observers.size > 0
         }, t.prototype.tearDownQuery = function() {
             this.isTornDown || (this.concast && this.observer && (this.concast.removeObserver(this.observer), delete this.concast, delete this.observer), this.stopPolling(), this.subscriptions.forEach(function(n) {
                 return n.unsubscribe()
             }), this.subscriptions.clear(), this.queryManager.stopQuery(this.queryId), this.observers.clear(), this.isTornDown = !0)
         }, t.prototype.transformDocument = function(n) {
             return this.queryManager.transform(n)
         }, t
-    }(Ce);
+    }(ke);
 Od(Ys);
 
 function zd(e) {
     var t = e.options,
         n = t.fetchPolicy,
         r = t.nextFetchPolicy;
     return n === "cache-and-network" || n === "network-only" ? e.reobserve({
@@ -10742,32 +10742,32 @@
             return rn(this, void 0, void 0, function() {
                 var o, s, a, l, u, c = this;
                 return on(this, function(d) {
                     return o = i.fragmentMap, s = i.context, a = i.variables, l = [r], u = function(f) {
                         return rn(c, void 0, void 0, function() {
                             var h, p;
                             return on(this, function(m) {
-                                return !n && !i.selectionsToResolve.has(f) ? [2] : di(f, a) ? yn(f) ? [2, this.resolveField(f, n, r, i).then(function(b) {
+                                return !n && !i.selectionsToResolve.has(f) ? [2] : di(f, a) ? gn(f) ? [2, this.resolveField(f, n, r, i).then(function(b) {
                                     var y;
-                                    typeof b < "u" && l.push((y = {}, y[mn(f)] = b, y))
+                                    typeof b < "u" && l.push((y = {}, y[yn(f)] = b, y))
                                 })] : (Vy(f) ? h = f : (h = o[f.name.value], ce(h, 18, f.name.value)), h && h.typeCondition && (p = h.typeCondition.name.value, i.fragmentMatcher(r, p, s)) ? [2, this.resolveSelectionSet(h.selectionSet, n, r, i).then(function(b) {
                                     l.push(b)
                                 })] : [2]) : [2]
                             })
                         })
                     }, [2, Promise.all(t.selections.map(u)).then(function() {
                         return Co(l)
                     })]
                 })
             })
         }, e.prototype.resolveField = function(t, n, r, i) {
             return rn(this, void 0, void 0, function() {
                 var o, s, a, l, u, c, d, f, h, p = this;
                 return on(this, function(m) {
-                    return r ? (o = i.variables, s = t.name.value, a = mn(t), l = s !== a, u = r[a] || r[s], c = Promise.resolve(u), (!i.onlyRunForcedResolvers || this.shouldForceResolvers(t)) && (d = r.__typename || i.defaultOperationType, f = this.resolvers && this.resolvers[d], f && (h = f[l ? s : a], h && (c = Promise.resolve(Ja.withValue(this.cache, h, [r, So(t, o), i.context, {
+                    return r ? (o = i.variables, s = t.name.value, a = yn(t), l = s !== a, u = r[a] || r[s], c = Promise.resolve(u), (!i.onlyRunForcedResolvers || this.shouldForceResolvers(t)) && (d = r.__typename || i.defaultOperationType, f = this.resolvers && this.resolvers[d], f && (h = f[l ? s : a], h && (c = Promise.resolve(Ja.withValue(this.cache, h, [r, So(t, o), i.context, {
                         field: t,
                         fragmentMap: i.fragmentMap
                     }]))))), [2, c.then(function(b) {
                         var y, _;
                         if (b === void 0 && (b = u), t.directives && t.directives.forEach(function(S) {
                                 S.name.value === "export" && S.arguments && S.arguments.forEach(function(T) {
                                     T.name.value === "as" && T.value.kind === "StringValue" && (i.exportedVariables[T.value.value] = b)
@@ -10835,16 +10835,16 @@
 var rs = function() {
     function e(t, n) {
         n === void 0 && (n = t.generateQueryId()), this.queryId = n, this.listeners = new Set, this.document = null, this.lastRequestId = 1, this.stopped = !1, this.dirty = !1, this.observableQuery = null;
         var r = this.cache = t.cache;
         Xn.has(r) || (Xn.set(r, 0), ns(r, "evict"), ns(r, "modify"), ns(r, "reset"))
     }
     return e.prototype.init = function(t) {
-        var n = t.networkStatus || Te.loading;
-        return this.variables && this.networkStatus !== Te.loading && !Re(this.variables, t.variables) && (n = Te.setVariables), Re(t.variables, this.variables) || (this.lastDiff = void 0), Object.assign(this, {
+        var n = t.networkStatus || Ce.loading;
+        return this.variables && this.networkStatus !== Ce.loading && !Re(this.variables, t.variables) && (n = Ce.setVariables), Re(t.variables, this.variables) || (this.lastDiff = void 0), Object.assign(this, {
             document: t.document,
             variables: t.variables,
             networkError: null,
             graphQLErrors: this.graphQLErrors || [],
             networkStatus: n
         }), t.observableQuery && this.setObservableQuery(t.observableQuery), t.lastRequestId && (this.lastRequestId = t.lastRequestId), this
     }, e.prototype.reset = function() {
@@ -10921,15 +10921,15 @@
     }, e.prototype.resetLastWrite = function() {
         this.lastWrite = void 0
     }, e.prototype.shouldWrite = function(t, n) {
         var r = this.lastWrite;
         return !(r && r.dmCount === Xn.get(this.cache) && Re(n, r.variables) && Re(t.data, r.result.data))
     }, e.prototype.markResult = function(t, n, r, i) {
         var o = this,
-            s = new bn,
+            s = new En,
             a = Ft(t.errors) ? t.errors.slice(0) : [];
         if (this.reset(), "incremental" in t && Ft(t.incremental)) {
             var l = Td(this.getDiff().result, t);
             t.data = l
         } else if ("hasNext" in t && t.hasNext) {
             var u = this.getDiff();
             t.data = s.merge(u.result, t.data)
@@ -10953,17 +10953,17 @@
                 return
             }
             var d = o.getDiffOptions(r.variables),
                 f = c.diff(d);
             !o.stopped && Re(o.variables, r.variables) && o.updateWatch(r.variables), o.updateLastDiff(f, d), f.complete && (t.data = f.result)
         }) : this.lastWrite = void 0)
     }, e.prototype.markReady = function() {
-        return this.networkError = null, this.networkStatus = Te.ready
+        return this.networkError = null, this.networkStatus = Ce.ready
     }, e.prototype.markError = function(t) {
-        return this.networkStatus = Te.error, this.lastWrite = void 0, this.reset(), t.graphQLErrors && (this.graphQLErrors = t.graphQLErrors), t.networkError && (this.networkError = t.networkError), t
+        return this.networkStatus = Ce.error, this.lastWrite = void 0, this.reset(), t.graphQLErrors && (this.graphQLErrors = t.graphQLErrors), t.networkError && (this.networkError = t.networkError), t
     }, e
 }();
 
 function Js(e, t) {
     t === void 0 && (t = "none");
     var n = t === "ignore" || t === "all",
         r = !Vi(e);
@@ -11291,15 +11291,15 @@
         }, e.prototype.stopQueryInStoreNoBroadcast = function(t) {
             var n = this.queries.get(t);
             n && n.stop()
         }, e.prototype.clearStore = function(t) {
             return t === void 0 && (t = {
                 discardWatches: !0
             }), this.cancelPendingFetches(it(32)), this.queries.forEach(function(n) {
-                n.observableQuery ? n.networkStatus = Te.loading : n.stop()
+                n.observableQuery ? n.networkStatus = Ce.loading : n.stop()
             }), this.mutationStore && (this.mutationStore = Object.create(null)), this.cache.reset(t)
         }, e.prototype.getObservableQueries = function(t) {
             var n = this;
             t === void 0 && (t = "active");
             var r = new Map,
                 i = new Map,
                 o = new Set;
@@ -11370,15 +11370,15 @@
                         if (p && (b.graphQLErrors = h.errors), m && (b.protocolErrors = h.extensions[Ya]), s === "none" || m) throw new Dt(b)
                     }
                     return s === "ignore" && delete h.errors, h
                 })
             };
             if (this.getDocumentInfo(r).hasClientExports) {
                 var d = this.localState.addExportedVariables(r, a, u).then(c);
-                return new Ce(function(f) {
+                return new ke(function(f) {
                     var h = null;
                     return d.then(function(p) {
                             return h = p.subscribe(f)
                         }, f.error),
                         function() {
                             return h && h.unsubscribe()
                         }
@@ -11414,24 +11414,24 @@
                         operationName: Ms(u) || void 0,
                         context: this.prepareContext(w(w({}, n), {
                             forceFetch: !i
                         }))
                     };
                 if (n = p.context, i) {
                     var m = vi(u),
-                        b = hn(r),
+                        b = pn(r),
                         y = f.lookup(m, b);
                     if (a = y.observable, !a) {
                         var _ = new Wn([Qs(h, p)]);
                         a = y.observable = _, _.beforeNext(function() {
                             f.remove(m, b)
                         })
                     }
                 } else a = new Wn([Qs(h, p)])
-            } else a = new Wn([Ce.of({
+            } else a = new Wn([ke.of({
                 data: {}
             })]), n = this.prepareContext(n);
             return c && (a = Ko(a, function(E) {
                 return o.localState.runResolvers({
                     document: c,
                     remoteResult: E,
                     context: n,
@@ -11449,26 +11449,26 @@
                         graphQLErrors: a
                     }));
                     t.markResult(s, o, r, n), t.markReady()
                 }
                 var u = {
                     data: s.data,
                     loading: !1,
-                    networkStatus: Te.ready
+                    networkStatus: Ce.ready
                 };
-                return l && r.errorPolicy !== "ignore" && (u.errors = a, u.networkStatus = Te.error), u
+                return l && r.errorPolicy !== "ignore" && (u.errors = a, u.networkStatus = Ce.error), u
             }, function(s) {
                 var a = kd(s) ? s : new Dt({
                     networkError: s
                 });
                 throw i >= t.lastRequestId && t.markError(a), a
             })
         }, e.prototype.fetchConcastWithInfo = function(t, n, r, i) {
             var o = this;
-            r === void 0 && (r = Te.loading), i === void 0 && (i = n.query);
+            r === void 0 && (r = Ce.loading), i === void 0 && (i = n.query);
             var s = this.getVariables(i, n.variables),
                 a = this.getQuery(t),
                 l = this.defaultOptions.watchQuery,
                 u = n.fetchPolicy,
                 c = u === void 0 ? l && l.fetchPolicy || "cache-first" : u,
                 d = n.errorPolicy,
                 f = d === void 0 ? l && l.errorPolicy || "none" : d,
@@ -11577,19 +11577,19 @@
                 variables: s,
                 networkStatus: r
             });
             var p = function() {
                     return t.getDiff()
                 },
                 m = function(S, T) {
-                    T === void 0 && (T = t.networkStatus || Te.loading);
+                    T === void 0 && (T = t.networkStatus || Ce.loading);
                     var O = S.result;
                     globalThis.__DEV__ !== !1 && !c && !Re(O, {}) && Wd(S.missing);
                     var F = function(A) {
-                        return Ce.of(w({
+                        return ke.of(w({
                             data: A,
                             loading: ai(T),
                             networkStatus: T
                         }, S.complete ? null : {
                             partial: !0
                         }))
                     };
@@ -11599,17 +11599,17 @@
                             data: O
                         },
                         context: d,
                         variables: s,
                         onlyRunForcedResolvers: !0
                     }).then(function(A) {
                         return F(A.data || void 0)
-                    }) : u === "none" && T === Te.refetch && Array.isArray(S.missing) ? F(void 0) : F(O)
+                    }) : u === "none" && T === Ce.refetch && Array.isArray(S.missing) ? F(void 0) : F(O)
                 },
-                b = a === "no-cache" ? 0 : r === Te.refetch && l !== "merge" ? 1 : 2,
+                b = a === "no-cache" ? 0 : r === Ce.refetch && l !== "merge" ? 1 : 2,
                 y = function() {
                     return i.getResultsFromLink(t, b, {
                         query: o,
                         variables: s,
                         context: d,
                         fetchPolicy: a,
                         errorPolicy: u
@@ -12101,15 +12101,15 @@
 function $0(e) {
     return new Dt({
         graphQLErrors: e,
         errorMessage: `GraphQL response contains errors: ${e.map(t=>t.message).join(" | ")}`
     })
 }
 
-function x1(e, t, n) {
+function O1(e, t, n) {
     return q0(e, t, n)
 }
 
 function q0(e, t, n = {}, r = !1) {
     var i;
     const o = yr(),
         s = oe(),
@@ -12262,15 +12262,15 @@
     function Q() {
         !ne || Ee || (k || K(), fe())
     }
     let ee = a.value;
     const ye = oe(r),
         Ae = ue(() => !s.value || s.value.enabled == null || s.value.enabled),
         v = ue(() => Ae.value && !ye.value && !!a.value);
-    Le(() => ke(u), C => {
+    Le(() => Oe(u), C => {
         s.value && (s.value.throttle !== C.throttle || s.value.debounce !== C.debounce) && K(), s.value = C, Q()
     }, {
         deep: !0,
         immediate: !0
     }), Le(a, C => {
         ee = C, Q()
     });
@@ -12706,15 +12706,15 @@
       stackName
       serviceName
     }
   }
 `;
 
 function X0(e, t) {
-    return Oe(), Ye("svg", {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         viewBox: "0 0 24 24",
         fill: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
     }, [W("path", {
         "fill-rule": "evenodd",
@@ -12734,44 +12734,44 @@
     nb = {
         __name: "VAlert",
         props: {
             data: Object
         },
         setup(e) {
             const t = e;
-            return (n, r) => (Oe(), Ye("div", {
+            return (n, r) => (Te(), Ye("div", {
                 class: Vt(["rounded-md p-4 ring-1 ring-inset", t.data.bgColor, t.data.ringColor])
-            }, [W("div", Z0, [W("div", eb, [(Oe(), Tt(ho(t.data.icon), {
+            }, [W("div", Z0, [W("div", eb, [(Te(), Tt(ho(t.data.icon), {
                 class: Vt(["h-5 w-5", t.data.iconColor]),
                 "aria-hidden": "true"
             }, null, 8, ["class"]))]), W("div", tb, [W("span", {
                 class: Vt(["text-base font-medium", t.data.titleColor])
-            }, Fn(t.data.title), 3), W("div", null, [W("p", {
+            }, cn(t.data.title), 3), W("div", null, [W("p", {
                 class: Vt(["mt-2 text-sm", t.data.textColor])
-            }, Fn(t.data.text), 3)])])])], 2))
+            }, cn(t.data.text), 3)])])])], 2))
         }
     },
     rb = {
         __name: "VErrorAlert",
         props: {
             title: String,
             text: String
         },
         setup(e) {
             const t = e;
-            return (n, r) => (Oe(), Tt(nb, {
+            return (n, r) => (Te(), Tt(nb, {
                 data: {
                     title: t.title,
                     text: t.text,
                     bgColor: "bg-red-400/10",
                     ringColor: "ring-red-400/20",
                     iconColor: "text-red-400",
                     titleColor: "text-red-400",
                     textColor: "text-red-400",
-                    icon: ke(X0)
+                    icon: Oe(X0)
                 }
             }, null, 8, ["data"]))
         }
     },
     ib = {
         class: "flex items-center justify-between px-4 py-4 sm:px-6 sm:py-6 lg:px-8"
     },
@@ -12809,18 +12809,21 @@
         class: "h-2 w-2 rounded-full bg-current"
     }, null, -1),
     mb = [vb],
     yb = {
         class: "mt-3 truncate text-sm"
     },
     gb = {
+        class: "mt-1 truncate text-sm"
+    },
+    bb = {
         key: 2,
         class: "py-20 px-4 sm:px-6 lg:px-8"
     },
-    bb = W("div", {
+    Eb = W("div", {
         class: "text-center"
     }, [W("svg", {
         class: "mx-auto h-12 w-12 text-primary",
         fill: "none",
         viewBox: "0 0 24 24",
         stroke: "currentColor",
         "aria-hidden": "true"
@@ -12829,16 +12832,16 @@
         "stroke-linecap": "round",
         "stroke-linejoin": "round",
         "stroke-width": "2",
         d: "M9 13h6m-3-3v6m-9 1V7a2 2 0 012-2h6l2 2h6a2 2 0 012 2v8a2 2 0 01-2 2H5a2 2 0 01-2-2z"
     })]), W("h5", null, "No events"), W("p", {
         class: "mt-1 text-sm"
     }, "There is no container events to show for the moment !")], -1),
-    Eb = [bb],
-    _b = {
+    _b = [Eb],
+    wb = {
         __name: "VActivity",
         setup(e) {
             const t = oe([]),
                 n = {
                     die: {
                         classes: "text-neutral-400 bg-neutral-100/10",
                         text: "stopped"
@@ -12854,63 +12857,64 @@
                     stop: {
                         classes: "text-yellow-500 bg-yellow-400/10",
                         text: "stopping"
                     }
                 },
                 {
                     result: r,
-                    error: i
+                    error: i,
+                    loading: o
                 } = B0(J0, null, {
                     fetchPolicy: "no-cache"
                 });
-            Le(r, s => {
-                t.value.unshift(s.events)
+            Le(r, a => {
+                t.value.unshift(a.events)
             }, {
                 lazy: !0
             });
-            const o = () => t.value = [];
-            return (s, a) => (Oe(), Ye(Ke, null, [W("header", ib, [ob, W("button", {
-                onClick: a[0] || (a[0] = l => o()),
+            const s = () => t.value = [];
+            return (a, l) => (Te(), Ye(Ke, null, [W("header", ib, [ob, W("button", {
+                onClick: l[0] || (l[0] = u => s()),
                 class: "text-sm font-semibold leading-6 text-primary"
-            }, " Clear ")]), ke(i) ? (Oe(), Ye("div", sb, [W("div", ab, [me(rb, {
+            }, " Clear ")]), Oe(i) ? (Te(), Ye("div", sb, [W("div", ab, [me(rb, {
                 title: "Une erreur est survenue !",
                 text: "Veuillez réessayer plus tard. Si le problème persiste, contactez votre administrateur."
-            })])])) : !s.loading && t.value && t.value.length > 0 ? (Oe(), Ye("ul", lb, [(Oe(!0), Ye(Ke, null, df(t.value, l => (Oe(), Ye("li", {
-                key: l.id,
+            })])])) : !Oe(o) && t.value && t.value.length > 0 ? (Te(), Ye("ul", lb, [(Te(!0), Ye(Ke, null, df(t.value, u => (Te(), Ye("li", {
+                key: u.id,
                 class: "px-4 py-4 sm:px-6 lg:px-8"
-            }, [W("div", ub, [W("h5", cb, [W("a", fb, [W("span", db, Fn(l.stackName), 1), hb, W("span", pb, Fn(l.serviceName), 1)])]), W("div", {
-                class: Vt([n[l.action].classes, "flex-none rounded-full p-1"])
-            }, mb, 2)]), W("p", yb, "Container " + Fn(n[l.action].text), 1)]))), 128))])) : (Oe(), Ye("div", gb, Eb))], 64))
+            }, [W("div", ub, [W("h5", cb, [W("a", fb, [W("span", db, cn(u.stackName), 1), hb, W("span", pb, cn(u.serviceName), 1)])]), W("div", {
+                class: Vt([n[u.action].classes, "flex-none rounded-full p-1"])
+            }, mb, 2)]), W("p", yb, cn(u.containerName), 1), W("p", gb, "Container " + cn(n[u.action].text), 1)]))), 128))])) : (Te(), Ye("div", bb, _b))], 64))
         }
     },
-    wb = (e, t) => {
+    Sb = (e, t) => {
         const n = e.__vccOpts || e;
         for (const [r, i] of t) n[r] = i;
         return n
     },
-    Sb = {};
+    xb = {};
 
-function xb(e, t, n, r, i, o) {
-    return Oe(), Tt(Na, {
+function Ob(e, t, n, r, i, o) {
+    return Te(), Tt(Na, {
         name: "fade",
         mode: "out-in"
     }, {
         default: et(() => [tv(e.$slots, "default", {}, void 0, !0)]),
         _: 3
     })
 }
-const Ob = wb(Sb, [
-    ["render", xb],
+const Tb = Sb(xb, [
+    ["render", Ob],
     ["__scopeId", "data-v-a303cc25"]
 ]);
-let Tb = Symbol("headlessui.useid"),
-    Cb = 0;
+let Cb = Symbol("headlessui.useid"),
+    kb = 0;
 
 function tl() {
-    return Ie(Tb, () => `${++Cb}`)()
+    return Ie(Cb, () => `${++kb}`)()
 }
 
 function Qe(e) {
     var t;
     if (e == null || e.value == null) return null;
     let n = (t = e.value.$el) != null ? t : e.value;
     return n instanceof Node ? n : null
@@ -12920,23 +12924,23 @@
     if (e in t) {
         let i = t[e];
         return typeof i == "function" ? i(...n) : i
     }
     let r = new Error(`Tried to handle "${e}" but there is no handler defined. Only defined handlers are: ${Object.keys(t).map(i=>`"${i}"`).join(", ")}.`);
     throw Error.captureStackTrace && Error.captureStackTrace(r, Lt), r
 }
-var kb = Object.defineProperty,
-    Ab = (e, t, n) => t in e ? kb(e, t, {
+var Ab = Object.defineProperty,
+    Rb = (e, t, n) => t in e ? Ab(e, t, {
         enumerable: !0,
         configurable: !0,
         writable: !0,
         value: n
     }) : e[t] = n,
-    Zu = (e, t, n) => (Ab(e, typeof t != "symbol" ? t + "" : t, n), n);
-let Rb = class {
+    Zu = (e, t, n) => (Rb(e, typeof t != "symbol" ? t + "" : t, n), n);
+let Ib = class {
         constructor() {
             Zu(this, "current", this.detect()), Zu(this, "currentId", 0)
         }
         set(t) {
             this.current !== t && (this.currentId = 0, this.current = t)
         }
         reset() {
@@ -12951,36 +12955,36 @@
         get isClient() {
             return this.current === "client"
         }
         detect() {
             return typeof window > "u" || typeof document > "u" ? "server" : "client"
         }
     },
-    mi = new Rb;
+    mi = new Ib;
 
 function wr(e) {
     if (mi.isServer) return null;
     if (e instanceof Node) return e.ownerDocument;
     if (e != null && e.hasOwnProperty("value")) {
         let t = Qe(e);
         if (t) return t.ownerDocument
     }
     return document
 }
 let ta = ["[contentEditable=true]", "[tabindex]", "a[href]", "area[href]", "button:not([disabled])", "iframe", "input:not([disabled])", "select:not([disabled])", "textarea:not([disabled])"].map(e => `${e}:not([tabindex='-1'])`).join(",");
 var un = (e => (e[e.First = 1] = "First", e[e.Previous = 2] = "Previous", e[e.Next = 4] = "Next", e[e.Last = 8] = "Last", e[e.WrapAround = 16] = "WrapAround", e[e.NoScroll = 32] = "NoScroll", e))(un || {}),
     sh = (e => (e[e.Error = 0] = "Error", e[e.Overflow = 1] = "Overflow", e[e.Success = 2] = "Success", e[e.Underflow = 3] = "Underflow", e))(sh || {}),
-    Ib = (e => (e[e.Previous = -1] = "Previous", e[e.Next = 1] = "Next", e))(Ib || {});
+    Db = (e => (e[e.Previous = -1] = "Previous", e[e.Next = 1] = "Next", e))(Db || {});
 
-function Db(e = document.body) {
+function Nb(e = document.body) {
     return e == null ? [] : Array.from(e.querySelectorAll(ta)).sort((t, n) => Math.sign((t.tabIndex || Number.MAX_SAFE_INTEGER) - (n.tabIndex || Number.MAX_SAFE_INTEGER)))
 }
 var ah = (e => (e[e.Strict = 0] = "Strict", e[e.Loose = 1] = "Loose", e))(ah || {});
 
-function Nb(e, t = 0) {
+function Pb(e, t = 0) {
     var n;
     return e === ((n = wr(e)) == null ? void 0 : n.body) ? !1 : Lt(t, {
         0() {
             return e.matches(ta)
         },
         1() {
             let r = e;
@@ -12988,34 +12992,34 @@
                 if (r.matches(ta)) return !0;
                 r = r.parentElement
             }
             return !1
         }
     })
 }
-var Pb = (e => (e[e.Keyboard = 0] = "Keyboard", e[e.Mouse = 1] = "Mouse", e))(Pb || {});
+var Fb = (e => (e[e.Keyboard = 0] = "Keyboard", e[e.Mouse = 1] = "Mouse", e))(Fb || {});
 typeof window < "u" && typeof document < "u" && (document.addEventListener("keydown", e => {
     e.metaKey || e.altKey || e.ctrlKey || (document.documentElement.dataset.headlessuiFocusVisible = "")
 }, !0), document.addEventListener("click", e => {
     e.detail === 1 ? delete document.documentElement.dataset.headlessuiFocusVisible : e.detail === 0 && (document.documentElement.dataset.headlessuiFocusVisible = "")
 }, !0));
 
 function Vn(e) {
     e == null || e.focus({
         preventScroll: !0
     })
 }
-let Fb = ["textarea", "input"].join(",");
+let Lb = ["textarea", "input"].join(",");
 
-function Lb(e) {
+function Mb(e) {
     var t, n;
-    return (n = (t = e == null ? void 0 : e.matches) == null ? void 0 : t.call(e, Fb)) != null ? n : !1
+    return (n = (t = e == null ? void 0 : e.matches) == null ? void 0 : t.call(e, Lb)) != null ? n : !1
 }
 
-function Mb(e, t = n => n) {
+function jb(e, t = n => n) {
     return e.slice().sort((n, r) => {
         let i = t(n),
             o = t(r);
         if (i === null || o === null) return 0;
         let s = i.compareDocumentPosition(o);
         return s & Node.DOCUMENT_POSITION_FOLLOWING ? -1 : s & Node.DOCUMENT_POSITION_PRECEDING ? 1 : 0
     })
@@ -13024,15 +13028,15 @@
 function Qi(e, t, {
     sorted: n = !0,
     relativeTo: r = null,
     skipElements: i = []
 } = {}) {
     var o;
     let s = (o = Array.isArray(e) ? e.length > 0 ? e[0].ownerDocument : document : e == null ? void 0 : e.ownerDocument) != null ? o : document,
-        a = Array.isArray(e) ? n ? Mb(e) : e : Db(e);
+        a = Array.isArray(e) ? n ? jb(e) : e : Nb(e);
     i.length > 0 && a.length > 1 && (a = a.filter(p => !i.includes(p))), r = r ?? s.activeElement;
     let l = (() => {
             if (t & 5) return 1;
             if (t & 10) return -1;
             throw new Error("Missing Focus.First, Focus.Previous, Focus.Next or Focus.Last")
         })(),
         u = (() => {
@@ -13054,69 +13058,69 @@
         if (t & 16) p = (p + f) % f;
         else {
             if (p < 0) return 3;
             if (p >= f) return 1
         }
         h = a[p], h == null || h.focus(c), d += l
     } while (h !== s.activeElement);
-    return t & 6 && Lb(h) && h.select(), 2
+    return t & 6 && Mb(h) && h.select(), 2
 }
 
 function lh() {
     return /iPhone/gi.test(window.navigator.platform) || /Mac/gi.test(window.navigator.platform) && window.navigator.maxTouchPoints > 0
 }
 
-function jb() {
+function Vb() {
     return /Android/gi.test(window.navigator.userAgent)
 }
 
-function Vb() {
-    return lh() || jb()
+function $b() {
+    return lh() || Vb()
 }
 
 function Ri(e, t, n) {
     mi.isServer || Ot(r => {
         document.addEventListener(e, t, n), r(() => document.removeEventListener(e, t, n))
     })
 }
 
 function uh(e, t, n) {
     mi.isServer || Ot(r => {
         window.addEventListener(e, t, n), r(() => window.removeEventListener(e, t, n))
     })
 }
 
-function $b(e, t, n = ue(() => !0)) {
+function qb(e, t, n = ue(() => !0)) {
     function r(o, s) {
         if (!n.value || o.defaultPrevented) return;
         let a = s(o);
         if (a === null || !a.getRootNode().contains(a)) return;
         let l = function u(c) {
             return typeof c == "function" ? u(c()) : Array.isArray(c) || c instanceof Set ? c : [c]
         }(e);
         for (let u of l) {
             if (u === null) continue;
             let c = u instanceof HTMLElement ? u : Qe(u);
             if (c != null && c.contains(a) || o.composed && o.composedPath().includes(c)) return
         }
-        return !Nb(a, ah.Loose) && a.tabIndex !== -1 && o.preventDefault(), t(o, a)
+        return !Pb(a, ah.Loose) && a.tabIndex !== -1 && o.preventDefault(), t(o, a)
     }
     let i = oe(null);
     Ri("pointerdown", o => {
         var s, a;
         n.value && (i.value = ((a = (s = o.composedPath) == null ? void 0 : s.call(o)) == null ? void 0 : a[0]) || o.target)
     }, !0), Ri("mousedown", o => {
         var s, a;
         n.value && (i.value = ((a = (s = o.composedPath) == null ? void 0 : s.call(o)) == null ? void 0 : a[0]) || o.target)
     }, !0), Ri("click", o => {
-        Vb() || i.value && (r(o, () => i.value), i.value = null)
+        $b() || i.value && (r(o, () => i.value), i.value = null)
     }, !0), Ri("touchend", o => r(o, () => o.target instanceof HTMLElement ? o.target : null), !0), uh("blur", o => r(o, () => window.document.activeElement instanceof HTMLIFrameElement ? window.document.activeElement : null), !0)
 }
 var no = (e => (e[e.None = 0] = "None", e[e.RenderStrategy = 1] = "RenderStrategy", e[e.Static = 2] = "Static", e))(no || {}),
-    cn = (e => (e[e.Unmount = 0] = "Unmount", e[e.Hidden = 1] = "Hidden", e))(cn || {});
+    fn = (e => (e[e.Unmount = 0] = "Unmount", e[e.Hidden = 1] = "Hidden", e))(fn || {});
 
 function Wt({
     visible: e = !0,
     features: t = 0,
     ourProps: n,
     theirProps: r,
     ...i
@@ -13167,15 +13171,15 @@
             f = [];
         for (let [h, p] of Object.entries(r)) typeof p == "boolean" && (d = !0), p === !0 && f.push(h);
         d && (c["data-headlessui-state"] = f.join(" "))
     }
     if (a === "template") {
         if (u = ch(u ?? []), Object.keys(l).length > 0 || Object.keys(t).length > 0) {
             let [d, ...f] = u ?? [];
-            if (!qb(d) || f.length > 0) throw new Error(['Passing props on "template"!', "", `The current component <${i} /> is rendering a "template".`, "However we need to passthrough the following props:", Object.keys(l).concat(Object.keys(t)).map(m => m.trim()).filter((m, b, y) => y.indexOf(m) === b).sort((m, b) => m.localeCompare(b)).map(m => `  - ${m}`).join(`
+            if (!Bb(d) || f.length > 0) throw new Error(['Passing props on "template"!', "", `The current component <${i} /> is rendering a "template".`, "However we need to passthrough the following props:", Object.keys(l).concat(Object.keys(t)).map(m => m.trim()).filter((m, b, y) => y.indexOf(m) === b).sort((m, b) => m.localeCompare(b)).map(m => `  - ${m}`).join(`
 `), "", "You can apply a few solutions:", ['Add an `as="..."` prop, to ensure that we render an actual element instead of a "template".', "Render a single element as the child so that we can forward the props onto that element."].map(m => `  - ${m}`).join(`
 `)].join(`
 `));
             let h = fh((s = d.props) != null ? s : {}, l, c),
                 p = Bt(d, h, !0);
             for (let m in h) m.startsWith("on") && (p.props || (p.props = {}), p.props[m] = h[m]);
             return p
@@ -13213,15 +13217,15 @@
 
 function dh(e, t = []) {
     let n = Object.assign({}, e);
     for (let r of t) r in n && delete n[r];
     return n
 }
 
-function qb(e) {
+function Bb(e) {
     return e == null ? !1 : typeof e.type == "string" || typeof e.type == "object" || typeof e.type == "function"
 }
 var ro = (e => (e[e.None = 1] = "None", e[e.Focusable = 2] = "Focusable", e[e.Hidden = 4] = "Hidden", e))(ro || {});
 let na = gt({
         name: "Hidden",
         props: {
             as: {
@@ -13272,37 +13276,37 @@
                 })
             }
         }
     }),
     hh = Symbol("Context");
 var dt = (e => (e[e.Open = 1] = "Open", e[e.Closed = 2] = "Closed", e[e.Closing = 4] = "Closing", e[e.Opening = 8] = "Opening", e))(dt || {});
 
-function Bb() {
+function Qb() {
     return nl() !== null
 }
 
 function nl() {
     return Ie(hh, null)
 }
 
-function Qb(e) {
+function Ub(e) {
     rt(hh, e)
 }
 var ph = (e => (e.Space = " ", e.Enter = "Enter", e.Escape = "Escape", e.Backspace = "Backspace", e.Delete = "Delete", e.ArrowLeft = "ArrowLeft", e.ArrowUp = "ArrowUp", e.ArrowRight = "ArrowRight", e.ArrowDown = "ArrowDown", e.Home = "Home", e.End = "End", e.PageUp = "PageUp", e.PageDown = "PageDown", e.Tab = "Tab", e))(ph || {});
 
-function Ub(e) {
+function zb(e) {
     function t() {
         document.readyState !== "loading" && (e(), document.removeEventListener("DOMContentLoaded", t))
     }
     typeof window < "u" && typeof document < "u" && (document.addEventListener("DOMContentLoaded", t), t())
 }
-let Nn = [];
-Ub(() => {
+let Pn = [];
+zb(() => {
     function e(t) {
-        t.target instanceof HTMLElement && t.target !== document.body && Nn[0] !== t.target && (Nn.unshift(t.target), Nn = Nn.filter(n => n != null && n.isConnected), Nn.splice(10))
+        t.target instanceof HTMLElement && t.target !== document.body && Pn[0] !== t.target && (Pn.unshift(t.target), Pn = Pn.filter(n => n != null && n.isConnected), Pn.splice(10))
     }
     window.addEventListener("click", e, {
         capture: !0
     }), window.addEventListener("mousedown", e, {
         capture: !0
     }), window.addEventListener("focus", e, {
         capture: !0
@@ -13381,15 +13385,15 @@
 function vh(e, t, n, r) {
     mi.isServer || Ot(i => {
         e = e ?? window, e.addEventListener(t, n, r), i(() => e.removeEventListener(t, n, r))
     })
 }
 var Lr = (e => (e[e.Forwards = 0] = "Forwards", e[e.Backwards = 1] = "Backwards", e))(Lr || {});
 
-function zb() {
+function Wb() {
     let e = oe(0);
     return uh("keydown", t => {
         t.key === "Tab" && (e.value = t.shiftKey ? 1 : 0)
     }), e
 }
 
 function mh(e) {
@@ -13432,29 +13436,29 @@
         let i = oe(null);
         r({
             el: i,
             $el: i
         });
         let o = ue(() => wr(i)),
             s = oe(!1);
-        at(() => s.value = !0), yt(() => s.value = !1), Hb({
+        at(() => s.value = !0), yt(() => s.value = !1), Gb({
             ownerDocument: o
         }, ue(() => s.value && !!(e.features & 16)));
-        let a = Gb({
+        let a = Kb({
             ownerDocument: o,
             container: i,
             initialFocus: ue(() => e.initialFocus)
         }, ue(() => s.value && !!(e.features & 2)));
-        Kb({
+        Yb({
             ownerDocument: o,
             container: i,
             containers: e.containers,
             previousActiveElement: a
         }, ue(() => s.value && !!(e.features & 8)));
-        let l = zb();
+        let l = Wb();
 
         function u(h) {
             let p = Qe(i);
             p && (m => m())(() => {
                 Lt(l.value, {
                     [Lr.Forwards]: () => {
                         Qi(p, un.First, {
@@ -13527,45 +13531,45 @@
             })])
         }
     }
 }), {
     features: yh
 });
 
-function Wb(e) {
-    let t = oe(Nn.slice());
+function Hb(e) {
+    let t = oe(Pn.slice());
     return Le([e], ([n], [r]) => {
         r === !0 && n === !1 ? rl(() => {
             t.value.splice(0)
-        }) : r === !1 && n === !0 && (t.value = Nn.slice())
+        }) : r === !1 && n === !0 && (t.value = Pn.slice())
     }, {
         flush: "post"
     }), () => {
         var n;
         return (n = t.value.find(r => r != null && r.isConnected)) != null ? n : null
     }
 }
 
-function Hb({
+function Gb({
     ownerDocument: e
 }, t) {
-    let n = Wb(t);
+    let n = Hb(t);
     at(() => {
         Ot(() => {
             var r, i;
             t.value || ((r = e.value) == null ? void 0 : r.activeElement) === ((i = e.value) == null ? void 0 : i.body) && Vn(n())
         }, {
             flush: "post"
         })
     }), yt(() => {
         t.value && Vn(n())
     })
 }
 
-function Gb({
+function Kb({
     ownerDocument: e,
     container: t,
     initialFocus: n
 }, r) {
     let i = oe(null),
         o = oe(!1);
     return at(() => o.value = !0), yt(() => o.value = !1), at(() => {
@@ -13591,15 +13595,15 @@
         }, {
             immediate: !0,
             flush: "post"
         })
     }), i
 }
 
-function Kb({
+function Yb({
     ownerDocument: e,
     container: t,
     containers: n,
     previousActiveElement: r
 }, i) {
     var o;
     vh((o = e.value) == null ? void 0 : o.defaultView, "focus", s => {
@@ -13615,22 +13619,22 @@
 
 function gh(e, t) {
     for (let n of e)
         if (n.contains(t)) return !0;
     return !1
 }
 
-function Yb(e) {
+function Jb(e) {
     let t = Sa(e.getSnapshot());
     return yt(e.subscribe(() => {
         t.value = e.getSnapshot()
     })), t
 }
 
-function Jb(e, t) {
+function Xb(e, t) {
     let n = e(),
         r = new Set;
     return {
         getSnapshot() {
             return n
         },
         subscribe(i) {
@@ -13639,15 +13643,15 @@
         dispatch(i, ...o) {
             let s = t[i].call(n, ...o);
             s && (n = s, r.forEach(a => a()))
         }
     }
 }
 
-function Xb() {
+function Zb() {
     let e;
     return {
         before({
             doc: t
         }) {
             var n;
             let r = t.documentElement;
@@ -13661,15 +13665,15 @@
                 i = r.clientWidth - r.offsetWidth,
                 o = e - i;
             n.style(r, "paddingRight", `${o}px`)
         }
     }
 }
 
-function Zb() {
+function eE() {
     return lh() ? {
         before({
             doc: e,
             d: t,
             meta: n
         }) {
             function r(i) {
@@ -13716,31 +13720,31 @@
                     }), s = null)
                 })
             })
         }
     } : {}
 }
 
-function eE() {
+function tE() {
     return {
         before({
             doc: e,
             d: t
         }) {
             t.style(e.documentElement, "overflow", "hidden")
         }
     }
 }
 
-function tE(e) {
+function nE(e) {
     let t = {};
     for (let n of e) Object.assign(t, n(t));
     return t
 }
-let Pn = Jb(() => new Map, {
+let Fn = Xb(() => new Map, {
     PUSH(e, t) {
         var n;
         let r = (n = this.get(e)) != null ? n : {
             doc: e,
             count: 0,
             d: yi(),
             meta: new Set
@@ -13755,17 +13759,17 @@
         doc: e,
         d: t,
         meta: n
     }) {
         let r = {
                 doc: e,
                 d: t,
-                meta: tE(n)
+                meta: nE(n)
             },
-            i = [Zb(), Xb(), eE()];
+            i = [eE(), Zb(), tE()];
         i.forEach(({
             before: o
         }) => o == null ? void 0 : o(r)), i.forEach(({
             after: o
         }) => o == null ? void 0 : o(r))
     },
     SCROLL_ALLOW({
@@ -13775,37 +13779,37 @@
     },
     TEARDOWN({
         doc: e
     }) {
         this.delete(e)
     }
 });
-Pn.subscribe(() => {
-    let e = Pn.getSnapshot(),
+Fn.subscribe(() => {
+    let e = Fn.getSnapshot(),
         t = new Map;
     for (let [n] of e) t.set(n, n.documentElement.style.overflow);
     for (let n of e.values()) {
         let r = t.get(n.doc) === "hidden",
             i = n.count !== 0;
-        (i && !r || !i && r) && Pn.dispatch(n.count > 0 ? "SCROLL_PREVENT" : "SCROLL_ALLOW", n), n.count === 0 && Pn.dispatch("TEARDOWN", n)
+        (i && !r || !i && r) && Fn.dispatch(n.count > 0 ? "SCROLL_PREVENT" : "SCROLL_ALLOW", n), n.count === 0 && Fn.dispatch("TEARDOWN", n)
     }
 });
 
-function nE(e, t, n) {
-    let r = Yb(Pn),
+function rE(e, t, n) {
+    let r = Jb(Fn),
         i = ue(() => {
             let o = e.value ? r.value.get(e.value) : void 0;
             return o ? o.count > 0 : !1
         });
     return Le([e, t], ([o, s], [a], l) => {
         if (!o || !s) return;
-        Pn.dispatch("PUSH", o, n);
+        Fn.dispatch("PUSH", o, n);
         let u = !1;
         l(() => {
-            u || (Pn.dispatch("POP", a ?? o, n), u = !0)
+            u || (Fn.dispatch("POP", a ?? o, n), u = !0)
         })
     }, {
         immediate: !0
     }), i
 }
 let as = new Map,
     Ir = new Map;
@@ -13828,15 +13832,15 @@
         Ir.set(i, o + 1), o === 0 && (as.set(i, {
             "aria-hidden": i.getAttribute("aria-hidden"),
             inert: i.inert
         }), i.setAttribute("aria-hidden", "true"), i.inert = !0)
     })
 }
 
-function rE({
+function iE({
     defaultContainers: e = [],
     portals: t,
     mainTreeNodeRef: n
 } = {}) {
     let r = oe(null),
         i = wr(r);
 
@@ -13861,15 +13865,15 @@
                 ref: r
             })
         }
     }
 }
 let bh = Symbol("ForcePortalRootContext");
 
-function iE() {
+function oE() {
     return Ie(bh, !1)
 }
 let tc = gt({
         name: "ForcePortalRoot",
         props: {
             as: {
                 type: [Object, String],
@@ -13899,25 +13903,25 @@
                 })
             }
         }
     }),
     Eh = Symbol("StackContext");
 var ra = (e => (e[e.Add = 0] = "Add", e[e.Remove = 1] = "Remove", e))(ra || {});
 
-function oE() {
+function sE() {
     return Ie(Eh, () => {})
 }
 
-function sE({
+function aE({
     type: e,
     enabled: t,
     element: n,
     onUpdate: r
 }) {
-    let i = oE();
+    let i = sE();
 
     function o(...s) {
         r == null || r(...s), i(...s)
     }
     at(() => {
         Le(t, (s, a) => {
             s ? o(0, e, n) : a === !0 && o(1, e, n)
@@ -13925,65 +13929,65 @@
             immediate: !0,
             flush: "sync"
         })
     }), yt(() => {
         t.value && o(1, e, n)
     }), rt(Eh, o)
 }
-let aE = Symbol("DescriptionContext");
+let lE = Symbol("DescriptionContext");
 
-function lE({
+function uE({
     slot: e = oe({}),
     name: t = "Description",
     props: n = {}
 } = {}) {
     let r = oe([]);
 
     function i(o) {
         return r.value.push(o), () => {
             let s = r.value.indexOf(o);
             s !== -1 && r.value.splice(s, 1)
         }
     }
-    return rt(aE, {
+    return rt(lE, {
         register: i,
         slot: e,
         name: t,
         props: n
     }), ue(() => r.value.length > 0 ? r.value.join(" ") : void 0)
 }
 
-function uE(e) {
+function cE(e) {
     let t = wr(e);
     if (!t) {
         if (e === null) return null;
         throw new Error(`[Headless UI]: Cannot find ownerDocument for contextElement: ${e}`)
     }
     let n = t.getElementById("headlessui-portal-root");
     if (n) return n;
     let r = t.createElement("div");
     return r.setAttribute("id", "headlessui-portal-root"), t.body.appendChild(r)
 }
-let cE = gt({
+let fE = gt({
         name: "Portal",
         props: {
             as: {
                 type: [Object, String],
                 default: "div"
             }
         },
         setup(e, {
             slots: t,
             attrs: n
         }) {
             let r = oe(null),
                 i = ue(() => wr(r)),
-                o = iE(),
+                o = oE(),
                 s = Ie(_h, null),
-                a = oe(o === !0 || s == null ? uE(r.value) : s.resolveTarget()),
+                a = oe(o === !0 || s == null ? cE(r.value) : s.resolveTarget()),
                 l = oe(!1);
             at(() => {
                 l.value = !0
             }), Ot(() => {
                 o || s != null && (a.value = s.resolveTarget())
             });
             let u = Ie(ia, null),
@@ -14014,15 +14018,15 @@
                     name: "Portal"
                 }))
             }
         }
     }),
     ia = Symbol("PortalParentContext");
 
-function fE() {
+function dE() {
     let e = Ie(ia, null),
         t = oe([]);
 
     function n(o) {
         return t.value.push(o), e && e.register(o), () => r(o)
     }
 
@@ -14044,15 +14048,15 @@
                 var a;
                 return (a = s.default) == null ? void 0 : a.call(s)
             }
         }
     })]
 }
 let _h = Symbol("PortalGroupContext"),
-    dE = gt({
+    hE = gt({
         name: "PortalGroup",
         props: {
             as: {
                 type: [Object, String],
                 default: "template"
             },
             target: {
@@ -14081,15 +14085,15 @@
                     attrs: t,
                     slots: n,
                     name: "PortalGroup"
                 })
             }
         }
     });
-var hE = (e => (e[e.Open = 0] = "Open", e[e.Closed = 1] = "Closed", e))(hE || {});
+var pE = (e => (e[e.Open = 0] = "Open", e[e.Closed = 1] = "Closed", e))(pE || {});
 let oa = Symbol("DialogContext");
 
 function wh(e) {
     let t = Ie(oa, null);
     if (t === null) {
         let n = new Error(`<${e} /> is missing a parent <Dialog /> component.`);
         throw Error.captureStackTrace && Error.captureStackTrace(n, wh), n
@@ -14157,20 +14161,20 @@
                     $el: p
                 }), !(e.open !== Ii || f !== null)) throw new Error("You forgot to provide an `open` prop to the `Dialog`.");
             if (typeof h.value != "boolean") throw new Error(`You provided an \`open\` prop to the \`Dialog\`, but the value is not a boolean. Received: ${h.value===Ii?void 0:e.open}`);
             let b = ue(() => l.value && h.value ? 0 : 1),
                 y = ue(() => b.value === 0),
                 _ = ue(() => d.value > 1),
                 E = Ie(oa, null) !== null,
-                [S, T] = fE(),
+                [S, T] = dE(),
                 {
                     resolveContainers: O,
                     mainTreeNodeRef: F,
                     MainTreeNode: A
-                } = rE({
+                } = iE({
                     portals: S,
                     defaultContainers: [ue(() => {
                         var G;
                         return (G = $.panelRef.value) != null ? G : p.value
                     })]
                 }),
                 R = ue(() => _.value ? "parent" : "leaf"),
@@ -14182,26 +14186,26 @@
                 });
             ec(V, ne);
             let Y = ue(() => _.value ? !0 : y.value),
                 he = ue(() => {
                     var G, re, ve;
                     return (ve = Array.from((re = (G = m.value) == null ? void 0 : G.querySelectorAll("[data-headlessui-portal]")) != null ? re : []).find(Ee => Ee.contains(Qe(F)) && Ee instanceof HTMLElement)) != null ? ve : null
                 });
-            ec(he, Y), sE({
+            ec(he, Y), aE({
                 type: "Dialog",
                 enabled: ue(() => b.value === 0),
                 element: p,
                 onUpdate: (G, re) => {
                     if (re === "Dialog") return Lt(G, {
                         [ra.Add]: () => d.value += 1,
                         [ra.Remove]: () => d.value -= 1
                     })
                 }
             });
-            let H = lE({
+            let H = uE({
                     name: "DialogDescription",
                     slot: ue(() => ({
                         open: h.value
                     }))
                 }),
                 L = oe(null),
                 $ = {
@@ -14213,23 +14217,23 @@
                     },
                     close() {
                         t("close", !1)
                     }
                 };
             rt(oa, $);
             let U = ue(() => !(!y.value || _.value));
-            $b(O, (G, re) => {
+            qb(O, (G, re) => {
                 G.preventDefault(), $.close(), $t(() => re == null ? void 0 : re.focus())
             }, U);
             let ie = ue(() => !(_.value || b.value !== 0));
             vh((s = m.value) == null ? void 0 : s.defaultView, "keydown", G => {
                 ie.value && (G.defaultPrevented || G.key === ph.Escape && (G.preventDefault(), G.stopPropagation(), $.close()))
             });
             let we = ue(() => !(M.value || b.value !== 0 || E));
-            return nE(m, we, G => {
+            return rE(m, we, G => {
                 var re;
                 return {
                     containers: [...(re = G.containers) != null ? re : [], O]
                 }
             }), Ot(G => {
                 if (b.value !== 0) return;
                 let re = Qe(p);
@@ -14255,15 +14259,15 @@
                     "aria-labelledby": L.value,
                     "aria-describedby": H.value
                 }, qe = {
                     open: b.value === 0
                 };
                 return ze(tc, {
                     force: !0
-                }, () => [ze(cE, () => ze(dE, {
+                }, () => [ze(fE, () => ze(hE, {
                     target: p.value
                 }, () => ze(tc, {
                     force: !1
                 }, () => ze(Rr, {
                     initialFocus: re,
                     containers: O,
                     features: y.value ? Lt(R.value, {
@@ -14332,15 +14336,15 @@
                     slots: n,
                     name: "DialogPanel"
                 })
             }
         }
     });
 
-function pE(e) {
+function vE(e) {
     let t = {
         called: !1
     };
     return (...n) => {
         if (!t.called) return t.called = !0, e(...n)
     }
 }
@@ -14350,52 +14354,52 @@
 }
 
 function Di(e, ...t) {
     e && t.length > 0 && e.classList.remove(...t)
 }
 var sa = (e => (e.Finished = "finished", e.Cancelled = "cancelled", e))(sa || {});
 
-function vE(e, t) {
+function mE(e, t) {
     let n = yi();
     if (!e) return n.dispose;
     let {
         transitionDuration: r,
         transitionDelay: i
     } = getComputedStyle(e), [o, s] = [r, i].map(a => {
         let [l = 0] = a.split(",").filter(Boolean).map(u => u.includes("ms") ? parseFloat(u) : parseFloat(u) * 1e3).sort((u, c) => c - u);
         return l
     });
     return o !== 0 ? n.setTimeout(() => t("finished"), o + s) : t("finished"), n.add(() => t("cancelled")), n.dispose
 }
 
 function nc(e, t, n, r, i, o) {
     let s = yi(),
-        a = o !== void 0 ? pE(o) : () => {};
+        a = o !== void 0 ? vE(o) : () => {};
     return Di(e, ...i), ls(e, ...t, ...n), s.nextFrame(() => {
-        Di(e, ...n), ls(e, ...r), s.add(vE(e, l => (Di(e, ...r, ...t), ls(e, ...i), a(l))))
+        Di(e, ...n), ls(e, ...r), s.add(mE(e, l => (Di(e, ...r, ...t), ls(e, ...i), a(l))))
     }), s.add(() => Di(e, ...t, ...n, ...r, ...i)), s.add(() => a("cancelled")), s.dispose
 }
 
-function Cn(e = "") {
+function kn(e = "") {
     return e.split(/\s+/).filter(t => t.length > 1)
 }
 let il = Symbol("TransitionContext");
-var mE = (e => (e.Visible = "visible", e.Hidden = "hidden", e))(mE || {});
+var yE = (e => (e.Visible = "visible", e.Hidden = "hidden", e))(yE || {});
 
-function yE() {
+function gE() {
     return Ie(il, null) !== null
 }
 
-function gE() {
+function bE() {
     let e = Ie(il, null);
     if (e === null) throw new Error("A <TransitionChild /> is used but it is missing a parent <TransitionRoot />.");
     return e
 }
 
-function bE() {
+function EE() {
     let e = Ie(ol, null);
     if (e === null) throw new Error("A <TransitionChild /> is used but it is missing a parent <TransitionRoot />.");
     return e
 }
 let ol = Symbol("NestingContext");
 
 function Ao(e) {
@@ -14405,36 +14409,36 @@
 }
 
 function Oh(e) {
     let t = oe([]),
         n = oe(!1);
     at(() => n.value = !0), yt(() => n.value = !1);
 
-    function r(o, s = cn.Hidden) {
+    function r(o, s = fn.Hidden) {
         let a = t.value.findIndex(({
             id: l
         }) => l === o);
         a !== -1 && (Lt(s, {
-            [cn.Unmount]() {
+            [fn.Unmount]() {
                 t.value.splice(a, 1)
             },
-            [cn.Hidden]() {
+            [fn.Hidden]() {
                 t.value[a].state = "hidden"
             }
         }), !Ao(t) && n.value && (e == null || e()))
     }
 
     function i(o) {
         let s = t.value.find(({
             id: a
         }) => a === o);
         return s ? s.state !== "visible" && (s.state = "visible") : t.value.push({
             id: o,
             state: "visible"
-        }), () => r(o, cn.Unmount)
+        }), () => r(o, fn.Unmount)
     }
     return {
         children: t,
         register: i,
         unregister: r
     }
 }
@@ -14511,62 +14515,62 @@
             function l() {
                 o.value |= dt.Closing, t("beforeLeave")
             }
 
             function u() {
                 o.value &= ~dt.Closing, t("afterLeave")
             }
-            if (!yE() && Bb()) return () => ze(sl, {
+            if (!gE() && Qb()) return () => ze(sl, {
                 ...e,
                 onBeforeEnter: s,
                 onAfterEnter: a,
                 onBeforeLeave: l,
                 onAfterLeave: u
             }, r);
             let c = oe(null),
-                d = ue(() => e.unmount ? cn.Unmount : cn.Hidden);
+                d = ue(() => e.unmount ? fn.Unmount : fn.Hidden);
             i({
                 el: c,
                 $el: c
             });
             let {
                 show: f,
                 appear: h
-            } = gE(), {
+            } = bE(), {
                 register: p,
                 unregister: m
-            } = bE(), b = oe(f.value ? "visible" : "hidden"), y = {
+            } = EE(), b = oe(f.value ? "visible" : "hidden"), y = {
                 value: !0
             }, _ = tl(), E = {
                 value: !1
             }, S = Oh(() => {
                 !E.value && b.value !== "hidden" && (b.value = "hidden", m(_), u())
             });
             at(() => {
                 let Y = p(_);
                 yt(Y)
             }), Ot(() => {
-                if (d.value === cn.Hidden && _) {
+                if (d.value === fn.Hidden && _) {
                     if (f.value && b.value !== "visible") {
                         b.value = "visible";
                         return
                     }
                     Lt(b.value, {
                         hidden: () => m(_),
                         visible: () => p(_)
                     })
                 }
             });
-            let T = Cn(e.enter),
-                O = Cn(e.enterFrom),
-                F = Cn(e.enterTo),
-                A = Cn(e.entered),
-                R = Cn(e.leave),
-                M = Cn(e.leaveFrom),
-                ne = Cn(e.leaveTo);
+            let T = kn(e.enter),
+                O = kn(e.enterFrom),
+                F = kn(e.enterTo),
+                A = kn(e.entered),
+                R = kn(e.leave),
+                M = kn(e.leaveFrom),
+                ne = kn(e.leaveTo);
             at(() => {
                 Ot(() => {
                     if (b.value === "visible") {
                         let Y = Qe(c);
                         if (Y instanceof Comment && Y.data === "") throw new Error("Did you forget to passthrough the `ref` to the actual DOM node?")
                     }
                 })
@@ -14583,15 +14587,15 @@
             }
             return at(() => {
                 Le([f], (Y, he, H) => {
                     V(H), y.value = !1
                 }, {
                     immediate: !0
                 })
-            }), rt(ol, S), Qb(ue(() => Lt(b.value, {
+            }), rt(ol, S), Ub(ue(() => Lt(b.value, {
                 visible: dt.Open,
                 hidden: dt.Closed
             }) | o.value)), () => {
                 let {
                     appear: Y,
                     show: he,
                     enter: H,
@@ -14619,15 +14623,15 @@
                     features: Th,
                     visible: b.value === "visible",
                     name: "TransitionChild"
                 })
             }
         }
     }),
-    EE = ar,
+    _E = ar,
     sl = gt({
         inheritAttrs: !1,
         props: {
             as: {
                 type: [Object, String],
                 default: "div"
             },
@@ -14711,15 +14715,15 @@
                         ...d,
                         as: "template"
                     },
                     theirProps: {},
                     slot: {},
                     slots: {
                         ...r,
-                        default: () => [ze(EE, {
+                        default: () => [ze(_E, {
                             onBeforeEnter: () => t("beforeEnter"),
                             onAfterEnter: () => t("afterEnter"),
                             onBeforeLeave: () => t("beforeLeave"),
                             onAfterLeave: () => t("afterLeave"),
                             ...n,
                             ...d,
                             ...c
@@ -14730,62 +14734,62 @@
                     visible: s.value === "visible",
                     name: "Transition"
                 })
             }
         }
     });
 
-function _E(e, t) {
-    return Oe(), Ye("svg", {
+function wE(e, t) {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         viewBox: "0 0 20 20",
         fill: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
     }, [W("path", {
         "fill-rule": "evenodd",
         d: "M2 4.75A.75.75 0 0 1 2.75 4h14.5a.75.75 0 0 1 0 1.5H2.75A.75.75 0 0 1 2 4.75ZM2 10a.75.75 0 0 1 .75-.75h14.5a.75.75 0 0 1 0 1.5H2.75A.75.75 0 0 1 2 10Zm0 5.25a.75.75 0 0 1 .75-.75h14.5a.75.75 0 0 1 0 1.5H2.75a.75.75 0 0 1-.75-.75Z",
         "clip-rule": "evenodd"
     })])
 }
 
-function wE(e, t) {
-    return Oe(), Ye("svg", {
+function SE(e, t) {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
         stroke: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
     }, [W("path", {
         "stroke-linecap": "round",
         "stroke-linejoin": "round",
         d: "M7.5 14.25v2.25m3-4.5v4.5m3-6.75v6.75m3-9v9M6 20.25h12A2.25 2.25 0 0 0 20.25 18V6A2.25 2.25 0 0 0 18 3.75H6A2.25 2.25 0 0 0 3.75 6v12A2.25 2.25 0 0 0 6 20.25Z"
     })])
 }
 
-function SE(e, t) {
-    return Oe(), Ye("svg", {
+function xE(e, t) {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
         stroke: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
     }, [W("path", {
         "stroke-linecap": "round",
         "stroke-linejoin": "round",
         d: "M20.25 6.375c0 2.278-3.694 4.125-8.25 4.125S3.75 8.653 3.75 6.375m16.5 0c0-2.278-3.694-4.125-8.25-4.125S3.75 4.097 3.75 6.375m16.5 0v11.25c0 2.278-3.694 4.125-8.25 4.125s-8.25-1.847-8.25-4.125V6.375m16.5 0v3.75m-16.5-3.75v3.75m16.5 0v3.75C20.25 16.153 16.556 18 12 18s-8.25-1.847-8.25-4.125v-3.75m16.5 0c0 2.278-3.694 4.125-8.25 4.125s-8.25-1.847-8.25-4.125"
     })])
 }
 
-function xE(e, t) {
-    return Oe(), Ye("svg", {
+function OE(e, t) {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
         stroke: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
@@ -14796,48 +14800,48 @@
     }), W("path", {
         "stroke-linecap": "round",
         "stroke-linejoin": "round",
         d: "M15 12a3 3 0 1 1-6 0 3 3 0 0 1 6 0Z"
     })])
 }
 
-function OE(e, t) {
-    return Oe(), Ye("svg", {
+function TE(e, t) {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
         stroke: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
     }, [W("path", {
         "stroke-linecap": "round",
         "stroke-linejoin": "round",
         d: "M12 9v3.75m9-.75a9 9 0 1 1-18 0 9 9 0 0 1 18 0Zm-9 3.75h.008v.008H12v-.008Z"
     })])
 }
 
-function TE(e, t) {
-    return Oe(), Ye("svg", {
+function CE(e, t) {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
         stroke: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
     }, [W("path", {
         "stroke-linecap": "round",
         "stroke-linejoin": "round",
         d: "M3.75 6A2.25 2.25 0 0 1 6 3.75h2.25A2.25 2.25 0 0 1 10.5 6v2.25a2.25 2.25 0 0 1-2.25 2.25H6a2.25 2.25 0 0 1-2.25-2.25V6ZM3.75 15.75A2.25 2.25 0 0 1 6 13.5h2.25a2.25 2.25 0 0 1 2.25 2.25V18a2.25 2.25 0 0 1-2.25 2.25H6A2.25 2.25 0 0 1 3.75 18v-2.25ZM13.5 6a2.25 2.25 0 0 1 2.25-2.25H18A2.25 2.25 0 0 1 20.25 6v2.25A2.25 2.25 0 0 1 18 10.5h-2.25a2.25 2.25 0 0 1-2.25-2.25V6ZM13.5 15.75a2.25 2.25 0 0 1 2.25-2.25H18a2.25 2.25 0 0 1 2.25 2.25V18A2.25 2.25 0 0 1 18 20.25h-2.25A2.25 2.25 0 0 1 13.5 18v-2.25Z"
     })])
 }
 
-function CE(e, t) {
-    return Oe(), Ye("svg", {
+function kE(e, t) {
+    return Te(), Ye("svg", {
         xmlns: "http://www.w3.org/2000/svg",
         fill: "none",
         viewBox: "0 0 24 24",
         "stroke-width": "1.5",
         stroke: "currentColor",
         "aria-hidden": "true",
         "data-slot": "icon"
@@ -14850,15 +14854,15 @@
 /*!
  * vue-router v4.3.2
  * (c) 2024 Eduardo San Martin Morote
  * @license MIT
  */
 const Hn = typeof document < "u";
 
-function kE(e) {
+function AE(e) {
     return e.__esModule || e[Symbol.toStringTag] === "Module"
 }
 const xe = Object.assign;
 
 function us(e, t) {
     const n = {};
     for (const r in t) {
@@ -14866,110 +14870,110 @@
         n[r] = Ct(i) ? i.map(e) : e(i)
     }
     return n
 }
 const Gr = () => {},
     Ct = Array.isArray,
     Ch = /#/g,
-    AE = /&/g,
-    RE = /\//g,
-    IE = /=/g,
-    DE = /\?/g,
+    RE = /&/g,
+    IE = /\//g,
+    DE = /=/g,
+    NE = /\?/g,
     kh = /\+/g,
-    NE = /%5B/g,
-    PE = /%5D/g,
+    PE = /%5B/g,
+    FE = /%5D/g,
     Ah = /%5E/g,
-    FE = /%60/g,
+    LE = /%60/g,
     Rh = /%7B/g,
-    LE = /%7C/g,
+    ME = /%7C/g,
     Ih = /%7D/g,
-    ME = /%20/g;
+    jE = /%20/g;
 
 function al(e) {
-    return encodeURI("" + e).replace(LE, "|").replace(NE, "[").replace(PE, "]")
+    return encodeURI("" + e).replace(ME, "|").replace(PE, "[").replace(FE, "]")
 }
 
-function jE(e) {
+function VE(e) {
     return al(e).replace(Rh, "{").replace(Ih, "}").replace(Ah, "^")
 }
 
 function aa(e) {
-    return al(e).replace(kh, "%2B").replace(ME, "+").replace(Ch, "%23").replace(AE, "%26").replace(FE, "`").replace(Rh, "{").replace(Ih, "}").replace(Ah, "^")
-}
-
-function VE(e) {
-    return aa(e).replace(IE, "%3D")
+    return al(e).replace(kh, "%2B").replace(jE, "+").replace(Ch, "%23").replace(RE, "%26").replace(LE, "`").replace(Rh, "{").replace(Ih, "}").replace(Ah, "^")
 }
 
 function $E(e) {
-    return al(e).replace(Ch, "%23").replace(DE, "%3F")
+    return aa(e).replace(DE, "%3D")
 }
 
 function qE(e) {
-    return e == null ? "" : $E(e).replace(RE, "%2F")
+    return al(e).replace(Ch, "%23").replace(NE, "%3F")
+}
+
+function BE(e) {
+    return e == null ? "" : qE(e).replace(IE, "%2F")
 }
 
 function li(e) {
     try {
         return decodeURIComponent("" + e)
     } catch {}
     return "" + e
 }
-const BE = /\/$/,
-    QE = e => e.replace(BE, "");
+const QE = /\/$/,
+    UE = e => e.replace(QE, "");
 
 function cs(e, t, n = "/") {
     let r, i = {},
         o = "",
         s = "";
     const a = t.indexOf("#");
     let l = t.indexOf("?");
-    return a < l && a >= 0 && (l = -1), l > -1 && (r = t.slice(0, l), o = t.slice(l + 1, a > -1 ? a : t.length), i = e(o)), a > -1 && (r = r || t.slice(0, a), s = t.slice(a, t.length)), r = HE(r ?? t, n), {
+    return a < l && a >= 0 && (l = -1), l > -1 && (r = t.slice(0, l), o = t.slice(l + 1, a > -1 ? a : t.length), i = e(o)), a > -1 && (r = r || t.slice(0, a), s = t.slice(a, t.length)), r = GE(r ?? t, n), {
         fullPath: r + (o && "?") + o + s,
         path: r,
         query: i,
         hash: li(s)
     }
 }
 
-function UE(e, t) {
+function zE(e, t) {
     const n = t.query ? e(t.query) : "";
     return t.path + (n && "?") + n + (t.hash || "")
 }
 
 function rc(e, t) {
     return !t || !e.toLowerCase().startsWith(t.toLowerCase()) ? e : e.slice(t.length) || "/"
 }
 
-function zE(e, t, n) {
+function WE(e, t, n) {
     const r = t.matched.length - 1,
         i = n.matched.length - 1;
     return r > -1 && r === i && pr(t.matched[r], n.matched[i]) && Dh(t.params, n.params) && e(t.query) === e(n.query) && t.hash === n.hash
 }
 
 function pr(e, t) {
     return (e.aliasOf || e) === (t.aliasOf || t)
 }
 
 function Dh(e, t) {
     if (Object.keys(e).length !== Object.keys(t).length) return !1;
     for (const n in e)
-        if (!WE(e[n], t[n])) return !1;
+        if (!HE(e[n], t[n])) return !1;
     return !0
 }
 
-function WE(e, t) {
+function HE(e, t) {
     return Ct(e) ? ic(e, t) : Ct(t) ? ic(t, e) : e === t
 }
 
 function ic(e, t) {
     return Ct(t) ? e.length === t.length && e.every((n, r) => n === t[r]) : e.length === 1 && e[0] === t
 }
 
-function HE(e, t) {
+function GE(e, t) {
     if (e.startsWith("/")) return e;
     if (!e) return t;
     const n = t.split("/"),
         r = e.split("/"),
         i = r[r.length - 1];
     (i === ".." || i === ".") && r.push("");
     let o = n.length - 1,
@@ -14985,68 +14989,68 @@
     e.pop = "pop", e.push = "push"
 })(ui || (ui = {}));
 var Kr;
 (function(e) {
     e.back = "back", e.forward = "forward", e.unknown = ""
 })(Kr || (Kr = {}));
 
-function GE(e) {
+function KE(e) {
     if (!e)
         if (Hn) {
             const t = document.querySelector("base");
             e = t && t.getAttribute("href") || "/", e = e.replace(/^\w+:\/\/[^\/]+/, "")
         } else e = "/";
-    return e[0] !== "/" && e[0] !== "#" && (e = "/" + e), QE(e)
+    return e[0] !== "/" && e[0] !== "#" && (e = "/" + e), UE(e)
 }
-const KE = /^[^#]+#/;
+const YE = /^[^#]+#/;
 
-function YE(e, t) {
-    return e.replace(KE, "#") + t
+function JE(e, t) {
+    return e.replace(YE, "#") + t
 }
 
-function JE(e, t) {
+function XE(e, t) {
     const n = document.documentElement.getBoundingClientRect(),
         r = e.getBoundingClientRect();
     return {
         behavior: t.behavior,
         left: r.left - n.left - (t.left || 0),
         top: r.top - n.top - (t.top || 0)
     }
 }
 const Ro = () => ({
     left: window.scrollX,
     top: window.scrollY
 });
 
-function XE(e) {
+function ZE(e) {
     let t;
     if ("el" in e) {
         const n = e.el,
             r = typeof n == "string" && n.startsWith("#"),
             i = typeof n == "string" ? r ? document.getElementById(n.slice(1)) : document.querySelector(n) : n;
         if (!i) return;
-        t = JE(i, e)
+        t = XE(i, e)
     } else t = e;
     "scrollBehavior" in document.documentElement.style ? window.scrollTo(t) : window.scrollTo(t.left != null ? t.left : window.scrollX, t.top != null ? t.top : window.scrollY)
 }
 
 function oc(e, t) {
     return (history.state ? history.state.position - t : -1) + e
 }
 const la = new Map;
 
-function ZE(e, t) {
+function e_(e, t) {
     la.set(e, t)
 }
 
-function e_(e) {
+function t_(e) {
     const t = la.get(e);
     return la.delete(e), t
 }
-let t_ = () => location.protocol + "//" + location.host;
+let n_ = () => location.protocol + "//" + location.host;
 
 function Nh(e, t) {
     const {
         pathname: n,
         search: r,
         hash: i
     } = t, o = e.indexOf("#");
@@ -15054,15 +15058,15 @@
         let a = i.includes(e.slice(o)) ? e.slice(o).length : 1,
             l = i.slice(a);
         return l[0] !== "/" && (l = "/" + l), rc(l, "")
     }
     return rc(n, e) + r + i
 }
 
-function n_(e, t, n, r) {
+function r_(e, t, n, r) {
     let i = [],
         o = [],
         s = null;
     const a = ({
         state: f
     }) => {
         const h = Nh(e, location),
@@ -15127,15 +15131,15 @@
         forward: n,
         replaced: r,
         position: window.history.length,
         scroll: i ? Ro() : null
     }
 }
 
-function r_(e) {
+function i_(e) {
     const {
         history: t,
         location: n
     } = window, r = {
         value: Nh(e, n)
     }, i = {
         value: t.state
@@ -15147,15 +15151,15 @@
         position: t.length - 1,
         replaced: !0,
         scroll: null
     }, !0);
 
     function o(l, u, c) {
         const d = e.indexOf("#"),
-            f = d > -1 ? (n.host && document.querySelector("base") ? e : e.slice(d)) + l : t_() + e + l;
+            f = d > -1 ? (n.host && document.querySelector("base") ? e : e.slice(d)) + l : n_() + e + l;
         try {
             t[c ? "replaceState" : "pushState"](u, "", f), i.value = u
         } catch (h) {
             console.error(h), n[c ? "replace" : "assign"](f)
         }
     }
 
@@ -15181,38 +15185,38 @@
         location: r,
         state: i,
         push: a,
         replace: s
     }
 }
 
-function i_(e) {
-    e = GE(e);
-    const t = r_(e),
-        n = n_(e, t.state, t.location, t.replace);
+function o_(e) {
+    e = KE(e);
+    const t = i_(e),
+        n = r_(e, t.state, t.location, t.replace);
 
     function r(o, s = !0) {
         s || n.pauseListeners(), history.go(o)
     }
     const i = xe({
         location: "",
         base: e,
         go: r,
-        createHref: YE.bind(null, e)
+        createHref: JE.bind(null, e)
     }, t, n);
     return Object.defineProperty(i, "location", {
         enumerable: !0,
         get: () => t.location.value
     }), Object.defineProperty(i, "state", {
         enumerable: !0,
         get: () => t.state.value
     }), i
 }
 
-function o_(e) {
+function s_(e) {
     return typeof e == "string" || e && typeof e == "object"
 }
 
 function Ph(e) {
     return typeof e == "string" || typeof e == "symbol"
 }
 const Yt = {
@@ -15239,34 +15243,34 @@
     }, t)
 }
 
 function jt(e, t) {
     return e instanceof Error && Fh in e && (t == null || !!(e.type & t))
 }
 const lc = "[^/]+?",
-    s_ = {
+    a_ = {
         sensitive: !1,
         strict: !1,
         start: !0,
         end: !0
     },
-    a_ = /[.+*?^${}()[\]/\\]/g;
+    l_ = /[.+*?^${}()[\]/\\]/g;
 
-function l_(e, t) {
-    const n = xe({}, s_, t),
+function u_(e, t) {
+    const n = xe({}, a_, t),
         r = [];
     let i = n.start ? "^" : "";
     const o = [];
     for (const u of e) {
         const c = u.length ? [] : [90];
         n.strict && !u.length && (i += "/");
         for (let d = 0; d < u.length; d++) {
             const f = u[d];
             let h = 40 + (n.sensitive ? .25 : 0);
-            if (f.type === 0) d || (i += "/"), i += f.value.replace(a_, "\\$&"), h += 40;
+            if (f.type === 0) d || (i += "/"), i += f.value.replace(l_, "\\$&"), h += 40;
             else if (f.type === 1) {
                 const {
                     value: p,
                     repeatable: m,
                     optional: b,
                     regexp: y
                 } = f;
@@ -15338,56 +15342,56 @@
         score: r,
         keys: o,
         parse: a,
         stringify: l
     }
 }
 
-function u_(e, t) {
+function c_(e, t) {
     let n = 0;
     for (; n < e.length && n < t.length;) {
         const r = t[n] - e[n];
         if (r) return r;
         n++
     }
     return e.length < t.length ? e.length === 1 && e[0] === 80 ? -1 : 1 : e.length > t.length ? t.length === 1 && t[0] === 80 ? 1 : -1 : 0
 }
 
-function c_(e, t) {
+function f_(e, t) {
     let n = 0;
     const r = e.score,
         i = t.score;
     for (; n < r.length && n < i.length;) {
-        const o = u_(r[n], i[n]);
+        const o = c_(r[n], i[n]);
         if (o) return o;
         n++
     }
     if (Math.abs(i.length - r.length) === 1) {
         if (uc(r)) return 1;
         if (uc(i)) return -1
     }
     return i.length - r.length
 }
 
 function uc(e) {
     const t = e[e.length - 1];
     return e.length > 0 && t[t.length - 1] < 0
 }
-const f_ = {
+const d_ = {
         type: 0,
         value: ""
     },
-    d_ = /[a-zA-Z0-9_]/;
+    h_ = /[a-zA-Z0-9_]/;
 
-function h_(e) {
+function p_(e) {
     if (!e) return [
         []
     ];
     if (e === "/") return [
-        [f_]
+        [d_]
     ];
     if (!e.startsWith("/")) throw new Error(`Invalid path "${e}"`);
 
     function t(h) {
         throw new Error(`ERR (${n})/"${u}": ${h}`)
     }
     let n = 0,
@@ -15427,15 +15431,15 @@
             case 0:
                 l === "/" ? (u && d(), s()) : l === ":" ? (d(), n = 1) : f();
                 break;
             case 4:
                 f(), n = r;
                 break;
             case 1:
-                l === "(" ? n = 2 : d_.test(l) ? f() : (d(), n = 0, l !== "*" && l !== "?" && l !== "+" && a--);
+                l === "(" ? n = 2 : h_.test(l) ? f() : (d(), n = 0, l !== "*" && l !== "?" && l !== "+" && a--);
                 break;
             case 2:
                 l === ")" ? c[c.length - 1] == "\\" ? c = c.slice(0, -1) + l : n = 3 : c += l;
                 break;
             case 3:
                 d(), n = 0, l !== "*" && l !== "?" && l !== "+" && a--, c = "";
                 break;
@@ -15443,41 +15447,41 @@
                 t("Unknown state");
                 break
         }
     }
     return n === 2 && t(`Unfinished custom RegExp for param "${u}"`), d(), s(), i
 }
 
-function p_(e, t, n) {
-    const r = l_(h_(e.path), n),
+function v_(e, t, n) {
+    const r = u_(p_(e.path), n),
         i = xe(r, {
             record: e,
             parent: t,
             children: [],
             alias: []
         });
     return t && !i.record.aliasOf == !t.record.aliasOf && t.children.push(i), i
 }
 
-function v_(e, t) {
+function m_(e, t) {
     const n = [],
         r = new Map;
     t = dc({
         strict: !1,
         end: !0,
         sensitive: !1
     }, t);
 
     function i(c) {
         return r.get(c)
     }
 
     function o(c, d, f) {
         const h = !f,
-            p = m_(c);
+            p = y_(c);
         p.aliasOf = f && f.record;
         const m = dc(t, c),
             b = [p];
         if ("alias" in c) {
             const E = typeof c.alias == "string" ? [c.alias] : c.alias;
             for (const S of E) b.push(xe({}, p, {
                 components: f ? f.record.components : p.components,
@@ -15491,15 +15495,15 @@
                 path: S
             } = E;
             if (d && S[0] !== "/") {
                 const T = d.record.path,
                     O = T[T.length - 1] === "/" ? "" : "/";
                 E.path = d.record.path + (S && O + S)
             }
-            if (y = p_(E, d, m), f ? f.alias.push(y) : (_ = _ || y, _ !== y && _.alias.push(y), h && c.name && !fc(y) && s(c.name)), p.children) {
+            if (y = v_(E, d, m), f ? f.alias.push(y) : (_ = _ || y, _ !== y && _.alias.push(y), h && c.name && !fc(y) && s(c.name)), p.children) {
                 const T = p.children;
                 for (let O = 0; O < T.length; O++) o(T[O], y, f && f.children[O])
             }
             f = f || y, (y.record.components && Object.keys(y.record.components).length || y.record.name || y.record.redirect) && l(y)
         }
         return _ ? () => {
             s(_)
@@ -15518,15 +15522,15 @@
 
     function a() {
         return n
     }
 
     function l(c) {
         let d = 0;
-        for (; d < n.length && c_(c, n[d]) >= 0 && (c.record.path !== n[d].record.path || !Lh(c, n[d]));) d++;
+        for (; d < n.length && f_(c, n[d]) >= 0 && (c.record.path !== n[d].record.path || !Lh(c, n[d]));) d++;
         n.splice(d, 0, c), c.record.name && !fc(c) && r.set(c.record.name, c)
     }
 
     function u(c, d) {
         let f, h = {},
             p, m;
         if ("name" in c && c.name) {
@@ -15546,15 +15550,15 @@
         let y = f;
         for (; y;) b.unshift(y.record), y = y.parent;
         return {
             name: m,
             path: p,
             params: h,
             matched: b,
-            meta: g_(b)
+            meta: b_(b)
         }
     }
     return e.forEach(c => o(c)), {
         addRoute: o,
         resolve: u,
         removeRoute: s,
         getRoutes: a,
@@ -15564,35 +15568,35 @@
 
 function cc(e, t) {
     const n = {};
     for (const r of t) r in e && (n[r] = e[r]);
     return n
 }
 
-function m_(e) {
+function y_(e) {
     return {
         path: e.path,
         redirect: e.redirect,
         name: e.name,
         meta: e.meta || {},
         aliasOf: void 0,
         beforeEnter: e.beforeEnter,
-        props: y_(e),
+        props: g_(e),
         children: e.children || [],
         instances: {},
         leaveGuards: new Set,
         updateGuards: new Set,
         enterCallbacks: {},
         components: "components" in e ? e.components || null : e.component && {
             default: e.component
         }
     }
 }
 
-function y_(e) {
+function g_(e) {
     const t = {},
         n = e.props || !1;
     if ("component" in e) t.default = n;
     else
         for (const r in e.components) t[r] = typeof n == "object" ? n[r] : n;
     return t
 }
@@ -15601,29 +15605,29 @@
     for (; e;) {
         if (e.record.aliasOf) return !0;
         e = e.parent
     }
     return !1
 }
 
-function g_(e) {
+function b_(e) {
     return e.reduce((t, n) => xe(t, n.meta), {})
 }
 
 function dc(e, t) {
     const n = {};
     for (const r in e) n[r] = r in t ? t[r] : e[r];
     return n
 }
 
 function Lh(e, t) {
     return t.children.some(n => n === e || Lh(e, n))
 }
 
-function b_(e) {
+function E_(e) {
     const t = {};
     if (e === "" || e === "?") return t;
     const r = (e[0] === "?" ? e.slice(1) : e).split("&");
     for (let i = 0; i < r.length; ++i) {
         const o = r[i].replace(kh, " "),
             s = o.indexOf("="),
             a = li(s < 0 ? o : o.slice(0, s)),
@@ -15636,33 +15640,33 @@
     return t
 }
 
 function hc(e) {
     let t = "";
     for (let n in e) {
         const r = e[n];
-        if (n = VE(n), r == null) {
+        if (n = $E(n), r == null) {
             r !== void 0 && (t += (t.length ? "&" : "") + n);
             continue
         }(Ct(r) ? r.map(o => o && aa(o)) : [r && aa(r)]).forEach(o => {
             o !== void 0 && (t += (t.length ? "&" : "") + n, o != null && (t += "=" + o))
         })
     }
     return t
 }
 
-function E_(e) {
+function __(e) {
     const t = {};
     for (const n in e) {
         const r = e[n];
         r !== void 0 && (t[n] = Ct(r) ? r.map(i => i == null ? null : "" + i) : r == null ? r : "" + r)
     }
     return t
 }
-const __ = Symbol(""),
+const w_ = Symbol(""),
     pc = Symbol(""),
     Io = Symbol(""),
     ll = Symbol(""),
     ua = Symbol("");
 
 function Dr() {
     let e = [];
@@ -15687,15 +15691,15 @@
 function ln(e, t, n, r, i, o = s => s()) {
     const s = r && (r.enterCallbacks[i] = r.enterCallbacks[i] || []);
     return () => new Promise((a, l) => {
         const u = f => {
                 f === !1 ? l(vr(4, {
                     from: n,
                     to: t
-                })) : f instanceof Error ? l(f) : o_(f) ? l(vr(2, {
+                })) : f instanceof Error ? l(f) : s_(f) ? l(vr(2, {
                     from: t,
                     to: f
                 })) : (s && r.enterCallbacks[i] === s && typeof f == "function" && s.push(f), a())
             },
             c = o(() => e.call(r && r.instances[i], t, n, u));
         let d = Promise.resolve(c);
         e.length < 3 && (d = d.then(u)), d.catch(f => l(f))
@@ -15704,69 +15708,69 @@
 
 function fs(e, t, n, r, i = o => o()) {
     const o = [];
     for (const s of e)
         for (const a in s.components) {
             let l = s.components[a];
             if (!(t !== "beforeRouteEnter" && !s.instances[a]))
-                if (w_(l)) {
+                if (S_(l)) {
                     const c = (l.__vccOpts || l)[t];
                     c && o.push(ln(c, n, r, s, a, i))
                 } else {
                     let u = l();
                     o.push(() => u.then(c => {
                         if (!c) return Promise.reject(new Error(`Couldn't resolve component "${a}" at "${s.path}"`));
-                        const d = kE(c) ? c.default : c;
+                        const d = AE(c) ? c.default : c;
                         s.components[a] = d;
                         const h = (d.__vccOpts || d)[t];
                         return h && ln(h, n, r, s, a, i)()
                     }))
                 }
         }
     return o
 }
 
-function w_(e) {
+function S_(e) {
     return typeof e == "object" || "displayName" in e || "props" in e || "__vccOpts" in e
 }
 
 function vc(e) {
     const t = Ie(Io),
         n = Ie(ll),
         r = ue(() => {
-            const l = ke(e.to);
+            const l = Oe(e.to);
             return t.resolve(l)
         }),
         i = ue(() => {
             const {
                 matched: l
             } = r.value, {
                 length: u
             } = l, c = l[u - 1], d = n.matched;
             if (!c || !d.length) return -1;
             const f = d.findIndex(pr.bind(null, c));
             if (f > -1) return f;
             const h = mc(l[u - 2]);
             return u > 1 && mc(c) === h && d[d.length - 1].path !== h ? d.findIndex(pr.bind(null, l[u - 2])) : f
         }),
-        o = ue(() => i.value > -1 && O_(n.params, r.value.params)),
+        o = ue(() => i.value > -1 && T_(n.params, r.value.params)),
         s = ue(() => i.value > -1 && i.value === n.matched.length - 1 && Dh(n.params, r.value.params));
 
     function a(l = {}) {
-        return x_(l) ? t[ke(e.replace) ? "replace" : "push"](ke(e.to)).catch(Gr) : Promise.resolve()
+        return O_(l) ? t[Oe(e.replace) ? "replace" : "push"](Oe(e.to)).catch(Gr) : Promise.resolve()
     }
     return {
         route: r,
         href: ue(() => r.value.href),
         isActive: o,
         isExactActive: s,
         navigate: a
     }
 }
-const S_ = gt({
+const x_ = gt({
         name: "RouterLink",
         compatConfig: {
             MODE: 3
         },
         props: {
             to: {
                 type: [String, Object],
@@ -15800,42 +15804,42 @@
                     href: n.href,
                     onClick: n.navigate,
                     class: i.value
                 }, o)
             }
         }
     }),
-    Mh = S_;
+    Mh = x_;
 
-function x_(e) {
+function O_(e) {
     if (!(e.metaKey || e.altKey || e.ctrlKey || e.shiftKey) && !e.defaultPrevented && !(e.button !== void 0 && e.button !== 0)) {
         if (e.currentTarget && e.currentTarget.getAttribute) {
             const t = e.currentTarget.getAttribute("target");
             if (/\b_blank\b/i.test(t)) return
         }
         return e.preventDefault && e.preventDefault(), !0
     }
 }
 
-function O_(e, t) {
+function T_(e, t) {
     for (const n in t) {
         const r = t[n],
             i = e[n];
         if (typeof r == "string") {
             if (r !== i) return !1
         } else if (!Ct(i) || i.length !== r.length || r.some((o, s) => o !== i[s])) return !1
     }
     return !0
 }
 
 function mc(e) {
     return e ? e.aliasOf ? e.aliasOf.path : e.path : ""
 }
 const yc = (e, t, n) => e ?? t ?? n,
-    T_ = gt({
+    C_ = gt({
         name: "RouterView",
         inheritAttrs: !1,
         props: {
             name: {
                 type: String,
                 default: "default"
             },
@@ -15848,25 +15852,25 @@
             attrs: t,
             slots: n
         }) {
             const r = Ie(ua),
                 i = ue(() => e.route || r.value),
                 o = Ie(pc, 0),
                 s = ue(() => {
-                    let u = ke(o);
+                    let u = Oe(o);
                     const {
                         matched: c
                     } = i.value;
                     let d;
                     for (;
                         (d = c[u]) && !d.components;) u++;
                     return u
                 }),
                 a = ue(() => i.value.matched[s.value]);
-            rt(pc, ue(() => s.value + 1)), rt(__, a), rt(ua, i);
+            rt(pc, ue(() => s.value + 1)), rt(w_, a), rt(ua, i);
             const l = oe();
             return Le(() => [l.value, a.value, e.name], ([u, c, d], [f, h, p]) => {
                 c && (c.instances[d] = u, h && h !== c && u && u === f && (c.leaveGuards.size || (c.leaveGuards = h.leaveGuards), c.updateGuards.size || (c.updateGuards = h.updateGuards))), u && c && (!h || !pr(c, h) || !f) && (c.enterCallbacks[d] || []).forEach(m => m(u))
             }, {
                 flush: "post"
             }), () => {
                 const u = i.value,
@@ -15894,29 +15898,29 @@
     });
 
 function gc(e, t) {
     if (!e) return null;
     const n = e(t);
     return n.length === 1 ? n[0] : n
 }
-const jh = T_;
+const jh = C_;
 
-function C_(e) {
-    const t = v_(e.routes, e),
-        n = e.parseQuery || b_,
+function k_(e) {
+    const t = m_(e.routes, e),
+        n = e.parseQuery || E_,
         r = e.stringifyQuery || hc,
         i = e.history,
         o = Dr(),
         s = Dr(),
         a = Dr(),
         l = Sa(Yt);
     let u = Yt;
     Hn && e.scrollBehavior && "scrollRestoration" in history && (history.scrollRestoration = "manual");
     const c = us.bind(null, k => "" + k),
-        d = us.bind(null, qE),
+        d = us.bind(null, BE),
         f = us.bind(null, li);
 
     function h(k, K) {
         let Q, ee;
         return Ph(k) ? (Q = t.getRecordMatcher(k), ee = K) : ee = k, t.addRoute(ee, Q)
     }
 
@@ -15957,23 +15961,23 @@
             Q = xe({}, k, {
                 params: d(g)
             }), K.params = d(K.params)
         }
         const ee = t.resolve(Q, K),
             ye = k.hash || "";
         ee.params = c(f(ee.params));
-        const Ae = UE(r, xe({}, k, {
-                hash: jE(ye),
+        const Ae = zE(r, xe({}, k, {
+                hash: VE(ye),
                 path: ee.path
             })),
             v = i.createHref(Ae);
         return xe({
             fullPath: Ae,
             hash: ye,
-            query: r === hc ? E_(k.query) : k.query || {}
+            query: r === hc ? __(k.query) : k.query || {}
         }, ee, {
             redirectedFrom: void 0,
             href: v
         })
     }
 
     function _(k) {
@@ -16025,15 +16029,15 @@
             state: typeof g == "object" ? xe({}, ye, g.state) : ye,
             force: Ae,
             replace: v
         }), K || Q);
         const x = Q;
         x.redirectedFrom = K;
         let P;
-        return !Ae && zE(r, ee, Q) && (P = vr(16, {
+        return !Ae && WE(r, ee, Q) && (P = vr(16, {
             to: x,
             from: ee
         }), G(ee, ee, !0, !1)), (P ? Promise.resolve(P) : M(x, ee)).catch(D => jt(D) ? jt(D, 2) ? D : we(D) : U(D, x, ee)).then(D => {
             if (D) {
                 if (jt(D, 2)) return F(xe({
                     replace: v
                 }, _(D.to), {
@@ -16053,15 +16057,15 @@
     function R(k) {
         const K = Ee.values().next().value;
         return K && typeof K.runWithContext == "function" ? K.runWithContext(k) : k()
     }
 
     function M(k, K) {
         let Q;
-        const [ee, ye, Ae] = k_(k, K);
+        const [ee, ye, Ae] = A_(k, K);
         Q = fs(ee.reverse(), "beforeRouteLeave", k, K);
         for (const g of ee) g.leaveGuards.forEach(x => {
             Q.push(ln(x, k, K))
         });
         const v = A.bind(null, k, K);
         return Q.push(v), fe(Q).then(() => {
             Q = [];
@@ -16112,15 +16116,15 @@
                 F(xe(ye, {
                     replace: !0
                 }), ee).catch(Gr);
                 return
             }
             u = ee;
             const Ae = l.value;
-            Hn && ZE(oc(Ae.fullPath, Q.delta), Ro()), M(ee, Ae).catch(v => jt(v, 12) ? v : jt(v, 2) ? (F(v.to, ee).then(g => {
+            Hn && e_(oc(Ae.fullPath, Q.delta), Ro()), M(ee, Ae).catch(v => jt(v, 12) ? v : jt(v, 2) ? (F(v.to, ee).then(g => {
                 jt(g, 20) && !Q.delta && Q.type === ui.pop && i.go(-1, !1)
             }).catch(Gr), Promise.reject()) : (Q.delta && i.go(-Q.delta, !1), U(v, ee, Ae))).then(v => {
                 v = v || V(ee, Ae, !1), v && (Q.delta && !jt(v, 8) ? i.go(-Q.delta, !1) : Q.type === ui.pop && jt(v, 20) && i.go(-1, !1)), ne(ee, Ae, v)
             }).catch(Gr)
         }))
     }
     let H = Dr(),
@@ -16144,16 +16148,16 @@
     }
 
     function G(k, K, Q, ee) {
         const {
             scrollBehavior: ye
         } = e;
         if (!Hn || !ye) return Promise.resolve();
-        const Ae = !Q && e_(oc(k.fullPath, 0)) || (ee || !Q) && history.state && history.state.scroll || null;
-        return $t().then(() => ye(k, K, Ae)).then(v => v && XE(v)).catch(v => U(v, k, K))
+        const Ae = !Q && t_(oc(k.fullPath, 0)) || (ee || !Q) && history.state && history.state.scroll || null;
+        return $t().then(() => ye(k, K, Ae)).then(v => v && ZE(v)).catch(v => U(v, k, K))
     }
     const re = k => i.go(k);
     let ve;
     const Ee = new Set,
         qe = {
             currentRoute: l,
             listening: !0,
@@ -16173,15 +16177,15 @@
             afterEach: a.add,
             onError: L.add,
             isReady: ie,
             install(k) {
                 const K = this;
                 k.component("RouterLink", Mh), k.component("RouterView", jh), k.config.globalProperties.$router = K, Object.defineProperty(k.config.globalProperties, "$route", {
                     enumerable: !0,
-                    get: () => ke(l)
+                    get: () => Oe(l)
                 }), Hn && !ve && l.value === Yt && (ve = !0, S(i.location).catch(ye => {}));
                 const Q = {};
                 for (const ye in Yt) Object.defineProperty(Q, ye, {
                     get: () => l.value[ye],
                     enumerable: !0
                 });
                 k.provide(Io, K), k.provide(ll, Uc(Q)), k.provide(ua, l);
@@ -16194,33 +16198,33 @@
 
     function fe(k) {
         return k.reduce((K, Q) => K.then(() => R(Q)), Promise.resolve())
     }
     return qe
 }
 
-function k_(e, t) {
+function A_(e, t) {
     const n = [],
         r = [],
         i = [],
         o = Math.max(t.matched.length, e.matched.length);
     for (let s = 0; s < o; s++) {
         const a = t.matched[s];
         a && (e.matched.find(u => pr(u, a)) ? r.push(a) : n.push(a));
         const l = e.matched[s];
         l && (t.matched.find(u => pr(u, l)) || i.push(l))
     }
     return [n, r, i]
 }
 
-function T1() {
+function C1() {
     return Ie(Io)
 }
 
-function C1() {
+function k1() {
     return Ie(ll)
 }
 const ul = Y0("modal", () => {
         const e = oe({}),
             t = oe(!1),
             n = o => {
                 e.value = o, t.value = !0
@@ -16234,270 +16238,270 @@
             openModal: n,
             closeModal: r,
             runCallbackModal: (o = null) => {
                 o ? e.value.callback(o) : e.value.callback(), r()
             }
         }
     }),
-    A_ = W("div", {
+    R_ = W("div", {
         class: "fixed inset-0 bg-black bg-opacity-75 transition-opacity"
     }, null, -1),
-    R_ = {
+    I_ = {
         class: "fixed inset-0 z-50 w-screen overflow-y-auto"
     },
-    I_ = {
+    D_ = {
         class: "flex min-h-full items-end justify-center p-4 text-center sm:items-center sm:p-0"
     },
-    D_ = {
+    N_ = {
         __name: "VModal",
         setup(e) {
             const t = ul();
-            return (n, r) => (Oe(), Tt(ke(sl), {
+            return (n, r) => (Te(), Tt(Oe(sl), {
                 as: "template",
-                show: ke(t).open
+                show: Oe(t).open
             }, {
-                default: et(() => [me(ke(Sh), {
+                default: et(() => [me(Oe(Sh), {
                     as: "div",
                     class: "relative z-50",
-                    onClose: r[0] || (r[0] = i => ke(t).closeModal())
+                    onClose: r[0] || (r[0] = i => Oe(t).closeModal())
                 }, {
-                    default: et(() => [me(ke(ar), {
+                    default: et(() => [me(Oe(ar), {
                         as: "template",
                         enter: "ease-out duration-300",
                         "enter-from": "opacity-0",
                         "enter-to": "opacity-100",
                         leave: "ease-in duration-200",
                         "leave-from": "opacity-100",
                         "leave-to": "opacity-0"
                     }, {
-                        default: et(() => [A_]),
+                        default: et(() => [R_]),
                         _: 1
-                    }), W("div", R_, [W("div", I_, [me(ke(ar), {
+                    }), W("div", I_, [W("div", D_, [me(Oe(ar), {
                         as: "template",
                         enter: "ease-out duration-300",
                         "enter-from": "opacity-0 translate-y-4 sm:translate-y-0 sm:scale-95",
                         "enter-to": "opacity-100 translate-y-0 sm:scale-100",
                         leave: "ease-in duration-200",
                         "leave-from": "opacity-100 translate-y-0 sm:scale-100",
                         "leave-to": "opacity-0 translate-y-4 sm:translate-y-0 sm:scale-95"
                     }, {
-                        default: et(() => [(Oe(), Tt(ho(ke(t).data.component)))]),
+                        default: et(() => [(Te(), Tt(ho(Oe(t).data.component)))]),
                         _: 1
                     })])])]),
                     _: 1
                 })]),
                 _: 1
             }, 8, ["show"]))
         }
     },
-    N_ = {
+    P_ = {
         class: "flex grow flex-col gap-y-5 overflow-y-auto bg-black/20 px-6"
     },
-    P_ = W("div", {
+    F_ = W("div", {
         class: "flex h-16 shrink-0 items-center"
     }, [W("svg", {
         class: "h-10 w-auto fill-primary stroke-primary stroke-[0.5px]",
         viewBox: "0 0 32 32",
         xmlns: "http://www.w3.org/2000/svg"
     }, [W("path", {
         d: "M 16 3 C 14.0625 3 12.570313 3.507813 11.5 4.34375 C 10.429688 5.179688 9.8125 6.304688 9.375 7.34375 C 8.9375 8.382813 8.65625 9.378906 8.375 10.09375 C 8.09375 10.808594 7.859375 11.085938 7.65625 11.15625 C 4.828125 12.160156 3 14.863281 3 18 L 3 19 L 4 19 C 5.347656 19 6.003906 19.28125 6.3125 19.53125 C 6.621094 19.78125 6.742188 20.066406 6.8125 20.5625 C 6.882813 21.058594 6.847656 21.664063 6.9375 22.34375 C 6.984375 22.683594 7.054688 23.066406 7.28125 23.4375 C 7.507813 23.808594 7.917969 24.128906 8.375 24.28125 C 9.433594 24.632813 10.113281 24.855469 10.53125 25.09375 C 10.949219 25.332031 11.199219 25.546875 11.53125 26.25 C 11.847656 26.917969 12.273438 27.648438 13.03125 28.1875 C 13.789063 28.726563 14.808594 29.015625 16.09375 29 C 18.195313 28.972656 19.449219 27.886719 20.09375 26.9375 C 20.417969 26.460938 20.644531 26.050781 20.84375 25.78125 C 21.042969 25.511719 21.164063 25.40625 21.375 25.34375 C 22.730469 24.9375 23.605469 24.25 24.09375 23.46875 C 24.582031 22.6875 24.675781 21.921875 24.8125 21.40625 C 24.949219 20.890625 25.046875 20.6875 25.375 20.46875 C 25.703125 20.25 26.453125 20 28 20 L 29 20 L 29 19 C 29 17.621094 29.046875 16.015625 28.4375 14.5 C 27.828125 12.984375 26.441406 11.644531 24.15625 11.125 C 24.132813 11.121094 24.105469 11.132813 24 11 C 23.894531 10.867188 23.734375 10.601563 23.59375 10.25 C 23.3125 9.550781 23.042969 8.527344 22.59375 7.46875 C 22.144531 6.410156 21.503906 5.269531 20.4375 4.40625 C 19.371094 3.542969 17.90625 3 16 3 Z M 16 5 C 17.539063 5 18.480469 5.394531 19.1875 5.96875 C 19.894531 6.542969 20.367188 7.347656 20.75 8.25 C 21.132813 9.152344 21.402344 10.128906 21.75 11 C 21.921875 11.433594 22.109375 11.839844 22.40625 12.21875 C 22.703125 12.597656 23.136719 12.96875 23.6875 13.09375 C 25.488281 13.503906 26.15625 14.242188 26.5625 15.25 C 26.871094 16.015625 26.878906 17.066406 26.90625 18.09375 C 25.796875 18.1875 24.886719 18.386719 24.25 18.8125 C 23.40625 19.378906 23.050781 20.25 22.875 20.90625 C 22.699219 21.5625 22.632813 22.042969 22.40625 22.40625 C 22.179688 22.769531 21.808594 23.128906 20.78125 23.4375 C 20.070313 23.652344 19.558594 24.140625 19.21875 24.59375 C 18.878906 25.046875 18.675781 25.460938 18.4375 25.8125 C 17.960938 26.515625 17.617188 26.980469 16.0625 27 C 15.078125 27.011719 14.550781 26.820313 14.1875 26.5625 C 13.824219 26.304688 13.558594 25.929688 13.3125 25.40625 C 12.867188 24.460938 12.269531 23.765625 11.53125 23.34375 C 10.792969 22.921875 10.023438 22.714844 9 22.375 C 8.992188 22.359375 8.933594 22.285156 8.90625 22.09375 C 8.855469 21.710938 8.886719 21.035156 8.78125 20.28125 C 8.675781 19.527344 8.367188 18.613281 7.5625 17.96875 C 7 17.515625 6.195313 17.289063 5.25 17.15625 C 5.542969 15.230469 6.554688 13.65625 8.3125 13.03125 C 9.375 12.65625 9.898438 11.730469 10.25 10.84375 C 10.601563 9.957031 10.851563 8.96875 11.21875 8.09375 C 11.585938 7.21875 12.019531 6.480469 12.71875 5.9375 C 13.417969 5.394531 14.402344 5 16 5 Z M 13 9 C 12.449219 9 12 9.671875 12 10.5 C 12 11.328125 12.449219 12 13 12 C 13.550781 12 14 11.328125 14 10.5 C 14 9.671875 13.550781 9 13 9 Z M 17 9 C 16.449219 9 16 9.671875 16 10.5 C 16 11.328125 16.449219 12 17 12 C 17.550781 12 18 11.328125 18 10.5 C 18 9.671875 17.550781 9 17 9 Z"
     })])], -1),
-    F_ = {
+    L_ = {
         class: "flex flex-1 flex-col"
     },
-    L_ = {
+    M_ = {
         role: "list",
         class: "flex flex-1 flex-col gap-y-7"
     },
-    M_ = {
+    j_ = {
         role: "list",
         class: "-mx-2 space-y-2"
     },
     bc = {
         __name: "VSidebar",
         setup(e) {
             const t = [{
                 name: "Dashboard",
                 href: {
                     name: "dashboard"
                 },
-                icon: TE
+                icon: CE
             }, {
                 name: "Stacks",
                 href: {
                     name: "stacks"
                 },
-                icon: SE
+                icon: xE
             }, {
                 name: "Containers",
                 href: {
                     name: "containers"
                 },
-                icon: wE
+                icon: SE
             }, {
                 name: "Settings",
                 href: {
                     name: "settings"
                 },
-                icon: xE
+                icon: OE
             }];
-            return (n, r) => (Oe(), Ye("div", N_, [P_, W("nav", F_, [W("ul", L_, [W("li", null, [W("ul", M_, [(Oe(), Ye(Ke, null, df(t, i => W("li", {
+            return (n, r) => (Te(), Ye("div", P_, [F_, W("nav", L_, [W("ul", M_, [W("li", null, [W("ul", j_, [(Te(), Ye(Ke, null, df(t, i => W("li", {
                 key: i.name
-            }, [me(ke(Mh), {
+            }, [me(Oe(Mh), {
                 to: i.href,
                 class: "group flex gap-x-3 rounded-md p-2 text-sm leading-6 font-semibold text-neutral-400 hover:text-white hover:bg-white/5 transition-colors",
                 "active-class": "!text-primary"
             }, {
-                default: et(() => [(Oe(), Tt(ho(i.icon), {
+                default: et(() => [(Te(), Tt(ho(i.icon), {
                     class: "h-6 w-6 shrink-0",
                     "aria-hidden": "true"
-                })), Af(" " + Fn(i.name), 1)]),
+                })), Af(" " + cn(i.name), 1)]),
                 _: 2
             }, 1032, ["to"])])), 64))])])])])]))
         }
     },
-    j_ = W("div", {
+    V_ = W("div", {
         class: "fixed inset-0 bg-neutral-900/80"
     }, null, -1),
-    V_ = {
+    $_ = {
         class: "fixed inset-0 flex"
     },
-    $_ = {
+    q_ = {
         class: "absolute left-full top-0 flex w-16 justify-center pt-5"
     },
-    q_ = {
+    B_ = {
         class: "hidden xl:fixed xl:inset-y-0 xl:z-50 xl:flex xl:w-72 xl:flex-col"
     },
-    B_ = {
+    Q_ = {
         class: "xl:pl-72 h-full"
     },
-    Q_ = {
+    U_ = {
         class: "sticky top-0 z-40 flex h-16 shrink-0 items-center gap-x-6 px-4 shadow-sm sm:px-6 lg:px-8 xl:hidden"
     },
-    U_ = {
+    z_ = {
         class: "lg:pr-96 h-full flex flex-col"
     },
-    z_ = {
+    W_ = {
         class: "relative h-full flex flex-col shell-space bg-neutral-950"
     },
-    W_ = {
+    H_ = {
         class: "flex-1"
     },
-    H_ = {
+    G_ = {
         class: "mx-auto w-full max-w-2xl space-y-10 lg:max-w-5xl"
     },
-    G_ = {
+    K_ = {
         class: "flex flex-col items-center justify-between gap-5 border-t pt-8 border-white/5 sm:flex-row"
     },
-    K_ = {
+    Y_ = {
         class: "text-xs text-neutral-400"
     },
-    Y_ = W("div", {
+    J_ = W("div", {
         class: "flex gap-4"
     }, [W("a", {
         href: "https://github.com/remyz17/odooghost",
         target: "_blank"
     }, [W("svg", {
         viewBox: "0 0 20 20",
         "aria-hidden": "true",
         class: "h-5 w-5 fill-neutral-700 transition group-hover:fill-neurtral-500"
     }, [W("path", {
         fillRule: "evenodd",
         clipRule: "evenodd",
         d: "M10 1.667c-4.605 0-8.334 3.823-8.334 8.544 0 3.78 2.385 6.974 5.698 8.106.417.075.573-.182.573-.406 0-.203-.011-.875-.011-1.592-2.093.397-2.635-.522-2.802-1.002-.094-.246-.5-1.005-.854-1.207-.291-.16-.708-.556-.01-.567.656-.01 1.124.62 1.281.876.75 1.292 1.948.93 2.427.705.073-.555.291-.93.531-1.143-1.854-.213-3.791-.95-3.791-4.218 0-.929.322-1.698.854-2.296-.083-.214-.375-1.09.083-2.265 0 0 .698-.224 2.292.876a7.576 7.576 0 0 1 2.083-.288c.709 0 1.417.096 2.084.288 1.593-1.11 2.291-.875 2.291-.875.459 1.174.167 2.05.084 2.263.53.599.854 1.357.854 2.297 0 3.278-1.948 4.005-3.802 4.219.302.266.563.78.563 1.58 0 1.143-.011 2.061-.011 2.35 0 .224.156.491.573.405a8.365 8.365 0 0 0 4.11-3.116 8.707 8.707 0 0 0 1.567-4.99c0-4.721-3.73-8.545-8.334-8.545Z"
     })])])], -1),
-    J_ = {
+    X_ = {
         class: "bg-black/10 lg:fixed lg:bottom-0 lg:right-0 lg:top-0 lg:w-96 lg:overflow-y-auto"
     },
-    X_ = {
+    Z_ = {
         __name: "App",
         setup(e) {
             const t = oe(!1);
-            return (n, r) => (Oe(), Ye(Ke, null, [me(ke(sl), {
+            return (n, r) => (Te(), Ye(Ke, null, [me(Oe(sl), {
                 as: "template",
                 show: t.value
             }, {
-                default: et(() => [me(ke(Sh), {
+                default: et(() => [me(Oe(Sh), {
                     as: "div",
                     class: "relative z-50 xl:hidden",
                     onClose: r[1] || (r[1] = i => t.value = !1)
                 }, {
-                    default: et(() => [me(ke(ar), {
+                    default: et(() => [me(Oe(ar), {
                         as: "template",
                         enter: "transition-opacity ease-linear duration-300",
                         "enter-from": "opacity-0",
                         "enter-to": "opacity-100",
                         leave: "transition-opacity ease-linear duration-300",
                         "leave-from": "opacity-100",
                         "leave-to": "opacity-0"
                     }, {
-                        default: et(() => [j_]),
+                        default: et(() => [V_]),
                         _: 1
-                    }), W("div", V_, [me(ke(ar), {
+                    }), W("div", $_, [me(Oe(ar), {
                         as: "template",
                         enter: "transition ease-in-out duration-300 transform",
                         "enter-from": "-translate-x-full",
                         "enter-to": "translate-x-0",
                         leave: "transition ease-in-out duration-300 transform",
                         "leave-from": "translate-x-0",
                         "leave-to": "-translate-x-full"
                     }, {
-                        default: et(() => [me(ke(xh), {
+                        default: et(() => [me(Oe(xh), {
                             class: "relative mr-16 flex w-full max-w-xs flex-1"
                         }, {
-                            default: et(() => [me(ke(ar), {
+                            default: et(() => [me(Oe(ar), {
                                 as: "template",
                                 enter: "ease-in-out duration-300",
                                 "enter-from": "opacity-0",
                                 "enter-to": "opacity-100",
                                 leave: "ease-in-out duration-300",
                                 "leave-from": "opacity-100",
                                 "leave-to": "opacity-0"
                             }, {
-                                default: et(() => [W("div", $_, [W("button", {
+                                default: et(() => [W("div", q_, [W("button", {
                                     type: "button",
                                     class: "-m-2.5 p-2.5",
                                     onClick: r[0] || (r[0] = i => t.value = !1)
-                                }, [me(ke(CE), {
+                                }, [me(Oe(kE), {
                                     class: "h-6 w-6 text-white",
                                     "aria-hidden": "true"
                                 })])])]),
                                 _: 1
                             }), me(bc)]),
                             _: 1
                         })]),
                         _: 1
                     })])]),
                     _: 1
                 })]),
                 _: 1
-            }, 8, ["show"]), W("div", q_, [me(bc)]), W("div", B_, [W("div", Q_, [W("button", {
+            }, 8, ["show"]), W("div", B_, [me(bc)]), W("div", Q_, [W("div", U_, [W("button", {
                 type: "button",
                 class: "-m-2.5 p-2.5 text-white xl:hidden",
                 onClick: r[2] || (r[2] = i => t.value = !0)
-            }, [me(ke(_E), {
+            }, [me(Oe(wE), {
                 class: "h-5 w-5",
                 "aria-hidden": "true"
-            })])]), W("div", U_, [W("div", z_, [W("main", W_, [me(ke(jh), null, {
+            })])]), W("div", z_, [W("div", W_, [W("main", H_, [me(Oe(jh), null, {
                 default: et(({
                     Component: i
-                }) => [me(Ob, null, {
-                    default: et(() => [(Oe(), Tt(ho(i)))]),
+                }) => [me(Tb, null, {
+                    default: et(() => [(Te(), Tt(ho(i)))]),
                     _: 2
                 }, 1024)]),
                 _: 1
-            })]), W("footer", H_, [W("div", G_, [W("p", K_, " © Copyright " + Fn(new Date().getFullYear()) + ". All rights reserved. ", 1), Y_])])])]), W("aside", J_, [me(_b)])]), (Oe(), Tt(Of, {
+            })]), W("footer", G_, [W("div", K_, [W("p", Y_, " © Copyright " + cn(new Date().getFullYear()) + ". All rights reserved. ", 1), J_])])])]), W("aside", X_, [me(wb)])]), (Te(), Tt(Of, {
                 to: "body"
-            }, [me(D_)]))], 64))
+            }, [me(N_)]))], 64))
         }
     };
 
 function Vh(e) {
     return new Mt(function(t, n) {
-        return new Ce(function(r) {
+        return new ke(function(r) {
             var i, o, s;
             try {
                 i = n(t).subscribe({
                     next: function(a) {
                         if (a.errors && (s = e({
                                 graphQLErrors: a.errors,
                                 response: a,
@@ -16553,130 +16557,130 @@
         return r.link = Vh(n), r
     }
     return t.prototype.request = function(n, r) {
         return this.link.request(n, r)
     }, t
 })(Mt);
 
-function Z_(e) {
+function e1(e) {
     return Fe(e) && "code" in e && "reason" in e
 }
 
-function e1(e) {
+function t1(e) {
     var t;
     return Fe(e) && ((t = e.target) === null || t === void 0 ? void 0 : t.readyState) === WebSocket.CLOSED
 }
-var t1 = function(e) {
+var n1 = function(e) {
     bt(t, e);
 
     function t(n) {
         var r = e.call(this) || this;
         return r.client = n, r
     }
     return t.prototype.request = function(n) {
         var r = this;
-        return new Ce(function(i) {
+        return new ke(function(i) {
             return r.client.subscribe(w(w({}, n), {
                 query: vi(n.query)
             }), {
                 next: i.next.bind(i),
                 complete: i.complete.bind(i),
                 error: function(o) {
                     if (o instanceof Error) return i.error(o);
-                    var s = Z_(o);
-                    return s || e1(o) ? i.error(new Error("Socket closed".concat(s ? " with event ".concat(o.code) : "").concat(s ? " ".concat(o.reason) : ""))) : i.error(new Dt({
+                    var s = e1(o);
+                    return s || t1(o) ? i.error(new Error("Socket closed".concat(s ? " with event ".concat(o.code) : "").concat(s ? " ".concat(o.reason) : ""))) : i.error(new Dt({
                         graphQLErrors: Array.isArray(o) ? o : [o]
                     }))
                 }
             })
         })
     }, t
 }(Mt);
 
 function ot(e) {
     return e === null ? "null" : Array.isArray(e) ? "array" : typeof e
 }
 
-function An(e) {
+function Rn(e) {
     return ot(e) === "object"
 }
 
-function n1(e) {
+function r1(e) {
     return Array.isArray(e) && e.length > 0 && e.every(t => "message" in t)
 }
 
 function Ec(e, t) {
     return e.length < 124 ? e : t
 }
-const r1 = "graphql-transport-ws";
+const i1 = "graphql-transport-ws";
 var ct;
 (function(e) {
     e[e.InternalServerError = 4500] = "InternalServerError", e[e.InternalClientError = 4005] = "InternalClientError", e[e.BadRequest = 4400] = "BadRequest", e[e.BadResponse = 4004] = "BadResponse", e[e.Unauthorized = 4401] = "Unauthorized", e[e.Forbidden = 4403] = "Forbidden", e[e.SubprotocolNotAcceptable = 4406] = "SubprotocolNotAcceptable", e[e.ConnectionInitialisationTimeout = 4408] = "ConnectionInitialisationTimeout", e[e.ConnectionAcknowledgementTimeout = 4504] = "ConnectionAcknowledgementTimeout", e[e.SubscriberAlreadyExists = 4409] = "SubscriberAlreadyExists", e[e.TooManyInitialisationRequests = 4429] = "TooManyInitialisationRequests"
 })(ct || (ct = {}));
 var $e;
 (function(e) {
     e.ConnectionInit = "connection_init", e.ConnectionAck = "connection_ack", e.Ping = "ping", e.Pong = "pong", e.Subscribe = "subscribe", e.Next = "next", e.Error = "error", e.Complete = "complete"
 })($e || ($e = {}));
 
 function $h(e) {
-    if (!An(e)) throw new Error(`Message is expected to be an object, but got ${ot(e)}`);
+    if (!Rn(e)) throw new Error(`Message is expected to be an object, but got ${ot(e)}`);
     if (!e.type) throw new Error("Message is missing the 'type' property");
     if (typeof e.type != "string") throw new Error(`Message is expects the 'type' property to be a string, but got ${ot(e.type)}`);
     switch (e.type) {
         case $e.ConnectionInit:
         case $e.ConnectionAck:
         case $e.Ping:
         case $e.Pong: {
-            if (e.payload != null && !An(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an object or nullish or missing, but got "${e.payload}"`);
+            if (e.payload != null && !Rn(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an object or nullish or missing, but got "${e.payload}"`);
             break
         }
         case $e.Subscribe: {
             if (typeof e.id != "string") throw new Error(`"${e.type}" message expects the 'id' property to be a string, but got ${ot(e.id)}`);
             if (!e.id) throw new Error(`"${e.type}" message requires a non-empty 'id' property`);
-            if (!An(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an object, but got ${ot(e.payload)}`);
+            if (!Rn(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an object, but got ${ot(e.payload)}`);
             if (typeof e.payload.query != "string") throw new Error(`"${e.type}" message payload expects the 'query' property to be a string, but got ${ot(e.payload.query)}`);
-            if (e.payload.variables != null && !An(e.payload.variables)) throw new Error(`"${e.type}" message payload expects the 'variables' property to be a an object or nullish or missing, but got ${ot(e.payload.variables)}`);
+            if (e.payload.variables != null && !Rn(e.payload.variables)) throw new Error(`"${e.type}" message payload expects the 'variables' property to be a an object or nullish or missing, but got ${ot(e.payload.variables)}`);
             if (e.payload.operationName != null && ot(e.payload.operationName) !== "string") throw new Error(`"${e.type}" message payload expects the 'operationName' property to be a string or nullish or missing, but got ${ot(e.payload.operationName)}`);
-            if (e.payload.extensions != null && !An(e.payload.extensions)) throw new Error(`"${e.type}" message payload expects the 'extensions' property to be a an object or nullish or missing, but got ${ot(e.payload.extensions)}`);
+            if (e.payload.extensions != null && !Rn(e.payload.extensions)) throw new Error(`"${e.type}" message payload expects the 'extensions' property to be a an object or nullish or missing, but got ${ot(e.payload.extensions)}`);
             break
         }
         case $e.Next: {
             if (typeof e.id != "string") throw new Error(`"${e.type}" message expects the 'id' property to be a string, but got ${ot(e.id)}`);
             if (!e.id) throw new Error(`"${e.type}" message requires a non-empty 'id' property`);
-            if (!An(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an object, but got ${ot(e.payload)}`);
+            if (!Rn(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an object, but got ${ot(e.payload)}`);
             break
         }
         case $e.Error: {
             if (typeof e.id != "string") throw new Error(`"${e.type}" message expects the 'id' property to be a string, but got ${ot(e.id)}`);
             if (!e.id) throw new Error(`"${e.type}" message requires a non-empty 'id' property`);
-            if (!n1(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an array of GraphQL errors, but got ${JSON.stringify(e.payload)}`);
+            if (!r1(e.payload)) throw new Error(`"${e.type}" message expects the 'payload' property to be an array of GraphQL errors, but got ${JSON.stringify(e.payload)}`);
             break
         }
         case $e.Complete: {
             if (typeof e.id != "string") throw new Error(`"${e.type}" message expects the 'id' property to be a string, but got ${ot(e.id)}`);
             if (!e.id) throw new Error(`"${e.type}" message requires a non-empty 'id' property`);
             break
         }
         default:
             throw new Error(`Invalid message 'type' property "${e.type}"`)
     }
     return e
 }
 
-function i1(e, t) {
+function o1(e, t) {
     return $h(typeof e == "string" ? JSON.parse(e, t) : e)
 }
 
 function Nr(e, t) {
     return $h(e), JSON.stringify(e, t)
 }
 var lr = function(e) {
         return this instanceof lr ? (this.v = e, this) : new lr(e)
     },
-    o1 = function(e, t, n) {
+    s1 = function(e, t, n) {
         if (!Symbol.asyncIterator) throw new TypeError("Symbol.asyncIterator is not defined.");
         var r = n.apply(e, t || []),
             i, o = [];
         return i = {}, s("next"), s("throw"), s("return"), i[Symbol.asyncIterator] = function() {
             return this
         }, i;
 
@@ -16709,15 +16713,15 @@
         }
 
         function d(f, h) {
             f(h), o.shift(), o.length && a(o[0][0], o[0][1])
         }
     };
 
-function s1(e) {
+function a1(e) {
     const {
         url: t,
         connectionParams: n,
         lazy: r = !0,
         onNonLazyError: i = console.error,
         lazyCloseTimeout: o = 0,
         keepAlive: s = 0,
@@ -16740,15 +16744,15 @@
             })
         },
         jsonMessageReplacer: b,
         jsonMessageReviver: y
     } = e;
     let _;
     if (p) {
-        if (!l1(p)) throw new Error("Invalid WebSocket implementation provided");
+        if (!u1(p)) throw new Error("Invalid WebSocket implementation provided");
         _ = p
     } else typeof WebSocket < "u" ? _ = WebSocket : typeof global < "u" ? _ = global.WebSocket || global.MozWebSocket : typeof window < "u" && (_ = window.WebSocket || window.MozWebSocket);
     if (!_) throw new Error("WebSocket implementation missing; on Node you can `import WebSocket from 'ws';` and pass `webSocketImpl: WebSocket` to `createClient`");
     const E = _,
         S = (() => {
             const H = (() => {
                     const $ = {};
@@ -16806,15 +16810,15 @@
                 if (await c(M), !F) return O = void 0, we({
                     code: 1e3,
                     reason: "All Subscriptions Gone"
                 });
                 M++
             }
             S.emit("connecting", R);
-            const G = new E(typeof t == "function" ? await t() : t, r1);
+            const G = new E(typeof t == "function" ? await t() : t, i1);
             let re, ve;
 
             function Ee() {
                 isFinite(s) && s > 0 && (clearTimeout(ve), ve = setTimeout(() => {
                     G.readyState === E.OPEN && (G.send(Nr({
                         type: $e.Ping
                     })), S.emit("ping", !1, void 0))
@@ -16840,15 +16844,15 @@
                 }
             };
             let qe = !1;
             G.onmessage = ({
                 data: fe
             }) => {
                 try {
-                    const k = i1(fe, y);
+                    const k = o1(fe, y);
                     if (S.emit("message", k), k.type === "ping" || k.type === "pong") {
                         S.emit(k.type, !0, k.payload), k.type === "pong" ? Ee() : a || (G.send(Nr(k.payload ? {
                             type: $e.Pong,
                             payload: k.payload
                         } : {
                             type: $e.Pong
                         })), S.emit("pong", !1, k.payload));
@@ -16872,15 +16876,15 @@
                     H.readyState === E.OPEN && ie()
                 }, o) : ie()
             }
         }), L])]
     }
 
     function Y(H) {
-        if (ds(H) && (a1(H.code) || [ct.InternalServerError, ct.InternalClientError, ct.BadRequest, ct.BadResponse, ct.Unauthorized, ct.SubprotocolNotAcceptable, ct.SubscriberAlreadyExists, ct.TooManyInitialisationRequests].includes(H.code))) throw H;
+        if (ds(H) && (l1(H.code) || [ct.InternalServerError, ct.InternalClientError, ct.BadRequest, ct.BadResponse, ct.Unauthorized, ct.SubprotocolNotAcceptable, ct.SubscriberAlreadyExists, ct.TooManyInitialisationRequests].includes(H.code))) throw H;
         if (ne) return !1;
         if (ds(H) && H.code === 1e3) return F > 0;
         if (!u || M >= u || !d(H) || f != null && f(H)) throw H;
         return R = !0
     }
     r || (async () => {
         for (F++;;) try {
@@ -16962,15 +16966,15 @@
                         $.done = !0, $.error = we, $.resolve()
                     },
                     complete() {
                         $.done = !0, $.resolve()
                     }
                 }),
                 ie = function() {
-                    return o1(this, arguments, function*() {
+                    return s1(this, arguments, function*() {
                         for (;;) {
                             for (L.length || (yield lr(new Promise(re => $.resolve = re))); L.length;) yield yield lr(L.shift());
                             if ($.error) throw $.error;
                             if ($.done) return yield lr(void 0)
                         }
                     })
                 }();
@@ -16996,165 +17000,165 @@
 class _c extends Error {
     constructor() {
         super(...arguments), this.name = "TerminatedCloseEvent", this.message = "4499: Terminated", this.code = 4499, this.reason = "Terminated", this.wasClean = !1
     }
 }
 
 function ds(e) {
-    return An(e) && "code" in e && "reason" in e
+    return Rn(e) && "code" in e && "reason" in e
 }
 
-function a1(e) {
+function l1(e) {
     return [1e3, 1001, 1006, 1005, 1012, 1013, 1014].includes(e) ? !1 : e >= 1e3 && e <= 1999
 }
 
-function l1(e) {
+function u1(e) {
     return typeof e == "function" && "constructor" in e && "CLOSED" in e && "CLOSING" in e && "CONNECTING" in e && "OPEN" in e
 }
-const u1 = {
+const c1 = {
         class: "mx-auto flex h-12 w-12 items-center justify-center rounded-full bg-rose-600/10"
     },
-    c1 = W("div", {
+    f1 = W("div", {
         class: "mt-3 text-center sm:mt-5"
     }, [W("h2", null, "Error"), W("div", {
         class: "mt-2"
     }, [W("p", null, " An error has occured while querying the server. Make sur odooghost web server is running ! ")])], -1),
-    f1 = {
+    d1 = {
         class: "mt-5 sm:mt-6 flex justify-center"
     },
-    d1 = {
+    h1 = {
         __name: "VNetworkError",
         setup(e) {
             const t = ul(),
                 n = () => {
                     t.closeModal(), location.reload(!0)
                 };
-            return (r, i) => (Oe(), Tt(ke(xh), {
+            return (r, i) => (Te(), Tt(Oe(xh), {
                 class: "relative transform overflow-hidden rounded-lg bg-neutral-950 px-4 pb-4 pt-5 text-left shadow-xl transition-all sm:my-8 sm:w-full sm:max-w-sm sm:p-6"
             }, {
-                default: et(() => [W("div", null, [W("div", u1, [me(ke(OE), {
+                default: et(() => [W("div", null, [W("div", c1, [me(Oe(TE), {
                     class: "h-6 w-6 text-rose-500",
                     "aria-hidden": "true"
-                })]), c1]), W("div", f1, [W("button", {
+                })]), f1]), W("div", d1, [W("button", {
                     type: "button",
                     class: "button-primary",
                     onClick: i[0] || (i[0] = o => n())
                 }, "Refresh page")])]),
                 _: 1
             }))
         }
     },
-    h1 = new t1(s1({
+    p1 = new n1(a1({
         url: "ws://localhost:8000/graphql"
     })),
-    p1 = Vh(({
+    v1 = Vh(({
         networkError: e
     }) => {
         const t = ul();
         e && (e.statusCode >= 500 || e.statusCode == null) && t.openModal({
             title: "Voulez-vous continuer ?",
             message: "Vous êtes sur le point de fermer un ticket. Celui-ci ne pourra pas être réouvert.",
             callback: null,
-            component: uo(d1)
+            component: uo(h1)
         })
     }),
-    v1 = new Rd({
+    m1 = new Rd({
         uri: "/graphql"
     }),
-    m1 = Tg(({
+    y1 = Tg(({
         query: e
     }) => {
         const t = _r(e);
         return t.kind === "OperationDefinition" && t.operation === "subscription"
-    }, h1, v1),
-    y1 = new Gd({
-        link: Mt.from([p1, m1]),
+    }, p1, m1),
+    g1 = new Gd({
+        link: Mt.from([v1, y1]),
         cache: new Ud
     }),
-    g1 = "modulepreload",
-    b1 = function(e) {
+    b1 = "modulepreload",
+    E1 = function(e) {
         return "/" + e
     },
     wc = {},
     Rt = function(t, n, r) {
         let i = Promise.resolve();
         if (n && n.length > 0) {
             const o = document.getElementsByTagName("link"),
                 s = document.querySelector("meta[property=csp-nonce]"),
                 a = (s == null ? void 0 : s.nonce) || (s == null ? void 0 : s.getAttribute("nonce"));
             i = Promise.all(n.map(l => {
-                if (l = b1(l), l in wc) return;
+                if (l = E1(l), l in wc) return;
                 wc[l] = !0;
                 const u = l.endsWith(".css"),
                     c = u ? '[rel="stylesheet"]' : "";
                 if (!!r)
                     for (let h = o.length - 1; h >= 0; h--) {
                         const p = o[h];
                         if (p.href === l && (!u || p.rel === "stylesheet")) return
                     } else if (document.querySelector(`link[href="${l}"]${c}`)) return;
                 const f = document.createElement("link");
-                if (f.rel = u ? "stylesheet" : g1, u || (f.as = "script", f.crossOrigin = ""), f.href = l, a && f.setAttribute("nonce", a), document.head.appendChild(f), u) return new Promise((h, p) => {
+                if (f.rel = u ? "stylesheet" : b1, u || (f.as = "script", f.crossOrigin = ""), f.href = l, a && f.setAttribute("nonce", a), document.head.appendChild(f), u) return new Promise((h, p) => {
                     f.addEventListener("load", h), f.addEventListener("error", () => p(new Error(`Unable to preload CSS for ${l}`)))
                 })
             }))
         }
         return i.then(() => t()).catch(o => {
             const s = new Event("vite:preloadError", {
                 cancelable: !0
             });
             if (s.payload = o, window.dispatchEvent(s), !s.defaultPrevented) throw o
         })
     },
-    E1 = C_({
-        history: i_("/"),
+    _1 = k_({
+        history: o_("/"),
         routes: [{
             path: "/",
             name: "dashboard",
-            component: () => Rt(() => import("./DashboardView-QC2AjQPk.js"), __vite__mapDeps([0, 1, 2, 3, 4, 5]))
+            component: () => Rt(() => import("./DashboardView-9fL2PusH.js"), __vite__mapDeps([0, 1, 2, 3, 4, 5]))
         }, {
             path: "/stacks",
             name: "stacks",
-            component: () => Rt(() => import("./StackView-DOsjJPZv.js"), __vite__mapDeps([6, 7, 2, 3, 4, 8]))
+            component: () => Rt(() => import("./StackView-Ce0Va4Vr.js"), __vite__mapDeps([6, 7, 2, 3, 4, 8]))
         }, {
             path: "/stack/:stackId",
             name: "stack",
-            component: () => Rt(() => import("./StackItemView-ieiARAXz.js"), __vite__mapDeps([9, 7, 3, 4, 8])),
+            component: () => Rt(() => import("./StackItemView-NraLa75A.js"), __vite__mapDeps([9, 7, 3, 4, 8])),
             children: [{
                 path: "",
                 name: "stackIndex",
-                component: () => Rt(() => import("./StackItemIndexView-BOSojVnH.js"), __vite__mapDeps([10, 1, 5]))
+                component: () => Rt(() => import("./StackItemIndexView-BMo8NmFy.js"), __vite__mapDeps([10, 1, 5]))
             }, {
                 path: "services",
                 name: "stackServices",
-                component: () => Rt(() => import("./StackItemServicesView-XPZCOPql.js"), [])
+                component: () => Rt(() => import("./StackItemServicesView--A44eQAS.js"), [])
             }, {
                 path: "containers",
                 name: "stackContainers",
-                component: () => Rt(() => import("./StackItemContainersView-DI931aio.js"), [])
+                component: () => Rt(() => import("./StackItemContainersView-DtnjBFd6.js"), [])
             }, {
                 path: "logs",
                 name: "stackLogs",
-                component: () => Rt(() => import("./StackItemLogsView-Bgz593Fu.js"), [])
+                component: () => Rt(() => import("./StackItemLogsView-CToeth34.js"), [])
             }]
         }, {
             path: "/containers",
             name: "containers",
-            component: () => Rt(() => import("./ContainersView-vBrHvCnL.js"), __vite__mapDeps([11, 7, 2, 3, 4, 1]))
+            component: () => Rt(() => import("./ContainersView-DEOoJDOr.js"), __vite__mapDeps([11, 7, 2, 3, 4, 1]))
         }, {
             path: "/usage",
             name: "usage",
-            component: () => Rt(() => import("./UsageView-CwbrZuiW.js"), [])
+            component: () => Rt(() => import("./UsageView-DgJ9FyX7.js"), [])
         }, {
             path: "/settings",
             name: "settings",
-            component: () => Rt(() => import("./SettingsView-BS_D169E.js"), [])
+            component: () => Rt(() => import("./SettingsView-CwpsckXe.js"), [])
         }]
     });
 fm({
     setup() {
-        rt(Jd, y1)
+        rt(Jd, g1)
     },
-    render: () => ze(X_)
-}).use(U0()).use(E1).mount("#app");
+    render: () => ze(Z_)
+}).use(U0()).use(_1).mount("#app");
 export {
-    pa as A, nb as B, Ke as F, jh as R, Ob as V, rb as _, me as a, ke as b, Ye as c, W as d, df as e, Tt as f, P0 as g, T1 as h, w1 as i, tv as j, Af as k, C1 as l, Bn as m, Vt as n, Oe as o, Le as p, ue as q, _1 as r, rt as s, Fn as t, x1 as u, ho as v, et as w, Ie as x, wb as y, Op as z
+    pa as A, nb as B, Ke as F, jh as R, Tb as V, rb as _, me as a, Oe as b, Ye as c, W as d, df as e, Tt as f, P0 as g, C1 as h, S1 as i, tv as j, Af as k, k1 as l, Bn as m, Vt as n, Te as o, Le as p, ue as q, w1 as r, rt as s, cn as t, O1 as u, ho as v, et as w, Ie as x, Sb as y, Op as z
 };
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/assets/stack-C5Mp2ADT.js` & `odooghost-0.8.1/odooghost/web/dist/assets/stack-DYu-LgCo.js`

 * *Files 22% similar despite different names*

#### js-beautify {}

```diff
@@ -1,10 +1,10 @@
 import {
     g as e
-} from "./index-s10VwhOf.js";
+} from "./index-DDQ87HFV.js";
 const t = e`
   query getStack($name: String!) {
     stack(name: $name) {
       id
       name
       state
       odooVersion
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/favicon-16x16.png` & `odooghost-0.8.1/odooghost/web/dist/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/favicon-32x32.png` & `odooghost-0.8.1/odooghost/web/dist/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/favicon.ico` & `odooghost-0.8.1/odooghost/web/dist/favicon.ico`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/odooghost/web/dist/index.html` & `odooghost-0.8.1/odooghost/web/dist/index.html`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,14 @@
     <link rel="icon" href="/favicon.ico" />
     <link rel="icon" type="image/png" sizes="32x32" href="/favicon-32x32.png" />
     <link rel="icon" type="image/png" sizes="16x16" href="/favicon-16x16.png" />
     <link rel="apple-touch-icon" sizes="180x180" href="/apple-touch-icon.png" />
     <link rel="manifest" href="/site.webmanifest" />
     <meta name="viewport" content="width=device-width, initial-scale=1.0" />
     <title>OdooGhost</title>
-    <script type="module" crossorigin src="/assets/index-s10VwhOf.js"></script>
+    <script type="module" crossorigin src="/assets/index-DDQ87HFV.js"></script>
     <link rel="stylesheet" crossorigin href="/assets/index-BCu_nn1R.css">
   </head>
   <body class="h-full">
     <div id="app" class="h-full"></div>
   </body>
 </html>
```

### Comparing `odooghost-0.8.0/odooghost/web/dist/logo.svg` & `odooghost-0.8.1/odooghost/web/dist/logo.svg`

 * *Files identical despite different names*

### Comparing `odooghost-0.8.0/pyproject.toml` & `odooghost-0.8.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "odooghost"
-version = "0.8.0"
+version = "0.8.1"
 description = "Odoo developpement made easy"
 authors = ["Remy Zulauff <remy.zulauff@gmail.com>"]
 readme = "README.md"
 homepage = "https://remyz17.github.io/odooghost/"
 repository = "https://github.com/remyz17/odooghost"
 license = "MIT"
 include = ["odooghost/web/dist/**/*"]
```

### Comparing `odooghost-0.8.0/PKG-INFO` & `odooghost-0.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odooghost
-Version: 0.8.0
+Version: 0.8.1
 Summary: Odoo developpement made easy
 Home-page: https://remyz17.github.io/odooghost/
 License: MIT
 Author: Remy Zulauff
 Author-email: remy.zulauff@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

