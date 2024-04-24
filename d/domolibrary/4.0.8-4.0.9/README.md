# Comparing `tmp/domolibrary-4.0.8.tar.gz` & `tmp/domolibrary-4.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domolibrary-4.0.8.tar", last modified: Mon Mar  4 22:30:56 2024, max compression
+gzip compressed data, was "domolibrary-4.0.9.tar", last modified: Tue Mar  5 00:04:22 2024, max compression
```

## Comparing `domolibrary-4.0.8.tar` & `domolibrary-4.0.9.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.125794 domolibrary-4.0.8/
--rw-r--r--   0 root         (0) root         (0)    11337 2024-03-04 17:50:59.000000 domolibrary-4.0.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)      111 2024-03-04 17:50:59.000000 domolibrary-4.0.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    11329 2024-03-04 22:30:56.125794 domolibrary-4.0.8/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    10653 2024-03-04 17:50:59.000000 domolibrary-4.0.8/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.115794 domolibrary-4.0.8/domolibrary/
--rw-r--r--   0 root         (0) root         (0)       22 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/__init__.py
--rw-r--r--   0 root         (0) root         (0)   287320 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/_modidx.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.115794 domolibrary-4.0.8/domolibrary/classes/
--rw-r--r--   0 root         (0) root         (0)     3254 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoAccessToken.py
--rw-r--r--   0 root         (0) root         (0)    26916 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoAccount.py
--rw-r--r--   0 root         (0) root         (0)    18160 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoAccount_Config.py
--rw-r--r--   0 root         (0) root         (0)     4145 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoActivityLog.py
--rw-r--r--   0 root         (0) root         (0)     4882 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoApplication.py
--rw-r--r--   0 root         (0) root         (0)     9139 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoApplication_Job.py
--rw-r--r--   0 root         (0) root         (0)     4881 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoBootstrap.py
--rw-r--r--   0 root         (0) root         (0)     3705 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoCard.py
--rw-r--r--   0 root         (0) root         (0)      999 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoCertification.py
--rw-r--r--   0 root         (0) root         (0)     8113 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoDatacenter.py
--rw-r--r--   0 root         (0) root         (0)     5349 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoDataflow.py
--rw-r--r--   0 root         (0) root         (0)     3100 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoDataflow_Action.py
--rw-r--r--   0 root         (0) root         (0)     6112 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoDataflow_History.py
--rw-r--r--   0 root         (0) root         (0)    28304 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoDataset.py
--rw-r--r--   0 root         (0) root         (0)     1870 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoGrant.py
--rw-r--r--   0 root         (0) root         (0)    19933 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoGroup.py
--rw-r--r--   0 root         (0) root         (0)    29813 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoInstanceConfig.py
--rw-r--r--   0 root         (0) root         (0)     8907 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoInstanceConfig_UserAttribute.py
--rw-r--r--   0 root         (0) root         (0)     5290 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoJupyter.py
--rw-r--r--   0 root         (0) root         (0)     7275 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoLineage.py
--rw-r--r--   0 root         (0) root         (0)     9719 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoPDP.py
--rw-r--r--   0 root         (0) root         (0)    21078 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoPage.py
--rw-r--r--   0 root         (0) root         (0)    10818 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoPage_Content.py
--rw-r--r--   0 root         (0) root         (0)    12048 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoPublish.py
--rw-r--r--   0 root         (0) root         (0)    14313 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoRole.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoSandbox.py
--rw-r--r--   0 root         (0) root         (0)     5559 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoStream.py
--rw-r--r--   0 root         (0) root         (0)    18264 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/DomoUser.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/classes/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.115794 domolibrary-4.0.8/domolibrary/client/
--rw-r--r--   0 root         (0) root         (0)    13221 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/client/DomoAuth.py
--rw-r--r--   0 root         (0) root         (0)     2429 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/client/DomoError.py
--rw-r--r--   0 root         (0) root         (0)     7156 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/client/Logger.py
--rw-r--r--   0 root         (0) root         (0)     7328 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/client/ResponseGetData.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/client/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19253 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/client/get_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.115794 domolibrary-4.0.8/domolibrary/integrations/
--rw-r--r--   0 root         (0) root         (0)     2915 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/integrations/Automation.py
--rw-r--r--   0 root         (0) root         (0)    15378 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/integrations/DomoJupyter.py
--rw-r--r--   0 root         (0) root         (0)     1247 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/integrations/MonitDataset.py
--rw-r--r--   0 root         (0) root         (0)     3106 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/integrations/RoleHierarchy.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/integrations/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.125794 domolibrary-4.0.8/domolibrary/routes/
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5004 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/access_token.py
--rw-r--r--   0 root         (0) root         (0)    19912 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/account.py
--rw-r--r--   0 root         (0) root         (0)     2427 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/activity_log.py
--rw-r--r--   0 root         (0) root         (0)    12164 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/application.py
--rw-r--r--   0 root         (0) root         (0)     9463 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/auth.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/bootstrap.py
--rw-r--r--   0 root         (0) root         (0)     4925 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/card.py
--rw-r--r--   0 root         (0) root         (0)    10634 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/datacenter.py
--rw-r--r--   0 root         (0) root         (0)     4778 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/dataflow.py
--rw-r--r--   0 root         (0) root         (0)    23232 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/dataset.py
--rw-r--r--   0 root         (0) root         (0)     1530 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/grant.py
--rw-r--r--   0 root         (0) root         (0)    16761 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/group.py
--rw-r--r--   0 root         (0) root         (0)    18807 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/instance_config.py
--rw-r--r--   0 root         (0) root         (0)     6410 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/jupyter.py
--rw-r--r--   0 root         (0) root         (0)     8935 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/page.py
--rw-r--r--   0 root         (0) root         (0)     8981 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/pdp.py
--rw-r--r--   0 root         (0) root         (0)     6334 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/publish.py
--rw-r--r--   0 root         (0) root         (0)    12591 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/role.py
--rw-r--r--   0 root         (0) root         (0)     4255 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/sandbox.py
--rw-r--r--   0 root         (0) root         (0)     2247 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/stream.py
--rw-r--r--   0 root         (0) root         (0)    24304 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/user.py
--rw-r--r--   0 root         (0) root         (0)     9826 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/routes/user_attributes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.125794 domolibrary-4.0.8/domolibrary/utils/
--rw-r--r--   0 root         (0) root         (0)     1626 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/utils/DictDot.py
--rw-r--r--   0 root         (0) root         (0)     2444 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/utils/Image.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/utils/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1335 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/utils/chunk_execution.py
--rw-r--r--   0 root         (0) root         (0)     2820 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/utils/convert.py
--rw-r--r--   0 root         (0) root         (0)     1138 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/utils/read_creds_from_dotenv.py
--rw-r--r--   0 root         (0) root         (0)     4813 2024-03-04 22:17:07.000000 domolibrary-4.0.8/domolibrary/utils/upload_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-04 22:30:56.115794 domolibrary-4.0.8/domolibrary.egg-info/
--rw-r--r--   0 root         (0) root         (0)    11329 2024-03-04 22:30:56.000000 domolibrary-4.0.8/domolibrary.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2747 2024-03-04 22:30:56.000000 domolibrary-4.0.8/domolibrary.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 22:30:56.000000 domolibrary-4.0.8/domolibrary.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       65 2024-03-04 22:30:56.000000 domolibrary-4.0.8/domolibrary.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 18:25:12.000000 domolibrary-4.0.8/domolibrary.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      129 2024-03-04 22:30:56.000000 domolibrary-4.0.8/domolibrary.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       12 2024-03-04 22:30:56.000000 domolibrary-4.0.8/domolibrary.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     1106 2024-03-04 22:17:04.000000 domolibrary-4.0.8/settings.ini
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-04 22:30:56.125794 domolibrary-4.0.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2669 2024-03-04 17:50:59.000000 domolibrary-4.0.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.179417 domolibrary-4.0.9/
+-rw-r--r--   0 root         (0) root         (0)    11337 2024-03-04 17:50:59.000000 domolibrary-4.0.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      111 2024-03-04 17:50:59.000000 domolibrary-4.0.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    11329 2024-03-05 00:04:22.179417 domolibrary-4.0.9/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    10653 2024-03-04 17:50:59.000000 domolibrary-4.0.9/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.169417 domolibrary-4.0.9/domolibrary/
+-rw-r--r--   0 root         (0) root         (0)       22 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   287320 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/_modidx.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.169417 domolibrary-4.0.9/domolibrary/classes/
+-rw-r--r--   0 root         (0) root         (0)     3254 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoAccessToken.py
+-rw-r--r--   0 root         (0) root         (0)    26916 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoAccount.py
+-rw-r--r--   0 root         (0) root         (0)    18160 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoAccount_Config.py
+-rw-r--r--   0 root         (0) root         (0)     4145 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoActivityLog.py
+-rw-r--r--   0 root         (0) root         (0)     4882 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoApplication.py
+-rw-r--r--   0 root         (0) root         (0)     9139 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoApplication_Job.py
+-rw-r--r--   0 root         (0) root         (0)     4881 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoBootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     3705 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoCard.py
+-rw-r--r--   0 root         (0) root         (0)      999 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoCertification.py
+-rw-r--r--   0 root         (0) root         (0)     8113 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoDatacenter.py
+-rw-r--r--   0 root         (0) root         (0)     5349 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoDataflow.py
+-rw-r--r--   0 root         (0) root         (0)     3100 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoDataflow_Action.py
+-rw-r--r--   0 root         (0) root         (0)     6112 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoDataflow_History.py
+-rw-r--r--   0 root         (0) root         (0)    28304 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoDataset.py
+-rw-r--r--   0 root         (0) root         (0)     1870 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoGrant.py
+-rw-r--r--   0 root         (0) root         (0)    19933 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoGroup.py
+-rw-r--r--   0 root         (0) root         (0)    29813 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoInstanceConfig.py
+-rw-r--r--   0 root         (0) root         (0)     8907 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoInstanceConfig_UserAttribute.py
+-rw-r--r--   0 root         (0) root         (0)     5290 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoJupyter.py
+-rw-r--r--   0 root         (0) root         (0)     7275 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoLineage.py
+-rw-r--r--   0 root         (0) root         (0)     9719 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoPDP.py
+-rw-r--r--   0 root         (0) root         (0)    21078 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoPage.py
+-rw-r--r--   0 root         (0) root         (0)    10818 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoPage_Content.py
+-rw-r--r--   0 root         (0) root         (0)    12048 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoPublish.py
+-rw-r--r--   0 root         (0) root         (0)    14313 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoRole.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoSandbox.py
+-rw-r--r--   0 root         (0) root         (0)     5559 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoStream.py
+-rw-r--r--   0 root         (0) root         (0)    18264 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/classes/DomoUser.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/classes/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.169417 domolibrary-4.0.9/domolibrary/client/
+-rw-r--r--   0 root         (0) root         (0)    13221 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/client/DomoAuth.py
+-rw-r--r--   0 root         (0) root         (0)     2429 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/client/DomoError.py
+-rw-r--r--   0 root         (0) root         (0)     7156 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/client/Logger.py
+-rw-r--r--   0 root         (0) root         (0)     7328 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/client/ResponseGetData.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/client/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19253 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/client/get_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.169417 domolibrary-4.0.9/domolibrary/integrations/
+-rw-r--r--   0 root         (0) root         (0)     2915 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/integrations/Automation.py
+-rw-r--r--   0 root         (0) root         (0)    15378 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/integrations/DomoJupyter.py
+-rw-r--r--   0 root         (0) root         (0)     1247 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/integrations/MonitDataset.py
+-rw-r--r--   0 root         (0) root         (0)     3106 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/integrations/RoleHierarchy.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/integrations/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.179417 domolibrary-4.0.9/domolibrary/routes/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/routes/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5004 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/access_token.py
+-rw-r--r--   0 root         (0) root         (0)    19912 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/account.py
+-rw-r--r--   0 root         (0) root         (0)     2427 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/activity_log.py
+-rw-r--r--   0 root         (0) root         (0)    12164 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/application.py
+-rw-r--r--   0 root         (0) root         (0)     9463 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/auth.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/bootstrap.py
+-rw-r--r--   0 root         (0) root         (0)     4925 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/card.py
+-rw-r--r--   0 root         (0) root         (0)    10634 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/datacenter.py
+-rw-r--r--   0 root         (0) root         (0)     4778 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/dataflow.py
+-rw-r--r--   0 root         (0) root         (0)    23232 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/dataset.py
+-rw-r--r--   0 root         (0) root         (0)     1530 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/grant.py
+-rw-r--r--   0 root         (0) root         (0)    16761 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/group.py
+-rw-r--r--   0 root         (0) root         (0)    18807 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/instance_config.py
+-rw-r--r--   0 root         (0) root         (0)     6410 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/jupyter.py
+-rw-r--r--   0 root         (0) root         (0)     8935 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/page.py
+-rw-r--r--   0 root         (0) root         (0)     8981 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/pdp.py
+-rw-r--r--   0 root         (0) root         (0)     6334 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/publish.py
+-rw-r--r--   0 root         (0) root         (0)    12591 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/role.py
+-rw-r--r--   0 root         (0) root         (0)     4255 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/sandbox.py
+-rw-r--r--   0 root         (0) root         (0)     2247 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/stream.py
+-rw-r--r--   0 root         (0) root         (0)    24304 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/user.py
+-rw-r--r--   0 root         (0) root         (0)     9826 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/routes/user_attributes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.179417 domolibrary-4.0.9/domolibrary/utils/
+-rw-r--r--   0 root         (0) root         (0)     1626 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/utils/DictDot.py
+-rw-r--r--   0 root         (0) root         (0)     2444 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/utils/Image.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-03-05 00:01:03.000000 domolibrary-4.0.9/domolibrary/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1335 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/utils/chunk_execution.py
+-rw-r--r--   0 root         (0) root         (0)     2820 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/utils/convert.py
+-rw-r--r--   0 root         (0) root         (0)     1138 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/utils/read_creds_from_dotenv.py
+-rw-r--r--   0 root         (0) root         (0)     4813 2024-03-04 22:17:07.000000 domolibrary-4.0.9/domolibrary/utils/upload_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-05 00:04:22.169417 domolibrary-4.0.9/domolibrary.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    11329 2024-03-05 00:04:22.000000 domolibrary-4.0.9/domolibrary.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2747 2024-03-05 00:04:22.000000 domolibrary-4.0.9/domolibrary.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-05 00:04:22.000000 domolibrary-4.0.9/domolibrary.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       65 2024-03-05 00:04:22.000000 domolibrary-4.0.9/domolibrary.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-03-04 18:25:12.000000 domolibrary-4.0.9/domolibrary.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      129 2024-03-05 00:04:22.000000 domolibrary-4.0.9/domolibrary.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       12 2024-03-05 00:04:22.000000 domolibrary-4.0.9/domolibrary.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-03-05 00:01:30.000000 domolibrary-4.0.9/settings.ini
+-rw-r--r--   0 root         (0) root         (0)       38 2024-03-05 00:04:22.179417 domolibrary-4.0.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2669 2024-03-04 17:50:59.000000 domolibrary-4.0.9/setup.py
```

### Comparing `domolibrary-4.0.8/LICENSE` & `domolibrary-4.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/PKG-INFO` & `domolibrary-4.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 4.0.8
+Version: 4.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-4.0.8/README.md` & `domolibrary-4.0.9/README.md`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/_modidx.py` & `domolibrary-4.0.9/domolibrary/_modidx.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoAccessToken.py` & `domolibrary-4.0.9/domolibrary/classes/DomoAccessToken.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoAccount.py` & `domolibrary-4.0.9/domolibrary/classes/DomoAccount.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoAccount_Config.py` & `domolibrary-4.0.9/domolibrary/classes/DomoAccount_Config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoActivityLog.py` & `domolibrary-4.0.9/domolibrary/classes/DomoActivityLog.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoApplication.py` & `domolibrary-4.0.9/domolibrary/classes/DomoApplication.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoApplication_Job.py` & `domolibrary-4.0.9/domolibrary/classes/DomoApplication_Job.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoBootstrap.py` & `domolibrary-4.0.9/domolibrary/classes/DomoBootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoCard.py` & `domolibrary-4.0.9/domolibrary/classes/DomoCard.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoCertification.py` & `domolibrary-4.0.9/domolibrary/classes/DomoCertification.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoDatacenter.py` & `domolibrary-4.0.9/domolibrary/classes/DomoDatacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoDataflow.py` & `domolibrary-4.0.9/domolibrary/classes/DomoDataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoDataflow_Action.py` & `domolibrary-4.0.9/domolibrary/classes/DomoDataflow_Action.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoDataflow_History.py` & `domolibrary-4.0.9/domolibrary/classes/DomoDataflow_History.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoDataset.py` & `domolibrary-4.0.9/domolibrary/classes/DomoDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoGrant.py` & `domolibrary-4.0.9/domolibrary/classes/DomoGrant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoGroup.py` & `domolibrary-4.0.9/domolibrary/classes/DomoGroup.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoInstanceConfig.py` & `domolibrary-4.0.9/domolibrary/classes/DomoInstanceConfig.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoInstanceConfig_UserAttribute.py` & `domolibrary-4.0.9/domolibrary/classes/DomoInstanceConfig_UserAttribute.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoJupyter.py` & `domolibrary-4.0.9/domolibrary/classes/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoLineage.py` & `domolibrary-4.0.9/domolibrary/classes/DomoLineage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoPDP.py` & `domolibrary-4.0.9/domolibrary/classes/DomoPDP.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoPage.py` & `domolibrary-4.0.9/domolibrary/classes/DomoPage.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoPage_Content.py` & `domolibrary-4.0.9/domolibrary/classes/DomoPage_Content.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoPublish.py` & `domolibrary-4.0.9/domolibrary/classes/DomoPublish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoRole.py` & `domolibrary-4.0.9/domolibrary/classes/DomoRole.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoSandbox.py` & `domolibrary-4.0.9/domolibrary/classes/DomoSandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoStream.py` & `domolibrary-4.0.9/domolibrary/classes/DomoStream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/classes/DomoUser.py` & `domolibrary-4.0.9/domolibrary/classes/DomoUser.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/client/DomoAuth.py` & `domolibrary-4.0.9/domolibrary/client/DomoAuth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/client/DomoError.py` & `domolibrary-4.0.9/domolibrary/client/DomoError.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/client/Logger.py` & `domolibrary-4.0.9/domolibrary/client/Logger.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/client/ResponseGetData.py` & `domolibrary-4.0.9/domolibrary/client/ResponseGetData.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/client/get_data.py` & `domolibrary-4.0.9/domolibrary/client/get_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/integrations/Automation.py` & `domolibrary-4.0.9/domolibrary/integrations/Automation.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/integrations/DomoJupyter.py` & `domolibrary-4.0.9/domolibrary/integrations/DomoJupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/integrations/MonitDataset.py` & `domolibrary-4.0.9/domolibrary/integrations/MonitDataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/integrations/RoleHierarchy.py` & `domolibrary-4.0.9/domolibrary/integrations/RoleHierarchy.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/access_token.py` & `domolibrary-4.0.9/domolibrary/routes/access_token.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/account.py` & `domolibrary-4.0.9/domolibrary/routes/account.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/activity_log.py` & `domolibrary-4.0.9/domolibrary/routes/activity_log.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/application.py` & `domolibrary-4.0.9/domolibrary/routes/application.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/auth.py` & `domolibrary-4.0.9/domolibrary/routes/auth.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/bootstrap.py` & `domolibrary-4.0.9/domolibrary/routes/bootstrap.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/card.py` & `domolibrary-4.0.9/domolibrary/routes/card.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/datacenter.py` & `domolibrary-4.0.9/domolibrary/routes/datacenter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/dataflow.py` & `domolibrary-4.0.9/domolibrary/routes/dataflow.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/dataset.py` & `domolibrary-4.0.9/domolibrary/routes/dataset.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/grant.py` & `domolibrary-4.0.9/domolibrary/routes/grant.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/group.py` & `domolibrary-4.0.9/domolibrary/routes/group.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/instance_config.py` & `domolibrary-4.0.9/domolibrary/routes/instance_config.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/jupyter.py` & `domolibrary-4.0.9/domolibrary/routes/jupyter.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/page.py` & `domolibrary-4.0.9/domolibrary/routes/page.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/pdp.py` & `domolibrary-4.0.9/domolibrary/routes/pdp.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/publish.py` & `domolibrary-4.0.9/domolibrary/routes/publish.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/role.py` & `domolibrary-4.0.9/domolibrary/routes/role.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/sandbox.py` & `domolibrary-4.0.9/domolibrary/routes/sandbox.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/stream.py` & `domolibrary-4.0.9/domolibrary/routes/stream.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/user.py` & `domolibrary-4.0.9/domolibrary/routes/user.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/routes/user_attributes.py` & `domolibrary-4.0.9/domolibrary/routes/user_attributes.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/utils/DictDot.py` & `domolibrary-4.0.9/domolibrary/utils/DictDot.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/utils/Image.py` & `domolibrary-4.0.9/domolibrary/utils/Image.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/utils/chunk_execution.py` & `domolibrary-4.0.9/domolibrary/utils/chunk_execution.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/utils/convert.py` & `domolibrary-4.0.9/domolibrary/utils/convert.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/utils/read_creds_from_dotenv.py` & `domolibrary-4.0.9/domolibrary/utils/read_creds_from_dotenv.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary/utils/upload_data.py` & `domolibrary-4.0.9/domolibrary/utils/upload_data.py`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/domolibrary.egg-info/PKG-INFO` & `domolibrary-4.0.9/domolibrary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: domolibrary
-Version: 4.0.8
+Version: 4.0.9
 Summary: UNKNOWN
 Home-page: https://github.com/jaewilson07/domo_library
 Author: Jae Wilson
 Author-email: jaewilson07@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Platform: UNKNOWN
```

### Comparing `domolibrary-4.0.8/domolibrary.egg-info/SOURCES.txt` & `domolibrary-4.0.9/domolibrary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `domolibrary-4.0.8/settings.ini` & `domolibrary-4.0.9/settings.ini`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = domo_library
 lib_name = domolibrary
-version = 4.0.8
+version = 4.0.9
 min_python = 3.9
 license = apache2
 
 ### nbdev ###
 doc_path = _docs
 lib_path = domolibrary
 nbs_path = nbs
```

### Comparing `domolibrary-4.0.8/setup.py` & `domolibrary-4.0.9/setup.py`

 * *Files identical despite different names*

