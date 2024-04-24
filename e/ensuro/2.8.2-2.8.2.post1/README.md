# Comparing `tmp/ensuro-2.8.2.tar.gz` & `tmp/ensuro-2.8.2.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ensuro-2.8.2.tar", last modified: Wed Apr 17 20:18:33 2024, max compression
+gzip compressed data, was "ensuro-2.8.2.post1.tar", last modified: Wed Apr 24 08:48:55 2024, max compression
```

## Comparing `ensuro-2.8.2.tar` & `ensuro-2.8.2.post1.tar`

### file list

```diff
@@ -1,78 +1,81 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.277724 ensuro-2.8.2/
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-17 20:18:27.000000 ensuro-2.8.2/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-17 20:18:27.000000 ensuro-2.8.2/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.261724 ensuro-2.8.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.265724 ensuro-2.8.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-17 20:18:27.000000 ensuro-2.8.2/.github/workflows/publish.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-17 20:18:27.000000 ensuro-2.8.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-17 20:18:27.000000 ensuro-2.8.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-17 20:18:27.000000 ensuro-2.8.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-17 20:18:27.000000 ensuro-2.8.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-04-17 20:18:27.000000 ensuro-2.8.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-17 20:18:27.000000 ensuro-2.8.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-17 20:18:33.277724 ensuro-2.8.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-17 20:18:27.000000 ensuro-2.8.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.265724 ensuro-2.8.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.265724 ensuro-2.8.2/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-17 20:18:27.000000 ensuro-2.8.2/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-17 20:18:27.000000 ensuro-2.8.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1379 2024-04-17 20:18:33.281725 ensuro-2.8.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-17 20:18:27.000000 ensuro-2.8.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.261724 ensuro-2.8.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.269724 ensuro-2.8.2/src/ensuro/
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.277724 ensuro-2.8.2/src/ensuro/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)    40709 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/AccessManager.json
--rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/ERC1967Proxy.json
--rw-r--r--   0 runner    (1001) docker     (127)    27833 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/ERC4626AssetManager.json
--rw-r--r--   0 runner    (1001) docker     (127)   125707 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/EToken.json
--rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IAccessManager.json
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IAssetManager.json
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IERC20.json
--rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IERC20Metadata.json
--rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IERC721.json
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IEToken.json
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/ILPWhitelist.json
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IPolicyHolder.json
--rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IPolicyHolderV2.json
--rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IPolicyPool.json
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IPolicyPoolComponent.json
--rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IPremiumsAccount.json
--rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/IRiskModule.json
--rw-r--r--   0 runner    (1001) docker     (127)    51950 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/LPManualWhitelist.json
--rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/LiquidityThresholdAssetManager.json
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/Policy.json
--rw-r--r--   0 runner    (1001) docker     (127)   137197 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/PolicyPool.json
--rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/PolicyPoolComponent.json
--rw-r--r--   0 runner    (1001) docker     (127)   110486 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/PremiumsAccount.json
--rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/Reserve.json
--rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/RiskModule.json
--rw-r--r--   0 runner    (1001) docker     (127)   125764 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/SignedBucketRiskModule.json
--rw-r--r--   0 runner    (1001) docker     (127)   111859 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/SignedQuoteRiskModule.json
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/TimeScaled.json
--rw-r--r--   0 runner    (1001) docker     (127)   114915 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/TrustfulRiskModule.json
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/contracts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    58867 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/prototype.py
--rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    37817 2024-04-17 20:18:27.000000 ensuro-2.8.2/src/ensuro/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.277724 ensuro-2.8.2/src/ensuro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5414 2024-04-17 20:18:33.000000 ensuro-2.8.2/src/ensuro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-04-17 20:18:33.000000 ensuro-2.8.2/src/ensuro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:18:33.000000 ensuro-2.8.2/src/ensuro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 20:18:32.000000 ensuro-2.8.2/src/ensuro.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-17 20:18:33.000000 ensuro-2.8.2/src/ensuro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 20:18:33.000000 ensuro-2.8.2/src/ensuro.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 20:18:33.277724 ensuro-2.8.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-17 20:18:27.000000 ensuro-2.8.2/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-17 20:18:27.000000 ensuro-2.8.2/tests/test_prototype.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2024-04-17 20:18:27.000000 ensuro-2.8.2/tests/test_wrappers_w3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2320 2024-04-17 20:18:27.000000 ensuro-2.8.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.805293 ensuro-2.8.2.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      622 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.785293 ensuro-2.8.2.post1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.789293 ensuro-2.8.2.post1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      521 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/.github/workflows/tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       95 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    13846 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-24 08:48:55.805293 ensuro-2.8.2.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4495 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.793294 ensuro-2.8.2.post1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1154 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.793294 ensuro-2.8.2.post1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9752 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-04-24 08:48:55.805293 ensuro-2.8.2.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.785293 ensuro-2.8.2.post1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.793294 ensuro-2.8.2.post1/src/ensuro/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.801293 ensuro-2.8.2.post1/src/ensuro/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)    40709 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/AccessManager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6729 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/ERC1967Proxy.json
+-rw-r--r--   0 runner    (1001) docker     (127)    27833 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/ERC4626AssetManager.json
+-rw-r--r--   0 runner    (1001) docker     (127)   125707 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/EToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7281 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IAccessManager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2610 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IAssetManager.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IERC20.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4767 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IERC20Metadata.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6217 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IERC721.json
+-rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IEToken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/ILPWhitelist.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyHolder.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3051 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyHolderV2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20476 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyPool.json
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyPoolComponent.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12307 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IPremiumsAccount.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3577 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/IRiskModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    51950 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/LPManualWhitelist.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4605 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/LiquidityThresholdAssetManager.json
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/Policy.json
+-rw-r--r--   0 runner    (1001) docker     (127)   137197 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/PolicyPool.json
+-rw-r--r--   0 runner    (1001) docker     (127)     6999 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/PolicyPoolComponent.json
+-rw-r--r--   0 runner    (1001) docker     (127)   110486 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/PremiumsAccount.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8468 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/Reserve.json
+-rw-r--r--   0 runner    (1001) docker     (127)    12266 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/RiskModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)   125764 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/SignedBucketRiskModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)   111859 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/SignedQuoteRiskModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)    20261 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/TestCurrency.json
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/TimeScaled.json
+-rw-r--r--   0 runner    (1001) docker     (127)   114915 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/TrustfulRiskModule.json
+-rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/contracts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    58867 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/prototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6025 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37817 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/src/ensuro/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.801293 ensuro-2.8.2.post1/src/ensuro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5578 2024-04-24 08:48:55.000000 ensuro-2.8.2.post1/src/ensuro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-04-24 08:48:55.000000 ensuro-2.8.2.post1/src/ensuro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:48:55.000000 ensuro-2.8.2.post1/src/ensuro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:48:55.000000 ensuro-2.8.2.post1/src/ensuro.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 08:48:55.000000 ensuro-2.8.2.post1/src/ensuro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 08:48:55.000000 ensuro-2.8.2.post1/src/ensuro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:48:55.801293 ensuro-2.8.2.post1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/tests/test_contract_path_handling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/tests/test_prototype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/tests/test_wrappers_w3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2322 2024-04-24 08:48:35.000000 ensuro-2.8.2.post1/tox.ini
```

### Comparing `ensuro-2.8.2/.coveragerc` & `ensuro-2.8.2.post1/.coveragerc`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/.editorconfig` & `ensuro-2.8.2.post1/.editorconfig`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/.github/workflows/publish.yaml` & `ensuro-2.8.2.post1/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/.gitignore` & `ensuro-2.8.2.post1/.gitignore`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/CONTRIBUTING.rst` & `ensuro-2.8.2.post1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/LICENSE.txt` & `ensuro-2.8.2.post1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/PKG-INFO` & `ensuro-2.8.2.post1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensuro
-Version: 2.8.2
+Version: 2.8.2.post1
 Summary: Prototype and wrappers to work with Ensuro Smart Contracts
 Home-page: https://github.com/ensuro/ensuro/
 Author: Guillermo M. Narvaja
 Author-email: guillermo@ensuro.co
 License: Apache-2.0
 Project-URL: Documentation, https://docs.ensuro.co/
 Project-URL: Source, https://github.com/ensuro/ensuro/
@@ -12,24 +12,24 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: pyyaml>=5.1
-Requires-Dist: eth-prototype>=1.0.0
+Requires-Dist: eth-prototype>=1.0.1
 Provides-Extra: web3
-Requires-Dist: eth-prototype[web3]>=1.0.0; extra == "web3"
+Requires-Dist: eth-prototype[web3]>=1.0.1; extra == "web3"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: ipdb; extra == "testing"
 Requires-Dist: web3[tester]; extra == "testing"
-Requires-Dist: eth-prototype[web3]; extra == "testing"
+Requires-Dist: eth-prototype[web3]>=1.0.1; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/ensuro.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/ensuro
@@ -101,28 +101,29 @@
 
 
 Copying files from Ensuro main repository
 =========================================
 
 Instructions to copy files from ensuro repository::
 
+    rm src/ensuro/contracts/*.json
     for x in `find ../ensuro/artifacts/contracts/ -maxdepth 2 -name "*.json" -not -name "*.dbg.json" `; do
         cp $x src/ensuro/contracts/ ;
     done
     for x in `find ../ensuro/artifacts/contracts/interfaces/ -maxdepth 2 -name "*.json" -not -name "*.dbg.json" `; do
         cp $x src/ensuro/contracts/ ;
     done
     for x in ERC1967Proxy.json IERC20Metadata.json IERC20.json IERC721.json ; do
         cp `find ../ensuro/artifacts/@openzeppelin/ -name $x` src/ensuro/contracts/$x ;
     done
+    cp ../ensuro/artifacts/contracts/mocks/TestCurrency.sol/TestCurrency.json src/ensuro/contracts/TestCurrency.json
     cp ../ensuro/prototype/ensuro.py src/ensuro/prototype.py
     cp ../ensuro/prototype/wrappers.py src/ensuro/wrappers.py
     cp ../ensuro/prototype/utils.py src/ensuro/utils.py
 
-
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.1.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `ensuro-2.8.2/README.rst` & `ensuro-2.8.2.post1/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -72,28 +72,29 @@
 
 
 Copying files from Ensuro main repository
 =========================================
 
 Instructions to copy files from ensuro repository::
 
+    rm src/ensuro/contracts/*.json
     for x in `find ../ensuro/artifacts/contracts/ -maxdepth 2 -name "*.json" -not -name "*.dbg.json" `; do
         cp $x src/ensuro/contracts/ ;
     done
     for x in `find ../ensuro/artifacts/contracts/interfaces/ -maxdepth 2 -name "*.json" -not -name "*.dbg.json" `; do
         cp $x src/ensuro/contracts/ ;
     done
     for x in ERC1967Proxy.json IERC20Metadata.json IERC20.json IERC721.json ; do
         cp `find ../ensuro/artifacts/@openzeppelin/ -name $x` src/ensuro/contracts/$x ;
     done
+    cp ../ensuro/artifacts/contracts/mocks/TestCurrency.sol/TestCurrency.json src/ensuro/contracts/TestCurrency.json
     cp ../ensuro/prototype/ensuro.py src/ensuro/prototype.py
     cp ../ensuro/prototype/wrappers.py src/ensuro/wrappers.py
     cp ../ensuro/prototype/utils.py src/ensuro/utils.py
 
-
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.1.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `ensuro-2.8.2/docs/Makefile` & `ensuro-2.8.2.post1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/docs/conf.py` & `ensuro-2.8.2.post1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/docs/index.rst` & `ensuro-2.8.2.post1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/setup.cfg` & `ensuro-2.8.2.post1/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -22,30 +22,33 @@
 include_package_data = True
 package_dir = 
 	=src
 python_requires = >=3.9
 install_requires = 
 	importlib-metadata; python_version<"3.8"
 	pyyaml>=5.1
-	eth-prototype>=1.0.0
+	eth-prototype>=1.0.1
+
+[options.package_data]
+* = *.json
 
 [options.packages.find]
 where = src
 exclude = 
 	tests
 
 [options.extras_require]
-web3 = eth-prototype[web3]>=1.0.0
+web3 = eth-prototype[web3]>=1.0.1
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 	ipdb
 	web3[tester]
-	eth-prototype[web3]
+	eth-prototype[web3]>=1.0.1
 
 [options.entry_points]
 
 [tool:pytest]
 addopts = 
 	--cov ensuro --cov-report term-missing
 	--verbose
```

### Comparing `ensuro-2.8.2/setup.py` & `ensuro-2.8.2.post1/setup.py`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/__init__.py` & `ensuro-2.8.2.post1/src/ensuro/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,9 +13,8 @@
     __version__ = version(dist_name)
 except PackageNotFoundError:  # pragma: no cover
     __version__ = "unknown"
 finally:
     del version, PackageNotFoundError
 
 
-def contracts_path():
-    return os.path.join(os.path.dirname(__file__), "contracts")
+from .contracts import get_contracts_path, register_contract_path  # noqa: F401
```

### Comparing `ensuro-2.8.2/src/ensuro/contracts/AccessManager.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/AccessManager.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/ERC1967Proxy.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/ERC1967Proxy.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/ERC4626AssetManager.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/ERC4626AssetManager.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/EToken.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/EToken.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IAccessManager.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IAccessManager.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IAssetManager.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IAssetManager.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IERC20.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IERC20.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IERC20Metadata.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IERC20Metadata.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IERC721.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IERC721.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IEToken.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IEToken.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/ILPWhitelist.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/ILPWhitelist.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IPolicyHolder.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyHolder.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IPolicyHolderV2.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyHolderV2.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IPolicyPool.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyPool.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IPolicyPoolComponent.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IPolicyPoolComponent.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IPremiumsAccount.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IPremiumsAccount.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/IRiskModule.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/IRiskModule.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/LPManualWhitelist.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/LPManualWhitelist.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/LiquidityThresholdAssetManager.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/LiquidityThresholdAssetManager.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/Policy.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/Policy.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/PolicyPool.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/PolicyPool.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/PolicyPoolComponent.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/PolicyPoolComponent.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/PremiumsAccount.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/PremiumsAccount.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/Reserve.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/Reserve.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/RiskModule.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/RiskModule.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/SignedBucketRiskModule.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/SignedBucketRiskModule.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/SignedQuoteRiskModule.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/SignedQuoteRiskModule.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/TimeScaled.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/TimeScaled.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/contracts/TrustfulRiskModule.json` & `ensuro-2.8.2.post1/src/ensuro/contracts/TrustfulRiskModule.json`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/prototype.py` & `ensuro-2.8.2.post1/src/ensuro/prototype.py`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/utils.py` & `ensuro-2.8.2.post1/src/ensuro/utils.py`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro/wrappers.py` & `ensuro-2.8.2.post1/src/ensuro/wrappers.py`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/src/ensuro.egg-info/PKG-INFO` & `ensuro-2.8.2.post1/src/ensuro.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ensuro
-Version: 2.8.2
+Version: 2.8.2.post1
 Summary: Prototype and wrappers to work with Ensuro Smart Contracts
 Home-page: https://github.com/ensuro/ensuro/
 Author: Guillermo M. Narvaja
 Author-email: guillermo@ensuro.co
 License: Apache-2.0
 Project-URL: Documentation, https://docs.ensuro.co/
 Project-URL: Source, https://github.com/ensuro/ensuro/
@@ -12,24 +12,24 @@
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.9
 Description-Content-Type: text/x-rst; charset=UTF-8
 License-File: LICENSE.txt
 Requires-Dist: importlib-metadata; python_version < "3.8"
 Requires-Dist: pyyaml>=5.1
-Requires-Dist: eth-prototype>=1.0.0
+Requires-Dist: eth-prototype>=1.0.1
 Provides-Extra: web3
-Requires-Dist: eth-prototype[web3]>=1.0.0; extra == "web3"
+Requires-Dist: eth-prototype[web3]>=1.0.1; extra == "web3"
 Provides-Extra: testing
 Requires-Dist: setuptools; extra == "testing"
 Requires-Dist: pytest; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: ipdb; extra == "testing"
 Requires-Dist: web3[tester]; extra == "testing"
-Requires-Dist: eth-prototype[web3]; extra == "testing"
+Requires-Dist: eth-prototype[web3]>=1.0.1; extra == "testing"
 
 .. These are examples of badges you might want to add to your README:
    please update the URLs accordingly
 
     .. image:: https://api.cirrus-ci.com/github/<USER>/ensuro.svg?branch=main
         :alt: Built Status
         :target: https://cirrus-ci.com/github/<USER>/ensuro
@@ -101,28 +101,29 @@
 
 
 Copying files from Ensuro main repository
 =========================================
 
 Instructions to copy files from ensuro repository::
 
+    rm src/ensuro/contracts/*.json
     for x in `find ../ensuro/artifacts/contracts/ -maxdepth 2 -name "*.json" -not -name "*.dbg.json" `; do
         cp $x src/ensuro/contracts/ ;
     done
     for x in `find ../ensuro/artifacts/contracts/interfaces/ -maxdepth 2 -name "*.json" -not -name "*.dbg.json" `; do
         cp $x src/ensuro/contracts/ ;
     done
     for x in ERC1967Proxy.json IERC20Metadata.json IERC20.json IERC721.json ; do
         cp `find ../ensuro/artifacts/@openzeppelin/ -name $x` src/ensuro/contracts/$x ;
     done
+    cp ../ensuro/artifacts/contracts/mocks/TestCurrency.sol/TestCurrency.json src/ensuro/contracts/TestCurrency.json
     cp ../ensuro/prototype/ensuro.py src/ensuro/prototype.py
     cp ../ensuro/prototype/wrappers.py src/ensuro/wrappers.py
     cp ../ensuro/prototype/utils.py src/ensuro/utils.py
 
-
 .. _pyscaffold-notes:
 
 Note
 ====
 
 This project has been set up using PyScaffold 4.1.1. For details and usage
 information on PyScaffold see https://pyscaffold.org/.
```

### Comparing `ensuro-2.8.2/src/ensuro.egg-info/SOURCES.txt` & `ensuro-2.8.2.post1/src/ensuro.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 LICENSE.txt
 README.rst
 pyproject.toml
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/publish.yaml
+.github/workflows/tests.yaml
 docs/Makefile
 docs/authors.rst
 docs/changelog.rst
 docs/conf.py
 docs/contributing.rst
 docs/index.rst
 docs/license.rst
@@ -55,13 +56,15 @@
 src/ensuro/contracts/PolicyPool.json
 src/ensuro/contracts/PolicyPoolComponent.json
 src/ensuro/contracts/PremiumsAccount.json
 src/ensuro/contracts/Reserve.json
 src/ensuro/contracts/RiskModule.json
 src/ensuro/contracts/SignedBucketRiskModule.json
 src/ensuro/contracts/SignedQuoteRiskModule.json
+src/ensuro/contracts/TestCurrency.json
 src/ensuro/contracts/TimeScaled.json
 src/ensuro/contracts/TrustfulRiskModule.json
 src/ensuro/contracts/__init__.py
 tests/conftest.py
+tests/test_contract_path_handling.py
 tests/test_prototype.py
 tests/test_wrappers_w3.py
```

### Comparing `ensuro-2.8.2/tests/test_prototype.py` & `ensuro-2.8.2.post1/tests/test_prototype.py`

 * *Files identical despite different names*

### Comparing `ensuro-2.8.2/tox.ini` & `ensuro-2.8.2.post1/tox.ini`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Tox configuration file
 # Read more under https://tox.readthedocs.io/
 # THIS SCRIPT IS SUPPOSED TO BE AN EXAMPLE. MODIFY IT ACCORDING TO YOUR NEEDS!
 
 [tox]
 minversion = 3.15
-envlist = py37,py38,py39
+envlist = py39,py310,py311
 isolated_build = True
 
 
 [testenv]
 description = Invoke pytest to run automated tests
 setenv =
     TOXINIDIR = {toxinidir}
```

