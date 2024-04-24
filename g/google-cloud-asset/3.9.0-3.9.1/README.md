# Comparing `tmp/google-cloud-asset-3.9.0.tar.gz` & `tmp/google-cloud-asset-3.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-asset-3.9.0.tar", last modified: Thu May 19 12:39:53 2022, max compression
+gzip compressed data, was "google-cloud-asset-3.9.1.tar", last modified: Tue Jun  7 10:41:30 2022, max compression
```

## Comparing `google-cloud-asset-3.9.0.tar` & `google-cloud-asset-3.9.1.tar`

### file list

```diff
@@ -1,148 +1,148 @@
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/
--rw-rw-r--   0 root         (0)     1003    11358 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     3794 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     2966 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.568591 google-cloud-asset-3.9.0/google/
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.568591 google-cloud-asset-3.9.0/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.572589 google-cloud-asset-3.9.0/google/cloud/asset/
--rw-rw-r--   0 root         (0)     1003     7185 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset/__init__.py
--rw-rw-r--   0 root         (0)     1003       79 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.572589 google-cloud-asset-3.9.0/google/cloud/asset_v1/
--rw-rw-r--   0 root         (0)     1003     5755 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     5359 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.572589 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.572589 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/
--rw-rw-r--   0 root         (0)     1003      761 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    94383 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/async_client.py
--rw-rw-r--   0 root         (0)     1003   106089 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/client.py
--rw-rw-r--   0 root         (0)     1003    21015 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.576587 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    17620 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    35839 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    36622 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.576587 google-cloud-asset-3.9.0/google/cloud/asset_v1/types/
--rw-rw-r--   0 root         (0)     1003     3984 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    98390 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/types/asset_service.py
--rw-rw-r--   0 root         (0)     1003    54163 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1/types/assets.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.576587 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003     1386 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1091 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.576587 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.576587 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/
--rw-rw-r--   0 root         (0)     1003      761 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    20682 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    28452 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/client.py
--rw-rw-r--   0 root         (0)     1003    11209 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.576587 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     7235 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13690 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    13928 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.576587 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/types/
--rw-rw-r--   0 root         (0)     1003     1092 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     6841 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/types/asset_service.py
--rw-rw-r--   0 root         (0)     1003     6574 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/types/assets.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.580585 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003     1849 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1693 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.580585 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.580585 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/
--rw-rw-r--   0 root         (0)     1003      761 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    28959 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    37267 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.580585 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     8696 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    15828 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    16161 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.580585 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/types/
--rw-rw-r--   0 root         (0)     1003     1310 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    10061 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/types/asset_service.py
--rw-rw-r--   0 root         (0)     1003     6709 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/types/assets.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.580585 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003     1440 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003     1095 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.580585 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.584583 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/
--rw-rw-r--   0 root         (0)     1003      761 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    16820 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    25007 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/client.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.584583 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6973 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    13996 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    14297 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.584583 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/types/
--rw-rw-r--   0 root         (0)     1003     1132 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    21551 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/types/asset_service.py
--rw-rw-r--   0 root         (0)     1003    11773 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/types/assets.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.584583 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/
--rw-rw-r--   0 root         (0)     1003     1103 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003      781 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003       79 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.584583 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.584583 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/
--rw-rw-r--   0 root         (0)     1003      761 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/__init__.py
--rw-rw-r--   0 root         (0)     1003    13183 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/async_client.py
--rw-rw-r--   0 root         (0)     1003    22601 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/client.py
--rw-rw-r--   0 root         (0)     1003     5769 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.588581 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/
--rw-rw-r--   0 root         (0)     1003     1176 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003     6247 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/base.py
--rw-rw-r--   0 root         (0)     1003    11579 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    11809 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc_asyncio.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.588581 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/types/
--rw-rw-r--   0 root         (0)     1003      858 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003     4502 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/types/asset_service.py
--rw-rw-r--   0 root         (0)     1003     7310 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/types/assets.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.588581 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/
--rw-r--r--   0 root         (0)     1003     3794 2022-05-19 12:39:52.000000 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     5376 2022-05-19 12:39:53.000000 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2022-05-19 12:39:52.000000 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003       20 2022-05-19 12:39:53.000000 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/namespace_packages.txt
--rw-r--r--   0 root         (0)     1003        1 2022-05-19 12:39:52.000000 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      282 2022-05-19 12:39:53.000000 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2022-05-19 12:39:53.000000 google-cloud-asset-3.9.0/google_cloud_asset.egg-info/top_level.txt
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.588581 google-cloud-asset-3.9.0/scripts/
--rw-rw-r--   0 root         (0)     1003     7352 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/scripts/fixup_asset_v1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6111 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/scripts/fixup_asset_v1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6087 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/scripts/fixup_asset_v1p1beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6104 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/scripts/fixup_asset_v1p2beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6046 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/scripts/fixup_asset_v1p4beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003     6003 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/scripts/fixup_asset_v1p5beta1_keywords.py
--rw-rw-r--   0 root         (0)     1003       67 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3395 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.588581 google-cloud-asset-3.9.0/tests/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.588581 google-cloud-asset-3.9.0/tests/system/
--rw-rw-r--   0 root         (0)     1003     2827 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/system/test_vpcsc.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   226370 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1/test_asset_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p1beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p1beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    79563 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p1beta1/test_asset_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p2beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p2beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    89244 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p2beta1/test_asset_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p4beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p4beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    60156 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p4beta1/test_asset_service.py
-drwxr-sr-x   0 root         (0)     1003        0 2022-05-19 12:39:53.592579 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p5beta1/
--rw-rw-r--   0 root         (0)     1003      600 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p5beta1/__init__.py
--rw-rw-r--   0 root         (0)     1003    61056 2022-05-19 12:37:03.000000 google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p5beta1/test_asset_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.710438 google-cloud-asset-3.9.1/
+-rw-rw-r--   0 root         (0)     1003    11358 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     3794 2022-06-07 10:41:30.710438 google-cloud-asset-3.9.1/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     2966 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.682452 google-cloud-asset-3.9.1/google/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.686450 google-cloud-asset-3.9.1/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.690448 google-cloud-asset-3.9.1/google/cloud/asset/
+-rw-rw-r--   0 root         (0)     1003     7185 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset/__init__.py
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.690448 google-cloud-asset-3.9.1/google/cloud/asset_v1/
+-rw-rw-r--   0 root         (0)     1003     5755 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     5359 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.690448 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.690448 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/
+-rw-rw-r--   0 root         (0)     1003      761 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    94383 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003   106089 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/client.py
+-rw-rw-r--   0 root         (0)     1003    21015 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.690448 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    17620 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    35839 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    36622 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.690448 google-cloud-asset-3.9.1/google/cloud/asset_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3984 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    98390 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/types/asset_service.py
+-rw-rw-r--   0 root         (0)     1003    54163 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1/types/assets.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003     1386 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1091 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/
+-rw-rw-r--   0 root         (0)     1003      761 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    20682 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    28452 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/client.py
+-rw-rw-r--   0 root         (0)     1003    11209 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     7235 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13690 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    13928 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1092 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6841 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/types/asset_service.py
+-rw-rw-r--   0 root         (0)     1003     6574 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/types/assets.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003     1849 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1693 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.694446 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/
+-rw-rw-r--   0 root         (0)     1003      761 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    28959 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    37267 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.698444 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     8696 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    15828 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    16161 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.698444 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1310 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    10061 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/types/asset_service.py
+-rw-rw-r--   0 root         (0)     1003     6709 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/types/assets.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.698444 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003     1440 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     1095 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.698444 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.698444 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/
+-rw-rw-r--   0 root         (0)     1003      761 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    16820 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    25007 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/client.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.698444 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6973 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    13996 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    14297 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.698444 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/types/
+-rw-rw-r--   0 root         (0)     1003     1132 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    21551 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/types/asset_service.py
+-rw-rw-r--   0 root         (0)     1003    11773 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/types/assets.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.702442 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/
+-rw-rw-r--   0 root         (0)     1003     1103 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003      781 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003       79 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.702442 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.702442 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/
+-rw-rw-r--   0 root         (0)     1003      761 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/__init__.py
+-rw-rw-r--   0 root         (0)     1003    13183 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/async_client.py
+-rw-rw-r--   0 root         (0)     1003    22601 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/client.py
+-rw-rw-r--   0 root         (0)     1003     5769 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.702442 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/
+-rw-rw-r--   0 root         (0)     1003     1176 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003     6247 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    11579 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    11809 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc_asyncio.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.702442 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/types/
+-rw-rw-r--   0 root         (0)     1003      858 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003     4502 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/types/asset_service.py
+-rw-rw-r--   0 root         (0)     1003     7310 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/types/assets.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/
+-rw-r--r--   0 root         (0)     1003     3794 2022-06-07 10:41:29.000000 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     5376 2022-06-07 10:41:30.000000 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-06-07 10:41:30.000000 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003       20 2022-06-07 10:41:30.000000 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/namespace_packages.txt
+-rw-r--r--   0 root         (0)     1003        1 2022-06-07 10:41:29.000000 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      320 2022-06-07 10:41:30.000000 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2022-06-07 10:41:30.000000 google-cloud-asset-3.9.1/google_cloud_asset.egg-info/top_level.txt
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/scripts/
+-rw-rw-r--   0 root         (0)     1003     7352 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/scripts/fixup_asset_v1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6111 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/scripts/fixup_asset_v1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6087 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/scripts/fixup_asset_v1p1beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6104 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/scripts/fixup_asset_v1p2beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6046 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/scripts/fixup_asset_v1p4beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003     6003 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/scripts/fixup_asset_v1p5beta1_keywords.py
+-rw-rw-r--   0 root         (0)     1003       67 2022-06-07 10:41:30.710438 google-cloud-asset-3.9.1/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3441 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/tests/system/
+-rw-rw-r--   0 root         (0)     1003     2827 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/system/test_vpcsc.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   226525 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1/test_asset_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p1beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p1beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    79718 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p1beta1/test_asset_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.706440 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p2beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p2beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    89399 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p2beta1/test_asset_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.710438 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p4beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p4beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    60311 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p4beta1/test_asset_service.py
+drwxr-sr-x   0 root         (0)     1003        0 2022-06-07 10:41:30.710438 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p5beta1/
+-rw-rw-r--   0 root         (0)     1003      600 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p5beta1/__init__.py
+-rw-rw-r--   0 root         (0)     1003    61211 2022-06-07 10:38:52.000000 google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p5beta1/test_asset_service.py
```

### Comparing `google-cloud-asset-3.9.0/LICENSE` & `google-cloud-asset-3.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/MANIFEST.in` & `google-cloud-asset-3.9.1/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/PKG-INFO` & `google-cloud-asset-3.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-asset
-Version: 3.9.0
+Version: 3.9.1
 Summary: Cloud Asset API API client library
 Home-page: https://github.com/googleapis/python-asset
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-asset-3.9.0/README.rst` & `google-cloud-asset-3.9.1/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/gapic_metadata.json` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/async_client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/pagers.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/base.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/grpc.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/services/asset_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/types/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/types/asset_service.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/types/asset_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1/types/assets.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1/types/assets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/gapic_metadata.json` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/async_client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/pagers.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/base.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc_asyncio.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/services/asset_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/types/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/types/asset_service.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/types/asset_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p1beta1/types/assets.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p1beta1/types/assets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/gapic_metadata.json` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/async_client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/base.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc_asyncio.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/services/asset_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/types/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/types/asset_service.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/types/asset_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p2beta1/types/assets.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p2beta1/types/assets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/gapic_metadata.json` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/async_client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/base.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc_asyncio.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/services/asset_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/types/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/types/asset_service.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/types/asset_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p4beta1/types/assets.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p4beta1/types/assets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/gapic_metadata.json` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/async_client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/client.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/pagers.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/base.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc_asyncio.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/services/asset_service/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/types/__init__.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/types/asset_service.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/types/asset_service.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google/cloud/asset_v1p5beta1/types/assets.py` & `google-cloud-asset-3.9.1/google/cloud/asset_v1p5beta1/types/assets.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/google_cloud_asset.egg-info/PKG-INFO` & `google-cloud-asset-3.9.1/google_cloud_asset.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-asset
-Version: 3.9.0
+Version: 3.9.1
 Summary: Cloud Asset API API client library
 Home-page: https://github.com/googleapis/python-asset
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `google-cloud-asset-3.9.0/google_cloud_asset.egg-info/SOURCES.txt` & `google-cloud-asset-3.9.1/google_cloud_asset.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/scripts/fixup_asset_v1_keywords.py` & `google-cloud-asset-3.9.1/scripts/fixup_asset_v1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/scripts/fixup_asset_v1beta1_keywords.py` & `google-cloud-asset-3.9.1/scripts/fixup_asset_v1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/scripts/fixup_asset_v1p1beta1_keywords.py` & `google-cloud-asset-3.9.1/scripts/fixup_asset_v1p1beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/scripts/fixup_asset_v1p2beta1_keywords.py` & `google-cloud-asset-3.9.1/scripts/fixup_asset_v1p2beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/scripts/fixup_asset_v1p4beta1_keywords.py` & `google-cloud-asset-3.9.1/scripts/fixup_asset_v1p4beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/scripts/fixup_asset_v1p5beta1_keywords.py` & `google-cloud-asset-3.9.1/scripts/fixup_asset_v1p5beta1_keywords.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/setup.py` & `google-cloud-asset-3.9.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,30 +17,31 @@
 
 import setuptools
 
 # Package metadata.
 
 name = "google-cloud-asset"
 description = "Cloud Asset API API client library"
-version = "3.9.0"
+version = "3.9.1"
 # Should be one of:
 # 'Development Status :: 3 - Alpha'
 # 'Development Status :: 4 - Beta'
 # 'Development Status :: 5 - Production/Stable'
 release_status = "Development Status :: 5 - Production/Stable"
 dependencies = [
     # NOTE: Maintainers, please do not require google-api-core>=2.x.x
     # Until this issue is closed
     # https://github.com/googleapis/google-cloud-python/issues/10566
     "google-api-core[grpc] >= 1.31.5, <3.0.0dev,!=2.0.*,!=2.1.*,!=2.2.*,!=2.3.0",
-    "grpc-google-iam-v1 >= 0.12.3, < 0.13dev",
-    "google-cloud-access-context-manager >= 0.1.2, < 0.2.0dev",
+    "grpc-google-iam-v1 >=0.12.4, <1.0.0dev",
+    "google-cloud-access-context-manager >= 0.1.2, <1.0.0dev",
     "google-cloud-org-policy>=0.1.2, <2.0.0",
     "google-cloud-os-config >= 1.0.0, <2.0.0dev",
-    "proto-plus >= 1.15.0",
+    "proto-plus >= 1.15.0, <2.0.0dev",
+    "protobuf >= 3.19.0, <4.0.0dev",
 ]
 
 extras = {"libcst": "libcst >= 0.2.5"}
 
 # Setup boilerplate below this line.
 
 package_root = os.path.abspath(os.path.dirname(__file__))
```

### Comparing `google-cloud-asset-3.9.0/tests/__init__.py` & `google-cloud-asset-3.9.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/system/test_vpcsc.py` & `google-cloud-asset-3.9.1/tests/system/test_vpcsc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/__init__.py` & `google-cloud-asset-3.9.1/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/__init__.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1/__init__.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1/test_asset_service.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1/test_asset_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
```

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p1beta1/__init__.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p1beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p1beta1/test_asset_service.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p1beta1/test_asset_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
```

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p2beta1/__init__.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p2beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p2beta1/test_asset_service.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p2beta1/test_asset_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
```

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p4beta1/__init__.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p4beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p4beta1/test_asset_service.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p4beta1/test_asset_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
```

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p5beta1/__init__.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p5beta1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-asset-3.9.0/tests/unit/gapic/asset_v1p5beta1/test_asset_service.py` & `google-cloud-asset-3.9.1/tests/unit/gapic/asset_v1p5beta1/test_asset_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,21 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 import os
-import mock
+
+# try/except added for compatibility with python < 3.8
+try:
+    from unittest import mock
+    from unittest.mock import AsyncMock
+except ImportError:
+    import mock
 
 import grpc
 from grpc.experimental import aio
 import math
 import pytest
 from proto.marshal.rules.dates import DurationRule, TimestampRule
```

