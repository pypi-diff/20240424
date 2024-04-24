# Comparing `tmp/pulumi_onelogin-0.6.3a1713561172.tar.gz` & `tmp/pulumi_onelogin-0.6.3a1713902376.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_onelogin-0.6.3a1713561172.tar", last modified: Fri Apr 19 21:15:42 2024, max compression
+gzip compressed data, was "pulumi_onelogin-0.6.3a1713902376.tar", last modified: Wed Apr 24 17:24:38 2024, max compression
```

## Comparing `pulumi_onelogin-0.6.3a1713561172.tar` & `pulumi_onelogin-0.6.3a1713902376.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:42.429297 pulumi_onelogin-0.6.3a1713561172/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-19 21:15:42.429297 pulumi_onelogin-0.6.3a1713561172/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:42.421297 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   102325 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    46699 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:42.425297 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40858 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_actions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_actions_values.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_conditions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_conditions_operators.py
--rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_rules_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    31903 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    16458 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/auth_servers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:42.425297 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/config/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers.py
--rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers_claims.py
--rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers_scopes.py
--rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_privileges_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_risk_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_risk_rules_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    80388 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/privileges.py
--rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/risk_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/role.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:42.425297 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    24716 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_admins.py
--rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    65498 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/user.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:42.429297 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    23790 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_v1.py
--rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_v1_apps.py
--rw-r--r--   0 runner    (1001) docker     (127)    23915 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_v1_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    65455 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/v1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 21:15:42.429297 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-19 21:15:42.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-19 21:15:42.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 21:15:42.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-19 21:15:42.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 21:15:42.000000 pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-19 21:15:35.000000 pulumi_onelogin-0.6.3a1713561172/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 21:15:42.429297 pulumi_onelogin-0.6.3a1713561172/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:38.719400 pulumi_onelogin-0.6.3a1713902376/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-24 17:24:38.719400 pulumi_onelogin-0.6.3a1713902376/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2235 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:38.711400 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102325 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9248 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46699 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:38.715400 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40858 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4155 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_actions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_actions_values.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_conditions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_conditions_operators.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15328 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6557 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6262 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_rules_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24603 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31903 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16458 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9614 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/auth_servers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:38.715400 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4797 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15653 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4610 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9437 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers_claims.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4201 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers_scopes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6145 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4489 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_privileges_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_risk_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5655 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_risk_rules_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    80388 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7823 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/privileges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6039 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    15475 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/risk_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11413 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/role.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:38.715400 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3056 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24716 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_admins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4149 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4060 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4657 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24621 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2316 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65498 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/user.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:38.719400 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6440 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23658 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24069 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23790 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_v1.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7671 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_v1_apps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23915 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_v1_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2803 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65455 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/v1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 17:24:38.719400 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2695 2024-04-24 17:24:38.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-24 17:24:38.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 17:24:38.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-24 17:24:38.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 17:24:38.000000 pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 17:24:32.000000 pulumi_onelogin-0.6.3a1713902376/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 17:24:38.719400 pulumi_onelogin-0.6.3a1713902376/setup.cfg
```

### Comparing `pulumi_onelogin-0.6.3a1713561172/PKG-INFO` & `pulumi_onelogin-0.6.3a1713902376/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_onelogin
-Version: 0.6.3a1713561172
+Version: 0.6.3a1713902376
 Summary: A Pulumi package for creating and managing OneLogin cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-onelogin
 Keywords: pulumi,onelogin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_onelogin-0.6.3a1713561172/README.md` & `pulumi_onelogin-0.6.3a1713902376/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/__init__.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/_inputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/_utilities.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/app.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/app.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/__init__.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/_inputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_actions.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_actions.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_actions_values.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_actions_values.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_conditions.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_conditions.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_conditions_operators.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_conditions_operators.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_rules.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_rules_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_rules_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/get_users.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/outputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/apps/rules.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/apps/rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/auth_servers.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/auth_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/config/outputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/config/vars.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_apps.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers_claims.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers_claims.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_auth_servers_scopes.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_auth_servers_scopes.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_mappings.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_mappings.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_privileges.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_privileges.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_privileges_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_privileges_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_risk_rules.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_risk_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/get_risk_rules_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/get_risk_rules_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/outputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/privileges.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/privileges.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/provider.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/risk_rules.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/risk_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/role.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/_inputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_admins.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_admins.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_apps.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_roles.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/get_users.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/roles/outputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/roles/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/user.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/__init__.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/_inputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_apps.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_devices.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_devices.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_users.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_v1.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_v1_apps.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_v1_apps.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/get_v1_instance.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/get_v1_instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/outputs.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin/users/v1.py` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin/users/v1.py`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/PKG-INFO` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_onelogin
-Version: 0.6.3a1713561172
+Version: 0.6.3a1713902376
 Summary: A Pulumi package for creating and managing OneLogin cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-onelogin
 Keywords: pulumi,onelogin
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_onelogin-0.6.3a1713561172/pulumi_onelogin.egg-info/SOURCES.txt` & `pulumi_onelogin-0.6.3a1713902376/pulumi_onelogin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_onelogin-0.6.3a1713561172/pyproject.toml` & `pulumi_onelogin-0.6.3a1713902376/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_onelogin"
   description = "A Pulumi package for creating and managing OneLogin cloud resources."
   dependencies = ["parver>=0.2.1", "pulumi>=3.0.0,<4.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "onelogin"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.6.3a1713561172"
+  version = "0.6.3a1713902376"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.io"
     Repository = "https://github.com/pulumi/pulumi-onelogin"
 
 [build-system]
```

