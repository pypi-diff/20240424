# Comparing `tmp/seatsio-76.5.0.tar.gz` & `tmp/seatsio-76.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "seatsio-76.5.0.tar", last modified: Mon Mar  4 08:58:56 2024, max compression
+gzip compressed data, was "seatsio-76.6.0.tar", last modified: Wed Apr 24 11:23:49 2024, max compression
```

## Comparing `seatsio-76.5.0.tar` & `seatsio-76.6.0.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-03-04 08:58:48.000000 seatsio-76.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-03-04 08:58:48.000000 seatsio-76.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-04 08:58:56.531534 seatsio-76.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-03-04 08:58:48.000000 seatsio-76.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.527533 seatsio-76.5.0/seatsio/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.527533 seatsio-76.5.0/seatsio/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/charts/chartsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/charts/chartsRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    15082 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/domain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.527533 seatsio-76.5.0/seatsio/eventlog/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/eventlog/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/eventlog/eventLogClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/changeObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/channelProperties.py
--rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/channelsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/channelsRequests.py
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/createMultipleEventsRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      895 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/createSingleEventRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      787 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/eventProperties.py
--rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/eventsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/extraDataRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      265 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/forSaleRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/objectProperties.py
--rw-r--r--   0 runner    (1001) docker     (127)      105 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/overrideSeasonObjectStatusRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/statusChangeRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/events/updateEventRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/holdtokens/
--rw-r--r--   0 runner    (1001) docker     (127)      837 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/holdtokens/HoldTokenClient.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/holdtokens/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/httpClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/pagination/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/pagination/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/pagination/listableObjectsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/pagination/lister.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/pagination/page.py
--rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/pagination/pageFetcher.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/pagination/pagedIterator.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/region.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/reports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/reports/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/reports/charts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/reports/charts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/reports/charts/chartReports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/reports/events/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/reports/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/reports/events/eventReports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/reports/usage/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/reports/usage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/reports/usage/usageReports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/seasons/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/seasons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/seasons/seasonsClient.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.531534 seatsio-76.5.0/seatsio/workspaces/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/workspaces/UpdateWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/workspaces/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/workspaces/createWorkspaceRequest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-03-04 08:58:48.000000 seatsio-76.5.0/seatsio/workspaces/workspacesClient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-04 08:58:56.527533 seatsio-76.5.0/seatsio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-03-04 08:58:56.000000 seatsio-76.5.0/seatsio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-03-04 08:58:56.000000 seatsio-76.5.0/seatsio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-04 08:58:56.000000 seatsio-76.5.0/seatsio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-04 08:58:56.000000 seatsio-76.5.0/seatsio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-04 08:58:56.000000 seatsio-76.5.0/seatsio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-04 08:58:56.531534 seatsio-76.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-03-04 08:58:54.000000 seatsio-76.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 11:23:44.000000 seatsio-76.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 11:23:44.000000 seatsio-76.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-24 11:23:49.213226 seatsio-76.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6353 2024-04-24 11:23:44.000000 seatsio-76.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.205226 seatsio-76.6.0/seatsio/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5980 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/charts/chartsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/charts/chartsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/domain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/eventlog/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/eventlog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/eventlog/eventLogClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/changeBestAvailableObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1879 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/changeObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/channelProperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1972 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/channelsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/channelsRequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/createMultipleEventsRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/createSingleEventRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      787 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/eventProperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11568 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/eventsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/extraDataRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      265 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/forSaleRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/objectProperties.py
+-rw-r--r--   0 runner    (1001) docker     (127)      105 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/overrideSeasonObjectStatusRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/statusChangeRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/events/updateEventRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio/holdtokens/
+-rw-r--r--   0 runner    (1001) docker     (127)      837 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/holdtokens/HoldTokenClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/holdtokens/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5983 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/httpClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/pagination/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/listableObjectsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/lister.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1129 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/pageFetcher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/pagination/pagedIterator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/region.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/charts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/charts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/charts/chartReports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/events/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4590 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/events/eventReports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/reports/usage/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/usage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/reports/usage/usageReports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/seasons/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/seasons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/seasons/seasonsClient.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.213226 seatsio-76.6.0/seatsio/workspaces/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/UpdateWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/createWorkspaceRequest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1970 2024-04-24 11:23:44.000000 seatsio-76.6.0/seatsio/workspaces/workspacesClient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 11:23:49.209226 seatsio-76.6.0/seatsio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6666 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 11:23:49.000000 seatsio-76.6.0/seatsio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 11:23:49.213226 seatsio-76.6.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-04-24 11:23:46.000000 seatsio-76.6.0/setup.py
```

### Comparing `seatsio-76.5.0/LICENSE` & `seatsio-76.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/PKG-INFO` & `seatsio-76.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 76.5.0
+Version: 76.6.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-76.5.0/README.md` & `seatsio-76.6.0/README.md`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/charts/chartsClient.py` & `seatsio-76.6.0/seatsio/charts/chartsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/client.py` & `seatsio-76.6.0/seatsio/client.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/domain.py` & `seatsio-76.6.0/seatsio/domain.py`

 * *Files 0% similar despite different names*

```diff
@@ -291,14 +291,15 @@
         self.channel = item_data.get('channel')
         self.distance_to_focal_point = item_data.get('distanceToFocalPoint')
         self.holds = item_data.get('holds')
         self.num_seats = item_data.get('numSeats')
         self.variable_occupancy = item_data.get('variableOccupancy')
         self.min_occupancy = item_data.get('minOccupancy')
         self.max_occupancy = item_data.get('maxOccupancy')
+        self.season_status_overridden_quantity = item_data.get('seasonStatusOverriddenQuantity')
 
 
 class UsageSummaryForAllMonths:
     def __init__(self, json):
         self.usage = list(map(lambda x: UsageSummaryForMonth(x), json.get("usage")))
         self.usage_cutoff_date = parse_date(json.get("usageCutoffDate"))
```

### Comparing `seatsio-76.5.0/seatsio/events/changeBestAvailableObjectStatusRequest.py` & `seatsio-76.6.0/seatsio/events/changeBestAvailableObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/changeObjectStatusRequest.py` & `seatsio-76.6.0/seatsio/events/changeObjectStatusRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/channelsClient.py` & `seatsio-76.6.0/seatsio/events/channelsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/channelsRequests.py` & `seatsio-76.6.0/seatsio/events/channelsRequests.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/createSingleEventRequest.py` & `seatsio-76.6.0/seatsio/events/createSingleEventRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/eventProperties.py` & `seatsio-76.6.0/seatsio/events/eventProperties.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/eventsClient.py` & `seatsio-76.6.0/seatsio/events/eventsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/statusChangeRequest.py` & `seatsio-76.6.0/seatsio/events/statusChangeRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/events/updateEventRequest.py` & `seatsio-76.6.0/seatsio/events/updateEventRequest.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/exceptions.py` & `seatsio-76.6.0/seatsio/exceptions.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/holdtokens/HoldTokenClient.py` & `seatsio-76.6.0/seatsio/holdtokens/HoldTokenClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/httpClient.py` & `seatsio-76.6.0/seatsio/httpClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/pagination/listableObjectsClient.py` & `seatsio-76.6.0/seatsio/pagination/listableObjectsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/pagination/lister.py` & `seatsio-76.6.0/seatsio/pagination/lister.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/pagination/page.py` & `seatsio-76.6.0/seatsio/pagination/page.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/pagination/pageFetcher.py` & `seatsio-76.6.0/seatsio/pagination/pageFetcher.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/pagination/pagedIterator.py` & `seatsio-76.6.0/seatsio/pagination/pagedIterator.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/reports/charts/chartReports.py` & `seatsio-76.6.0/seatsio/reports/charts/chartReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/reports/events/eventReports.py` & `seatsio-76.6.0/seatsio/reports/events/eventReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/reports/usage/usageReports.py` & `seatsio-76.6.0/seatsio/reports/usage/usageReports.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/seasons/seasonsClient.py` & `seatsio-76.6.0/seatsio/seasons/seasonsClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio/workspaces/workspacesClient.py` & `seatsio-76.6.0/seatsio/workspaces/workspacesClient.py`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/seatsio.egg-info/PKG-INFO` & `seatsio-76.6.0/seatsio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: seatsio
-Version: 76.5.0
+Version: 76.6.0
 Summary: The official Seats.io Python client library
 Home-page: https://github.com/seatsio/seatsio-python
 Author: The seats.io dev team
 Author-email: hello@seats.io
 License: MIT
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `seatsio-76.5.0/seatsio.egg-info/SOURCES.txt` & `seatsio-76.6.0/seatsio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `seatsio-76.5.0/setup.py` & `seatsio-76.6.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.md') as f:
     readme = f.read()
 
 setup(
     name='seatsio',
-    version='v76.5.0',
+    version='v76.6.0',
     description='The official Seats.io Python client library',
     author='The seats.io dev team',
     author_email='hello@seats.io',
     url='https://github.com/seatsio/seatsio-python',
     license="MIT",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
```

