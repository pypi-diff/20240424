# Comparing `tmp/oarepo-dashboard-1.0.4.tar.gz` & `tmp/oarepo_dashboard-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oarepo-dashboard-1.0.4.tar", last modified: Fri Apr  5 13:56:05 2024, max compression
+gzip compressed data, was "oarepo_dashboard-1.0.5.tar", last modified: Wed Apr 24 08:18:11 2024, max compression
```

## Comparing `oarepo-dashboard-1.0.4.tar` & `oarepo_dashboard-1.0.5.tar`

### file list

```diff
@@ -1,101 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/translations.json
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.953760 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po
--rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/messages.mo
--rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/messages.pot
--rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/
--rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.945761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/RestrictedLabel.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/templates/DashboardCommunitiesPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/
--rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.957761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/templates/DashboardRecordsPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.949761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/
--rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/TypeIcons.jsx
--rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/
--rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/templates/DashboardRequestsPage.jinja
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/webpack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 13:56:05.961761 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3722 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 13:56:05.000000 oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1679 2024-04-05 13:56:05.965761 oarepo-dashboard-1.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 13:53:57.000000 oarepo-dashboard-1.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.439001 oarepo_dashboard-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 08:18:11.439001 oarepo_dashboard-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.427001 oarepo_dashboard-1.0.5/oarepo_dashboard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.427001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.419001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.427001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.427001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.419001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.427001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.419001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.427001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)        2 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/en/LC_MESSAGES/translations.json
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/cs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3842 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/en/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po
+-rw-r--r--   0 runner    (1001) docker     (127)      395 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/messages.mo
+-rw-r--r--   0 runner    (1001) docker     (127)     1785 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/messages.pot
+-rw-r--r--   0 runner    (1001) docker     (127)      368 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/
+-rw-r--r--   0 runner    (1001) docker     (127)     1437 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4500 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4804 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/RestrictedLabel.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/templates/DashboardCommunitiesPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2688 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     5238 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4918 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.431001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/collections/
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/collections/grid.overrides
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/collections/grid.variables
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/elements/
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/elements/button.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/views/
+-rw-r--r--   0 runner    (1001) docker     (127)      405 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/views/item.overrides
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      484 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/
+-rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      414 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/templates/DashboardRecordsPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.423001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.427001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/
+-rw-r--r--   0 runner    (1001) docker     (127)     3552 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/icons/TypeIcons.jsx
+-rw-r--r--   0 runner    (1001) docker     (127)     4028 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)      522 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/templates/DashboardRequestsPage.jinja
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/webpack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:18:11.435001 oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      612 2024-04-24 08:18:11.000000 oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4183 2024-04-24 08:18:11.000000 oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:18:11.000000 oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      903 2024-04-24 08:18:11.000000 oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 08:18:11.000000 oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 08:18:11.000000 oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-24 08:18:11.439001 oarepo_dashboard-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:15:24.000000 oarepo_dashboard-1.0.5/setup.py
```

### Comparing `oarepo-dashboard-1.0.4/PKG-INFO` & `oarepo_dashboard-1.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-dashboard
-Version: 1.0.4
+Version: 1.0.5
 Summary: Support for user dashboard (records, communities, requests)
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
 Requires-Dist: cachetools
 Provides-Extra: dev
```

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js` & `oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/i18next.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json` & `oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/semantic-ui/translations/messages/cs/LC_MESSAGES/translations.json`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo` & `oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.mo`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po` & `oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/cs/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po` & `oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/en/LC_MESSAGES/messages.po`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/i18n/translations/messages.pot` & `oarepo_dashboard-1.0.5/oarepo_dashboard/i18n/translations/messages.pot`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/__init__.py` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/CommunityTypeLabel.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/ComputerTabletCommunitiesListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/MobileCommunitiesListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_communities/semantic-ui/js/dashboard_communities/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_components/webpack.py` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_components/webpack.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/__init__.py` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/__init__.py` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/ComputerTabletRequestsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/MobileRequestsListItem.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/RequestTypeSpecificComponents.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/index.js`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx` & `oarepo_dashboard-1.0.5/oarepo_dashboard/ui/dashboard_requests/semantic-ui/js/dashboard_requests/search/labels/TypeLabels.jsx`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/PKG-INFO` & `oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oarepo-dashboard
-Version: 1.0.4
+Version: 1.0.5
 Summary: Support for user dashboard (records, communities, requests)
 Description-Content-Type: text/markdown
 Requires-Dist: oarepo-runtime>=1.4.44
 Requires-Dist: openpyxl
 Requires-Dist: oarepo-ui>=5.0.91
 Requires-Dist: cachetools
 Provides-Extra: dev
```

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/SOURCES.txt` & `oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -36,14 +36,18 @@
 oarepo_dashboard/ui/dashboard_components/webpack.py
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/custom-components.js
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/FacetsButtonGroupNameToggler.jsx
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppLayout.jsx
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/UserDashboardSearchAppResultView.jsx
 oarepo_dashboard/ui/dashboard_components/semantic-ui/js/dashboard_components/search/index.js
 oarepo_dashboard/ui/dashboard_components/semantic-ui/less/custom-components.less
+oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/collections/grid.overrides
+oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/collections/grid.variables
+oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/elements/button.overrides
+oarepo_dashboard/ui/dashboard_components/semantic-ui/less/oarepo_dashboard/themes/default/views/item.overrides
 oarepo_dashboard/ui/dashboard_components/templates/Header.jinja
 oarepo_dashboard/ui/dashboard_records/__init__.py
 oarepo_dashboard/ui/dashboard_records/webpack.py
 oarepo_dashboard/ui/dashboard_records/semantic-ui/js/dashboard_records/search/index.js
 oarepo_dashboard/ui/dashboard_records/templates/DashboardRecordsPage.jinja
 oarepo_dashboard/ui/dashboard_requests/__init__.py
 oarepo_dashboard/ui/dashboard_requests/webpack.py
```

### Comparing `oarepo-dashboard-1.0.4/oarepo_dashboard.egg-info/entry_points.txt` & `oarepo_dashboard-1.0.5/oarepo_dashboard.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `oarepo-dashboard-1.0.4/setup.cfg` & `oarepo_dashboard-1.0.5/setup.cfg`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [metadata]
 name = oarepo-dashboard
-version = 1.0.4
+version = 1.0.5
 description = Support for user dashboard (records, communities, requests)
 authors = Mirek Simek <miroslav.simek@cesnet.cz>
 readme = README.md
 long_description = file:README.md
 long_description_content_type = text/markdown
 
 [options]
-python = >=3.9
+python = >=3.10
 install_requires = 
 	oarepo-runtime>=1.4.44
 	openpyxl
 	oarepo-ui>=5.0.91
 	cachetools
 packages = find:
 include_package_data = True
@@ -28,15 +28,15 @@
 	autoflake
 
 [options.packages.find]
 exclude = 
 	tests
 
 [options.package_data]
-* = *.json, *.rst, *.md, *.json5, *.jinja2, *.po, *.mo, *.pot, *.js, *.jsx, *.less, *.jinja
+* = *.json, *.rst, *.md, *.json5, *.jinja2, *.po, *.mo, *.pot, *.js, *.jsx, *.less, *.jinja, *.overrides, *.variables
 
 [options.entry_points]
 invenio_base.blueprints = 
 	oarepo_dashboard_records = oarepo_dashboard.ui.dashboard_records:create_blueprint
 	oarepo_dashboard_requests = oarepo_dashboard.ui.dashboard_requests:create_blueprint
 	oarepo_dashboard_communities  = oarepo_dashboard.ui.dashboard_communities:create_blueprint
 	oarepo_dashboard_components  = oarepo_dashboard.ui.dashboard_components:create_blueprint
```

