# Comparing `tmp/matlab-proxy-0.9.0.tar.gz` & `tmp/matlab-proxy-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matlab-proxy-0.9.0.tar", last modified: Wed Oct 18 09:00:22 2023, max compression
+gzip compressed data, was "matlab-proxy-0.9.1.tar", last modified: Tue Oct 31 12:57:45 2023, max compression
```

## Comparing `matlab-proxy-0.9.0.tar` & `matlab-proxy-0.9.1.tar`

### file list

```diff
@@ -1,166 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8399 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.585584 matlab-proxy-0.9.0/gui/
--rw-r--r--   0 runner    (1001) docker     (127)      310 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/README.md
--rw-r--r--   0 runner    (1001) docker     (127)  1289839 2023-10-18 09:00:04.000000 matlab-proxy-0.9.0/gui/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.585584 matlab-proxy-0.9.0/gui/public/
--rw-r--r--   0 runner    (1001) docker     (127)   130876 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.585584 matlab-proxy-0.9.0/gui/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.585584 matlab-proxy-0.9.0/gui/src/actionCreators/
--rw-r--r--   0 runner    (1001) docker     (127)    12525 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/actionCreators/actionCreators.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     9179 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/actionCreators/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.585584 matlab-proxy-0.9.0/gui/src/actions/
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/actions/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.581584 matlab-proxy-0.9.0/gui/src/components/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.585584 matlab-proxy-0.9.0/gui/src/components/App/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.581584 matlab-proxy-0.9.0/gui/src/components/App/3p/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.585584 matlab-proxy-0.9.0/gui/src/components/App/3p/css/
--rw-r--r--   0 runner    (1001) docker     (127)   121200 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/css/bootstrap.min.css
--rw-r--r--   0 runner    (1001) docker     (127)   153678 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/css/site7.min.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.589584 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/
--rw-r--r--   0 runner    (1001) docker     (127)    20127 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
--rw-r--r--   0 runner    (1001) docker     (127)   108738 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
--rw-r--r--   0 runner    (1001) docker     (127)    45404 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    23424 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
--rw-r--r--   0 runner    (1001) docker     (127)    18028 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    16377 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-eps.svg
--rw-r--r--   0 runner    (1001) docker     (127)     6448 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-eps.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     6528 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-eps.woff
--rw-r--r--   0 runner    (1001) docker     (127)   289658 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
--rw-r--r--   0 runner    (1001) docker     (127)    70212 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    70288 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
--rw-r--r--   0 runner    (1001) docker     (127)   138707 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks.svg
--rw-r--r--   0 runner    (1001) docker     (127)    38656 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    38732 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks.woff
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.581584 matlab-proxy-0.9.0/gui/src/components/App/3p/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.589584 matlab-proxy-0.9.0/gui/src/components/App/3p/images/bug_reports/
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/images/bug_reports/workaround.gif
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.581584 matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.589584 matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4774 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
--rw-r--r--   0 runner    (1001) docker     (127)    11438 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
--rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/App.css
--rw-r--r--   0 runner    (1001) docker     (127)     8694 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/App.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)   220290 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/MATLAB-env-blur.png
--rw-r--r--   0 runner    (1001) docker     (127)     7327 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/App/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.589584 matlab-proxy-0.9.0/gui/src/components/Confirmation/
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Confirmation/Confirmation.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Confirmation/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/Controls/
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/Controls.css
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/Controls.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/feedback.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/help.svg
--rw-r--r--   0 runner    (1001) docker     (127)     8259 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/restart.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/sign-out.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/start.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/stop.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1875 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Controls/terminate.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/EntitlementSelector/
--rw-r--r--   0 runner    (1001) docker     (127)     4032 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/EntitlementSelector/EntitlementSelector.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/EntitlementSelector/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/Error/
--rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Error/Error.css
--rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Error/Error.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Error/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/Help/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Help/Help.css
--rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Help/Help.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Help/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/Information/
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Information/Information.css
--rw-r--r--   0 runner    (1001) docker     (127)     5836 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Information/Information.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     9249 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Information/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/ExistingLicense.css
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/ExistingLicense.js
--rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/LicensingGatherer.css
--rw-r--r--   0 runner    (1001) docker     (127)     4486 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/MHLM.js
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/NLM.js
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/MatlabJsd/
--rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/MatlabJsd/MatlabJsd.css
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/MatlabJsd/MatlabJsd.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)      474 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/MatlabJsd/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/Overlay/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Overlay/Overlay.css
--rw-r--r--   0 runner    (1001) docker     (127)      757 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Overlay/Overlay.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)      532 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/Overlay/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/
--rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/OverlayTrigger.css
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/arrow.svg
--rw-r--r--   0 runner    (1001) docker     (127)      405 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/gripper.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/index.js
--rw-r--r--   0 runner    (1001) docker     (127)     5017 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/trigger-error.svg
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/trigger-ok.svg
--rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/index.js
--rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/jest.config.json
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/reducers/
--rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/reducers/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    13874 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/reducers/reducers.spec.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/selectors/
--rw-r--r--   0 runner    (1001) docker     (127)     6986 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/selectors/index.js
--rw-r--r--   0 runner    (1001) docker     (127)    14121 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/selectors/selectors.spec.js
--rw-r--r--   0 runner    (1001) docker     (127)     5956 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/serviceWorker.js
--rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/setupTests.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.581584 matlab-proxy-0.9.0/gui/src/test/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.593584 matlab-proxy-0.9.0/gui/src/test/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      738 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/gui/src/test/utils/react-test.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/matlab_proxy/
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28186 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/app.py
--rw-r--r--   0 runner    (1001) docker     (127)    52053 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/app_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/default_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14310 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/devel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/matlab_proxy/icons/
--rw-r--r--   0 runner    (1001) docker     (127)    13366 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/icons/matlab.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/matlab_proxy/matlab/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1535 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/matlab/startup.m
--rw-r--r--   0 runner    (1001) docker     (127)    18556 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/matlab_proxy/util/
--rw-r--r--   0 runner    (1001) docker     (127)     7714 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/event_loop.py
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/list_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)    11048 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mw.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/matlab_proxy/util/mwi/
--rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7154 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/custom_http_headers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/matlab_proxy/util/mwi/embedded_connector/
--rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/embedded_connector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/embedded_connector/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/embedded_connector/request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4961 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/environment_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4628 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     9846 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/token_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    11745 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/mwi/validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/system.py
--rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/matlab_proxy/util/windows.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/matlab_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10724 2023-10-18 08:59:39.000000 matlab-proxy-0.9.0/matlab_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5124 2023-10-18 08:59:39.000000 matlab-proxy-0.9.0/matlab_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 08:59:39.000000 matlab-proxy-0.9.0/matlab_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-18 08:59:39.000000 matlab-proxy-0.9.0/matlab_proxy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-18 08:59:39.000000 matlab-proxy-0.9.0/matlab_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-18 08:59:39.000000 matlab-proxy-0.9.0/matlab_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-18 08:59:39.000000 matlab-proxy-0.9.0/matlab_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-18 09:00:22.597584 matlab-proxy-0.9.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-10-18 08:59:03.000000 matlab-proxy-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.986539 matlab-proxy-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2023-10-31 12:57:45.986539 matlab-proxy-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8359 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.962539 matlab-proxy-0.9.1/gui/
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2891 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)  1289839 2023-10-31 12:57:21.000000 matlab-proxy-0.9.1/gui/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.962539 matlab-proxy-0.9.1/gui/public/
+-rw-r--r--   0 runner    (1001) docker     (127)   130876 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      632 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.966539 matlab-proxy-0.9.1/gui/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.966539 matlab-proxy-0.9.1/gui/src/actionCreators/
+-rw-r--r--   0 runner    (1001) docker     (127)    12525 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/actionCreators/actionCreators.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9179 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/actionCreators/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.966539 matlab-proxy-0.9.1/gui/src/actions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/actions/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.958539 matlab-proxy-0.9.1/gui/src/components/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.966539 matlab-proxy-0.9.1/gui/src/components/App/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.958539 matlab-proxy-0.9.1/gui/src/components/App/3p/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.966539 matlab-proxy-0.9.1/gui/src/components/App/3p/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   121200 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/css/bootstrap.min.css
+-rw-r--r--   0 runner    (1001) docker     (127)   153678 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/css/site7.min.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.970538 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/
+-rw-r--r--   0 runner    (1001) docker     (127)    20127 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   108738 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    45404 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    23424 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    18028 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    16377 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-eps.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     6448 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-eps.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     6528 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-eps.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   289658 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-pictograms.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    70212 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    70288 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-pictograms.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   138707 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    38656 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    38732 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks.woff
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.958539 matlab-proxy-0.9.1/gui/src/components/App/3p/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.970538 matlab-proxy-0.9.1/gui/src/components/App/3p/images/bug_reports/
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/images/bug_reports/workaround.gif
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.958539 matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.974539 matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4774 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1392 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    11438 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-sprite.png
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/App.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8694 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/App.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)   220290 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/MATLAB-env-blur.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7327 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/App/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.974539 matlab-proxy-0.9.1/gui/src/components/Confirmation/
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Confirmation/Confirmation.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Confirmation/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.974539 matlab-proxy-0.9.1/gui/src/components/Controls/
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/Controls.css
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/Controls.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2135 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/feedback.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1467 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/help.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     8246 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/restart.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1077 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/sign-out.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/start.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/stop.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1875 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Controls/terminate.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.974539 matlab-proxy-0.9.1/gui/src/components/EntitlementSelector/
+-rw-r--r--   0 runner    (1001) docker     (127)     4032 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/EntitlementSelector/EntitlementSelector.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/EntitlementSelector/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.974539 matlab-proxy-0.9.1/gui/src/components/Error/
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Error/Error.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1449 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Error/Error.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Error/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.974539 matlab-proxy-0.9.1/gui/src/components/Help/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Help/Help.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2888 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Help/Help.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3161 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Help/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.978539 matlab-proxy-0.9.1/gui/src/components/Information/
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Information/Information.css
+-rw-r--r--   0 runner    (1001) docker     (127)     5836 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Information/Information.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     9249 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Information/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.978539 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/ExistingLicense.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/ExistingLicense.js
+-rw-r--r--   0 runner    (1001) docker     (127)     4730 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/LicensingGatherer.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4486 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/MHLM.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/NLM.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5114 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.978539 matlab-proxy-0.9.1/gui/src/components/MatlabJsd/
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/MatlabJsd/MatlabJsd.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/MatlabJsd/MatlabJsd.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/MatlabJsd/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.978539 matlab-proxy-0.9.1/gui/src/components/Overlay/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Overlay/Overlay.css
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Overlay/Overlay.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/Overlay/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.978539 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/
+-rw-r--r--   0 runner    (1001) docker     (127)     2204 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/OverlayTrigger.css
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2519 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/arrow.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/gripper.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4759 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5017 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/trigger-error.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/trigger-ok.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/jest.config.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.978539 matlab-proxy-0.9.1/gui/src/reducers/
+-rw-r--r--   0 runner    (1001) docker     (127)     7614 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/reducers/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    13874 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/reducers/reducers.spec.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.982539 matlab-proxy-0.9.1/gui/src/selectors/
+-rw-r--r--   0 runner    (1001) docker     (127)     6986 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/selectors/index.js
+-rw-r--r--   0 runner    (1001) docker     (127)    14121 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/selectors/selectors.spec.js
+-rw-r--r--   0 runner    (1001) docker     (127)     5956 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/serviceWorker.js
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/setupTests.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.958539 matlab-proxy-0.9.1/gui/src/test/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.982539 matlab-proxy-0.9.1/gui/src/test/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      738 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/gui/src/test/utils/react-test.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.982539 matlab-proxy-0.9.1/matlab_proxy/
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28548 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52053 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/app_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/default_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14310 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/devel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.982539 matlab-proxy-0.9.1/matlab_proxy/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)    13366 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/icons/matlab.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.982539 matlab-proxy-0.9.1/matlab_proxy/matlab/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1535 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/matlab/startup.m
+-rw-r--r--   0 runner    (1001) docker     (127)    18556 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.982539 matlab-proxy-0.9.1/matlab_proxy/util/
+-rw-r--r--   0 runner    (1001) docker     (127)     7714 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/event_loop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/list_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11048 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mw.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.986539 matlab-proxy-0.9.1/matlab_proxy/util/mwi/
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7154 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/custom_http_headers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.986539 matlab-proxy-0.9.1/matlab_proxy/util/mwi/embedded_connector/
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/embedded_connector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/embedded_connector/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/embedded_connector/request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4961 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/environment_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4628 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3049 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9846 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/token_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11745 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/mwi/validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1692 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/system.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3440 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/matlab_proxy/util/windows.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-31 12:57:45.982539 matlab-proxy-0.9.1/matlab_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10684 2023-10-31 12:56:52.000000 matlab-proxy-0.9.1/matlab_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5124 2023-10-31 12:56:52.000000 matlab-proxy-0.9.1/matlab_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 12:56:52.000000 matlab-proxy-0.9.1/matlab_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2023-10-31 12:56:52.000000 matlab-proxy-0.9.1/matlab_proxy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-31 12:56:52.000000 matlab-proxy-0.9.1/matlab_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2023-10-31 12:56:52.000000 matlab-proxy-0.9.1/matlab_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2023-10-31 12:56:52.000000 matlab-proxy-0.9.1/matlab_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2023-10-31 12:57:45.986539 matlab-proxy-0.9.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3750 2023-10-31 12:56:09.000000 matlab-proxy-0.9.1/setup.py
```

### Comparing `matlab-proxy-0.9.0/LICENSE.md` & `matlab-proxy-0.9.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/PKG-INFO` & `matlab-proxy-0.9.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
@@ -126,20 +126,20 @@
           <img width="800" src="https://github.com/mathworks/matlab-proxy/raw/main/img/status_panel.png">
         </p>
         
         The following options are available in the status panel (some options are only available in a specific context):
         
         | Option |  Description |
         | ---- | ---- |
-        | Start MATLAB Session | Start your MATLAB session. Available if MATLAB is stopped.|
-        | Restart MATLAB Session | Restart your MATLAB session. Available if MATLAB is running or starting.|
-        | Stop MATLAB Session | Stop your MATLAB session. Use this option if you want to free up RAM and CPU resources. Available if MATLAB is running or starting.|
-        | Sign Out | Sign out of MATLAB. Use this to stop MATLAB and sign in with an alternative account. Available if using online licensing.|
+        | Start MATLAB | Start your MATLAB session. Available if MATLAB is stopped.|
+        | Restart MATLAB | Restart your MATLAB session. Available if MATLAB is running or starting.|
+        | Stop MATLAB | Stop your MATLAB session. Use this option if you want to free up RAM and CPU resources. Available if MATLAB is running or starting.|
+        | Sign Out | Sign out of MATLAB session. Use this to stop MATLAB and sign in with an alternative account. Available if using online licensing.|
         | Unset License Server Address | Unset network license manager server address. Use this to stop MATLAB and enter new licensing information. Available if using network license manager.|
-        | Feedback | Send feedback about the MATLAB Proxy. This action opens your default email application.|
+        | Feedback | Provide feedback. Opens a new tab to create an issue on GitHub.|
         | Help | Open a help pop-up for a detailed description of the options.|
         
         ## Examples
         * For installing/usage in a Docker container, see this [Dockerfile](./examples/Dockerfile) and its [README](./examples/README.md).
         * For upgrading **matlab-proxy** in an existing Docker image, see this [Dockerfile.upgrade.matlab-proxy](./examples/Dockerfile.upgrade.matlab-proxy) and its [README](./examples/README.md#upgrading-matlab-proxy-package-in-a-docker-image).*
         * For usage in a Jupyter environment, see [jupyter-matlab-proxy](https://github.com/mathworks/jupyter-matlab-proxy).
```

### Comparing `matlab-proxy-0.9.0/README.md` & `matlab-proxy-0.9.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -118,20 +118,20 @@
   <img width="800" src="https://github.com/mathworks/matlab-proxy/raw/main/img/status_panel.png">
 </p>
 
 The following options are available in the status panel (some options are only available in a specific context):
 
 | Option |  Description |
 | ---- | ---- |
-| Start MATLAB Session | Start your MATLAB session. Available if MATLAB is stopped.|
-| Restart MATLAB Session | Restart your MATLAB session. Available if MATLAB is running or starting.|
-| Stop MATLAB Session | Stop your MATLAB session. Use this option if you want to free up RAM and CPU resources. Available if MATLAB is running or starting.|
-| Sign Out | Sign out of MATLAB. Use this to stop MATLAB and sign in with an alternative account. Available if using online licensing.|
+| Start MATLAB | Start your MATLAB session. Available if MATLAB is stopped.|
+| Restart MATLAB | Restart your MATLAB session. Available if MATLAB is running or starting.|
+| Stop MATLAB | Stop your MATLAB session. Use this option if you want to free up RAM and CPU resources. Available if MATLAB is running or starting.|
+| Sign Out | Sign out of MATLAB session. Use this to stop MATLAB and sign in with an alternative account. Available if using online licensing.|
 | Unset License Server Address | Unset network license manager server address. Use this to stop MATLAB and enter new licensing information. Available if using network license manager.|
-| Feedback | Send feedback about the MATLAB Proxy. This action opens your default email application.|
+| Feedback | Provide feedback. Opens a new tab to create an issue on GitHub.|
 | Help | Open a help pop-up for a detailed description of the options.|
 
 ## Examples
 * For installing/usage in a Docker container, see this [Dockerfile](./examples/Dockerfile) and its [README](./examples/README.md).
 * For upgrading **matlab-proxy** in an existing Docker image, see this [Dockerfile.upgrade.matlab-proxy](./examples/Dockerfile.upgrade.matlab-proxy) and its [README](./examples/README.md#upgrading-matlab-proxy-package-in-a-docker-image).*
 * For usage in a Jupyter environment, see [jupyter-matlab-proxy](https://github.com/mathworks/jupyter-matlab-proxy).
```

### Comparing `matlab-proxy-0.9.0/gui/README.md` & `matlab-proxy-0.9.1/gui/README.md`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/package-lock.json` & `matlab-proxy-0.9.1/gui/package-lock.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/package.json` & `matlab-proxy-0.9.1/gui/package.json`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/public/favicon.ico` & `matlab-proxy-0.9.1/gui/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/public/index.html` & `matlab-proxy-0.9.1/gui/public/index.html`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/actionCreators/actionCreators.spec.js` & `matlab-proxy-0.9.1/gui/src/actionCreators/actionCreators.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/actionCreators/index.js` & `matlab-proxy-0.9.1/gui/src/actionCreators/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/actions/index.js` & `matlab-proxy-0.9.1/gui/src/actions/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/css/bootstrap.min.css` & `matlab-proxy-0.9.1/gui/src/components/App/3p/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/css/site7.min.css` & `matlab-proxy-0.9.1/gui/src/components/App/3p/css/site7.min.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.eot`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/glyphicons-halflings-regular.woff2`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-eps.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-eps.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-eps.ttf` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-eps.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-eps.woff` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-eps.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-pictograms.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-pictograms.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-pictograms.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks-pictograms.woff` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks-pictograms.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks.ttf` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks.ttf`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/fonts/mathworks.woff` & `matlab-proxy-0.9.1/gui/src/components/App/3p/fonts/mathworks.woff`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/images/bug_reports/workaround.gif` & `matlab-proxy-0.9.1/gui/src/components/App/3p/images/bug_reports/workaround.gif`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-account-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-account.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-contact-hover.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg` & `matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-header-contact.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/3p/images/responsive/global/ico-sprite.png` & `matlab-proxy-0.9.1/gui/src/components/App/3p/images/responsive/global/ico-sprite.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/App.css` & `matlab-proxy-0.9.1/gui/src/components/App/App.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/App.spec.js` & `matlab-proxy-0.9.1/gui/src/components/App/App.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/MATLAB-env-blur.png` & `matlab-proxy-0.9.1/gui/src/components/App/MATLAB-env-blur.png`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/App/index.js` & `matlab-proxy-0.9.1/gui/src/components/App/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Confirmation/Confirmation.spec.js` & `matlab-proxy-0.9.1/gui/src/components/Confirmation/Confirmation.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Confirmation/index.js` & `matlab-proxy-0.9.1/gui/src/components/Confirmation/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/Controls.css` & `matlab-proxy-0.9.1/gui/src/components/Controls/Controls.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/Controls.spec.js` & `matlab-proxy-0.9.1/gui/src/components/Controls/Controls.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/feedback.svg` & `matlab-proxy-0.9.1/gui/src/components/Controls/feedback.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/help.svg` & `matlab-proxy-0.9.1/gui/src/components/Controls/help.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/index.js` & `matlab-proxy-0.9.1/gui/src/components/Controls/index.js`

 * *Files 7% similar despite different names*

#### js-beautify {}

```diff
@@ -26,15 +26,15 @@
     fetchTerminateIntegration,
     fetchUnsetLicensing
 } from '../../actionCreators';
 import './Controls.css';
 
 // Suggested actions for certain errors
 const ERROR_TYPE_MAP = {
-    'sign-out': ['NetworkLicensingError', 'EntitlementError'],
+    'sign-out': ['NetworkLicensingError', 'EntitlementError', 'UIVisibleFatalError'],
     'restart': ['OnlineLicensingError']
 };
 
 function Controls({
     callback
 }) {
     const submitting = useSelector(selectSubmittingServerStatus);
@@ -179,15 +179,15 @@
         className = {
             getBtnClass('sign-out')
         }
         onClick = {
             () => callback(Confirmations.SIGN_OUT)
         }
         disabled = {
-            !canResetLicensing || (authEnabled && !isAuthenticated) || (licensingIsMhlm && !isEntitled)
+            !canResetLicensing || (authEnabled && !isAuthenticated)
         }
         data -
         for = "control-button-tooltip"
         data - tip = {
             licensingData.dataTip
         } >
         <
```

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/restart.svg` & `matlab-proxy-0.9.1/gui/src/components/Controls/restart.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/sign-out.svg` & `matlab-proxy-0.9.1/gui/src/components/Controls/sign-out.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/start.svg` & `matlab-proxy-0.9.1/gui/src/components/Controls/start.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/stop.svg` & `matlab-proxy-0.9.1/gui/src/components/Controls/stop.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Controls/terminate.svg` & `matlab-proxy-0.9.1/gui/src/components/Controls/terminate.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/EntitlementSelector/EntitlementSelector.spec.js` & `matlab-proxy-0.9.1/gui/src/components/EntitlementSelector/EntitlementSelector.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/EntitlementSelector/index.js` & `matlab-proxy-0.9.1/gui/src/components/EntitlementSelector/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Error/Error.css` & `matlab-proxy-0.9.1/gui/src/components/Error/Error.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Error/Error.spec.js` & `matlab-proxy-0.9.1/gui/src/components/Error/Error.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Error/index.js` & `matlab-proxy-0.9.1/gui/src/components/Error/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Help/Help.spec.js` & `matlab-proxy-0.9.1/gui/src/components/Help/Help.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Help/index.js` & `matlab-proxy-0.9.1/gui/src/components/Help/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Information/Information.css` & `matlab-proxy-0.9.1/gui/src/components/Information/Information.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Information/Information.spec.js` & `matlab-proxy-0.9.1/gui/src/components/Information/Information.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Information/index.js` & `matlab-proxy-0.9.1/gui/src/components/Information/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/ExistingLicense.js` & `matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/ExistingLicense.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js` & `matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/LicenseGatherer.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/MHLM.js` & `matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/MHLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/NLM.js` & `matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/NLM.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/LicensingGatherer/index.js` & `matlab-proxy-0.9.1/gui/src/components/LicensingGatherer/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/MatlabJsd/MatlabJsd.spec.js` & `matlab-proxy-0.9.1/gui/src/components/MatlabJsd/MatlabJsd.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Overlay/Overlay.css` & `matlab-proxy-0.9.1/gui/src/components/Overlay/Overlay.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Overlay/Overlay.spec.js` & `matlab-proxy-0.9.1/gui/src/components/Overlay/Overlay.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/Overlay/index.js` & `matlab-proxy-0.9.1/gui/src/components/Overlay/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/OverlayTrigger.css` & `matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/OverlayTrigger.css`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js` & `matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/OverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js` & `matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/ResizeOverlayTrigger.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/index.js` & `matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/trigger-error.svg` & `matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/trigger-error.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/components/OverlayTrigger/trigger-ok.svg` & `matlab-proxy-0.9.1/gui/src/components/OverlayTrigger/trigger-ok.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/index.js` & `matlab-proxy-0.9.1/gui/src/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/logo.svg` & `matlab-proxy-0.9.1/gui/src/logo.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/reducers/index.js` & `matlab-proxy-0.9.1/gui/src/reducers/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/reducers/reducers.spec.js` & `matlab-proxy-0.9.1/gui/src/reducers/reducers.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/selectors/index.js` & `matlab-proxy-0.9.1/gui/src/selectors/index.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/selectors/selectors.spec.js` & `matlab-proxy-0.9.1/gui/src/selectors/selectors.spec.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/serviceWorker.js` & `matlab-proxy-0.9.1/gui/src/serviceWorker.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/gui/src/test/utils/react-test.js` & `matlab-proxy-0.9.1/gui/src/test/utils/react-test.js`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/__init__.py` & `matlab-proxy-0.9.1/matlab_proxy/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/app.py` & `matlab-proxy-0.9.1/matlab_proxy/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -465,14 +465,22 @@
 
     state = req.app["state"]
     matlab_port = state.matlab_port
     matlab_protocol = req.app["settings"]["matlab_protocol"]
     mwapikey = req.app["settings"]["mwapikey"]
     matlab_base_url = f"{matlab_protocol}://127.0.0.1:{matlab_port}"
 
+    # If we are trying to send request to matlab while the matlab_port is still not assigned
+    # by embedded connector, return service not available and log a message
+    if not matlab_port:
+        logger.debug(
+            "MATLAB hasn't fully started, please retry after embedded connector has started"
+        )
+        raise web.HTTPServiceUnavailable()
+
     # WebSocket
     # According to according to RFC6455 (https://www.rfc-editor.org/rfc/rfc6455.html)
     # the values of 'connection' and 'upgrade'  keys of request header
     # should be ASCII case-insensitive matches.
     if (
         reqH.get(CONNECTION, "").lower() == UPGRADE
         and reqH.get(UPGRADE, "").lower() == "websocket"
```

### Comparing `matlab-proxy-0.9.0/matlab_proxy/app_state.py` & `matlab-proxy-0.9.1/matlab_proxy/app_state.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/default_configuration.py` & `matlab-proxy-0.9.1/matlab_proxy/default_configuration.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/devel.py` & `matlab-proxy-0.9.1/matlab_proxy/devel.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/icons/matlab.svg` & `matlab-proxy-0.9.1/matlab_proxy/icons/matlab.svg`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/matlab/startup.m` & `matlab-proxy-0.9.1/matlab_proxy/matlab/startup.m`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/settings.py` & `matlab-proxy-0.9.1/matlab_proxy/settings.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/__init__.py` & `matlab-proxy-0.9.1/matlab_proxy/util/__init__.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/event_loop.py` & `matlab-proxy-0.9.1/matlab_proxy/util/event_loop.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/list_servers.py` & `matlab-proxy-0.9.1/matlab_proxy/util/list_servers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mw.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mw.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/custom_http_headers.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/custom_http_headers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/embedded_connector/helpers.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/embedded_connector/helpers.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/embedded_connector/request.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/embedded_connector/request.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/environment_variables.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/environment_variables.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/exceptions.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/exceptions.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/logger.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/logger.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/token_auth.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/token_auth.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/mwi/validators.py` & `matlab-proxy-0.9.1/matlab_proxy/util/mwi/validators.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/system.py` & `matlab-proxy-0.9.1/matlab_proxy/util/system.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy/util/windows.py` & `matlab-proxy-0.9.1/matlab_proxy/util/windows.py`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/matlab_proxy.egg-info/PKG-INFO` & `matlab-proxy-0.9.1/matlab_proxy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matlab-proxy
-Version: 0.9.0
+Version: 0.9.1
 Summary: Python® package enables you to launch MATLAB® and access it from a web browser.
 Home-page: https://github.com/mathworks/matlab-proxy/
 Author: The MathWorks, Inc.
 Author-email: cloud@mathworks.com
 License: MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE
 Description: # MATLAB Proxy
         [![GitHub Workflow Status](https://img.shields.io/github/actions/workflow/status/mathworks/matlab-proxy/run-tests.yml?branch=main&logo=github)](https://github.com/mathworks/matlab-proxy/actions) &nbsp; [![PyPI badge](https://img.shields.io/pypi/v/matlab-proxy.svg?logo=pypi)](https://pypi.python.org/pypi/matlab-proxy) &nbsp;  [![codecov](https://codecov.io/gh/mathworks/matlab-proxy/branch/main/graph/badge.svg?token=ZW3SESKCSS)](https://codecov.io/gh/mathworks/matlab-proxy) &nbsp; [![Downloads](https://static.pepy.tech/personalized-badge/matlab-proxy?period=month&units=international_system&left_color=grey&right_color=blue&left_text=PyPI%20downloads/month)](https://pepy.tech/project/matlab-proxy)
@@ -126,20 +126,20 @@
           <img width="800" src="https://github.com/mathworks/matlab-proxy/raw/main/img/status_panel.png">
         </p>
         
         The following options are available in the status panel (some options are only available in a specific context):
         
         | Option |  Description |
         | ---- | ---- |
-        | Start MATLAB Session | Start your MATLAB session. Available if MATLAB is stopped.|
-        | Restart MATLAB Session | Restart your MATLAB session. Available if MATLAB is running or starting.|
-        | Stop MATLAB Session | Stop your MATLAB session. Use this option if you want to free up RAM and CPU resources. Available if MATLAB is running or starting.|
-        | Sign Out | Sign out of MATLAB. Use this to stop MATLAB and sign in with an alternative account. Available if using online licensing.|
+        | Start MATLAB | Start your MATLAB session. Available if MATLAB is stopped.|
+        | Restart MATLAB | Restart your MATLAB session. Available if MATLAB is running or starting.|
+        | Stop MATLAB | Stop your MATLAB session. Use this option if you want to free up RAM and CPU resources. Available if MATLAB is running or starting.|
+        | Sign Out | Sign out of MATLAB session. Use this to stop MATLAB and sign in with an alternative account. Available if using online licensing.|
         | Unset License Server Address | Unset network license manager server address. Use this to stop MATLAB and enter new licensing information. Available if using network license manager.|
-        | Feedback | Send feedback about the MATLAB Proxy. This action opens your default email application.|
+        | Feedback | Provide feedback. Opens a new tab to create an issue on GitHub.|
         | Help | Open a help pop-up for a detailed description of the options.|
         
         ## Examples
         * For installing/usage in a Docker container, see this [Dockerfile](./examples/Dockerfile) and its [README](./examples/README.md).
         * For upgrading **matlab-proxy** in an existing Docker image, see this [Dockerfile.upgrade.matlab-proxy](./examples/Dockerfile.upgrade.matlab-proxy) and its [README](./examples/README.md#upgrading-matlab-proxy-package-in-a-docker-image).*
         * For usage in a Jupyter environment, see [jupyter-matlab-proxy](https://github.com/mathworks/jupyter-matlab-proxy).
```

### Comparing `matlab-proxy-0.9.0/matlab_proxy.egg-info/SOURCES.txt` & `matlab-proxy-0.9.1/matlab_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `matlab-proxy-0.9.0/setup.py` & `matlab-proxy-0.9.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
 INSTALL_REQUIRES = ["aiohttp>=3.7.4", "psutil", "aiohttp_session[secure]"]
 
 HERE = Path(__file__).parent.resolve()
 long_description = (HERE / "README.md").read_text()
 
 setuptools.setup(
     name="matlab-proxy",
-    version="0.9.0",
+    version="0.9.1",
     url=config["doc_url"],
     author="The MathWorks, Inc.",
     author_email="cloud@mathworks.com",
     license="MATHWORKS CLOUD REFERENCE ARCHITECTURE LICENSE",
     description="Python® package enables you to launch MATLAB® and access it from a web browser.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

