# Comparing `tmp/Leonardo-Ai-SDK-5.3.5.tar.gz` & `tmp/Leonardo-Ai-SDK-5.3.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Leonardo-Ai-SDK-5.3.5.tar", last modified: Thu Apr 11 05:38:45 2024, max compression
+gzip compressed data, was "Leonardo-Ai-SDK-5.3.6.tar", last modified: Wed Apr 24 00:02:32 2024, max compression
```

## Comparing `Leonardo-Ai-SDK-5.3.5.tar` & `Leonardo-Ai-SDK-5.3.6.tar`

### file list

```diff
@@ -1,91 +1,91 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.545252 Leonardo-Ai-SDK-5.3.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (127)     9808 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 05:38:45.545252 Leonardo-Ai-SDK-5.3.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.529252 Leonardo-Ai-SDK-5.3.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 05:38:45.000000 Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/
--rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/sdkhooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/element.py
--rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/generation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/initimage.py
--rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.533252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/sdkerror.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createdataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    15019 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/creategeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createlcmgeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createtexturegeneration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationnobg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationunzoom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationupscale.py
--rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletedatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletemodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getdatasetbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14923 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)    15135 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getinitimagebyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getmodelbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getuserself.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getvariationbyid.py
--rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listelements.py
--rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listplatformmodels.py
--rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinpaintinglcm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinstantrefine.py
--rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptimprove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadinitimage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadmodelasset.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/controlnet_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/custom_model_type.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/element_input.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/job_status.py
--rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/lcm_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/model_asset_texture_types.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
--rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_generation_style.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/security.py
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/strength.py
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/variation_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/prompt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdk.py
--rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdkconfiguration.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 05:38:45.541252 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/retries.py
--rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-04-11 05:38:35.000000 Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/variation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9808 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1722 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.608148 Leonardo-Ai-SDK-5.3.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15589 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3766 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 00:02:32.000000 Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/
+-rw-r--r--   0 runner    (1001) docker     (127)      127 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2393 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/sdkhooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2468 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17316 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3437 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/element.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44786 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10020 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/initimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27064 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.612148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/sdkerror.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)     6405 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2240 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createdataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15044 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/creategeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4985 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createlcmgeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4542 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3490 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createtexturegeneration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationnobg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationunzoom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2227 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationupscale.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/delete3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletedatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1921 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deleteinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1892 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletemodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3856 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3749 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3558 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getdatasetbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14970 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15182 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getinitimagebyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4534 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getmodelbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5575 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4494 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getuserself.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getvariationbyid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3673 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listelements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3227 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listplatformmodels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6225 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5376 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinpaintinglcm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5063 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinstantrefine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2116 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptimprove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2968 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2530 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadinitimage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadmodelasset.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/controlnet_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/custom_model_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/element_input.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/job_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)      616 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/lcm_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/model_asset_texture_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_generation_schedulers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1316 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_generation_style.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      330 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/security.py
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/strength.py
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/variation_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6779 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/prompt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdk.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1394 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdkconfiguration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 00:02:32.620148 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3732 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/retries.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32089 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13748 2024-04-24 00:02:19.000000 Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/variation.py
```

### Comparing `Leonardo-Ai-SDK-5.3.5/LICENSE.md` & `Leonardo-Ai-SDK-5.3.6/LICENSE.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/PKG-INFO` & `Leonardo-Ai-SDK-5.3.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.5
+Version: 5.3.6
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.5 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.6 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
```

### Comparing `Leonardo-Ai-SDK-5.3.5/README.md` & `Leonardo-Ai-SDK-5.3.6/README.md`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/setup.py` & `Leonardo-Ai-SDK-5.3.6/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
             long_description,
         )
 except FileNotFoundError:
     long_description = ''
 
 setuptools.setup(
     name='Leonardo-Ai-SDK',
-    version='5.3.5',
+    version='5.3.6',
     author='Leonardo-Ai',
     description='Leonardo AI Python Client SDK',
     url='https://github.com/Leonardo-Interactive/leonardo-python-sdk.git',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=setuptools.find_packages(where='src'),
     install_requires=[
```

### Comparing `Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/PKG-INFO` & `Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Leonardo-Ai-SDK
-Version: 5.3.5
+Version: 5.3.6
 Summary: Leonardo AI Python Client SDK
 Home-page: https://github.com/Leonardo-Interactive/leonardo-python-sdk.git
 Author: Leonardo-Ai
 License: UNKNOWN
 Description: # Leonardo-Ai-SDK
         
         <a href="https://codespaces.new/Leonardo-Interactive/leonardo-python-sdk.git/tree/main"><img src="https://github.com/codespaces/badge.svg" /></a>
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.5 Summary: Leonardo AI
+Metadata-Version: 2.1 Name: Leonardo-Ai-SDK Version: 5.3.6 Summary: Leonardo AI
 Python Client SDK Home-page: https://github.com/Leonardo-Interactive/leonardo-
 python-sdk.git Author: Leonardo-Ai License: UNKNOWN Description: # Leonardo-Ai-
 SDK _[_h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_c_o_d_e_s_p_a_c_e_s_/_b_a_d_g_e_._s_v_g_]## SDK Installation ```bash pip
 install Leonardo-Ai-SDK ``` ## SDK Example Usage ### Example ```python import
 leonardoaisdk from leonardoaisdk.models import operations s =
 leonardoaisdk.LeonardoAiSDK( bearer_auth="", ) req =
 operations.CreateDatasetRequestBody( name='', ) res = s.dataset.create_dataset
```

### Comparing `Leonardo-Ai-SDK-5.3.5/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt` & `Leonardo-Ai-SDK-5.3.6/src/Leonardo_Ai_SDK.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/sdkhooks.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/sdkhooks.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/_hooks/types.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/_hooks/types.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/dataset.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/dataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/element.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/element.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/generation.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/generation.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/initimage.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/initimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/model.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/model.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/errors/sdkerror.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/errors/sdkerror.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/__init__.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createdataset.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createdataset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/creategeneration.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/creategeneration.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,60 +20,60 @@
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
 class CreateGenerationRequestBody:
     r"""Query parameters to be provided in the request body as a JSON object"""
     UNSET='__SPEAKEASY_UNSET__'
-    alchemy: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alchemy'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
+    alchemy: Optional[bool] = dataclasses.field(default=True, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('alchemy'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use Alchemy. Note: The appropriate Alchemy version is selected for the specified model. For example, XL models will use Alchemy V2."""
     contrast_ratio: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('contrastRatio'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Contrast Ratio to use with Alchemy. Must be a float between 0 and 1 inclusive."""
     control_net: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('controlNet'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use ControlNet. Requires an init image to be provided. Requires a model based on SD v1.5"""
     control_net_type: Optional[shared_controlnet_type.ControlnetType] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('controlNetType'), 'exclude': lambda f: f is None }})
     r"""The type of ControlNet to use."""
     elements: Optional[List[shared_element_input.ElementInput]] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('elements'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     expanded_domain: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('expandedDomain'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use the Expanded Domain feature of Alchemy."""
     fantasy_avatar: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('fantasyAvatar'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use the Fantasy Avatar feature."""
     guidance_scale: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('guidance_scale'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How strongly the generation should reflect the prompt. 7 is recommended. Must be between 1 and 20."""
-    height: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
+    height: Optional[int] = dataclasses.field(default=768, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('height'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The input height of the images. Must be between 32 and 1024 and be a multiple of 8. Note: Input resolution is not always the same as output resolution due to upscaling from other features."""
     high_contrast: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highContrast'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use the High Contrast feature of Prompt Magic. Note: Controls RAW mode. Set to false to enable RAW mode."""
     high_resolution: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('highResolution'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use the High Resolution feature of Prompt Magic."""
     image_prompt_weight: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('imagePromptWeight'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     image_prompts: Optional[List[str]] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('imagePrompts'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     init_generation_image_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('init_generation_image_id'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The ID of an existing image to use in image2image."""
     init_image_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('init_image_id'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The ID of an Init Image to use in image2image."""
     init_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('init_strength'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How strongly the generated images should reflect the original image in image2image. Must be a float between 0.1 and 0.9."""
-    model_id: Optional[str] = dataclasses.field(default='6bef9f1b-29cb-40c7-b9df-32b51c1f67d3', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
+    model_id: Optional[str] = dataclasses.field(default='b24e16ff-06e3-43eb-8d33-4416c2d75876', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The model ID used for image generation. If not provided, uses sd_version to determine the version of Stable Diffusion to use. In-app, model IDs are under the Finetune Models menu. Click on the platform model or your custom model, then click View More. For platform models, you can also use the List Platform Models API."""
     negative_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negative_prompt'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The negative prompt used for the image generation"""
-    num_images: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_images'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
+    num_images: Optional[int] = dataclasses.field(default=4, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_images'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The number of images to generate. Must be between 1 and 8. If either width or height is over 768, must be between 1 and 4."""
     num_inference_steps: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('num_inference_steps'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The number of inference steps to use for the generation. Must be between 30 and 60."""
     photo_real: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoReal'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable the photoReal feature. Requires enabling alchemy and unspecifying modelId (for photoRealVersion V1)."""
     photo_real_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealStrength'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Depth of field of photoReal. Must be 0.55 for low, 0.5 for medium, or 0.45 for high. Defaults to 0.55 if not specified."""
     photo_real_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealVersion'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The version of photoReal to use. Must be v1 or v2."""
-    preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
+    preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=shared_sd_generation_style.SdGenerationStyle.DYNAMIC, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
-    prompt: Optional[str] = dataclasses.field(default='An oil painting of a cat', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt'), 'exclude': lambda f: f is None }})
+    prompt: Optional[str] = dataclasses.field(default='A majestic cat in the snow', metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt'), 'exclude': lambda f: f is None }})
     r"""The prompt used to generate images"""
     prompt_magic: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagic'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Enable to use Prompt Magic."""
     prompt_magic_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicStrength'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Strength of prompt magic. Must be a float between 0.1 and 1.0"""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Prompt magic version v2 or v3, for use when promptMagic: true"""
@@ -82,25 +82,25 @@
     scheduler: Optional[shared_sd_generation_schedulers.SdGenerationSchedulers] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('scheduler'), 'exclude': lambda f: f is None }})
     r"""The scheduler to generate images with. Defaults to EULER_DISCRETE if not specified."""
     sd_version: Optional[shared_sd_versions.SdVersions] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('sd_version'), 'exclude': lambda f: f is None }})
     r"""The base version of stable diffusion to use if not using a custom model. v1_5 is 1.5, v2 is 2.1, if not specified it will default to v1_5. Also includes SDXL and SDXL Lightning models"""
     seed: Optional[int] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('seed'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     tiling: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('tiling'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Whether the generated images should tile on all axis."""
-    transparency: Optional[TransparencyType] = dataclasses.field(default=TransparencyType.DISABLED, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transparency'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
+    transparency: Optional[TransparencyType] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('transparency'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Which type of transparency this image should use"""
     unzoom: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unzoom'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""Whether the generated images should be unzoomed (requires unzoomAmount and init_image_id to be set)."""
     unzoom_amount: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('unzoomAmount'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How much the image should be unzoomed (requires an init_image_id and unzoom to be set to true)."""
     upscale_ratio: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('upscaleRatio'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How much the image should be upscaled. (Enterprise Only)"""
     weighting: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('weighting'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""How much weighting to use for generation."""
-    width: Optional[int] = dataclasses.field(default=512, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
+    width: Optional[int] = dataclasses.field(default=1024, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('width'), 'exclude': lambda f: f is CreateGenerationRequestBody.UNSET }})
     r"""The input width of the images. Must be between 32 and 1024 and be a multiple of 8. Note: Input resolution is not always the same as output resolution due to upscaling from other features."""
     
 
 
 
 @dataclass_json(undefined=Undefined.EXCLUDE)
 @dataclasses.dataclass
```

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createlcmgeneration.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createlcmgeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createmodel.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createmodel.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createsvdmotiongeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createtexturegeneration.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createtexturegeneration.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationnobg.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationnobg.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationunzoom.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationunzoom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/createvariationupscale.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/createvariationupscale.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/delete3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/delete3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletedatasetbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletedatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deleteinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deleteinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletemodelbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletemodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/deletetexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/get3dmodelsbyuserid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getdatasetbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getdatasetbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationbyid.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
     init_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('initStrength'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     model_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     negative_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negativePrompt'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     photo_real: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoReal'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""If photoReal feature was used."""
     photo_real_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealStrength'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""Depth of field of photoReal used. 0.55 is low, 0.5 is medium, and 0.45 is high. Default is 0.55."""
-    preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
+    preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=shared_sd_generation_style.SdGenerationStyle.DYNAMIC, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
     prompt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt'), 'exclude': lambda f: f is None }})
     prompt_magic: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagic'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""If prompt magic was used."""
     prompt_magic_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicStrength'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
     r"""Strength of prompt magic used."""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is GetGenerationByIDGenerations.UNSET }})
```

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getgenerationsbyuserid.py`

 * *Files 0% similar despite different names*

```diff
@@ -115,15 +115,15 @@
     init_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('initStrength'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     model_id: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('modelId'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     negative_prompt: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('negativePrompt'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     photo_real: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoReal'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""If photoReal feature was used."""
     photo_real_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('photoRealStrength'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""Depth of field of photoReal used. 0.55 is low, 0.5 is medium, and 0.45 is high. Default is 0.55."""
-    preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
+    preset_style: Optional[shared_sd_generation_style.SdGenerationStyle] = dataclasses.field(default=shared_sd_generation_style.SdGenerationStyle.DYNAMIC, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('presetStyle'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""The style to generate images with. When photoReal is enabled, refer to the Guide section for a full list. When alchemy is disabled, use LEONARDO or NONE. When alchemy is enabled, use ANIME, CREATIVE, DYNAMIC, ENVIRONMENT, GENERAL, ILLUSTRATION, PHOTOGRAPHY, RAYTRACED, RENDER_3D, SKETCH_BW, SKETCH_COLOR, or NONE."""
     prompt: Optional[str] = dataclasses.field(default=None, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('prompt'), 'exclude': lambda f: f is None }})
     prompt_magic: Optional[bool] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagic'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""If prompt magic was used."""
     prompt_magic_strength: Optional[float] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicStrength'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
     r"""Strength of prompt magic used."""
     prompt_magic_version: Optional[str] = dataclasses.field(default=UNSET, metadata={'dataclasses_json': { 'letter_case': utils.get_field_name('promptMagicVersion'), 'exclude': lambda f: f is GetGenerationsByUserIDGenerations.UNSET }})
```

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getinitimagebyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getinitimagebyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getmodelbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getmodelbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/gettexturegenerationsbymodelid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getuserself.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getuserself.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/getvariationbyid.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/getvariationbyid.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listelements.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listelements.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/listplatformmodels.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/listplatformmodels.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performalchemyupscalelcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinpaintinglcm.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinpaintinglcm.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/performinstantrefine.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/performinstantrefine.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptimprove.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptimprove.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/promptrandom.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/promptrandom.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimage.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploaddatasetimagefromgen.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadinitimage.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadinitimage.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/operations/uploadmodelasset.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/operations/uploadmodelasset.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/__init__.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/__init__.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/custom_model_type.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/custom_model_type.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/element_input.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/element_input.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/lcm_generation_style.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/lcm_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_generation_style.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_generation_style.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/models/shared/sd_versions.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/models/shared/sd_versions.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/prompt.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/prompt.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdk.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdk.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/sdkconfiguration.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/sdkconfiguration.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,17 +20,17 @@
 class SDKConfiguration:
     client: requests_http.Session
     security: Union[shared.Security,Callable[[], shared.Security]] = None
     server_url: Optional[str] = ''
     server_idx: Optional[int] = 0
     language: str = 'python'
     openapi_doc_version: str = 'v1.0.0'
-    sdk_version: str = '5.3.5'
-    gen_version: str = '2.302.1'
-    user_agent: str = 'speakeasy-sdk/python 5.3.5 2.302.1 v1.0.0 Leonardo-Ai-SDK'
+    sdk_version: str = '5.3.6'
+    gen_version: str = '2.312.0'
+    user_agent: str = 'speakeasy-sdk/python 5.3.6 2.312.0 v1.0.0 Leonardo-Ai-SDK'
     retry_config: Optional[RetryConfig] = None
 
     def __post_init__(self):
         self._hooks = SDKHooks()
 
     def get_server_details(self) -> Tuple[str, Dict[str, str]]:
         if self.server_url is not None and self.server_url != '':
```

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/user.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/user.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/retries.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/retries.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/utils/utils.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/utils/utils.py`

 * *Files identical despite different names*

### Comparing `Leonardo-Ai-SDK-5.3.5/src/leonardoaisdk/variation.py` & `Leonardo-Ai-SDK-5.3.6/src/leonardoaisdk/variation.py`

 * *Files identical despite different names*

