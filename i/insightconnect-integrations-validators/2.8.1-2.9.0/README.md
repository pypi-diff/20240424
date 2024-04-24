# Comparing `tmp/insightconnect_integrations_validators-2.8.1.tar.gz` & `tmp/insightconnect_integrations_validators-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/insightconnect_integrations_validators-2.8.1.tar", last modified: Tue Jan 21 19:13:09 2020, max compression
+gzip compressed data, was "dist/insightconnect_integrations_validators-2.9.0.tar", last modified: Wed Jan 22 22:15:14 2020, max compression
```

## Comparing `insightconnect_integrations_validators-2.8.1.tar` & `insightconnect_integrations_validators-2.9.0.tar`

### file list

```diff
@@ -1,52 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-21 19:13:09.041877 insightconnect_integrations_validators-2.8.1/
--rw-r--r--   0 runner    (1001) docker     (115)     5345 2020-01-21 19:13:09.041877 insightconnect_integrations_validators-2.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     3876 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-21 19:13:09.033877 insightconnect_integrations_validators-2.8.1/icon_validator/
--rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     2057 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-21 19:13:09.037877 insightconnect_integrations_validators-2.8.1/icon_validator/rules/
--rw-r--r--   0 runner    (1001) docker     (115)     2193 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (115)     3978 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/acronym_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     2438 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/changelog_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     2625 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/confidential_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1651 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/credentials_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1550 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/default_value_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     2650 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/description_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1674 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/docker_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1836 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/dockerfile_parent_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     2201 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/exception_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1541 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/files_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     6410 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/help_input_output_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     4877 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/help_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     2380 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/icon_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)      790 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/json_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1651 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/logging_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1924 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/output_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)      652 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/password_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1363 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/print_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1462 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/profanity_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)    11141 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/regeneration_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     3933 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/required_keys_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1665 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/required_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     4561 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/spec_properties_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)      306 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/spec_version_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)      654 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/tag_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     3645 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/title_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     4228 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/url_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1301 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/use_case_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)      298 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1669 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/vendor_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     1563 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/version_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)     2033 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/rules/workflow_help_validator.py
--rw-r--r--   0 runner    (1001) docker     (115)      159 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/styling.py
--rw-r--r--   0 runner    (1001) docker     (115)      398 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/timing.py
--rw-r--r--   0 runner    (1001) docker     (115)     1637 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/icon_validator/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-21 19:13:09.037877 insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/
--rw-r--r--   0 runner    (1001) docker     (115)     5345 2020-01-21 19:13:08.000000 insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (115)     1945 2020-01-21 19:13:08.000000 insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-21 19:13:08.000000 insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (115)       64 2020-01-21 19:13:08.000000 insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (115)      206 2020-01-21 19:13:08.000000 insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (115)       15 2020-01-21 19:13:08.000000 insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (115)       38 2020-01-21 19:13:09.041877 insightconnect_integrations_validators-2.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (115)     1395 2020-01-21 19:13:01.000000 insightconnect_integrations_validators-2.8.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:14.866662 insightconnect_integrations_validators-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (115)     5506 2020-01-22 22:15:14.866662 insightconnect_integrations_validators-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     4029 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:14.842662 insightconnect_integrations_validators-2.9.0/icon_validator/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2057 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (115)      175 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:14.846662 insightconnect_integrations_validators-2.9.0/icon_validator/rules/
+-rw-r--r--   0 runner    (1001) docker     (115)     4264 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:14.858662 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3998 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/acronym_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2462 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/changelog_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2645 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/confidential_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1672 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/credentials_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1568 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/default_value_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2643 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/description_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1694 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/docker_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1856 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/dockerfile_parent_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2221 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/exception_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1561 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/files_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     6432 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/help_input_output_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4897 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/help_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2398 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/icon_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      810 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/json_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1674 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/logging_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1944 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/output_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      672 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/password_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1386 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/print_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1484 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/profanity_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)    11178 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/regeneration_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3953 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/required_keys_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1648 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/required_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4581 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/spec_properties_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      327 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/spec_version_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1606 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/support_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      678 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/tag_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     3629 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/title_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     4248 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/url_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1323 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/use_case_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1574 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/vendor_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1512 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/version_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      298 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:14.862662 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/
+-rw-r--r--   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2600 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_change_log_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      745 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_extension_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      690 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_files_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     2243 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_help_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1578 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_profanity_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1770 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_support_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1738 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_vendor_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1646 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_version_validator.py
+-rw-r--r--   0 runner    (1001) docker     (115)      159 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/styling.py
+-rw-r--r--   0 runner    (1001) docker     (115)      398 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/timing.py
+-rw-r--r--   0 runner    (1001) docker     (115)     1921 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/icon_validator/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (115)        0 2020-01-22 22:15:14.866662 insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (115)     5506 2020-01-22 22:15:14.000000 insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (115)     3199 2020-01-22 22:15:14.000000 insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (115)        1 2020-01-22 22:15:14.000000 insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       64 2020-01-22 22:15:14.000000 insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (115)      206 2020-01-22 22:15:14.000000 insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       15 2020-01-22 22:15:14.000000 insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (115)       38 2020-01-22 22:15:14.866662 insightconnect_integrations_validators-2.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (115)     1395 2020-01-22 22:15:04.000000 insightconnect_integrations_validators-2.9.0/setup.py
```

### Comparing `insightconnect_integrations_validators-2.8.1/PKG-INFO` & `insightconnect_integrations_validators-2.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect_integrations_validators
-Version: 2.8.1
+Version: 2.9.0
 Summary: Validator tooling for InsightConnect integrations
 Home-page: https://github.com/rapid7/icon-integrations-validators
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Description: 
         # InsightConnect Integrations Validators
@@ -53,14 +53,15 @@
         validate("/path/to/plugin/directory", run_all=True)
         ```
         
         to simulate the `--all` flag.
         
         ## Changelog
         
+        * 2.9.0 - Add unit testing support. Add support, workflow files, workflow vendor, workflow version, workflow changelog and workflow extension validators
         * 2.8.1 - Bug fix for URLValidator when opening files
         * 2.8.0 - Update ChangelogValidator to validate plugin's version history with latest version number |
         Update HelpInputOutputValidator error messaging
         * 2.7.0 - Add URL Validator
         * 2.6.9 - Update HelpInputOutputValidator to fix error messaging |
         Fix issue with HelpInputOutputValidator when help.md has action and trigger with same name
         * 2.6.8 - Docker Validator to run with -a command line argument | Helpful message on failure
```

### Comparing `insightconnect_integrations_validators-2.8.1/README.md` & `insightconnect_integrations_validators-2.9.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -45,14 +45,15 @@
 validate("/path/to/plugin/directory", run_all=True)
 ```
 
 to simulate the `--all` flag.
 
 ## Changelog
 
+* 2.9.0 - Add unit testing support. Add support, workflow files, workflow vendor, workflow version, workflow changelog and workflow extension validators
 * 2.8.1 - Bug fix for URLValidator when opening files
 * 2.8.0 - Update ChangelogValidator to validate plugin's version history with latest version number |
 Update HelpInputOutputValidator error messaging
 * 2.7.0 - Add URL Validator
 * 2.6.9 - Update HelpInputOutputValidator to fix error messaging |
 Fix issue with HelpInputOutputValidator when help.md has action and trigger with same name
 * 2.6.8 - Docker Validator to run with -a command line argument | Helpful message on failure
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/__main__.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -5,29 +5,29 @@
 from pkg_resources import get_distribution
 
 from .styling import *
 from .validate import validate
 
 
 def main():
-    version_string = (f"{BULLET_OK} " + str(get_distribution('insightconnect-integrations-validators')))
-    if '--version' in sys.argv:
+    version_string = (f"{BULLET_OK} " + str(get_distribution("insightconnect-integrations-validators")))
+    if "--version" in sys.argv:
         print(version_string)
         sys.exit(0)
 
     arguments_parser = argparse.ArgumentParser(epilog=version_string,
-                                               description='Linting rules for plugins and workflows')
+                                               description="Linting rules for plugins and workflows")
     # required
-    arguments_parser.add_argument('path', help='Path to find the plugin or workflow code', default='.')
+    arguments_parser.add_argument("path", help="Path to find the plugin or workflow code", default=".")
 
     # optional
-    arguments_parser.add_argument('--all', help='Run all Validators', default=False,
-                                  dest='run_all_validators', action='store_true')
-    arguments_parser.add_argument('-a', help='Run all validators', default=False,
-                                  dest='run_all_validators', action='store_true')
+    arguments_parser.add_argument("--all", help="Run all Validators", default=False,
+                                  dest="run_all_validators", action="store_true")
+    arguments_parser.add_argument("-a", help="Run all validators", default=False,
+                                  dest="run_all_validators", action="store_true")
 
     the_arguments = arguments_parser.parse_args()
 
     # this is a required field, and argparse enforces it, so we are 100% sure this key exists:
     path = the_arguments.path
 
     if os.path.exists(path + "/workflow.spec.yaml"):
@@ -38,19 +38,19 @@
     else:
         spec_file_name = "plugin.spec.yaml"
 
     if not os.path.exists(path):
         sys.stderr.write(f"{BULLET_FAIL} Path '{path}' does not exist\n")
         sys.exit(1)
 
-    extension = spec_file_name.split('.')[0]
+    extension = spec_file_name.split(".")[0]
 
     if extension == "plugin" and the_arguments.run_all_validators:
         print(f"{BULLET_OK} Validating {extension} with all validators at {path}\n")
         validate(directory=path, run_all=True)
     else:
         print(f"{BULLET_OK} Validating {extension} at {path}\n")
         validate(directory=path, spec_file_name=spec_file_name)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     main()
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/acronym_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/acronym_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class AcronymValidator(KomandPluginValidator):
     acronyms = [
         'ACL', 'API', 'AMI', 'ANC', 'ANS', 'ARN', 'ASCII', 'ASN', 'AV', 'AWS',
         'BCC', 'BGP', 'BIOS',
         'CC', 'CEF', 'CI', 'CIDR', 'CIF', 'CLI', 'CNAME', 'CORS', 'CPU', 'CRLF', 'CRM', 'CSV', 'CVE', 'CVSS',
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/changelog_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/changelog_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,65 +1,65 @@
 import re
 from distutils.version import LooseVersion
 
 from icon_validator.styling import *
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class ChangelogValidator(KomandPluginValidator):
 
     @staticmethod
     def get_versions(help_content):
-        raw_versions = re.findall(r'Version History\n\n.*?\n\n', help_content, re.DOTALL)
+        raw_versions = re.findall(r"Version History\n\n.*?\n\n", help_content, re.DOTALL)
         if not raw_versions:
-            raise Exception("Incorrect Version History in help.md")
+            raise Exception("Incorrect Version History in help.md.")
 
-        versions_history = raw_versions[0].replace('Version History\n\n', '').replace('\n\n', '').split('\n')
+        versions_history = raw_versions[0].replace("Version History\n\n", "").replace("\n\n", "").split("\n")
         return versions_history
 
     @staticmethod
     def validate_version_numbers(versions_history):
         violated = False
         violations = []
         for version in versions_history:
             version_number = version.split(" - ")
-            version_found = re.findall(r'^\*\s\d+\.\d+\.\d+$', version_number[0])
+            version_found = re.findall(r"^\*\s\d+\.\d+\.\d+$", version_number[0])
 
             if not version_found:
-                violations.append(version_number[0].replace('* ', ''))
+                violations.append(version_number[0].replace("* ", ""))
                 violated = True
 
         if violated:
-            raise Exception(f"Incorrect version numbers specified in help.md: {YELLOW}{violations}")
+            raise Exception(f"Incorrect version numbers specified in help.md: {YELLOW}{violations}.")
 
     @staticmethod
     def validate_order(versions_history):
         versions = []
 
         for version in versions_history:
             version_number = version.split(" - ")[0]
             versions.append(version_number)
 
         sorted_versions = sorted(versions, key=LooseVersion, reverse=True)
 
         if versions != sorted_versions:
-            raise Exception("Version numbers in help.md are not sorted in descending order")
+            raise Exception("Version numbers in help.md are not sorted in descending order.")
 
     @staticmethod
     def validate_version_history_updated(versions_history, spec):
         violation = True
-        spec_version = spec.spec_dictionary()['version']
+        spec_version = spec.spec_dictionary()["version"]
 
         for version_detail in versions_history:
-            help_version = re.search(r'^\*\s\d+\.\d+\.\d+$', version_detail.split(" - ")[0])
+            help_version = re.search(r"^\*\s\d+\.\d+\.\d+$", version_detail.split(" - ")[0])
             if spec_version in help_version.group():
                 violation = False
                 break
 
         if violation:
-            raise Exception(f"Version history of help.md missing version {spec_version}. Please add missing version")
+            raise Exception(f"Version history of help.md missing version {spec_version}. Please add missing version.")
 
     def validate(self, spec):
         versions_history = ChangelogValidator.get_versions(spec.raw_help())
         ChangelogValidator.validate_version_numbers(versions_history)
         ChangelogValidator.validate_order(versions_history)
         ChangelogValidator.validate_version_history_updated(versions_history, spec)
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/confidential_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/confidential_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 import re
 
 from icon_plugin_spec.plugin_spec import KomandPluginSpec
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class ConfidentialValidator(KomandPluginValidator):
     # emails allowed
     emails = ["user@example.com"]
 
     # store violations per file
@@ -20,15 +20,15 @@
             help_lines: [str] = h.readlines()
 
         ConfidentialValidator.validate_emails(help_lines, "help.md")
 
     # Check content line by line for emails that validate the rule
     @staticmethod
     def validate_emails(content: [str], path_to_file: str):
-        email_pattern = re.compile(r'([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9_-]+){0,}')
+        email_pattern = re.compile(r"([a-zA-Z0-9._-]+@[a-zA-Z0-9._-]+\.[a-zA-Z0-9_-]+){0,}")
         for i in range(0, len(content)):
             matches = email_pattern.findall(content[i])
             while "" in matches:
                 matches.remove("")
             for match in matches:
                 if match not in ConfidentialValidator.emails:
                     ConfidentialValidator.violations.append(f"{path_to_file}, line: {i + 1}")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/credentials_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/credentials_validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class CredentialsValidator(KomandPluginValidator):
     def validate(self, spec):
         tests_dir = os.path.join(spec.directory, "tests")
         violating_files = []
         for path, _, files in os.walk(tests_dir):
@@ -33,8 +33,8 @@
                             for key in creds:
                                 if creds[key] != "":
                                     violating_files.append(f"tests/{name}")
                                     break
                     except AttributeError:
                         pass
         if len(violating_files) > 0:
-            raise Exception(f"Remove credentials from the following files: {violating_files}")
+            raise Exception(f"Remove credentials from the following files: {violating_files}.")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/default_value_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/default_value_validator.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,43 +1,43 @@
 import validators
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class DefaultValueValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_variables(validate_variables):
 
         if not validate_variables:
             return
 
         for k, v in validate_variables.items():
-            if 'default' in v:
-                if k == 'domain':
-                    if validators.domain(v['default']) is not True:
-                        raise Exception("Variable %s's default value is not a valid domain" % k)
-                elif k == 'email' or k == 'email_address':
-                    if validators.email(v['default']) is not True:
-                        raise Exception("Variable %s's default value is not a valid email address" % k)
+            if "default" in v:
+                if k == "domain":
+                    if validators.domain(v["default"]) is not True:
+                        raise Exception(f"Variable {k}'s default value is not a valid domain.")
+                elif k == "email" or k == "email_address":
+                    if validators.email(v["default"]) is not True:
+                        raise Exception(f"Variable {k}'s default value is not a valid email address.")
 
     @staticmethod
     def validate_action(action):
 
         if not action:
             return
 
         for key, value in action.items():
-            if 'input' in value:
-                DefaultValueValidator.validate_variables(value['input'])
-            if 'output' in value:
-                DefaultValueValidator.validate_variables(value['output'])
+            if "input" in value:
+                DefaultValueValidator.validate_variables(value["input"])
+            if "output" in value:
+                DefaultValueValidator.validate_variables(value["output"])
 
     def validate(self, spec):
         plugin_spec = spec.spec_dictionary()
-        if 'actions' in plugin_spec:
-            DefaultValueValidator.validate_action(plugin_spec['actions'])
-        if 'triggers' in plugin_spec:
-            DefaultValueValidator.validate_action(plugin_spec['triggers'])
-        if 'types' in plugin_spec:
-            for k, v in plugin_spec['types'].items():
+        if "actions" in plugin_spec:
+            DefaultValueValidator.validate_action(plugin_spec["actions"])
+        if "triggers" in plugin_spec:
+            DefaultValueValidator.validate_action(plugin_spec["triggers"])
+        if "types" in plugin_spec:
+            for k, v in plugin_spec["types"].items():
                 DefaultValueValidator.validate_variables(v)
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/description_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/description_validator.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,59 +1,58 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class DescriptionValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_description(description):
-        if description.endswith('.'):
-            raise Exception('Description ends with period when it should not')
+        if description.endswith("."):
+            raise Exception("Description ends with a period when it should not.")
         if description[0].islower():
-            raise Exception('Description should not start with a lower case letter')
+            raise Exception("Description should not start with a lower case letter.")
         if description[0].isspace():
-            raise Exception('Description should not start with a whitespace character')
+            raise Exception("Description should not start with a whitespace character.")
 
     @staticmethod
-    def validate_actions(dict, dict_key):
-        if dict_key in dict:
-            DescriptionValidator.validate_dictionary(dict, dict_key)
-            for key, value in dict[dict_key].items():
-                if 'input' in value:
-                    DescriptionValidator.validate_dictionary(value, 'input')
-                if 'output' in value:
-                    DescriptionValidator.validate_dictionary(value, 'output')
+    def validate_actions(dict_, dict_key):
+        if dict_key in dict_:
+            DescriptionValidator.validate_dictionary(dict_, dict_key)
+            for key, value in dict_[dict_key].items():
+                if "input" in value:
+                    DescriptionValidator.validate_dictionary(value, "input")
+                if "output" in value:
+                    DescriptionValidator.validate_dictionary(value, "output")
 
     @staticmethod
-    def validate_dictionary(dict, dict_key):
-        if dict_key in dict:
-            if not dict[dict_key]:
+    def validate_dictionary(dict_, dict_key):
+        if dict_key in dict_:
+            if not dict_[dict_key]:
                 return
 
-            for key, value in dict[dict_key].items():
-                if 'description' not in value:
-                    raise Exception('%s key "%s" is missing description field' % (dict_key, key))
+            for key, value in dict_[dict_key].items():
+                if "description" not in value:
+                    raise Exception(f"{dict_key} key '{key}' is missing description field.")
                 try:
-                    DescriptionValidator.validate_description(value['description'])
+                    DescriptionValidator.validate_description(value["description"])
                 except Exception as e:
-                    raise Exception('%s key "%s"\'s description ends with period when it should not'
-                                    % (dict_key, key), e)
+                    raise Exception(f"{dict_key} key '{key}'\'s description ends with a period when it should not", e)
 
     @staticmethod
     def validate_plugin_description(spec):
-        if 'description' not in spec.spec_dictionary():
-            raise Exception('Plugin description is missing')
+        if "description" not in spec.spec_dictionary():
+            raise Exception("Plugin description is missing.")
 
         try:
-            DescriptionValidator.validate_description(spec.spec_dictionary()['description'])
+            DescriptionValidator.validate_description(spec.spec_dictionary()["description"])
         except Exception as e:
-            raise Exception('Plugin description not valid', e)
+            raise Exception("Plugin description is not valid.", e)
 
     def validate(self, spec):
         DescriptionValidator.validate_plugin_description(spec)
-        DescriptionValidator.validate_actions(spec.spec_dictionary(), 'actions')
-        DescriptionValidator.validate_actions(spec.spec_dictionary(), 'triggers')
+        DescriptionValidator.validate_actions(spec.spec_dictionary(), "actions")
+        DescriptionValidator.validate_actions(spec.spec_dictionary(), "triggers")
 
         # Types do not have descriptions but their keys do.
         # TODO: disabling type descriptions until better plugin autogen support exists (for swagger, wasdl, etc)
-        # if 'types' in spec.spec_dictionary():
-        #     for key, value in spec.spec_dictionary()['types'].items():
-        #         DescriptionValidator.validate_dictionary(spec.spec_dictionary()['types'], key)
+        # if "types" in spec.spec_dictionary():
+        #     for key, value in spec.spec_dictionary()["types"].items():
+        #         DescriptionValidator.validate_dictionary(spec.spec_dictionary()["types"], key)
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/docker_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/docker_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 import os
 import subprocess
 import sys
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class DockerValidator(KomandPluginValidator):
     def validate(self, spec):
         # Using subprocess so we don't have to deal with connecting to different Docker environments
         # e.g docker-machine vs Docker for Mac vs native Docker
         # Directory of current plugin
         d = spec.directory
         build_image = ["docker", "build", "-q", "--pull", "-t", "docker_validator", d]
         run_image = ["docker", "run", "--rm", "-t", "docker_validator", "info"]
 
         with open(os.devnull, "w") as fd:
             try:
-                which = subprocess.check_call(['which', 'docker'], stdout=fd, stderr=fd)
+                which = subprocess.check_call(["which", "docker"], stdout=fd, stderr=fd)
             except subprocess.CalledProcessError as e:
-                sys.stdout.write('DockerValidator: docker binary missing in PATH, skipping...')
+                sys.stdout.write("DockerValidator: docker binary missing in PATH, skipping...")
             else:
                 try:
                     subprocess.check_call(build_image, stdout=fd, stderr=fd)
                 except subprocess.CalledProcessError as e:
-                    raise Exception('The plugin is either broken or the image might not be built.'
-                                    'Please try "icon-plugin build image" to rebuild the image.'
-                                    '"icon-plugin run -c bash" will open a bash shell on the build container.') from e
+                    raise Exception("The plugin is either broken or the image might not be built."
+                                    "Please try 'icon-plugin build image' to rebuild the image."
+                                    "'icon-plugin run -c bash' will open a bash shell on the build container.") from e
 
                 try:
                     subprocess.check_call(run_image, stdout=fd, stderr=fd)
                 except subprocess.CalledProcessError as e:
-                    raise Exception('Docker failed at running info command. '
-                                    'Check your plugin code for run-time errors.') from e
+                    raise Exception("Docker failed at running info command. "
+                                    "Check your plugin code for run-time errors.") from e
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/dockerfile_parent_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/dockerfile_parent_validator.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,34 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class DockerfileParentValidator(KomandPluginValidator):
     def validate(self, spec):
-        spec_str = ''.join(spec.raw_dockerfile())
+        spec_str = "".join(spec.raw_dockerfile())
 
         valid_images = [
-            'komand/go-plugin-2', 'komand/python-2-plugin', 'komand/python-3-plugin', 'komand/python-pypy3-plugin',
-            'komand/python-3-slim-plugin', 'komand/python-2-slim-plugin',
-            'komand/python-2-27-slim-plugin', 'komand/python-3-37-slim-plugin', 'komand/python-2-27-plugin',
-            'komand/python-3-37-plugin',
-            'komand/python-2-27-full-plugin', 'komand/python-pypy3-full-plugin'
+            "komand/go-plugin-2", "komand/python-2-plugin", "komand/python-3-plugin", "komand/python-pypy3-plugin",
+            "komand/python-3-slim-plugin", "komand/python-2-slim-plugin",
+            "komand/python-2-27-slim-plugin", "komand/python-3-37-slim-plugin", "komand/python-2-27-plugin",
+            "komand/python-3-37-plugin",
+            "komand/python-2-27-full-plugin", "komand/python-pypy3-full-plugin"
         ]
         root_spec_found = False
         for line in spec.raw_dockerfile():
-            if line.startswith('FROM'):
-                parent = line.replace('FROM', '').strip()
-                parts = parent.split(':')
+            if line.startswith("FROM"):
+                parent = line.replace("FROM", "").strip()
+                parts = parent.split(":")
                 image = parts[0].strip()
-                if image == 'komand/python-plugin':
-                    raise Exception('Parent Dockerfile komand/python-plugin is no longer supported. '
-                                    'Use komand/python-2-plugin, komand/python-3-plugin, or komand/python-pypy3-plugin instead.')
-                elif image == 'komand/go-plugin':
-                    raise Exception('Parent Dockerfile komand/go-plugin is no longer supported. '
-                                    'Use komand/go-plugin-2 instead.')
+                if image == "komand/python-plugin":
+                    raise Exception("Parent Dockerfile komand/python-plugin is no longer supported. "
+                                    "Use komand/python-2-plugin, komand/python-3-plugin, or komand/python-pypy3-plugin instead.")
+                elif image == "komand/go-plugin":
+                    raise Exception("Parent Dockerfile komand/go-plugin is no longer supported. "
+                                    "Use komand/go-plugin-2 instead.")
                 elif image not in valid_images:
-                    raise Exception('Unrecognized parent Dockerfile')
-            if line.startswith('ADD ./plugin.spec.yaml /plugin.spec.yaml'):
+                    raise Exception("Unrecognized parent Dockerfile")
+            if line.startswith("ADD ./plugin.spec.yaml /plugin.spec.yaml"):
                 root_spec_found = True
 
         # Komand code checks for /plugin.spec.yaml in the plugin container
         if not root_spec_found:
-            raise Exception('Dockerfile missing line: ADD ./plugin.spec.yaml /plugin.spec.yaml')
+            raise Exception("Dockerfile missing line: ADD ./plugin.spec.yaml /plugin.spec.yaml")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/exception_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/exception_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import os
 import re
 
 from icon_validator.styling import *
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class ExceptionValidator(KomandPluginValidator):
     def __init__(self):
         super().__init__()
         self._violating_files = []
 
     def validate_exceptions(self, spec_dir, path, name):
         joined_path = os.path.join(path, name)
-        with open(joined_path, 'r') as f:
+        with open(joined_path, "r") as f:
             text = f.readlines()
 
         violating_lines = []
         pattern = "raise [A-Za-z]*"
         for line_num in range(len(text)):
             matches = re.findall(pattern, text[line_num])
             violations = list(filter(lambda m: ExceptionValidator.violation_check(m), matches))
@@ -53,8 +53,8 @@
 
             for violating_file in self._violating_files:
                 violation_content = violating_file.split(":")
                 file_name = violation_content[0]
                 line_numbers = violation_content[1].split(",")
 
                 for line_number in line_numbers:
-                    print(f'{YELLOW}violation: {file_name}: line, {line_number}')
+                    print(f"{YELLOW}violation: {file_name}: line, {line_number}")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/files_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/files_validator.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import os
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class FilesValidator(KomandPluginValidator):
 
     def validate(self, spec):
         d = spec.directory
 
         # Go plugins
-        if os.path.isdir('{}/{}'.format(d, 'connection')):
-            if not os.path.isfile('{}/{}'.format(d, 'Makefile')):
-                raise Exception('File Makefile does not exist in: ', d)
-            if not os.path.isfile('{}/{}'.format(d, 'plugin.spec.yaml')):
-                raise Exception('File plugin.spec.yaml does not exist in: ', d)
-            if not os.path.isfile('{}/{}'.format(d, 'Dockerfile')):
-                raise Exception('File Dockerfile does not exist in: ', d)
+        if os.path.isdir("{}/{}".format(d, "connection")):
+            if not os.path.isfile("{}/{}".format(d, "Makefile")):
+                raise Exception("File Makefile does not exist in: ", d)
+            if not os.path.isfile("{}/{}".format(d, "plugin.spec.yaml")):
+                raise Exception("File plugin.spec.yaml does not exist in: ", d)
+            if not os.path.isfile("{}/{}".format(d, "Dockerfile")):
+                raise Exception("File Dockerfile does not exist in: ", d)
         else:
             # Python plugins
-            if os.path.isdir('{}/{}'.format(d, 'bin')):
-                if not os.path.isfile('{}/{}'.format(d, 'Dockerfile')):
-                    raise Exception('File Dockerfile does not exist in: ', d)
-                if not os.path.isfile('{}/{}'.format(d, 'Makefile')):
-                    raise Exception('File Makefile does not exist in: ', d)
-                if not os.path.isfile('{}/{}'.format(d, 'plugin.spec.yaml')):
-                    raise Exception('File plugin.spec.yaml does not exist in: ', d)
-                if not os.path.isfile('{}/{}'.format(d, 'setup.py')):
-                    raise Exception('File setup.py does not exist in: ', d)
-                if not os.path.isfile('{}/{}'.format(d, 'requirements.txt')):
-                    raise Exception('File requirements.txt does not exist in: ', d)
+            if os.path.isdir("{}/{}".format(d, "bin")):
+                if not os.path.isfile("{}/{}".format(d, "Dockerfile")):
+                    raise Exception("File Dockerfile does not exist in: ", d)
+                if not os.path.isfile("{}/{}".format(d, "Makefile")):
+                    raise Exception("File Makefile does not exist in: ", d)
+                if not os.path.isfile("{}/{}".format(d, "plugin.spec.yaml")):
+                    raise Exception("File plugin.spec.yaml does not exist in: ", d)
+                if not os.path.isfile("{}/{}".format(d, "setup.py")):
+                    raise Exception("File setup.py does not exist in: ", d)
+                if not os.path.isfile("{}/{}".format(d, "requirements.txt")):
+                    raise Exception("File requirements.txt does not exist in: ", d)
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/help_input_output_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/help_input_output_validator.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import re
 
 from icon_validator.styling import *
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class HelpInputOutputValidator(KomandPluginValidator):
     raw_help = ""
     violations = []
     violated = 0
     action_missing = 0
@@ -16,15 +16,15 @@
         if process_type == "actions":
             regex = regex + ".*?### Triggers"
 
         action_input_section = re.findall(regex, HelpInputOutputValidator.raw_help, re.DOTALL)
 
         if not action_input_section:
             print(
-                f"{YELLOW}{process_type[:-1].capitalize()} \"{action_title}\" could be missing or title is incorrect in help.md{RESET_ALL}")
+                f"{YELLOW}{process_type[:-1].capitalize()} \"{action_title}\" could be missing or title is incorrect in help.md{RESET_ALL}.")
             HelpInputOutputValidator.violated = 1
             HelpInputOutputValidator.action_missing = 1
             return
 
         regex = r"#### " + action_title + "\n.*?#+ Output"
         action_input_section = re.findall(regex, action_input_section[0], re.DOTALL)
 
@@ -49,78 +49,78 @@
                 regex = regex + ".*?### Triggers"
 
             action_help_section_temp = re.findall(regex, HelpInputOutputValidator.raw_help, re.DOTALL)
             regex = r"#### " + action_title + "\n.*?#+ Output\n\n.*?" + re.escape(
                 "|Name|Type|Required|Description|") + ".*?\n\n"
             action_output_section_temp = re.findall(regex, action_help_section_temp[0], re.DOTALL)
             action_output_section = re.findall(
-                r'#+ Output\n\n.*?' + re.escape("|Name|Type|Required|Description|") + ".*?\n\n",
+                r"#+ Output\n\n.*?" + re.escape("|Name|Type|Required|Description|") + ".*?\n\n",
                 action_output_section_temp[0], re.DOTALL)
         else:
             action_output_section = re.findall(r"#+ Output\n\n.*?\n\n", action_help_section[0], re.DOTALL)
 
         for output_fields in action_output:
             if output_fields not in action_output_section[0]:
                 HelpInputOutputValidator.violations.append(output_fields)
 
     @staticmethod
     def get_spec_input(input_content: dict) -> list:
         action_input = []
 
         for k, v in input_content.items():
             name_ = k
-            type_ = input_content.get(k).get('type')
-            default_ = input_content.get(k).get('default', None)
-            required = input_content.get(k).get('required')
-            description = input_content.get(k).get('description')
-            enum = input_content.get(k).get('enum', None)
-            action_input.append(f'|{name_}|{type_}|{default_}|{required}|{description}|{enum}|')
+            type_ = input_content.get(k).get("type")
+            default_ = input_content.get(k).get("default", None)
+            required = input_content.get(k).get("required")
+            description = input_content.get(k).get("description")
+            enum = input_content.get(k).get("enum", None)
+            action_input.append(f"|{name_}|{type_}|{default_}|{required}|{description}|{enum}|")
         return action_input
 
     @staticmethod
     def get_spec_output(output_content: dict) -> list:
         action_output = []
         for k, v in output_content.items():
             name_ = k
-            type_ = output_content.get(k).get('type')
-            required = output_content.get(k).get('required')
-            description = output_content.get(k).get('description')
-            action_output.append(f'|{name_}|{type_}|{required}|{description}|')
+            type_ = output_content.get(k).get("type")
+            required = output_content.get(k).get("required")
+            description = output_content.get(k).get("description")
+            action_output.append(f"|{name_}|{type_}|{required}|{description}|")
         return action_output
 
     def validate(self, spec):
         HelpInputOutputValidator.raw_help = spec.raw_help()
         raw_spec_yaml = spec.spec_dictionary()
         process_type = ["actions", "triggers"]
 
         for p_type in process_type:
             actions = raw_spec_yaml.get(p_type, {})
             for key, value in actions.items():
-                action_name = actions[key].get('title')
-                input_section = actions[key].get('input')
-                output_section = actions[key].get('output')
+                action_name = actions[key].get("title")
+                input_section = actions[key].get("input")
+                output_section = actions[key].get("output")
                 HelpInputOutputValidator.action_missing = 0
 
                 # Action with no input in spec file will skip input validation
                 if input_section:
                     action_input_fields = HelpInputOutputValidator.get_spec_input(input_section)
                     HelpInputOutputValidator.validate_input(action_name, action_input_fields, p_type)
 
                     if HelpInputOutputValidator.violations:
                         print(
-                            f'{YELLOW}Input violations: {p_type[:-1].capitalize()} -> \"{action_name}\": Missing {HelpInputOutputValidator.violations} in help.md{RESET_ALL}')
+                            f"{YELLOW}Input violations: {p_type[:-1].capitalize()} -> \"{action_name}\": Missing {HelpInputOutputValidator.violations} in help.md{RESET_ALL}")
                         HelpInputOutputValidator.violations = []
                         HelpInputOutputValidator.violated = 1
 
                 # Actions with no output in spec file will skip output validation. Also, skip output validation for actions not found in help.md
                 if output_section and not HelpInputOutputValidator.action_missing:
                     action_output_fields = HelpInputOutputValidator.get_spec_output(output_section)
                     HelpInputOutputValidator.validate_output(action_name, action_output_fields, p_type)
 
                     if HelpInputOutputValidator.violations:
                         print(
-                            f'{YELLOW}Output violations: {p_type[:-1].capitalize()}-> \"{action_name}\": Missing {HelpInputOutputValidator.violations} in help.md{RESET_ALL}')
+                            f"{YELLOW}Output violations: {p_type[:-1].capitalize()}-> \"{action_name}\": Missing {HelpInputOutputValidator.violations} in help.md{RESET_ALL}")
                         HelpInputOutputValidator.violations = []
                         HelpInputOutputValidator.violated = 1
 
         if HelpInputOutputValidator.violated:
-            raise Exception("Help.md is not in sync with plugin.spec.yaml. Please regenerate help.md by running 'icon-plugin generate python --regenerate' to rectify violations")
+            raise Exception("Help.md is not in sync with plugin.spec.yaml. Please regenerate help.md by running 'icon-plugin generate python --regenerate' to rectify violations.")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/help_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/help_validator.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,100 +1,100 @@
 import re
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class HelpValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_help_exists(spec):
-        if 'help' in spec:
-            raise Exception('Help section should exist in help.md and not in the plugin.spec.yaml file')
+        if "help" in spec:
+            raise Exception("Help section should exist in help.md and not in the plugin.spec.yaml file.")
 
     @staticmethod
     def validate_version_history(help_str):
-        if '- Initial plugin' not in help_str:
-            raise Exception("Initial plugin version line is missing: 1.0.0 - Initial plugin")
+        if "- Initial plugin" not in help_str:
+            raise Exception("Initial plugin version line is missing: 1.0.0 - Initial plugin.")
 
-        if 'Support web server mode' not in help_str and '1.0.0 - Initial plugin' not in help_str:
+        if "Support web server mode" not in help_str and "1.0.0 - Initial plugin" not in help_str:
             # Match legacy versioning which indicates this plugin came before web server mode existed
-            if '* 0.' in help_str:
+            if "* 0." in help_str:
                 # Takes advantage of the fact that versioning used to start from 0.1.0 instead of 1.0.0
                 raise Exception(
-                    "Initial plugin was released prior to schema V2 but versioning history "
-                    "does not document the upgrade to web server mode: Support web server mode"
+                    "Initial plugin was released prior to schema V2 but versioning history."
+                    "does not document the upgrade to web server mode: Support web server mode."
                 )
 
     @staticmethod
     def validate_same_actions_title(spec, help_):
-        if 'actions' in spec:
-            HelpValidator.validate_same_actions_loop(spec['actions'], help_)
-        if 'triggers' in spec:
-            HelpValidator.validate_same_actions_loop(spec['triggers'], help_)
+        if "actions" in spec:
+            HelpValidator.validate_same_actions_loop(spec["actions"], help_)
+        if "triggers" in spec:
+            HelpValidator.validate_same_actions_loop(spec["triggers"], help_)
 
     @staticmethod
     def validate_same_actions_loop(section, help_str):
         for i in section:
-            if 'title' in section[i]:
-                if '#### {}'.format(section[i]['title']) not in help_str:
-                    raise Exception('Help section is missing title of: #### {}'.format(section[i]['title']))
+            if "title" in section[i]:
+                if f"#### {section[i]['title']}" not in help_str:
+                    raise Exception(f"Help section is missing title of: #### {section[i]['title']}")
 
     @staticmethod
     def remove_example_output(help_content):
-        example_outputs = re.findall(r'Example output:\n\n```\n.*?```\n\n', help_content, re.DOTALL)
+        example_outputs = re.findall(r"Example output:\n\n```\n.*?```\n\n", help_content, re.DOTALL)
         for example_output in example_outputs:
-            help_content = help_content.replace(example_output, '')
+            help_content = help_content.replace(example_output, "")
         return help_content
 
     @staticmethod
     def validate_title_spelling(spec, help_):
-        if 'title' in spec:
-            title = spec['title']
+        if "title" in spec:
+            title = spec["title"]
             lower_title = title.lower()
             help_ = HelpValidator.remove_example_output(help_)
-            for line in help_.split('\n'):
+            for line in help_.split("\n"):
                 lower_line = line.lower()
                 if lower_title in lower_line:
                     if title not in line:
                         if lower_line[lower_line.find(title.lower()) - 1].isspace():
-                            if line.startswith('$'):
+                            if line.startswith("$"):
                                 pass
-                            elif line.startswith('>>>'):
+                            elif line.startswith(">>>"):
                                 pass
                             else:
-                                raise Exception('Help section contains non-matching title in line: {}'.format(line))
+                                raise Exception("Help section contains non-matching title in line: {}".format(line))
 
     @staticmethod
     def validate_help_headers(help_str):
-        if '# Description' not in help_str:
-            raise Exception("Help section is missing header: # Description")
-        if '# Key Features' not in help_str:
-            raise Exception("Help section is missing header: # Key Features")
-        if '# Requirements' not in help_str:
-            raise Exception("Help section is missing header: # Requirements")
-        if '# Documentation' not in help_str:
-            raise Exception("Help section is missing header: # Documentation")
-        if '## Setup' not in help_str:
-            raise Exception("Help section is missing header: ## Setup")
-        if '## Technical Details' not in help_str:
-            raise Exception("Help section is missing header: ## Technical Details")
-        if '### Actions' not in help_str:
-            raise Exception("Help section is missing header: ### Actions")
-        if '### Triggers' not in help_str:
-            raise Exception("Help section is missing header: ### Triggers")
-        if '### Custom Output Types' not in help_str:
-            raise Exception("Help section is missing header: ### Custom Output Types")
-        if '## Troubleshooting' not in help_str:
-            raise Exception("Help section is missing header: ## Troubleshooting")
-        if '# Version History' not in help_str:
-            raise Exception("Help section is missing header: # Version History")
-        if '# Links' not in help_str:
-            raise Exception("Help section is missing header: # Links")
-        if '## References' not in help_str:
-            raise Exception("Help section is missing header: ## References")
+        if "# Description" not in help_str:
+            raise Exception("Help section is missing header: # Description.")
+        if "# Key Features" not in help_str:
+            raise Exception("Help section is missing header: # Key Features.")
+        if "# Requirements" not in help_str:
+            raise Exception("Help section is missing header: # Requirements.")
+        if "# Documentation" not in help_str:
+            raise Exception("Help section is missing header: # Documentation.")
+        if "## Setup" not in help_str:
+            raise Exception("Help section is missing header: ## Setup.")
+        if "## Technical Details" not in help_str:
+            raise Exception("Help section is missing header: ## Technical Details.")
+        if "### Actions" not in help_str:
+            raise Exception("Help section is missing header: ### Actions.")
+        if "### Triggers" not in help_str:
+            raise Exception("Help section is missing header: ### Triggers.")
+        if "### Custom Output Types" not in help_str:
+            raise Exception("Help section is missing header: ### Custom Output Types.")
+        if "## Troubleshooting" not in help_str:
+            raise Exception("Help section is missing header: ## Troubleshooting.")
+        if "# Version History" not in help_str:
+            raise Exception("Help section is missing header: # Version History.")
+        if "# Links" not in help_str:
+            raise Exception("Help section is missing header: # Links.")
+        if "## References" not in help_str:
+            raise Exception("Help section is missing header: ## References.")
 
     def validate(self, spec):
         HelpValidator.validate_help_exists(spec.spec_dictionary())
         HelpValidator.validate_help_headers(spec.raw_help())
         HelpValidator.validate_version_history(spec.raw_help())
         HelpValidator.validate_same_actions_title(spec.spec_dictionary(), spec.raw_help())
         HelpValidator.validate_title_spelling(spec.spec_dictionary(), spec.raw_help())
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/icon_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/icon_validator.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from pathlib import Path
 
 import filetype
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class IconValidator(KomandPluginValidator):
 
     def validate(self, plugin_spec):
         """Base64 matches icon file valid base64, <=70kb in size, png"""
         IconValidator.check_icon_file_exists(plugin_spec)
@@ -19,46 +19,46 @@
     @staticmethod
     def check_icon_file_exists(plugin_spec):
         directory = plugin_spec.directory
         icon_file = directory + "/" + "icon.png"
 
         f = Path(icon_file)
         if not f.is_file():
-            raise Exception("icon.png file not included in plugin")
+            raise Exception("icon.png file not included in plugin.")
 
     @staticmethod
     def check_icon_less_than_equal_70kb(plugin_spec):
         directory = plugin_spec.directory
         icon_file = directory + "/" + "icon.png"
 
         info = os.stat(icon_file)
         if info.st_size >= 70000:
-            raise Exception("Included icon (%d) file exceeds maximum size limitation of 70kb" % info.st_size)
+            raise Exception(f"Included icon ({info.st_size}) file exceeds maximum size limitation of 70Kb.")
 
     @staticmethod
     def check_if_icon_is_png(plugin_spec):
         directory = plugin_spec.directory
         icon_file = directory + "/" + "icon.png"
         kind = filetype.guess(icon_file)
 
         if kind.extension != "png":
-            raise Exception("Included icon file (%s) is not PNG" % kind.extension)
+            raise Exception(f"Included icon file ({kind.extension}) is not PNG")
 
     @staticmethod
     def check_if_extension_image_file_exists(plugin_spec):
         directory = plugin_spec.directory
-        extension_image_file = directory + '/extension.png'
+        extension_image_file = f"{directory}/extension.png"
 
         file_item = Path(extension_image_file)
         if not file_item.is_file():
             raise Exception(
                 "extension.png file not included in plugin. Please include a color PNG image of a logo for this vendor or product.")
 
     @staticmethod
     def check_extension_image_file_is_nonzero_size(plugin_spec):
         directory = plugin_spec.directory
-        extension_image_file = directory + '/extension.png'
+        extension_image_file = f"{directory}/extension.png"
 
         image_file = os.stat(extension_image_file)
         if not image_file.st_size > 0:
             raise Exception(
                 "Extension image file is size zero. Please include a color PNG image of a logo for this vendor or product.")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/json_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/json_validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import json
 import os
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class JSONValidator(KomandPluginValidator):
     invalid_files = []
 
     def validate(self, spec):
         tests_dir = os.path.join(spec.directory, "tests")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/logging_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/logging_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,42 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class LoggingValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_import_logging(section):
         logging_found = False
         logging_getlogger_found = False
 
         for f in section:
-            if 'import logging' in f:
+            if "import logging" in f:
                 logging_found = True
-            if 'logging.getLogger' in f:
+            if "logging.getLogger" in f:
                 logging_getlogger_found = True
 
         # logging is imported without presence of logging.GetLogger
         if logging_found and not logging_getlogger_found:
-            raise Exception('One or more files imports logging, update to self.logger')
+            raise Exception("One or more files imports logging, update to self.logger.")
 
     def validate(self, spec):
         # Logging update is only for Python plugins
         image = None
         for line in spec.raw_dockerfile():
-            if line.startswith('FROM'):
-                parent = line.replace('FROM', '').strip()
-                parts = parent.split(':')
+            if line.startswith("FROM"):
+                parent = line.replace("FROM", "").strip()
+                parts = parent.split(":")
                 image = parts[0].strip()
                 break  # Only one FROM within a Dockerfile, so just exit early instead of continuing to loop
 
         if not image:
-            raise Exception('No FROM statement found within the Dockerfile')
+            raise Exception("No FROM statement found within the Dockerfile.")
 
-        if image == 'komand/go-plugin-2':
+        if image == "komand/go-plugin-2":
             return None
-        elif image == 'komand/go-plugin':
-            raise Exception('Plugin is using a deprecated Go parent image')
+        elif image == "komand/go-plugin":
+            raise Exception("Plugin is using a deprecated Go parent image.")
 
         LoggingValidator.validate_import_logging(spec.raw_trigger_files())
         LoggingValidator.validate_import_logging(spec.raw_action_files())
         LoggingValidator.validate_import_logging(spec.raw_connection_file())
         LoggingValidator.validate_import_logging(spec.raw_util_files())
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/output_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/output_validator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import os
 import re
 import sys
 
 from jsonschema import validate
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class OutputValidator(KomandPluginValidator):
     def __init__(self):
         super().__init__()
         self.missing_outputs = []
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/password_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/password_validator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class PasswordValidator(KomandPluginValidator):
     def validate(self, plugin_spec):
         connection = plugin_spec.spec_dictionary().get("connection")
         if connection is None:
             return
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/print_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/print_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,38 +1,38 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class PrintValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_print(section):
         print_found = False
 
         for f in section:
-            if 'print(' in f:
+            if "print(" in f:
                 print_found = True
 
         if print_found:
-            raise Exception('One or more files use print statements, update to use self.logger')
+            raise Exception("One or more files use print statements, update to use self.logger.")
 
     def validate(self, spec):
         # Logging update is only for Python plugins
         image = None
         for line in spec.raw_dockerfile():
-            if line.startswith('FROM'):
-                parent = line.replace('FROM', '').strip()
-                parts = parent.split(':')
+            if line.startswith("FROM"):
+                parent = line.replace("FROM", "").strip()
+                parts = parent.split(":")
                 image = parts[0].strip()
                 break  # Only one FROM within a Dockerfile, so just exit early instead of continuing to loop
 
         if not image:
-            raise Exception('No FROM statement found within the Dockerfile')
+            raise Exception("No FROM statement found within the Dockerfile.")
 
-        if image == 'komand/go-plugin-2':
+        if image == "komand/go-plugin-2":
             return None
-        elif image == 'komand/go-plugin':
-            raise Exception('Plugin is using a deprecated Go parent image')
+        elif image == "komand/go-plugin":
+            raise Exception("Plugin is using a deprecated Go parent image.")
 
         PrintValidator.validate_print(spec.raw_trigger_files())
         PrintValidator.validate_print(spec.raw_action_files())
         PrintValidator.validate_print(spec.raw_connection_file())
         PrintValidator.validate_print(spec.raw_util_files())
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/regeneration_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/regeneration_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 import os
 from hashlib import md5
 from typing import Optional
 
-from . import KomandPluginSpec
-from .validator import KomandPluginValidator
+from icon_validator.rules import KomandPluginSpec
+from icon_validator.rules.validator import KomandPluginValidator
 
 MD5 = str
 JSON = str
 _CHECKSUM = ".CHECKSUM"
 
 
 class SchemaHash(object):
@@ -30,15 +30,15 @@
         equals_hash = self.hash == other.hash
 
         return equals_identifier and equals_hash
 
     @classmethod
     def from_dict(cls, dict_: {str: str}):
         if "identifier" not in dict_ or "hash" not in dict_:
-            raise Exception("Fatal: Invalid dict provided for SchemaHash! Dict was: %s" % dict_)
+            raise Exception(f"Fatal: Invalid dict provided for SchemaHash! Dict was: {dict_}")
 
         return cls(identifier=dict_["identifier"], hash_=dict_["hash"])
 
 
 class Checksum(object):
 
     def __init__(self, spec: MD5, schemas: [SchemaHash], manifest: MD5, setup: MD5 = None):
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/required_keys_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/required_keys_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from icon_plugin_spec.plugin_spec import KomandPluginSpec
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class RequiredKeysValidator(KomandPluginValidator):
     missing_key_message = {
-        'plugin_spec_version': 'Specifies the version of the spec. Current version is v1',
-        'name': 'Name of the plugin, refers to the docker image name. Should be lower case',
-        'title': 'Formatted name',
-        'description': 'One sentence description',
-        'version': 'Semantic version of the plugin',
-        'vendor': 'Plugin vendor, refers to the docker image repository and komand marketplace user',
-        'status': 'List of development statuses to apply to the plugin',
-        'tags': 'List of tags to apply to the plugin',
+        "plugin_spec_version": "Specifies the version of the spec. Current version is v1",
+        "name": "Name of the plugin, refers to the docker image name. Should be lower case",
+        "title": "Formatted name",
+        "description": "One sentence description",
+        "version": "Semantic version of the plugin",
+        "vendor": "Plugin vendor, refers to the docker image repository and komand marketplace user",
+        "status": "List of development statuses to apply to the plugin",
+        "tags": "List of tags to apply to the plugin",
     }
 
     @staticmethod
     def validate_support(spec_dict: dict):
         accepted_values = ["rapid7", "community", "partner"]
         if "support" not in spec_dict or spec_dict["support"] not in accepted_values:
             RequiredKeysValidator.raise_exception("support",
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/required_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/required_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,43 +1,42 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class RequiredValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_required(required):
         if not isinstance(required, bool):
-            raise Exception('required must be boolean')
+            raise Exception("required must be boolean.")
 
     @staticmethod
-    def validate_actions(dict, dict_key):
-        if dict_key in dict:
-            for key, value in dict[dict_key].items():
-                if 'input' in value:
-                    RequiredValidator.validate_dictionary(value, 'input')
-                if 'output' in value:
-                    RequiredValidator.validate_dictionary(value, 'output')
+    def validate_actions(dict_, dict_key):
+        if dict_key in dict_:
+            for key, value in dict_[dict_key].items():
+                if "input" in value:
+                    RequiredValidator.validate_dictionary(value, "input")
+                if "output" in value:
+                    RequiredValidator.validate_dictionary(value, "output")
 
     @staticmethod
-    def validate_connection(dict, dict_key):
-        if dict_key in dict:
-            RequiredValidator.validate_dictionary(dict, dict_key)
+    def validate_connection(dict_, dict_key):
+        if dict_key in dict_:
+            RequiredValidator.validate_dictionary(dict_, dict_key)
 
     @staticmethod
-    def validate_dictionary(dict, dict_key):
-        if dict_key in dict:
-            if not dict[dict_key]:
+    def validate_dictionary(dict_, dict_key):
+        if dict_key in dict_:
+            if not dict_[dict_key]:
                 return
 
-            for key, value in dict[dict_key].items():
-                if 'required' not in value:
-                    raise Exception('%s key "%s" is missing required field' % (dict_key, key))
+            for key, value in dict_[dict_key].items():
+                if "required" not in value:
+                    raise Exception(f"{dict_key} key '{key}' is missing required field")
                 try:
-                    RequiredValidator.validate_required(value['required'])
+                    RequiredValidator.validate_required(value["required"])
                 except Exception as e:
-                    raise Exception('%s key "%s"\'s required must be boolean'
-                                    % (dict_key, key), e)
+                    raise Exception(f"{dict_key} key '{key}'\'s required must be boolean", e)
 
     def validate(self, spec):
-        RequiredValidator.validate_actions(spec.spec_dictionary(), 'actions')
-        RequiredValidator.validate_actions(spec.spec_dictionary(), 'triggers')
-        RequiredValidator.validate_connection(spec.spec_dictionary(), 'connection')
+        RequiredValidator.validate_actions(spec.spec_dictionary(), "actions")
+        RequiredValidator.validate_actions(spec.spec_dictionary(), "triggers")
+        RequiredValidator.validate_connection(spec.spec_dictionary(), "connection")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/spec_properties_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/spec_properties_validator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from icon_plugin_spec.plugin_spec import KomandPluginSpec, PluginComponent
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class SpecPropertiesValidator(KomandPluginValidator):
     _COMPONENT_WHITELIST = {
         "input",
         "output",
         "title",
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/tag_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/tag_validator.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class TagValidator(KomandPluginValidator):
     def validate(self, spec):
-        tags = spec.spec_dictionary().get('tags')
+        tags = spec.spec_dictionary().get("tags")
         if not tags:
-            raise Exception('Field "tags" not found')
+            raise Exception("Field 'tags' not found.")
         if not isinstance(tags, list):
-            raise Exception('Field "tags" is not a list')
+            raise Exception("Field 'tags' is not a list.")
         if len(tags) < 2:
-            raise Exception('Not enough tags. Each plugin should have at least 2 tags')
+            raise Exception("Not enough tags. Each plugin should have at least 2 tags.")
         i = 0
         for tag in tags:
             if not isinstance(tag, str):
-                raise Exception('Tag at index %d is not a string. All tags must be strings', i)
+                raise Exception("Tag at index %d is not a string. All tags must be strings.", i)
             i = i + 1
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/title_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/title_validator.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,76 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class TitleValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_title(title, plugin_title=False):
-        if title.endswith('.'):
-            raise Exception('Title ends with period when it should not')
+        if title.endswith("."):
+            raise Exception("Title ends with period when it should not.")
         if title[0].islower() and not plugin_title:
             # This plugin title is OK: minFraud
             # This plugin title is OK: ifconfig.co
-            raise Exception('Title should not start with a lower case letter')
+            raise Exception("Title should not start with a lower case letter.")
         if title[0].isspace():
-            raise Exception('Title should not start with a whitespace character')
+            raise Exception("Title should not start with a whitespace character.")
         if len(title.split()) > 7:
-            raise Exception('Title is too long, 6 words or less: contains ' + str(len(title.split())))
+            raise Exception("Title is too long, 6 words or less: contains " + str(len(title.split())))
         for word in title.split():
             if not title.startswith(word):
-                if 'The' == word:
-                    raise Exception('Title contains a capitalized "The" when it should not')
-                if 'By' == word and not title.endswith('By'):
+                if "The" == word:
+                    raise Exception("Title contains a capitalized 'The' when it should not.")
+                if "By" == word and not title.endswith("By"):
                     # This is OK: Order By
                     # This is NOT OK: Search By String
-                    raise Exception('Title contains a capitalized "By" when it should not')
-                if 'From' == word:
-                    raise Exception('Title contains a capitalized "From" when it should not')
-                if 'A' == word:
-                    raise Exception('Title contains a capitalized "A" when it should not')
-                if 'An' == word:
-                    raise Exception('Title contains a capitalized "An" when it should not')
-                if 'Of' == word and not title.endswith('Of'):
+                    raise Exception("Title contains a capitalized 'By' when it should not.")
+                if "From" == word:
+                    raise Exception("Title contains a capitalized 'From' when it should not.")
+                if "A" == word:
+                    raise Exception("Title contains a capitalized 'A' when it should not.")
+                if "An" == word:
+                    raise Exception("Title contains a capitalized 'An' when it should not.")
+                if "Of" == word and not title.endswith("Of"):
                     # This is OK: Member Of
                     # This is NOT OK: Type Of String
-                    raise Exception('Title contains a capitalized "Of" when it should not')
+                    raise Exception("Title contains a capitalized 'Of' when it should not.")
 
     @staticmethod
-    def validate_actions(dict, dict_key):
-        if dict_key in dict:
-            TitleValidator.validate_dictionary(dict, dict_key)
-            for key, value in dict[dict_key].items():
-                if 'input' in value:
-                    TitleValidator.validate_dictionary(value, 'input')
-                if 'output' in value:
-                    TitleValidator.validate_dictionary(value, 'output')
+    def validate_actions(dict_, dict_key):
+        if dict_key in dict_:
+            TitleValidator.validate_dictionary(dict_, dict_key)
+            for key, value in dict_[dict_key].items():
+                if "input" in value:
+                    TitleValidator.validate_dictionary(value, "input")
+                if "output" in value:
+                    TitleValidator.validate_dictionary(value, "output")
 
     @staticmethod
-    def validate_dictionary(dict, dict_key):
-        if dict_key in dict:
-            if not dict[dict_key]:
+    def validate_dictionary(dict_, dict_key):
+        if dict_key in dict_:
+            if not dict_[dict_key]:
                 return
 
-            for key, value in dict[dict_key].items():
-                if 'name' in value:
-                    raise Exception('Deprecated "name" key found when "title" should be used instead' % (dict_key, key))
-                if 'title' in value:
+            for key, value in dict_[dict_key].items():
+                if "name" in value:
+                    raise Exception(f"Deprecated 'name' key '{value}' found when 'title' should be used instead")
+                if "title" in value:
                     try:
-                        TitleValidator.validate_title(value['title'], plugin_title=False)
+                        TitleValidator.validate_title(value["title"], plugin_title=False)
                     except Exception as e:
-                        raise Exception('%s key "%s"\'s title ends with period when it should not'
-                                        % (dict_key, key), e)
+                        raise Exception(f"{dict_key} key '{key}'\'s title ends with period when it should not", e)
 
     @staticmethod
     def validate_plugin_title(spec):
-        if 'title' not in spec.spec_dictionary():
-            raise Exception('Plugin title is missing')
+        if "title" not in spec.spec_dictionary():
+            raise Exception("Plugin title is missing")
 
         try:
-            TitleValidator.validate_title(spec.spec_dictionary()['title'], plugin_title=True)
+            TitleValidator.validate_title(spec.spec_dictionary()["title"], plugin_title=True)
         except Exception as e:
-            raise Exception('Plugin title not valid', e)
+            raise Exception("Plugin title not valid", e)
 
     def validate(self, spec):
         TitleValidator.validate_plugin_title(spec)
-        TitleValidator.validate_actions(spec.spec_dictionary(), 'actions')
-        TitleValidator.validate_actions(spec.spec_dictionary(), 'triggers')
-        TitleValidator.validate_actions(spec.spec_dictionary(), 'connection')
+        TitleValidator.validate_actions(spec.spec_dictionary(), "actions")
+        TitleValidator.validate_actions(spec.spec_dictionary(), "triggers")
+        TitleValidator.validate_actions(spec.spec_dictionary(), "connection")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/url_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/url_validator.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import urllib
 import urllib.request
 from typing import List
 
 from urlextract import URLExtract
 
 from icon_validator.styling import *
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class URLValidator(KomandPluginValidator):
     """ Search for HTTP(s) links, and testing for invalid ones.  Namely, 400+ HTTP return codes"""
     maximum_timeout = 5
 
     def __init__(self):
@@ -26,57 +26,57 @@
         if not file_contents or not isinstance(file_contents, str):
             return return_list
 
         url_extractor = URLExtract()
         urls_from_file = list(set(url_extractor.find_urls(file_contents)))
 
         for web_address in urls_from_file:
-            if web_address.lower() in ['help.md', 'license.md', 'readme.md']:
+            if web_address.lower() in ["help.md", "license.md", "readme.md"]:
                 continue
-            if not web_address[0:4] == 'http':
-                web_address = 'http://' + web_address
+            if not web_address[0:4] == "http":
+                web_address = "http://" + web_address
             address_parts = urllib.parse.urlparse(web_address)
             cleaned_web_address = address_parts.netloc
 
-            path_to_test = r'/'
+            path_to_test = r"/"
             if address_parts.path:
                 path_to_test = address_parts.path
 
             url_tested = f"{cleaned_web_address}/{path_to_test}"
             if url_tested in self._urls_already_tried:
                 continue
 
             self._urls_already_tried.append(url_tested)
             try:
                 connection = http.client.HTTPConnection(cleaned_web_address, timeout=self.maximum_timeout, port=80)
-                connection.request('HEAD', path_to_test)
+                connection.request("HEAD", path_to_test)
                 response = connection.getresponse()
                 code = int(response.status)
 
                 if code >= 400:
                     return_list.append(web_address)
             except Exception as e:
                 return_list.append(web_address)
             finally:
                 if connection:
                     connection.close()
 
         return return_list
 
     def validate(self, spec):
-        specfile = spec.directory + '/' + spec.spec_file_name
+        specfile = spec.directory + "/" + spec.spec_file_name
         if os.path.exists(specfile):
             raw_spec_contents = spec.raw_spec()
             spec_file_bad_urls = self.inspect_file_for_urls_and_test_them(raw_spec_contents)
             if len(spec_file_bad_urls) > 0:
                 self._violating_files_to_urls_map[specfile] = spec_file_bad_urls
 
-        helpfile = spec.directory + '/help.md'
+        helpfile = spec.directory + "/help.md"
         if os.path.exists(helpfile):
-            help_file_contents = ''
+            help_file_contents = ""
             with open(helpfile) as h:
                 help_file_contents = h.read()
                 help_file_bad_urls = self.inspect_file_for_urls_and_test_them(help_file_contents)
                 if len(help_file_bad_urls) > 0:
                     self._violating_files_to_urls_map[helpfile] = help_file_bad_urls
 
         if len(self._violating_files_to_urls_map) > 0:
@@ -89,13 +89,13 @@
                 violating_urls = self._violating_files_to_urls_map[violating_file]
                 for url in violating_urls:
                     lines_with_url = list(filter(lambda i: url in file_lines[i], range(1, len(file_lines))))
 
                     for line in lines_with_url:
                         actual_line_number_in_file = str(int(line) + 1)
                         if not header_printed:
-                            header = ' '.join((f"{YELLOW}WARNING: URLs found that return a 4xx code.",
-                                               'Verify they are publicly accessible and if not, update with a working URL'))
+                            header = " ".join((f"{YELLOW}WARNING: URLs found that return a 4xx code.",
+                                               "Verify they are publicly accessible and if not, update with a working URL."))
                             print(header)
                             header_printed = True
                         file_name = os.path.basename(violating_file)
-                        print(f'{YELLOW}violation: {file_name}[{actual_line_number_in_file}]: ' + str(url))
+                        print(f"{YELLOW}violation: {file_name}[{actual_line_number_in_file}]: {str(url)}")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/use_case_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/use_case_validator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from icon_plugin_spec.plugin_spec import KomandPluginSpec
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class UseCaseValidator(KomandPluginValidator):
     use_case_ids = [
         "data_enrichment",
         "alerting_and_notifications",
         "application_management",
@@ -29,11 +29,11 @@
                 invalid_use_cases.append(use_case)
         return invalid_use_cases
 
     def validate(self, spec: KomandPluginSpec):
         try:
             result = UseCaseValidator.validate_use_cases(spec.spec_dictionary()["hub_tags"]["use_cases"])
             if len(result):
-                err = ', '.join(result)
-                raise Exception(f"Invalid use cases: {err}")
+                err = ", ".join(result)
+                raise Exception(f"Invalid use cases: {err}.")
         except KeyError:
-            raise Exception("Missing required field 'use_cases' in key 'hub_tags'")
+            raise Exception("Missing required field 'use_cases' in key 'hub_tags'.")
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/vendor_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/vendor_validator.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,37 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class VendorValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_vendor(vendor):
         lvendor = vendor.lower()
-        if lvendor == 'komand':
+        if lvendor == "komand":
             raise Exception("Vendor 'komand' not allowed. It's likely you meant 'rapid7'.")
-        if vendor.endswith('.'):
-            raise Exception('Vendor ends with period when it should not.')
+        if vendor.endswith("."):
+            raise Exception("Vendor ends with period when it should not.")
         if not vendor[0].islower():
-            raise Exception('Vendor starts with a capital letter when it should not.')
+            raise Exception("Vendor starts with a capital letter when it should not.")
         if " " in vendor:
-            raise Exception('Vendor should be separated by underscores, not spaces.')
+            raise Exception("Vendor should be separated by underscores, not spaces.")
 
     @staticmethod
     def validate_vendor_quotes(spec):
-        '''Requires raw spec to see the quotes'''
+        """Requires raw spec to see the quotes"""
         for line in spec.splitlines():
-            if line.startswith('vendor:'):
-                val = line[line.find(' ') + 1:]
-                if '"' in val:
-                    raise Exception('Vendor is surrounded by or contains quotes when it should not')
-                if "'" in val:
-                    raise Exception('Vendor is surrounded by or contains quotes when it should not')
+            if line.startswith("vendor:"):
+                val = line[line.find(" ") + 1:]
+                if "'" in val or '"' in val:
+                    raise Exception("Vendor is surrounded by or contains quotes when it should not.")
 
     @staticmethod
     def validate_plugin_vendor(spec):
-        if 'vendor' not in spec.spec_dictionary():
-            raise Exception('Plugin vendor is missing')
-        if not isinstance(spec.spec_dictionary()['vendor'], str):
-            raise Exception('Plugin vendor does not contain a string')
+        if "vendor" not in spec.spec_dictionary():
+            raise Exception("Plugin vendor is missing.")
+        if not isinstance(spec.spec_dictionary()["vendor"], str):
+            raise Exception("Plugin vendor does not contain a string.")
 
     def validate(self, spec):
         VendorValidator.validate_plugin_vendor(spec)
-        VendorValidator.validate_vendor(spec.spec_dictionary()['vendor'])
+        VendorValidator.validate_vendor(spec.spec_dictionary()["vendor"])
         VendorValidator.validate_vendor_quotes(spec.raw_spec())
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/version_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/plugin_validators/version_validator.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 import re
 
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
 
 
 class VersionValidator(KomandPluginValidator):
 
     @staticmethod
     def validate_version(version):
         if re.match("[1-9]+.[0-9]+.[0-9]+$", version) is None:
             raise Exception("Version does not match required semver format. "
                             "Version should be in form X.Y.Z with X, Y, and Z "
                             "being numbers. No special characters or spaces allowed. "
-                            "Versions start at 1.0.0.")
+                            "Versions start at 1.0.0, see https://semver.org/ for more information.")
 
     @staticmethod
     def validate_version_quotes(spec):
         """Requires raw spec to see the quotes"""
         for line in spec.splitlines():
-            if line.startswith('version:'):
-                val = line[line.find(' ') + 1:]
-                if '"' in val:
-                    raise Exception('Version is surrounded by or contains quotes when it should not')
-                if "'" in val:
-                    raise Exception('Version is surrounded by or contains quotes when it should not')
+            if line.startswith("version:"):
+                val = line[line.find(" ") + 1:]
+                if "'" in val or '"' in val:
+                    raise Exception("Vendor is surrounded by or contains quotes when it should not.")
 
     @staticmethod
     def validate_plugin_version(spec):
-        if 'version' not in spec.spec_dictionary():
-            raise Exception('Plugin version is missing')
-        if not isinstance(spec.spec_dictionary()['version'], str):
-            raise Exception('Plugin version does not contain a string')
+        if "version" not in spec.spec_dictionary():
+            raise Exception("Plugin version is missing.")
+        if not isinstance(spec.spec_dictionary()["version"], str):
+            raise Exception("Plugin version does not contain a string.")
 
     def validate(self, spec):
         VersionValidator.validate_plugin_version(spec)
-        VersionValidator.validate_version(spec.spec_dictionary()['version'])
+        VersionValidator.validate_version(spec.spec_dictionary()["version"])
         VersionValidator.validate_version_quotes(spec.raw_spec())
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/rules/workflow_help_validator.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/rules/workflow_validators/workflow_vendor_validator.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,42 +1,38 @@
-from .validator import KomandPluginValidator
+from icon_validator.rules.validator import KomandPluginValidator
+from icon_validator.exceptions import ValidationException
 
 
-class WorkflowHelpValidator(KomandPluginValidator):
+class WorkflowVendorValidator(KomandPluginValidator):
 
     @staticmethod
-    def validate_help_exists(spec):
-        if 'help' in spec:
-            raise Exception('Help section should exist in help.md and not in the workflow.spec.yaml file')
+    def validate_vendor(vendor):
+        lvendor = vendor.lower()
+        if lvendor == "komand":
+            raise ValidationException("Vendor 'komand' not allowed. It's likely you meant 'rapid7'.")
+        if vendor.endswith("."):
+            raise ValidationException("Vendor ends with period when it should not.")
+        if not vendor[0].islower():
+            raise ValidationException("Vendor starts with a capital letter when it should not.")
+        if " " in vendor:
+            raise ValidationException("Vendor should be separated by underscores, not spaces.")
 
     @staticmethod
-    def validate_version_history(help_str):
-        if '- Initial workflow' not in help_str:
-            raise Exception("Initial workflow version line is missing: 1.0.0 - Initial workflow")
+    def validate_vendor_quotes(spec):
+        """Requires raw spec to see the quotes"""
+        for line in spec.splitlines():
+            if line.startswith("vendor:"):
+                val = line[line.find(" ") + 1:]
+                if "'" in val or '"' in val:
+                    raise ValidationException("Vendor is surrounded by or contains quotes when it should not.")
 
     @staticmethod
-    def validate_help_headers(help_str):
-        if '# Description' not in help_str:
-            raise Exception("Help section is missing header: # Description")
-        if '# Key Features' not in help_str:
-            raise Exception("Help section is missing header: # Key Features")
-        if '# Requirements' not in help_str:
-            raise Exception("Help section is missing header: # Requirements")
-        if '# Documentation' not in help_str:
-            raise Exception("Help section is missing header: # Documentation")
-        if '## Setup' not in help_str:
-            raise Exception("Help section is missing header: ## Setup")
-        if '## Technical Details' not in help_str:
-            raise Exception("Help section is missing header: ## Technical Details")
-        if '## Troubleshooting' not in help_str:
-            raise Exception("Help section is missing header: ## Troubleshooting")
-        if '# Version History' not in help_str:
-            raise Exception("Help section is missing header: # Version History")
-        if '# Links' not in help_str:
-            raise Exception("Help section is missing header: # Links")
-        if '## References' not in help_str:
-            raise Exception("Help section is missing header: ## References")
+    def validate_workflow_vendor(spec):
+        if "vendor" not in spec.spec_dictionary():
+            raise ValidationException("Plugin vendor is missing.")
+        if not isinstance(spec.spec_dictionary()["vendor"], str):
+            raise ValidationException("Plugin vendor does not contain a string.")
 
     def validate(self, spec):
-        WorkflowHelpValidator.validate_help_exists(spec.spec_dictionary())
-        WorkflowHelpValidator.validate_help_headers(spec.raw_help())
-        WorkflowHelpValidator.validate_version_history(spec.raw_help())
+        WorkflowVendorValidator.validate_workflow_vendor(spec)
+        WorkflowVendorValidator.validate_vendor(spec.spec_dictionary()["vendor"])
+        WorkflowVendorValidator.validate_vendor_quotes(spec.raw_spec())
```

### Comparing `insightconnect_integrations_validators-2.8.1/icon_validator/validate.py` & `insightconnect_integrations_validators-2.9.0/icon_validator/validate.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,53 +1,56 @@
 #! /usr/bin/env python3
 
 import sys
 import traceback
 
 from icon_plugin_spec.plugin_spec import KomandPluginSpec
+from icon_validator.exceptions import ValidationException
 
 from .rules import VALIDATORS, JENKINS_VALIDATORS, WORKFLOW_VALIDATORS
 from .styling import *
 from .timing import *
 
 
-def validate(directory, spec_file_name='plugin.spec.yaml', fail_fast=False, run_all=False):
+# TODO refactor this into a class to allow for easier and better testing
+def validate(directory, spec_file_name="plugin.spec.yaml", fail_fast=False, run_all=False, validators=list()):
     spec = KomandPluginSpec(directory, spec_file_name)
     status = 0  # Resultant return code
-    validators = []
     start_time = time_now()
     print(f"{BULLET_OK} {BOLD}Running Integration Validators...{CEND}")
 
-    if spec_file_name == "plugin.spec.yaml":
-        validators = VALIDATORS
-        if run_all:
-            validators += JENKINS_VALIDATORS
-    elif spec_file_name == 'workflow.spec.yaml':
-        validators = WORKFLOW_VALIDATORS
+    if not validators:
+        if spec_file_name == "plugin.spec.yaml":
+            validators = VALIDATORS
+            if run_all:
+                validators += JENKINS_VALIDATORS
+        elif spec_file_name == "workflow.spec.yaml":
+            validators = WORKFLOW_VALIDATORS
 
     for v in validators:
         print(f"{BULLET_OK} Executing validator {v.name}")
         try:
             v.validate(spec)
             success = True
 
+        # TODO refactor to use ValidationException will require refactoring of all plugin validators first
         except Exception as e:
             print(f"Validator {v.name} failed!")
             ex_type, ex, tb = sys.exc_info()
             traceback.print_exception(Exception, e, tb)
             status = 1
             success = False
 
         if not success and fail_fast:
             break
 
     end_time = time_now()
     time_elapsed = format_time(start=start_time, end=end_time)
 
-    extension = spec_file_name.split('.')[0].capitalize()
+    extension = spec_file_name.split(".")[0].capitalize()
 
     if status == 0:
         print(f"{BULLET_OK} {BOLD}{extension} successfully validated!{CEND}")
     else:
         print(f"{BULLET_FAIL}{extension} failed validation!")
 
     print(f"\n----\n{BULLET_OK}{BOLD} Total time elapsed: {time_elapsed}ms{CEND}")
```

### Comparing `insightconnect_integrations_validators-2.8.1/insightconnect_integrations_validators.egg-info/PKG-INFO` & `insightconnect_integrations_validators-2.9.0/insightconnect_integrations_validators.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: insightconnect-integrations-validators
-Version: 2.8.1
+Version: 2.9.0
 Summary: Validator tooling for InsightConnect integrations
 Home-page: https://github.com/rapid7/icon-integrations-validators
 Author: Rapid7 Integrations Alliance
 Author-email: integrationalliance@rapid7.com
 License: MIT
 Description: 
         # InsightConnect Integrations Validators
@@ -53,14 +53,15 @@
         validate("/path/to/plugin/directory", run_all=True)
         ```
         
         to simulate the `--all` flag.
         
         ## Changelog
         
+        * 2.9.0 - Add unit testing support. Add support, workflow files, workflow vendor, workflow version, workflow changelog and workflow extension validators
         * 2.8.1 - Bug fix for URLValidator when opening files
         * 2.8.0 - Update ChangelogValidator to validate plugin's version history with latest version number |
         Update HelpInputOutputValidator error messaging
         * 2.7.0 - Add URL Validator
         * 2.6.9 - Update HelpInputOutputValidator to fix error messaging |
         Fix issue with HelpInputOutputValidator when help.md has action and trigger with same name
         * 2.6.8 - Docker Validator to run with -a command line argument | Helpful message on failure
```

### Comparing `insightconnect_integrations_validators-2.8.1/setup.py` & `insightconnect_integrations_validators-2.9.0/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,37 +1,37 @@
 #!/usr/bin/env python
 
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
-setup(name='insightconnect_integrations_validators',
-      version='2.8.1',
-      description='Validator tooling for InsightConnect integrations',
+setup(name="insightconnect_integrations_validators",
+      version="2.9.0",
+      description="Validator tooling for InsightConnect integrations",
       long_description=long_description,
       long_description_content_type="text/markdown",
-      author='Rapid7 Integrations Alliance',
-      author_email='integrationalliance@rapid7.com',
-      url='https://github.com/rapid7/icon-integrations-validators',
+      author="Rapid7 Integrations Alliance",
+      author_email="integrationalliance@rapid7.com",
+      url="https://github.com/rapid7/icon-integrations-validators",
       packages=find_packages(),
       install_requires=[
-          'python_jsonschema_objects==0.3.2',
-          'jsonschema==2.3.0',
-          'validators==0.12.1',
-          'filetype==1.0.0',
-          'pathlib==1.0.1',
-          'insightconnect-integrations-plugin-spec-tooling~=1.0',
-          'requests==2.22.0',
-          'urlextract==0.14.0',
-          'typing==3.7.4.1'
+          "python_jsonschema_objects==0.3.2",
+          "jsonschema==2.3.0",
+          "validators==0.12.1",
+          "filetype==1.0.0",
+          "pathlib==1.0.1",
+          "insightconnect-integrations-plugin-spec-tooling~=1.0",
+          "requests==2.22.0",
+          "urlextract==0.14.0",
+          "typing==3.7.4.1"
       ],
       entry_points={
-        'console_scripts': [
-            'icon-validate=icon_validator.__main__:main'
+        "console_scripts": [
+            "icon-validate=icon_validator.__main__:main"
         ]
       },
       classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
```

