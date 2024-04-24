# Comparing `tmp/gimme_aws_creds-2.8.1.tar.gz` & `tmp/gimme_aws_creds-2.8.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gimme_aws_creds-2.8.1.tar", last modified: Tue Apr 23 14:09:04 2024, max compression
+gzip compressed data, was "gimme_aws_creds-2.8.1.1.tar", last modified: Wed Apr 24 18:36:57 2024, max compression
```

## Comparing `gimme_aws_creds-2.8.1.tar` & `gimme_aws_creds-2.8.1.1.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/LONG_DESCRIPTION.md
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/NOTICE
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.253857 gimme_aws_creds-2.8.1/bin/
--rwxr-xr-x   0 runner    (1001) docker     (127)      753 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/bin/gimme-aws-creds
--rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/bin/gimme-aws-creds-autocomplete.sh
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/bin/gimme-aws-creds.cmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/gimme_aws_creds/
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/aws.py
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    31632 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/default.py
--rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/duo.py
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/duo_universal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    38953 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    50285 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/okta_classic.py
--rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/okta_identity_engine.py
--rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/registered_authenticators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/u2f.py
--rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/ui.py
--rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/gimme_aws_creds/webauthn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-23 14:09:04.000000 gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      889 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 14:09:04.257857 gimme_aws_creds-2.8.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_aws_resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_duo_universal_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_main.py
--rw-r--r--   0 runner    (1001) docker     (127)    61157 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_okta_classic_client.py
--rw-r--r--   0 runner    (1001) docker     (127)    70663 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_okta_identity_engine_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-23 14:08:38.000000 gimme_aws_creds-2.8.1/tests/test_registered_authenticators.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11340 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/LONG_DESCRIPTION.md
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    11040 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/NOTICE
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    20414 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.716482 gimme_aws_creds-2.8.1.1/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      753 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds
+-rw-r--r--   0 runner    (1001) docker     (127)     1827 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds-autocomplete.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds.cmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.720482 gimme_aws_creds-2.8.1.1/gimme_aws_creds/
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/aws.py
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31632 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2606 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/default.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9455 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo_universal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38953 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50285 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_classic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9371 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_identity_engine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3036 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/registered_authenticators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/u2f.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3429 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/ui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6444 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds/webauthn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1025 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 18:36:57.000000 gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       99 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 18:36:57.724482 gimme_aws_creds-2.8.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    14358 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_aws_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4573 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15786 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_duo_universal_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14269 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61157 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_okta_classic_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    70663 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_okta_identity_engine_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-04-24 18:36:47.000000 gimme_aws_creds-2.8.1.1/tests/test_registered_authenticators.py
```

### Comparing `gimme_aws_creds-2.8.1/LICENSE` & `gimme_aws_creds-2.8.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/LONG_DESCRIPTION.md` & `gimme_aws_creds-2.8.1.1/LONG_DESCRIPTION.md`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/NOTICE` & `gimme_aws_creds-2.8.1.1/NOTICE`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/PKG-INFO` & `gimme_aws_creds-2.8.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme_aws_creds
-Version: 2.8.1
+Version: 2.8.1.1
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme_aws_creds-2.8.1/README.md` & `gimme_aws_creds-2.8.1.1/README.md`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/bin/gimme-aws-creds` & `gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/bin/gimme-aws-creds-autocomplete.sh` & `gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds-autocomplete.sh`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/bin/gimme-aws-creds.cmd` & `gimme_aws_creds-2.8.1.1/bin/gimme-aws-creds.cmd`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/aws.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/aws.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/common.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/common.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/config.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/config.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/default.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/default.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/duo.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/duo_universal.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/duo_universal.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/errors.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/errors.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/main.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/main.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/okta_classic.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_classic.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/okta_identity_engine.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/okta_identity_engine.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/registered_authenticators.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/registered_authenticators.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/u2f.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/u2f.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/ui.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/ui.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds/webauthn.py` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds/webauthn.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/PKG-INFO` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gimme_aws_creds
-Version: 2.8.1
+Version: 2.8.1.1
 Summary: A CLI to get temporary AWS credentials from Okta
 Home-page: https://github.com/Nike-Inc/gimme-aws-creds
 Author: Eric Pierce
 Author-email: eric.pierce@nike.com
 License: Apache License, v2.0
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3 :: Only
```

### Comparing `gimme_aws_creds-2.8.1/gimme_aws_creds.egg-info/SOURCES.txt` & `gimme_aws_creds-2.8.1.1/gimme_aws_creds.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/setup.py` & `gimme_aws_creds-2.8.1.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('requirements.txt') as f:
     requirements = f.read().splitlines()
 
 setup(
     name='gimme_aws_creds',
-    version='2.8.1',
+    version='2.8.1.1',
     install_requires=requirements,
     author='Eric Pierce',
     author_email='eric.pierce@nike.com',
     description="A CLI to get temporary AWS credentials from Okta",
     url='https://github.com/Nike-Inc/gimme-aws-creds',
     long_description=open("LONG_DESCRIPTION.md").read(),
     python_requires=">=3.7",
```

### Comparing `gimme_aws_creds-2.8.1/tests/test_aws_resolver.py` & `gimme_aws_creds-2.8.1.1/tests/test_aws_resolver.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/tests/test_config.py` & `gimme_aws_creds-2.8.1.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/tests/test_duo_universal_client.py` & `gimme_aws_creds-2.8.1.1/tests/test_duo_universal_client.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/tests/test_main.py` & `gimme_aws_creds-2.8.1.1/tests/test_main.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/tests/test_okta_classic_client.py` & `gimme_aws_creds-2.8.1.1/tests/test_okta_classic_client.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/tests/test_okta_identity_engine_client.py` & `gimme_aws_creds-2.8.1.1/tests/test_okta_identity_engine_client.py`

 * *Files identical despite different names*

### Comparing `gimme_aws_creds-2.8.1/tests/test_registered_authenticators.py` & `gimme_aws_creds-2.8.1.1/tests/test_registered_authenticators.py`

 * *Files identical despite different names*

