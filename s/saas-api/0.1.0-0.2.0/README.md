# Comparing `tmp/saas_api-0.1.0.tar.gz` & `tmp/saas_api-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saas_api-0.1.0.tar", max compression
+gzip compressed data, was "saas_api-0.2.0.tar", max compression
```

## Comparing `saas_api-0.1.0.tar` & `saas_api-0.2.0.tar`

### file list

```diff
@@ -1,91 +1,107 @@
--rw-r--r--   0        0        0     1063 2024-04-22 11:13:40.769992 saas_api-0.1.0/LICENSE
--rw-r--r--   0        0        0      559 2024-04-22 11:13:40.769992 saas_api-0.1.0/README.md
--rw-r--r--   0        0        0      117 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/__init__.py
--rw-r--r--   0        0        0      178 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/__init__.py
--rw-r--r--   0        0        0       47 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/__init__.py
--rw-r--r--   0        0        0     4621 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/create_cluster.py
--rw-r--r--   0        0        0     3071 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py
--rw-r--r--   0        0        0     4393 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/get_cluster.py
--rw-r--r--   0        0        0     4573 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py
--rw-r--r--   0        0        0     4406 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/list_clusters.py
--rw-r--r--   0        0        0     3308 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py
--rw-r--r--   0        0        0     2932 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/start_cluster.py
--rw-r--r--   0        0        0     2927 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py
--rw-r--r--   0        0        0     3555 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/update_cluster.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/__init__.py
--rw-r--r--   0        0        0     4288 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/create_database.py
--rw-r--r--   0        0        0     2772 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/delete_database.py
--rw-r--r--   0        0        0     4085 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/get_database.py
--rw-r--r--   0        0        0     3998 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/list_databases.py
--rw-r--r--   0        0        0     2859 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/start_database.py
--rw-r--r--   0        0        0     2854 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/stop_database.py
--rw-r--r--   0        0        0     3119 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/databases/update_database.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/files/__init__.py
--rw-r--r--   0        0        0     2853 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/files/create_folder.py
--rw-r--r--   0        0        0     2874 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/files/delete_file.py
--rw-r--r--   0        0        0     2871 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/files/delete_folder.py
--rw-r--r--   0        0        0     4472 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/files/download_file.py
--rw-r--r--   0        0        0     4376 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/files/list_files.py
--rw-r--r--   0        0        0     4503 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/files/upload_file.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/platform/__init__.py
--rw-r--r--   0        0        0     4163 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py
--rw-r--r--   0        0        0     3640 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/platform/list_platforms.py
--rw-r--r--   0        0        0     4051 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/platform/list_regions.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/profile/__init__.py
--rw-r--r--   0        0        0     2743 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/profile/update_profile.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/security/__init__.py
--rw-r--r--   0        0        0     4450 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py
--rw-r--r--   0        0        0     2798 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py
--rw-r--r--   0        0        0     4011 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/security/get_allowed_ip.py
--rw-r--r--   0        0        0     4120 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py
--rw-r--r--   0        0        0     3079 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/security/update_allowed_ip.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/usage/__init__.py
--rw-r--r--   0        0        0     5024 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/usage/get_usage.py
--rw-r--r--   0        0        0        0 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/users/__init__.py
--rw-r--r--   0        0        0     2690 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/users/delete_user.py
--rw-r--r--   0        0        0     5423 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/users/list_users.py
--rw-r--r--   0        0        0     3014 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/api/users/patch_user.py
--rw-r--r--   0        0        0    12455 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/client.py
--rw-r--r--   0        0        0      546 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/errors.py
--rw-r--r--   0        0        0     2075 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/__init__.py
--rw-r--r--   0        0        0     2584 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/allowed_ip.py
--rw-r--r--   0        0        0     3009 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/api_error.py
--rw-r--r--   0        0        0     1371 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/api_error_causes.py
--rw-r--r--   0        0        0     1063 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/auto_stop.py
--rw-r--r--   0        0        0     3752 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/cluster.py
--rw-r--r--   0        0        0     1051 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/cluster_overview.py
--rw-r--r--   0        0        0     1639 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/cluster_size.py
--rw-r--r--   0        0        0     1143 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/connection_i_ps.py
--rw-r--r--   0        0        0     1734 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/connections.py
--rw-r--r--   0        0        0     1041 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/create_allowed_ip.py
--rw-r--r--   0        0        0     1786 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/create_cluster.py
--rw-r--r--   0        0        0     1722 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/create_database.py
--rw-r--r--   0        0        0     4463 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/database.py
--rw-r--r--   0        0        0      846 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/download_file.py
--rw-r--r--   0        0        0     2448 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/file.py
--rw-r--r--   0        0        0     2412 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/get_usage_response_200.py
--rw-r--r--   0        0        0      151 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/get_usage_type.py
--rw-r--r--   0        0        0     1205 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/integrations.py
--rw-r--r--   0        0        0     1105 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/patch_databases.py
--rw-r--r--   0        0        0     2108 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/patch_user.py
--rw-r--r--   0        0        0      961 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/platform.py
--rw-r--r--   0        0        0     4432 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/profile.py
--rw-r--r--   0        0        0     1453 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/region.py
--rw-r--r--   0        0        0      856 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/scale_cluster.py
--rw-r--r--   0        0        0      437 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/status.py
--rw-r--r--   0        0        0     1041 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/update_allowed_ip.py
--rw-r--r--   0        0        0     1643 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/update_cluster.py
--rw-r--r--   0        0        0      864 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/update_database.py
--rw-r--r--   0        0        0     1109 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/update_profile.py
--rw-r--r--   0        0        0      838 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/upload_file.py
--rw-r--r--   0        0        0     2469 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/usage_cluster.py
--rw-r--r--   0        0        0     2064 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/usage_database.py
--rw-r--r--   0        0        0      979 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/user_database.py
--rw-r--r--   0        0        0      963 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/user_role.py
--rw-r--r--   0        0        0      193 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/models/user_status.py
--rw-r--r--   0        0        0       25 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/py.typed
--rw-r--r--   0        0        0     1034 2024-04-22 11:13:40.773992 saas_api-0.1.0/exasol/saas/client/openapi/types.py
--rw-r--r--   0        0        0     1982 2024-04-22 11:13:40.777992 saas_api-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1961 1970-01-01 00:00:00.000000 saas_api-0.1.0/setup.py
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 saas_api-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1063 2024-04-24 14:07:40.682982 saas_api-0.2.0/LICENSE
+-rw-r--r--   0        0        0      559 2024-04-24 14:07:40.682982 saas_api-0.2.0/README.md
+-rw-r--r--   0        0        0      117 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/__init__.py
+-rw-r--r--   0        0        0      178 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/__init__.py
+-rw-r--r--   0        0        0       47 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/__init__.py
+-rw-r--r--   0        0        0     4453 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/create_cluster.py
+-rw-r--r--   0        0        0     2861 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py
+-rw-r--r--   0        0        0     4273 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/get_cluster.py
+-rw-r--r--   0        0        0     4412 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py
+-rw-r--r--   0        0        0     4206 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/list_clusters.py
+-rw-r--r--   0        0        0     3240 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py
+-rw-r--r--   0        0        0     2864 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/start_cluster.py
+-rw-r--r--   0        0        0     2863 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py
+-rw-r--r--   0        0        0     3241 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/update_cluster.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/__init__.py
+-rw-r--r--   0        0        0     4112 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/create_database.py
+-rw-r--r--   0        0        0     2656 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/delete_database.py
+-rw-r--r--   0        0        0     3941 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/get_database.py
+-rw-r--r--   0        0        0     3854 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/list_databases.py
+-rw-r--r--   0        0        0     2659 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/start_database.py
+-rw-r--r--   0        0        0     2658 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/stop_database.py
+-rw-r--r--   0        0        0     3043 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/databases/update_database.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/__init__.py
+-rw-r--r--   0        0        0     5559 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/create_extension_instance.py
+-rw-r--r--   0        0        0     3385 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/delete_extension_instance.py
+-rw-r--r--   0        0        0     4896 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/get_extension.py
+-rw-r--r--   0        0        0     3172 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/install_extension.py
+-rw-r--r--   0        0        0     5201 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/list_extension_instances.py
+-rw-r--r--   0        0        0     4234 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/list_extensions.py
+-rw-r--r--   0        0        0     3174 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/uninstall_extension.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/files/__init__.py
+-rw-r--r--   0        0        0     2773 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/files/create_folder.py
+-rw-r--r--   0        0        0     2774 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/files/delete_file.py
+-rw-r--r--   0        0        0     2775 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/files/delete_folder.py
+-rw-r--r--   0        0        0     4205 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/files/download_file.py
+-rw-r--r--   0        0        0     4164 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/files/list_files.py
+-rw-r--r--   0        0        0     4171 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/files/upload_file.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/platform/__init__.py
+-rw-r--r--   0        0        0     3851 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py
+-rw-r--r--   0        0        0     3460 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/platform/list_platforms.py
+-rw-r--r--   0        0        0     3787 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/platform/list_regions.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/profile/__init__.py
+-rw-r--r--   0        0        0     2607 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/profile/update_profile.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/security/__init__.py
+-rw-r--r--   0        0        0     4150 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py
+-rw-r--r--   0        0        0     2716 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py
+-rw-r--r--   0        0        0     4047 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/security/get_allowed_ip.py
+-rw-r--r--   0        0        0     3880 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py
+-rw-r--r--   0        0        0     3111 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/security/update_allowed_ip.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/usage/__init__.py
+-rw-r--r--   0        0        0     4841 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/usage/get_usage.py
+-rw-r--r--   0        0        0        0 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/users/__init__.py
+-rw-r--r--   0        0        0     2604 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/users/delete_user.py
+-rw-r--r--   0        0        0     3814 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/users/get_user.py
+-rw-r--r--   0        0        0     5224 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/users/list_users.py
+-rw-r--r--   0        0        0     2958 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/api/users/patch_user.py
+-rw-r--r--   0        0        0    12455 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/client.py
+-rw-r--r--   0        0        0      546 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/errors.py
+-rw-r--r--   0        0        0     2747 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/__init__.py
+-rw-r--r--   0        0        0     2584 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/allowed_ip.py
+-rw-r--r--   0        0        0     2332 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/api_error.py
+-rw-r--r--   0        0        0     1063 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/auto_stop.py
+-rw-r--r--   0        0        0     3752 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/cluster.py
+-rw-r--r--   0        0        0     1760 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/cluster_connection.py
+-rw-r--r--   0        0        0     1639 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/cluster_size.py
+-rw-r--r--   0        0        0     1143 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/connection_i_ps.py
+-rw-r--r--   0        0        0     1041 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/create_allowed_ip.py
+-rw-r--r--   0        0        0     1786 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/create_cluster.py
+-rw-r--r--   0        0        0     2607 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/create_database.py
+-rw-r--r--   0        0        0     1850 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/create_database_initial_cluster.py
+-rw-r--r--   0        0        0     1787 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/create_extension_instance.py
+-rw-r--r--   0        0        0     5263 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/database.py
+-rw-r--r--   0        0        0     1055 2024-04-24 14:07:40.682982 saas_api-0.2.0/exasol/saas/client/openapi/models/database_clusters.py
+-rw-r--r--   0        0        0     1962 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/database_integrations_item.py
+-rw-r--r--   0        0        0      846 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/download_file.py
+-rw-r--r--   0        0        0     2439 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/extension.py
+-rw-r--r--   0        0        0     2263 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/extension_detail.py
+-rw-r--r--   0        0        0      999 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/extension_instance.py
+-rw-r--r--   0        0        0     1396 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/extension_parameter_definitions.py
+-rw-r--r--   0        0        0     1035 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/extension_parameter_value.py
+-rw-r--r--   0        0        0     1467 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/extension_version.py
+-rw-r--r--   0        0        0     2448 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/file.py
+-rw-r--r--   0        0        0      151 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/get_usage_type.py
+-rw-r--r--   0        0        0     2151 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/patch_user.py
+-rw-r--r--   0        0        0     1123 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/patch_user_databases.py
+-rw-r--r--   0        0        0      961 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/platform.py
+-rw-r--r--   0        0        0     1453 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/region.py
+-rw-r--r--   0        0        0      856 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/scale_cluster.py
+-rw-r--r--   0        0        0      485 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/status.py
+-rw-r--r--   0        0        0     1041 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/update_allowed_ip.py
+-rw-r--r--   0        0        0     1643 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/update_cluster.py
+-rw-r--r--   0        0        0     1558 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/update_database.py
+-rw-r--r--   0        0        0     1109 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/update_profile.py
+-rw-r--r--   0        0        0      838 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/upload_file.py
+-rw-r--r--   0        0        0     2479 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/usage.py
+-rw-r--r--   0        0        0     2124 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/usage_additional_property_item.py
+-rw-r--r--   0        0        0     2469 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/usage_cluster.py
+-rw-r--r--   0        0        0     4420 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/user.py
+-rw-r--r--   0        0        0      979 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/user_database.py
+-rw-r--r--   0        0        0      963 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/user_role.py
+-rw-r--r--   0        0        0      193 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/models/user_status.py
+-rw-r--r--   0        0        0       25 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/py.typed
+-rw-r--r--   0        0        0     1034 2024-04-24 14:07:40.686982 saas_api-0.2.0/exasol/saas/client/openapi/types.py
+-rw-r--r--   0        0        0     1982 2024-04-24 14:07:40.686982 saas_api-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2007 1970-01-01 00:00:00.000000 saas_api-0.2.0/setup.py
+-rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 saas_api-0.2.0/PKG-INFO
```

### Comparing `saas_api-0.1.0/LICENSE` & `saas_api-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/README.md` & `saas_api-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/create_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/create_cluster.py`

 * *Files 9% similar despite different names*

```diff
@@ -78,18 +78,15 @@
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateCluster,
 
 ) -> Response[Cluster]:
-    """ Create cluster
-
-     Create a new cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         body (CreateCluster):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -117,18 +114,15 @@
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateCluster,
 
 ) -> Optional[Cluster]:
-    """ Create cluster
-
-     Create a new cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         body (CreateCluster):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -151,18 +145,15 @@
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateCluster,
 
 ) -> Response[Cluster]:
-    """ Create cluster
-
-     Create a new cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         body (CreateCluster):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -190,18 +181,15 @@
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateCluster,
 
 ) -> Optional[Cluster]:
-    """ Create cluster
-
-     Create a new cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         body (CreateCluster):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/start_cluster.py`

 * *Files 5% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "delete",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/clusters/{cluster_id}".format(account_id=account_id,database_id=database_id,cluster_id=cluster_id,),
+        "method": "put",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/clusters/{cluster_id}/start".format(account_id=account_id,database_id=database_id,cluster_id=cluster_id,),
     }
 
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
@@ -64,18 +64,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete cluster
-
-     Delete the cluster, if main cluster is deleted, the whole database will be deleted.
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -104,18 +101,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete cluster
-
-     Delete the cluster, if main cluster is deleted, the whole database will be deleted.
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/get_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/get_cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,18 +69,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Cluster]:
-    """ Get cluster
-
-     Get cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -108,18 +105,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[Cluster]:
-    """ Get cluster
-
-     Get cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -142,18 +136,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Cluster]:
-    """ Get cluster
-
-     Get cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -181,18 +172,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[Cluster]:
-    """ Get cluster
-
-     Get cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/get_cluster_connection.py`

 * *Files 16% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.connections import Connections
+from ...models.cluster_connection import ClusterConnection
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
@@ -39,28 +39,28 @@
         "url": "/api/v1/accounts/{account_id}/databases/{database_id}/clusters/{cluster_id}/connect".format(account_id=account_id,database_id=database_id,cluster_id=cluster_id,),
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Connections]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[ClusterConnection]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Connections.from_dict(response.json())
+        response_200 = ClusterConnection.from_dict(response.json())
 
 
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Connections]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[ClusterConnection]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
@@ -68,30 +68,27 @@
 def sync_detailed(
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[Connections]:
-    """ Get connection information
-
-     Get connection information
-
+) -> Response[ClusterConnection]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Connections]
+        Response[ClusterConnection]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
 cluster_id=cluster_id,
@@ -107,30 +104,27 @@
 def sync(
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[Connections]:
-    """ Get connection information
-
-     Get connection information
-
+) -> Optional[ClusterConnection]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Connections
+        ClusterConnection
      """
 
 
     return sync_detailed(
         account_id=account_id,
 database_id=database_id,
 cluster_id=cluster_id,
@@ -141,30 +135,27 @@
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[Connections]:
-    """ Get connection information
-
-     Get connection information
-
+) -> Response[ClusterConnection]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Connections]
+        Response[ClusterConnection]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
 cluster_id=cluster_id,
@@ -180,30 +171,27 @@
 async def asyncio(
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[Connections]:
-    """ Get connection information
-
-     Get connection information
-
+) -> Optional[ClusterConnection]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Connections
+        ClusterConnection
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
 database_id=database_id,
 cluster_id=cluster_id,
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/list_clusters.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/list_clusters.py`

 * *Files 8% similar despite different names*

```diff
@@ -72,18 +72,15 @@
 def sync_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[List['Cluster']]:
-    """ List clusters
-
-     List clusters from a database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -108,18 +105,15 @@
 def sync(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[List['Cluster']]:
-    """ List clusters
-
-     List clusters from a database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -139,18 +133,15 @@
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[List['Cluster']]:
-    """ List clusters
-
-     List clusters from a database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -175,18 +166,15 @@
 async def asyncio(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[List['Cluster']]:
-    """ List clusters
-
-     List clusters from a database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/scale_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,18 +75,15 @@
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
     body: ScaleCluster,
 
 ) -> Response[Any]:
-    """ Scale cluster
-
-     Scale cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
         body (ScaleCluster):
 
     Raises:
@@ -118,18 +115,15 @@
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
     body: ScaleCluster,
 
 ) -> Response[Any]:
-    """ Scale cluster
-
-     Scale cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
         body (ScaleCluster):
 
     Raises:
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/start_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/delete_cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/clusters/{cluster_id}/start".format(account_id=account_id,database_id=database_id,cluster_id=cluster_id,),
+        "method": "delete",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/clusters/{cluster_id}".format(account_id=account_id,database_id=database_id,cluster_id=cluster_id,),
     }
 
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
@@ -64,18 +64,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Start cluster
-
-     Start cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -104,18 +101,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Start cluster
-
-     Start cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/stop_cluster.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,18 +64,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Stop cluster
-
-     Stop cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
@@ -104,18 +101,15 @@
     account_id: str,
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Stop cluster
-
-     Stop cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/clusters/update_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/clusters/update_cluster.py`

 * *Files 8% similar despite different names*

```diff
@@ -75,19 +75,15 @@
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
     body: UpdateCluster,
 
 ) -> Response[Any]:
-    """ Update cluster
-
-     Update the cluster with the specified ID.
-     Only metadata can be changed. To scale the cluster size, use the scale cluster endpoint.
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
         body (UpdateCluster):
 
     Raises:
@@ -119,19 +115,15 @@
     database_id: str,
     cluster_id: str,
     *,
     client: AuthenticatedClient,
     body: UpdateCluster,
 
 ) -> Response[Any]:
-    """ Update cluster
-
-     Update the cluster with the specified ID.
-     Only metadata can be changed. To scale the cluster size, use the scale cluster endpoint.
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
         cluster_id (str):
         body (UpdateCluster):
 
     Raises:
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/databases/create_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/databases/create_database.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,18 +76,15 @@
 def sync_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateDatabase,
 
 ) -> Response[Database]:
-    """ Create database
-
-     Create a new database
-
+    """ 
     Args:
         account_id (str):
         body (CreateDatabase):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -112,18 +109,15 @@
 def sync(
     account_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateDatabase,
 
 ) -> Optional[Database]:
-    """ Create database
-
-     Create a new database
-
+    """ 
     Args:
         account_id (str):
         body (CreateDatabase):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -143,18 +137,15 @@
 async def asyncio_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateDatabase,
 
 ) -> Response[Database]:
-    """ Create database
-
-     Create a new database
-
+    """ 
     Args:
         account_id (str):
         body (CreateDatabase):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -179,18 +170,15 @@
 async def asyncio(
     account_id: str,
     *,
     client: AuthenticatedClient,
     body: CreateDatabase,
 
 ) -> Optional[Database]:
-    """ Create database
-
-     Create a new database
-
+    """ 
     Args:
         account_id (str):
         body (CreateDatabase):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/databases/delete_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/databases/delete_database.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,18 +62,15 @@
 def sync_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete database
-
-     Delete the database and all cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -99,18 +96,15 @@
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete database
-
-     Delete the database and all cluster
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/databases/get_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/files/upload_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,189 +11,190 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.database import Database
+from ...models.upload_file import UploadFile
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
+    key: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "get",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}".format(account_id=account_id,database_id=database_id,),
+        "method": "post",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/files/{key}".format(account_id=account_id,database_id=database_id,key=key,),
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Database]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[UploadFile]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = Database.from_dict(response.json())
+        response_200 = UploadFile.from_dict(response.json())
 
 
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Database]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[UploadFile]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[Database]:
-    """ Get database
-
-     Get the database
-
+) -> Response[UploadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Database]
+        Response[UploadFile]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
+key=key,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[Database]:
-    """ Get database
-
-     Get the database
-
+) -> Optional[UploadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Database
+        UploadFile
      """
 
 
     return sync_detailed(
         account_id=account_id,
 database_id=database_id,
+key=key,
 client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[Database]:
-    """ Get database
-
-     Get the database
-
+) -> Response[UploadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Database]
+        Response[UploadFile]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
+key=key,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[Database]:
-    """ Get database
-
-     Get the database
-
+) -> Optional[UploadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Database
+        UploadFile
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
 database_id=database_id,
+key=key,
 client=client,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/databases/list_databases.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/databases/list_databases.py`

 * *Files 5% similar despite different names*

```diff
@@ -70,18 +70,15 @@
 
 def sync_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[List['Database']]:
-    """ List databases
-
-     List databases
-
+    """ 
     Args:
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -103,18 +100,15 @@
 
 def sync(
     account_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[List['Database']]:
-    """ List databases
-
-     List databases
-
+    """ 
     Args:
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -131,18 +125,15 @@
 
 async def asyncio_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[List['Database']]:
-    """ List databases
-
-     List databases
-
+    """ 
     Args:
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -164,18 +155,15 @@
 
 async def asyncio(
     account_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[List['Database']]:
-    """ List databases
-
-     List databases
-
+    """ 
     Args:
         account_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/databases/start_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/databases/start_database.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,19 +62,15 @@
 def sync_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Start database
-
-     Start database
-    If database is from type main, workers will be also started
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -100,19 +96,15 @@
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Start database
-
-     Start database
-    If database is from type main, workers will be also started
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/databases/stop_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/databases/stop_database.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,19 +62,15 @@
 def sync_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Stop database
-
-     Stop database
-    If database is from type main, workers will be also stopped
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -100,19 +96,15 @@
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Stop database
-
-     Stop database
-    If database is from type main, workers will be also stopped
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/databases/update_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/files/delete_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,47 +11,38 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.update_database import UpdateDatabase
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
-    *,
-    body: UpdateDatabase,
+    key: str,
 
 ) -> Dict[str, Any]:
-    headers: Dict[str, Any] = {}
-
+    
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}".format(account_id=account_id,database_id=database_id,),
+        "method": "delete",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/files/{key}".format(account_id=account_id,database_id=database_id,key=key,),
     }
 
-    _body = body.to_dict()
-
-
-    _kwargs["json"] = _body
-    headers["Content-Type"] = "application/json"
 
-    _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.NO_CONTENT:
         return None
     if client.raise_on_unexpected_status:
@@ -68,81 +59,75 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
-    body: UpdateDatabase,
 
 ) -> Response[Any]:
-    """ Update database
-
-     Update database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        body (UpdateDatabase):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-body=body,
+key=key,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
-    body: UpdateDatabase,
 
 ) -> Response[Any]:
-    """ Update database
-
-     Update database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        body (UpdateDatabase):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-body=body,
+key=key,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/files/create_folder.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/files/delete_folder.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
-    path: str,
+    key: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/folder/{path}".format(account_id=account_id,database_id=database_id,path=path,),
+        "method": "delete",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/folder/{key}".format(account_id=account_id,database_id=database_id,key=key,),
     }
 
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
@@ -59,81 +59,75 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
-    path: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Create folder
-
-     Create folder
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
+key=key,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
-    path: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Create folder
-
-     Create folder
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
+key=key,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/files/delete_file.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/files/create_folder.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,26 +20,26 @@
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
-    path: str,
+    key: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "delete",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/files/{path}".format(account_id=account_id,database_id=database_id,path=path,),
+        "method": "post",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/folder/{key}".format(account_id=account_id,database_id=database_id,key=key,),
     }
 
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
@@ -59,81 +59,75 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
-    path: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete file
-
-     Delete file from database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
+key=key,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
-    path: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete file
-
-     Delete file from database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
+key=key,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/files/delete_folder.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/databases/update_database.py`

 * *Files 12% similar despite different names*

```diff
@@ -11,38 +11,47 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
+from ...models.update_database import UpdateDatabase
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
-    key: str,
+    *,
+    body: UpdateDatabase,
 
 ) -> Dict[str, Any]:
-    
+    headers: Dict[str, Any] = {}
+
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "delete",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/folder/{key}".format(account_id=account_id,database_id=database_id,key=key,),
+        "method": "put",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}".format(account_id=account_id,database_id=database_id,),
     }
 
+    _body = body.to_dict()
+
+
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
 
+    _kwargs["headers"] = headers
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
     if response.status_code == HTTPStatus.NO_CONTENT:
         return None
     if client.raise_on_unexpected_status:
@@ -59,81 +68,75 @@
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
-    key: str,
     *,
     client: AuthenticatedClient,
+    body: UpdateDatabase,
 
 ) -> Response[Any]:
-    """ Delete folder
-
-     Delete folder from database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        key (str):
+        body (UpdateDatabase):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-key=key,
+body=body,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
-    key: str,
     *,
     client: AuthenticatedClient,
+    body: UpdateDatabase,
 
 ) -> Response[Any]:
-    """ Delete folder
-
-     Delete folder from database
-
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        key (str):
+        body (UpdateDatabase):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-key=key,
+body=body,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/files/download_file.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/files/list_files.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,202 +11,182 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.download_file import DownloadFile
+from ...models.file import File
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
-    path: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/files/{path}".format(account_id=account_id,database_id=database_id,path=path,),
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/files".format(account_id=account_id,database_id=database_id,),
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[DownloadFile]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['File']]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = DownloadFile.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in (_response_200):
+            response_200_item = File.from_dict(response_200_item_data)
 
 
 
+            response_200.append(response_200_item)
+
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[DownloadFile]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['File']]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[DownloadFile]:
-    """ Download file
-
-     Download file from bucket via one time link
-
+) -> Response[List['File']]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[DownloadFile]
+        Response[List['File']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[DownloadFile]:
-    """ Download file
-
-     Download file from bucket via one time link
-
+) -> Optional[List['File']]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        DownloadFile
+        List['File']
      """
 
 
     return sync_detailed(
         account_id=account_id,
 database_id=database_id,
-path=path,
 client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[DownloadFile]:
-    """ Download file
-
-     Download file from bucket via one time link
-
+) -> Response[List['File']]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[DownloadFile]
+        Response[List['File']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[DownloadFile]:
-    """ Download file
-
-     Download file from bucket via one time link
-
+) -> Optional[List['File']]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        DownloadFile
+        List['File']
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
 database_id=database_id,
-path=path,
 client=client,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/files/list_files.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/files/download_file.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,194 +11,190 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.file import File
+from ...models.download_file import DownloadFile
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
+    key: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/files".format(account_id=account_id,database_id=database_id,),
+        "url": "/api/v1/internal/accounts/{account_id}/databases/{database_id}/files/{key}".format(account_id=account_id,database_id=database_id,key=key,),
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['File']]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[DownloadFile]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in (_response_200):
-            response_200_item = File.from_dict(response_200_item_data)
+        response_200 = DownloadFile.from_dict(response.json())
 
 
 
-            response_200.append(response_200_item)
-
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['File']]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[DownloadFile]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[List['File']]:
-    """ List files
-
-     List files uploaded to the database
-
+) -> Response[DownloadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['File']]
+        Response[DownloadFile]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
+key=key,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[List['File']]:
-    """ List files
-
-     List files uploaded to the database
-
+) -> Optional[DownloadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['File']
+        DownloadFile
      """
 
 
     return sync_detailed(
         account_id=account_id,
 database_id=database_id,
+key=key,
 client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[List['File']]:
-    """ List files
-
-     List files uploaded to the database
-
+) -> Response[DownloadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['File']]
+        Response[DownloadFile]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
+key=key,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
     database_id: str,
+    key: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[List['File']]:
-    """ List files
-
-     List files uploaded to the database
-
+) -> Optional[DownloadFile]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
+        key (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['File']
+        DownloadFile
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
 database_id=database_id,
+key=key,
 client=client,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/files/upload_file.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/databases/get_database.py`

 * *Files 13% similar despite different names*

```diff
@@ -11,202 +11,177 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.upload_file import UploadFile
+from ...models.database import Database
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     database_id: str,
-    path: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/files/{path}".format(account_id=account_id,database_id=database_id,path=path,),
+        "method": "get",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}".format(account_id=account_id,database_id=database_id,),
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[UploadFile]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Database]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = UploadFile.from_dict(response.json())
+        response_200 = Database.from_dict(response.json())
 
 
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[UploadFile]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Database]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[UploadFile]:
-    """ Get upload file url
-
-     Get one time url to upload any file to the database
-
+) -> Response[Database]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[UploadFile]
+        Response[Database]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[UploadFile]:
-    """ Get upload file url
-
-     Get one time url to upload any file to the database
-
+) -> Optional[Database]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        UploadFile
+        Database
      """
 
 
     return sync_detailed(
         account_id=account_id,
 database_id=database_id,
-path=path,
 client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[UploadFile]:
-    """ Get upload file url
-
-     Get one time url to upload any file to the database
-
+) -> Response[Database]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[UploadFile]
+        Response[Database]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 database_id=database_id,
-path=path,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
     database_id: str,
-    path: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[UploadFile]:
-    """ Get upload file url
-
-     Get one time url to upload any file to the database
-
+) -> Optional[Database]:
+    """ 
     Args:
         account_id (str):
         database_id (str):
-        path (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        UploadFile
+        Database
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
 database_id=database_id,
-path=path,
 client=client,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/platform/list_cluster_sizes.py`

 * *Files 16% similar despite different names*

```diff
@@ -70,18 +70,15 @@
 
 def sync_detailed(
     platform: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[List['ClusterSize']]:
-    """ Get cluster sizes for platform
-
-     Get available cluster sizes for platform
-
+    """ 
     Args:
         platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -103,18 +100,15 @@
 
 def sync(
     platform: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[List['ClusterSize']]:
-    """ Get cluster sizes for platform
-
-     Get available cluster sizes for platform
-
+    """ 
     Args:
         platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -131,18 +125,15 @@
 
 async def asyncio_detailed(
     platform: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[List['ClusterSize']]:
-    """ Get cluster sizes for platform
-
-     Get available cluster sizes for platform
-
+    """ 
     Args:
         platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -164,18 +155,15 @@
 
 async def asyncio(
     platform: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Optional[List['ClusterSize']]:
-    """ Get cluster sizes for platform
-
-     Get available cluster sizes for platform
-
+    """ 
     Args:
         platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/platform/list_platforms.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/platform/list_regions.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,160 +11,169 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.platform import Platform
+from ...models.region import Region
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
-    
+    platform: str,
+
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/v1/platforms",
+        "url": "/api/v1/platforms/{platform}/regions".format(platform=platform,),
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['Platform']]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['Region']]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in (_response_200):
-            response_200_item = Platform.from_dict(response_200_item_data)
+            response_200_item = Region.from_dict(response_200_item_data)
 
 
 
             response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['Platform']]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['Region']]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
+    platform: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[List['Platform']]:
-    """ List platforms
-
-     Get available platforms
+) -> Response[List['Region']]:
+    """ 
+    Args:
+        platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['Platform']]
+        Response[List['Region']]
      """
 
 
     kwargs = _get_kwargs(
-        
+        platform=platform,
+
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
+    platform: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[List['Platform']]:
-    """ List platforms
-
-     Get available platforms
+) -> Optional[List['Region']]:
+    """ 
+    Args:
+        platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['Platform']
+        List['Region']
      """
 
 
     return sync_detailed(
-        client=client,
+        platform=platform,
+client=client,
 
     ).parsed
 
 async def asyncio_detailed(
+    platform: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[List['Platform']]:
-    """ List platforms
-
-     Get available platforms
+) -> Response[List['Region']]:
+    """ 
+    Args:
+        platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['Platform']]
+        Response[List['Region']]
      """
 
 
     kwargs = _get_kwargs(
-        
+        platform=platform,
+
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
+    platform: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[List['Platform']]:
-    """ List platforms
-
-     Get available platforms
+) -> Optional[List['Region']]:
+    """ 
+    Args:
+        platform (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['Platform']
+        List['Region']
      """
 
 
     return (await asyncio_detailed(
-        client=client,
+        platform=platform,
+client=client,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/platform/list_regions.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,181 +11,186 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.region import Region
+from ...models.allowed_ip import AllowedIP
+from ...models.create_allowed_ip import CreateAllowedIP
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
-    platform: str,
+    account_id: str,
+    *,
+    body: CreateAllowedIP,
 
 ) -> Dict[str, Any]:
-    
+    headers: Dict[str, Any] = {}
+
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "get",
-        "url": "/api/v1/platforms/{platform}/regions".format(platform=platform,),
+        "method": "post",
+        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip".format(account_id=account_id,),
     }
 
+    _body = body.to_dict()
+
 
+    _kwargs["json"] = _body
+    headers["Content-Type"] = "application/json"
+
+    _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['Region']]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[AllowedIP]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in (_response_200):
-            response_200_item = Region.from_dict(response_200_item_data)
-
+        response_200 = AllowedIP.from_dict(response.json())
 
 
-            response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['Region']]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[AllowedIP]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    platform: str,
+    account_id: str,
     *,
     client: AuthenticatedClient,
+    body: CreateAllowedIP,
 
-) -> Response[List['Region']]:
-    """ Get regions for platform
-
-     Get available regions for platform
-
+) -> Response[AllowedIP]:
+    """ 
     Args:
-        platform (str):
+        account_id (str):
+        body (CreateAllowedIP):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['Region']]
+        Response[AllowedIP]
      """
 
 
     kwargs = _get_kwargs(
-        platform=platform,
+        account_id=account_id,
+body=body,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
-    platform: str,
+    account_id: str,
     *,
     client: AuthenticatedClient,
+    body: CreateAllowedIP,
 
-) -> Optional[List['Region']]:
-    """ Get regions for platform
-
-     Get available regions for platform
-
+) -> Optional[AllowedIP]:
+    """ 
     Args:
-        platform (str):
+        account_id (str):
+        body (CreateAllowedIP):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['Region']
+        AllowedIP
      """
 
 
     return sync_detailed(
-        platform=platform,
+        account_id=account_id,
 client=client,
+body=body,
 
     ).parsed
 
 async def asyncio_detailed(
-    platform: str,
+    account_id: str,
     *,
     client: AuthenticatedClient,
+    body: CreateAllowedIP,
 
-) -> Response[List['Region']]:
-    """ Get regions for platform
-
-     Get available regions for platform
-
+) -> Response[AllowedIP]:
+    """ 
     Args:
-        platform (str):
+        account_id (str):
+        body (CreateAllowedIP):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['Region']]
+        Response[AllowedIP]
      """
 
 
     kwargs = _get_kwargs(
-        platform=platform,
+        account_id=account_id,
+body=body,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
-    platform: str,
+    account_id: str,
     *,
     client: AuthenticatedClient,
+    body: CreateAllowedIP,
 
-) -> Optional[List['Region']]:
-    """ Get regions for platform
-
-     Get available regions for platform
-
+) -> Optional[AllowedIP]:
+    """ 
     Args:
-        platform (str):
+        account_id (str):
+        body (CreateAllowedIP):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['Region']
+        AllowedIP
      """
 
 
     return (await asyncio_detailed(
-        platform=platform,
+        account_id=account_id,
 client=client,
+body=body,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/profile/update_profile.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/profile/update_profile.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,18 +69,15 @@
 
 def sync_detailed(
     *,
     client: AuthenticatedClient,
     body: UpdateProfile,
 
 ) -> Response[Any]:
-    """ Update user profile
-
-     Set first and last name of a user profile
-
+    """ 
     Args:
         body (UpdateProfile):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
@@ -103,18 +100,15 @@
 
 async def asyncio_detailed(
     *,
     client: AuthenticatedClient,
     body: UpdateProfile,
 
 ) -> Response[Any]:
-    """ Update user profile
-
-     Set first and last name of a user profile
-
+    """ 
     Args:
         body (UpdateProfile):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/security/add_allowed_ip.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/extensions/list_extensions.py`

 * *Files 15% similar despite different names*

```diff
@@ -11,198 +11,182 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.allowed_ip import AllowedIP
-from ...models.create_allowed_ip import CreateAllowedIP
+from ...models.extension import Extension
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
-    *,
-    body: CreateAllowedIP,
+    database_id: str,
 
 ) -> Dict[str, Any]:
-    headers: Dict[str, Any] = {}
-
+    
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "post",
-        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip".format(account_id=account_id,),
+        "method": "get",
+        "url": "/api/v1/accounts/{account_id}/databases/{database_id}/extensions".format(account_id=account_id,database_id=database_id,),
     }
 
-    _body = body.to_dict()
-
 
-    _kwargs["json"] = _body
-    headers["Content-Type"] = "application/json"
-
-    _kwargs["headers"] = headers
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[AllowedIP]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['Extension']]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = AllowedIP.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in (_response_200):
+            response_200_item = Extension.from_dict(response_200_item_data)
+
 
 
+            response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[AllowedIP]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['Extension']]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
+    database_id: str,
     *,
     client: AuthenticatedClient,
-    body: CreateAllowedIP,
-
-) -> Response[AllowedIP]:
-    """ Add security rule (CIDR)
-
-     Add security rule to allow access from CIDR
 
+) -> Response[List['Extension']]:
+    """ 
     Args:
         account_id (str):
-        body (CreateAllowedIP):
+        database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[AllowedIP]
+        Response[List['Extension']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-body=body,
+database_id=database_id,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
+    database_id: str,
     *,
     client: AuthenticatedClient,
-    body: CreateAllowedIP,
-
-) -> Optional[AllowedIP]:
-    """ Add security rule (CIDR)
-
-     Add security rule to allow access from CIDR
 
+) -> Optional[List['Extension']]:
+    """ 
     Args:
         account_id (str):
-        body (CreateAllowedIP):
+        database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        AllowedIP
+        List['Extension']
      """
 
 
     return sync_detailed(
         account_id=account_id,
+database_id=database_id,
 client=client,
-body=body,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
+    database_id: str,
     *,
     client: AuthenticatedClient,
-    body: CreateAllowedIP,
-
-) -> Response[AllowedIP]:
-    """ Add security rule (CIDR)
-
-     Add security rule to allow access from CIDR
 
+) -> Response[List['Extension']]:
+    """ 
     Args:
         account_id (str):
-        body (CreateAllowedIP):
+        database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[AllowedIP]
+        Response[List['Extension']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-body=body,
+database_id=database_id,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
+    database_id: str,
     *,
     client: AuthenticatedClient,
-    body: CreateAllowedIP,
-
-) -> Optional[AllowedIP]:
-    """ Add security rule (CIDR)
-
-     Add security rule to allow access from CIDR
 
+) -> Optional[List['Extension']]:
+    """ 
     Args:
         account_id (str):
-        body (CreateAllowedIP):
+        database_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        AllowedIP
+        List['Extension']
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
+database_id=database_id,
 client=client,
-body=body,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/security/delete_allowed_ip.py`

 * *Files 12% similar despite different names*

```diff
@@ -19,26 +19,26 @@
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
-    id: str,
+    allowlist_ip_id: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
         "method": "delete",
-        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip/{id}".format(account_id=account_id,id=id,),
+        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip/{allowlist_ip_id}".format(account_id=account_id,allowlist_ip_id=allowlist_ip_id,),
     }
 
 
     return _kwargs
 
 
 def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
@@ -57,76 +57,70 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
-    id: str,
+    allowlist_ip_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete security rule (CIDR)
-
-     Delete security rule (CIDR). No access to database possible after deletion from CIDR
-
+    """ 
     Args:
         account_id (str):
-        id (str):
+        allowlist_ip_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-id=id,
+allowlist_ip_id=allowlist_ip_id,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     account_id: str,
-    id: str,
+    allowlist_ip_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Delete security rule (CIDR)
-
-     Delete security rule (CIDR). No access to database possible after deletion from CIDR
-
+    """ 
     Args:
         account_id (str):
-        id (str):
+        allowlist_ip_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-id=id,
+allowlist_ip_id=allowlist_ip_id,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/security/get_allowed_ip.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,180 +20,160 @@
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
-    id: str,
 
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip/{id}".format(account_id=account_id,id=id,),
+        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip".format(account_id=account_id,),
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[AllowedIP]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['AllowedIP']]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = AllowedIP.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in (_response_200):
+            response_200_item = AllowedIP.from_dict(response_200_item_data)
 
 
 
+            response_200.append(response_200_item)
+
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[AllowedIP]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['AllowedIP']]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
-    id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[AllowedIP]:
-    """ Get security rule (CIDR)
-
-     Get security rule (CIDR)
-
+) -> Response[List['AllowedIP']]:
+    """ 
     Args:
         account_id (str):
-        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[AllowedIP]
+        Response[List['AllowedIP']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-id=id,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
-    id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[AllowedIP]:
-    """ Get security rule (CIDR)
-
-     Get security rule (CIDR)
-
+) -> Optional[List['AllowedIP']]:
+    """ 
     Args:
         account_id (str):
-        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        AllowedIP
+        List['AllowedIP']
      """
 
 
     return sync_detailed(
         account_id=account_id,
-id=id,
 client=client,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
-    id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[AllowedIP]:
-    """ Get security rule (CIDR)
-
-     Get security rule (CIDR)
-
+) -> Response[List['AllowedIP']]:
+    """ 
     Args:
         account_id (str):
-        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[AllowedIP]
+        Response[List['AllowedIP']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-id=id,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
-    id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[AllowedIP]:
-    """ Get security rule (CIDR)
-
-     Get security rule (CIDR)
-
+) -> Optional[List['AllowedIP']]:
+    """ 
     Args:
         account_id (str):
-        id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        AllowedIP
+        List['AllowedIP']
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
-id=id,
 client=client,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/security/list_allowed_i_ps.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/platform/list_platforms.py`

 * *Files 22% similar despite different names*

```diff
@@ -11,181 +11,148 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.allowed_ip import AllowedIP
+from ...models.platform import Platform
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
-    account_id: str,
-
+    
 ) -> Dict[str, Any]:
     
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip".format(account_id=account_id,),
+        "url": "/api/v1/platforms",
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['AllowedIP']]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['Platform']]:
     if response.status_code == HTTPStatus.OK:
         response_200 = []
         _response_200 = response.json()
         for response_200_item_data in (_response_200):
-            response_200_item = AllowedIP.from_dict(response_200_item_data)
+            response_200_item = Platform.from_dict(response_200_item_data)
 
 
 
             response_200.append(response_200_item)
 
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['AllowedIP']]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['Platform']]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
-    account_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[List['AllowedIP']]:
-    """ List security rules (CIDR)
-
-     List security rules (CIDR)
-
-    Args:
-        account_id (str):
-
+) -> Response[List['Platform']]:
+    """ 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['AllowedIP']]
+        Response[List['Platform']]
      """
 
 
     kwargs = _get_kwargs(
-        account_id=account_id,
-
+        
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
-    account_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[List['AllowedIP']]:
-    """ List security rules (CIDR)
-
-     List security rules (CIDR)
-
-    Args:
-        account_id (str):
-
+) -> Optional[List['Platform']]:
+    """ 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['AllowedIP']
+        List['Platform']
      """
 
 
     return sync_detailed(
-        account_id=account_id,
-client=client,
+        client=client,
 
     ).parsed
 
 async def asyncio_detailed(
-    account_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Response[List['AllowedIP']]:
-    """ List security rules (CIDR)
-
-     List security rules (CIDR)
-
-    Args:
-        account_id (str):
-
+) -> Response[List['Platform']]:
+    """ 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['AllowedIP']]
+        Response[List['Platform']]
      """
 
 
     kwargs = _get_kwargs(
-        account_id=account_id,
-
+        
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
-    account_id: str,
     *,
     client: AuthenticatedClient,
 
-) -> Optional[List['AllowedIP']]:
-    """ List security rules (CIDR)
-
-     List security rules (CIDR)
-
-    Args:
-        account_id (str):
-
+) -> Optional[List['Platform']]:
+    """ 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['AllowedIP']
+        List['Platform']
      """
 
 
     return (await asyncio_detailed(
-        account_id=account_id,
-client=client,
+        client=client,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/security/update_allowed_ip.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/users/patch_user.py`

 * *Files 10% similar despite different names*

```diff
@@ -11,38 +11,38 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.update_allowed_ip import UpdateAllowedIP
+from ...models.patch_user import PatchUser
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
-    id: str,
+    user_id: str,
     *,
-    body: UpdateAllowedIP,
+    body: PatchUser,
 
 ) -> Dict[str, Any]:
     headers: Dict[str, Any] = {}
 
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "put",
-        "url": "/api/v1/accounts/{account_id}/security/allowlist_ip/{id}".format(account_id=account_id,id=id,),
+        "method": "patch",
+        "url": "/api/v1/accounts/{account_id}/users/{user_id}".format(account_id=account_id,user_id=user_id,),
     }
 
     _body = body.to_dict()
 
 
     _kwargs["json"] = _body
     headers["Content-Type"] = "application/json"
@@ -67,81 +67,75 @@
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
-    id: str,
+    user_id: str,
     *,
     client: AuthenticatedClient,
-    body: UpdateAllowedIP,
+    body: PatchUser,
 
 ) -> Response[Any]:
-    """ Update security rule (CIDR)
-
-     Update security rule (CIDR)
-
+    """ 
     Args:
         account_id (str):
-        id (str):
-        body (UpdateAllowedIP):
+        user_id (str):
+        body (PatchUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-id=id,
+user_id=user_id,
 body=body,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 
 async def asyncio_detailed(
     account_id: str,
-    id: str,
+    user_id: str,
     *,
     client: AuthenticatedClient,
-    body: UpdateAllowedIP,
+    body: PatchUser,
 
 ) -> Response[Any]:
-    """ Update security rule (CIDR)
-
-     Update security rule (CIDR)
-
+    """ 
     Args:
         account_id (str):
-        id (str):
-        body (UpdateAllowedIP):
+        user_id (str):
+        body (PatchUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
         Response[Any]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-id=id,
+user_id=user_id,
 body=body,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/usage/get_usage.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/users/list_users.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,218 +11,221 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.get_usage_response_200 import GetUsageResponse200
-from ...models.get_usage_type import GetUsageType
+from ...models.user import User
 from ...types import (
     UNSET,
     Response,
     Unset,
 )
 
 
 def _get_kwargs(
     account_id: str,
     *,
-    year_month: str,
-    type: Union[Unset, GetUsageType] = UNSET,
+    filter_: Union[Unset, str] = UNSET,
+    next_: Union[Unset, int] = UNSET,
+    limit: Union[Unset, int] = UNSET,
 
 ) -> Dict[str, Any]:
     
 
     
 
     params: Dict[str, Any] = {}
 
-    params["yearMonth"] = year_month
+    params["filter"] = filter_
 
-    json_type: Union[Unset, str] = UNSET
-    if not isinstance(type, Unset):
-        json_type = type.value
+    params["next"] = next_
 
-    params["type"] = json_type
+    params["limit"] = limit
 
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/v1/accounts/{account_id}/usage".format(account_id=account_id,),
+        "url": "/api/v1/accounts/{account_id}/users".format(account_id=account_id,),
         "params": params,
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[GetUsageResponse200]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['User']]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = GetUsageResponse200.from_dict(response.json())
+        response_200 = []
+        _response_200 = response.json()
+        for response_200_item_data in (_response_200):
+            response_200_item = User.from_dict(response_200_item_data)
 
 
 
+            response_200.append(response_200_item)
+
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[GetUsageResponse200]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['User']]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    year_month: str,
-    type: Union[Unset, GetUsageType] = UNSET,
-
-) -> Response[GetUsageResponse200]:
-    """ Get usage
-
-     Show usage for one month
+    filter_: Union[Unset, str] = UNSET,
+    next_: Union[Unset, int] = UNSET,
+    limit: Union[Unset, int] = UNSET,
 
+) -> Response[List['User']]:
+    """ 
     Args:
         account_id (str):
-        year_month (str):
-        type (Union[Unset, GetUsageType]):
+        filter_ (Union[Unset, str]):
+        next_ (Union[Unset, int]):
+        limit (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetUsageResponse200]
+        Response[List['User']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-year_month=year_month,
-type=type,
+filter_=filter_,
+next_=next_,
+limit=limit,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    year_month: str,
-    type: Union[Unset, GetUsageType] = UNSET,
-
-) -> Optional[GetUsageResponse200]:
-    """ Get usage
-
-     Show usage for one month
+    filter_: Union[Unset, str] = UNSET,
+    next_: Union[Unset, int] = UNSET,
+    limit: Union[Unset, int] = UNSET,
 
+) -> Optional[List['User']]:
+    """ 
     Args:
         account_id (str):
-        year_month (str):
-        type (Union[Unset, GetUsageType]):
+        filter_ (Union[Unset, str]):
+        next_ (Union[Unset, int]):
+        limit (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetUsageResponse200
+        List['User']
      """
 
 
     return sync_detailed(
         account_id=account_id,
 client=client,
-year_month=year_month,
-type=type,
+filter_=filter_,
+next_=next_,
+limit=limit,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    year_month: str,
-    type: Union[Unset, GetUsageType] = UNSET,
-
-) -> Response[GetUsageResponse200]:
-    """ Get usage
-
-     Show usage for one month
+    filter_: Union[Unset, str] = UNSET,
+    next_: Union[Unset, int] = UNSET,
+    limit: Union[Unset, int] = UNSET,
 
+) -> Response[List['User']]:
+    """ 
     Args:
         account_id (str):
-        year_month (str):
-        type (Union[Unset, GetUsageType]):
+        filter_ (Union[Unset, str]):
+        next_ (Union[Unset, int]):
+        limit (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[GetUsageResponse200]
+        Response[List['User']]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-year_month=year_month,
-type=type,
+filter_=filter_,
+next_=next_,
+limit=limit,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    year_month: str,
-    type: Union[Unset, GetUsageType] = UNSET,
-
-) -> Optional[GetUsageResponse200]:
-    """ Get usage
-
-     Show usage for one month
+    filter_: Union[Unset, str] = UNSET,
+    next_: Union[Unset, int] = UNSET,
+    limit: Union[Unset, int] = UNSET,
 
+) -> Optional[List['User']]:
+    """ 
     Args:
         account_id (str):
-        year_month (str):
-        type (Union[Unset, GetUsageType]):
+        filter_ (Union[Unset, str]):
+        next_ (Union[Unset, int]):
+        limit (Union[Unset, int]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        GetUsageResponse200
+        List['User']
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
 client=client,
-year_month=year_month,
-type=type,
+filter_=filter_,
+next_=next_,
+limit=limit,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/users/delete_user.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/users/delete_user.py`

 * *Files 6% similar despite different names*

```diff
@@ -62,18 +62,15 @@
 def sync_detailed(
     account_id: str,
     user_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Remove user
-
-     Remove user from account
-
+    """ 
     Args:
         account_id (str):
         user_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
@@ -99,18 +96,15 @@
 async def asyncio_detailed(
     account_id: str,
     user_id: str,
     *,
     client: AuthenticatedClient,
 
 ) -> Response[Any]:
-    """ Remove user
-
-     Remove user from account
-
+    """ 
     Args:
         account_id (str):
         user_id (str):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/users/list_users.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/usage/get_usage.py`

 * *Files 24% similar despite different names*

```diff
@@ -11,233 +11,206 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.profile import Profile
+from ...models.get_usage_type import GetUsageType
+from ...models.usage import Usage
 from ...types import (
     UNSET,
     Response,
     Unset,
 )
 
 
 def _get_kwargs(
     account_id: str,
     *,
-    filter_: Union[Unset, str] = UNSET,
-    next_: Union[Unset, int] = UNSET,
-    limit: Union[Unset, int] = UNSET,
+    year_month: Union[Unset, str] = UNSET,
+    type: Union[Unset, GetUsageType] = UNSET,
 
 ) -> Dict[str, Any]:
     
 
     
 
     params: Dict[str, Any] = {}
 
-    params["filter"] = filter_
+    params["yearMonth"] = year_month
 
-    params["next"] = next_
+    json_type: Union[Unset, str] = UNSET
+    if not isinstance(type, Unset):
+        json_type = type.value
 
-    params["limit"] = limit
+    params["type"] = json_type
 
 
     params = {k: v for k, v in params.items() if v is not UNSET and v is not None}
 
 
     _kwargs: Dict[str, Any] = {
         "method": "get",
-        "url": "/api/v1/accounts/{account_id}/users".format(account_id=account_id,),
+        "url": "/api/v1/accounts/{account_id}/usage".format(account_id=account_id,),
         "params": params,
     }
 
 
     return _kwargs
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[List['Profile']]:
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Usage]:
     if response.status_code == HTTPStatus.OK:
-        response_200 = []
-        _response_200 = response.json()
-        for response_200_item_data in (_response_200):
-            response_200_item = Profile.from_dict(response_200_item_data)
+        response_200 = Usage.from_dict(response.json())
 
 
 
-            response_200.append(response_200_item)
-
         return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[List['Profile']]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Usage]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    filter_: Union[Unset, str] = UNSET,
-    next_: Union[Unset, int] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-
-) -> Response[List['Profile']]:
-    """ List users
-
-     List users for account
+    year_month: Union[Unset, str] = UNSET,
+    type: Union[Unset, GetUsageType] = UNSET,
 
+) -> Response[Usage]:
+    """ 
     Args:
         account_id (str):
-        filter_ (Union[Unset, str]):
-        next_ (Union[Unset, int]):
-        limit (Union[Unset, int]):
+        year_month (Union[Unset, str]):
+        type (Union[Unset, GetUsageType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['Profile']]
+        Response[Usage]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-filter_=filter_,
-next_=next_,
-limit=limit,
+year_month=year_month,
+type=type,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
 def sync(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    filter_: Union[Unset, str] = UNSET,
-    next_: Union[Unset, int] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-
-) -> Optional[List['Profile']]:
-    """ List users
-
-     List users for account
+    year_month: Union[Unset, str] = UNSET,
+    type: Union[Unset, GetUsageType] = UNSET,
 
+) -> Optional[Usage]:
+    """ 
     Args:
         account_id (str):
-        filter_ (Union[Unset, str]):
-        next_ (Union[Unset, int]):
-        limit (Union[Unset, int]):
+        year_month (Union[Unset, str]):
+        type (Union[Unset, GetUsageType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['Profile']
+        Usage
      """
 
 
     return sync_detailed(
         account_id=account_id,
 client=client,
-filter_=filter_,
-next_=next_,
-limit=limit,
+year_month=year_month,
+type=type,
 
     ).parsed
 
 async def asyncio_detailed(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    filter_: Union[Unset, str] = UNSET,
-    next_: Union[Unset, int] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-
-) -> Response[List['Profile']]:
-    """ List users
-
-     List users for account
+    year_month: Union[Unset, str] = UNSET,
+    type: Union[Unset, GetUsageType] = UNSET,
 
+) -> Response[Usage]:
+    """ 
     Args:
         account_id (str):
-        filter_ (Union[Unset, str]):
-        next_ (Union[Unset, int]):
-        limit (Union[Unset, int]):
+        year_month (Union[Unset, str]):
+        type (Union[Unset, GetUsageType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[List['Profile']]
+        Response[Usage]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
-filter_=filter_,
-next_=next_,
-limit=limit,
+year_month=year_month,
+type=type,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
 async def asyncio(
     account_id: str,
     *,
     client: AuthenticatedClient,
-    filter_: Union[Unset, str] = UNSET,
-    next_: Union[Unset, int] = UNSET,
-    limit: Union[Unset, int] = UNSET,
-
-) -> Optional[List['Profile']]:
-    """ List users
-
-     List users for account
+    year_month: Union[Unset, str] = UNSET,
+    type: Union[Unset, GetUsageType] = UNSET,
 
+) -> Optional[Usage]:
+    """ 
     Args:
         account_id (str):
-        filter_ (Union[Unset, str]):
-        next_ (Union[Unset, int]):
-        limit (Union[Unset, int]):
+        year_month (Union[Unset, str]):
+        type (Union[Unset, GetUsageType]):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        List['Profile']
+        Usage
      """
 
 
     return (await asyncio_detailed(
         account_id=account_id,
 client=client,
-filter_=filter_,
-next_=next_,
-limit=limit,
+year_month=year_month,
+type=type,
 
     )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/api/users/patch_user.py` & `saas_api-0.2.0/exasol/saas/client/openapi/api/users/get_user.py`

 * *Files 20% similar despite different names*

```diff
@@ -11,140 +11,177 @@
 import httpx
 
 from ... import errors
 from ...client import (
     AuthenticatedClient,
     Client,
 )
-from ...models.patch_user import PatchUser
+from ...models.user import User
 from ...types import (
     UNSET,
     Response,
 )
 
 
 def _get_kwargs(
     account_id: str,
     user_id: str,
-    *,
-    body: PatchUser,
 
 ) -> Dict[str, Any]:
-    headers: Dict[str, Any] = {}
-
+    
 
     
 
     
 
     _kwargs: Dict[str, Any] = {
-        "method": "patch",
-        "url": "/api/v1/accounts/{account_id}/users/{user_id}".format(account_id=account_id,user_id=user_id,),
+        "method": "get",
+        "url": "/api/v1/internal/accounts/{account_id}/users/{user_id}".format(account_id=account_id,user_id=user_id,),
     }
 
-    _body = body.to_dict()
 
+    return _kwargs
 
-    _kwargs["json"] = _body
-    headers["Content-Type"] = "application/json"
 
-    _kwargs["headers"] = headers
-    return _kwargs
+def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[User]:
+    if response.status_code == HTTPStatus.OK:
+        response_200 = User.from_dict(response.json())
 
 
-def _parse_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Optional[Any]:
-    if response.status_code == HTTPStatus.NO_CONTENT:
-        return None
+
+        return response_200
     if client.raise_on_unexpected_status:
         raise errors.UnexpectedStatus(response.status_code, response.content)
     else:
         return None
 
 
-def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[Any]:
+def _build_response(*, client: Union[AuthenticatedClient, Client], response: httpx.Response) -> Response[User]:
     return Response(
         status_code=HTTPStatus(response.status_code),
         content=response.content,
         headers=response.headers,
         parsed=_parse_response(client=client, response=response),
     )
 
 
 def sync_detailed(
     account_id: str,
     user_id: str,
     *,
     client: AuthenticatedClient,
-    body: PatchUser,
-
-) -> Response[Any]:
-    """ Patch user
-
-     Patch user
 
+) -> Response[User]:
+    """ 
     Args:
         account_id (str):
         user_id (str):
-        body (PatchUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[User]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 user_id=user_id,
-body=body,
 
     )
 
     response = client.get_httpx_client().request(
         **kwargs,
     )
 
     return _build_response(client=client, response=response)
 
-
-async def asyncio_detailed(
+def sync(
     account_id: str,
     user_id: str,
     *,
     client: AuthenticatedClient,
-    body: PatchUser,
 
-) -> Response[Any]:
-    """ Patch user
+) -> Optional[User]:
+    """ 
+    Args:
+        account_id (str):
+        user_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
 
-     Patch user
+    Returns:
+        User
+     """
 
+
+    return sync_detailed(
+        account_id=account_id,
+user_id=user_id,
+client=client,
+
+    ).parsed
+
+async def asyncio_detailed(
+    account_id: str,
+    user_id: str,
+    *,
+    client: AuthenticatedClient,
+
+) -> Response[User]:
+    """ 
     Args:
         account_id (str):
         user_id (str):
-        body (PatchUser):
 
     Raises:
         errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
         httpx.TimeoutException: If the request takes longer than Client.timeout.
 
     Returns:
-        Response[Any]
+        Response[User]
      """
 
 
     kwargs = _get_kwargs(
         account_id=account_id,
 user_id=user_id,
-body=body,
 
     )
 
     response = await client.get_async_httpx_client().request(
         **kwargs
     )
 
     return _build_response(client=client, response=response)
 
+async def asyncio(
+    account_id: str,
+    user_id: str,
+    *,
+    client: AuthenticatedClient,
+
+) -> Optional[User]:
+    """ 
+    Args:
+        account_id (str):
+        user_id (str):
+
+    Raises:
+        errors.UnexpectedStatus: If the server returns an undocumented status code and Client.raise_on_unexpected_status is True.
+        httpx.TimeoutException: If the request takes longer than Client.timeout.
+
+    Returns:
+        User
+     """
+
+
+    return (await asyncio_detailed(
+        account_id=account_id,
+user_id=user_id,
+client=client,
+
+    )).parsed
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/client.py` & `saas_api-0.2.0/exasol/saas/client/openapi/client.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/errors.py` & `saas_api-0.2.0/exasol/saas/client/openapi/errors.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/allowed_ip.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/allowed_ip.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/api_error.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/usage_additional_property_item.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,134 +1,109 @@
-import datetime
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
+    List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
     Union,
     cast,
 )
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
-from dateutil.parser import isoparse
 
 from ..types import (
     UNSET,
     Unset,
 )
 
 if TYPE_CHECKING:
-  from ..models.api_error_causes import APIErrorCauses
+  from ..models.usage_cluster import UsageCluster
 
 
 
 
 
-T = TypeVar("T", bound="APIError")
+T = TypeVar("T", bound="UsageAdditionalPropertyItem")
 
 
 @_attrs_define
-class APIError:
+class UsageAdditionalPropertyItem:
     """ 
         Attributes:
-            code (int):
-            message (str):
-            causes (Union[Unset, APIErrorCauses]):
-            request_id (Union[Unset, str]):
-            timestamp (Union[Unset, datetime.datetime]):
-            api_id (Union[Unset, str]):
+            id (str):
+            name (str):
+            clusters (List['UsageCluster']):
+            used_storage (Union[Unset, float]):
      """
 
-    code: int
-    message: str
-    causes: Union[Unset, 'APIErrorCauses'] = UNSET
-    request_id: Union[Unset, str] = UNSET
-    timestamp: Union[Unset, datetime.datetime] = UNSET
-    api_id: Union[Unset, str] = UNSET
+    id: str
+    name: str
+    clusters: List['UsageCluster']
+    used_storage: Union[Unset, float] = UNSET
 
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.api_error_causes import APIErrorCauses
-        code = self.code
+        from ..models.usage_cluster import UsageCluster
+        id = self.id
 
-        message = self.message
+        name = self.name
 
-        causes: Union[Unset, Dict[str, Any]] = UNSET
-        if not isinstance(self.causes, Unset):
-            causes = self.causes.to_dict()
+        clusters = []
+        for clusters_item_data in self.clusters:
+            clusters_item = clusters_item_data.to_dict()
+            clusters.append(clusters_item)
 
-        request_id = self.request_id
 
-        timestamp: Union[Unset, str] = UNSET
-        if not isinstance(self.timestamp, Unset):
-            timestamp = self.timestamp.isoformat()
 
-        api_id = self.api_id
+
+
+        used_storage = self.used_storage
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update({
-            "code": code,
-            "message": message,
+            "id": id,
+            "name": name,
+            "clusters": clusters,
         })
-        if causes is not UNSET:
-            field_dict["causes"] = causes
-        if request_id is not UNSET:
-            field_dict["requestID"] = request_id
-        if timestamp is not UNSET:
-            field_dict["timestamp"] = timestamp
-        if api_id is not UNSET:
-            field_dict["apiID"] = api_id
+        if used_storage is not UNSET:
+            field_dict["usedStorage"] = used_storage
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.api_error_causes import APIErrorCauses
+        from ..models.usage_cluster import UsageCluster
         d = src_dict.copy()
-        code = d.pop("code")
-
-        message = d.pop("message")
-
-        _causes = d.pop("causes", UNSET)
-        causes: Union[Unset, APIErrorCauses]
-        if isinstance(_causes,  Unset):
-            causes = UNSET
-        else:
-            causes = APIErrorCauses.from_dict(_causes)
-
-
+        id = d.pop("id")
 
+        name = d.pop("name")
 
-        request_id = d.pop("requestID", UNSET)
+        clusters = []
+        _clusters = d.pop("clusters")
+        for clusters_item_data in (_clusters):
+            clusters_item = UsageCluster.from_dict(clusters_item_data)
 
-        _timestamp = d.pop("timestamp", UNSET)
-        timestamp: Union[Unset, datetime.datetime]
-        if isinstance(_timestamp,  Unset):
-            timestamp = UNSET
-        else:
-            timestamp = isoparse(_timestamp)
 
 
+            clusters.append(clusters_item)
 
 
-        api_id = d.pop("apiID", UNSET)
+        used_storage = d.pop("usedStorage", UNSET)
 
-        api_error = cls(
-            code=code,
-            message=message,
-            causes=causes,
-            request_id=request_id,
-            timestamp=timestamp,
-            api_id=api_id,
+        usage_additional_property_item = cls(
+            id=id,
+            name=name,
+            clusters=clusters,
+            used_storage=used_storage,
         )
 
-        return api_error
+        return usage_additional_property_item
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/api_error_causes.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/update_database.py`

 * *Files 17% similar despite different names*

```diff
@@ -15,52 +15,62 @@
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="APIErrorCauses")
+T = TypeVar("T", bound="UpdateDatabase")
 
 
 @_attrs_define
-class APIErrorCauses:
+class UpdateDatabase:
     """ 
+        Attributes:
+            name (str):
      """
 
-    additional_properties: Dict[str, bool] = _attrs_field(init=False, factory=dict)
+    name: str
+    additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        
+        name = self.name
+
+
         field_dict: Dict[str, Any] = {}
         field_dict.update(self.additional_properties)
+        field_dict.update({
+            "name": name,
+        })
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
-        api_error_causes = cls(
-        )
+        name = d.pop("name")
 
+        update_database = cls(
+            name=name,
+        )
 
-        api_error_causes.additional_properties = d
-        return api_error_causes
+        update_database.additional_properties = d
+        return update_database
 
     @property
     def additional_keys(self) -> List[str]:
         return list(self.additional_properties.keys())
 
-    def __getitem__(self, key: str) -> bool:
+    def __getitem__(self, key: str) -> Any:
         return self.additional_properties[key]
 
-    def __setitem__(self, key: str, value: bool) -> None:
+    def __setitem__(self, key: str, value: Any) -> None:
         self.additional_properties[key] = value
 
     def __delitem__(self, key: str) -> None:
         del self.additional_properties[key]
 
     def __contains__(self, key: str) -> bool:
         return key in self.additional_properties
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/auto_stop.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/auto_stop.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/cluster.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/cluster_overview.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/database_clusters.py`

 * *Files 15% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="ClusterOverview")
+T = TypeVar("T", bound="DatabaseClusters")
 
 
 @_attrs_define
-class ClusterOverview:
+class DatabaseClusters:
     """ 
         Attributes:
             total (int):
             running (int):
      """
 
     total: int
@@ -52,14 +52,14 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         total = d.pop("total")
 
         running = d.pop("running")
 
-        cluster_overview = cls(
+        database_clusters = cls(
             total=total,
             running=running,
         )
 
-        return cluster_overview
+        return database_clusters
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/cluster_size.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/cluster_size.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/connection_i_ps.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/connection_i_ps.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/connections.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/cluster_connection.py`

 * *Files 9% similar despite different names*

```diff
@@ -22,19 +22,19 @@
 if TYPE_CHECKING:
   from ..models.connection_i_ps import ConnectionIPs
 
 
 
 
 
-T = TypeVar("T", bound="Connections")
+T = TypeVar("T", bound="ClusterConnection")
 
 
 @_attrs_define
-class Connections:
+class ClusterConnection:
     """ 
         Attributes:
             dns (str):
             port (int):
             jdbc (str):
             ips (ConnectionIPs):
             db_username (str):
@@ -86,17 +86,17 @@
         ips = ConnectionIPs.from_dict(d.pop("ips"))
 
 
 
 
         db_username = d.pop("dbUsername")
 
-        connections = cls(
+        cluster_connection = cls(
             dns=dns,
             port=port,
             jdbc=jdbc,
             ips=ips,
             db_username=db_username,
         )
 
-        return connections
+        return cluster_connection
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/create_allowed_ip.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/create_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/create_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/create_cluster.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/create_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/create_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from typing import (
     TYPE_CHECKING,
     Any,
     BinaryIO,
     Dict,
+    List,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
     cast,
 )
@@ -16,69 +17,75 @@
 
 from ..types import (
     UNSET,
     Unset,
 )
 
 if TYPE_CHECKING:
-  from ..models.create_cluster import CreateCluster
+  from ..models.create_database_initial_cluster import CreateDatabaseInitialCluster
 
 
 
 
 
 T = TypeVar("T", bound="CreateDatabase")
 
 
 @_attrs_define
 class CreateDatabase:
     """ 
         Attributes:
             name (str):
-            initial_cluster (CreateCluster):
+            initial_cluster (CreateDatabaseInitialCluster):
             provider (str):
             region (str):
      """
 
     name: str
-    initial_cluster: 'CreateCluster'
+    initial_cluster: 'CreateDatabaseInitialCluster'
     provider: str
     region: str
+    additional_properties: Dict[str, Any] = _attrs_field(init=False, factory=dict)
 
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.create_cluster import CreateCluster
+        from ..models.create_database_initial_cluster import (
+            CreateDatabaseInitialCluster,
+        )
         name = self.name
 
         initial_cluster = self.initial_cluster.to_dict()
 
         provider = self.provider
 
         region = self.region
 
 
         field_dict: Dict[str, Any] = {}
+        field_dict.update(self.additional_properties)
         field_dict.update({
             "name": name,
             "initialCluster": initial_cluster,
             "provider": provider,
             "region": region,
         })
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.create_cluster import CreateCluster
+        from ..models.create_database_initial_cluster import (
+            CreateDatabaseInitialCluster,
+        )
         d = src_dict.copy()
         name = d.pop("name")
 
-        initial_cluster = CreateCluster.from_dict(d.pop("initialCluster"))
+        initial_cluster = CreateDatabaseInitialCluster.from_dict(d.pop("initialCluster"))
 
 
 
 
         provider = d.pop("provider")
 
         region = d.pop("region")
@@ -86,9 +93,25 @@
         create_database = cls(
             name=name,
             initial_cluster=initial_cluster,
             provider=provider,
             region=region,
         )
 
+        create_database.additional_properties = d
         return create_database
 
+    @property
+    def additional_keys(self) -> List[str]:
+        return list(self.additional_properties.keys())
+
+    def __getitem__(self, key: str) -> Any:
+        return self.additional_properties[key]
+
+    def __setitem__(self, key: str, value: Any) -> None:
+        self.additional_properties[key] = value
+
+    def __delitem__(self, key: str) -> None:
+        del self.additional_properties[key]
+
+    def __contains__(self, key: str) -> bool:
+        return key in self.additional_properties
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/download_file.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/download_file.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/file.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/file.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/integrations.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/platform.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,72 +4,62 @@
     BinaryIO,
     Dict,
     Optional,
     TextIO,
     Tuple,
     Type,
     TypeVar,
-    Union,
 )
 
 from attrs import define as _attrs_define
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="Integrations")
+T = TypeVar("T", bound="Platform")
 
 
 @_attrs_define
-class Integrations:
+class Platform:
     """ 
         Attributes:
             id (str):
             name (str):
-            url (Union[Unset, str]):
      """
 
     id: str
     name: str
-    url: Union[Unset, str] = UNSET
 
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
         name = self.name
 
-        url = self.url
-
 
         field_dict: Dict[str, Any] = {}
         field_dict.update({
             "id": id,
             "name": name,
         })
-        if url is not UNSET:
-            field_dict["url"] = url
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         name = d.pop("name")
 
-        url = d.pop("url", UNSET)
-
-        integrations = cls(
+        platform = cls(
             id=id,
             name=name,
-            url=url,
         )
 
-        return integrations
+        return platform
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/patch_databases.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/patch_user_databases.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,19 +16,19 @@
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="PatchDatabases")
+T = TypeVar("T", bound="PatchUserDatabases")
 
 
 @_attrs_define
-class PatchDatabases:
+class PatchUserDatabases:
     """ 
         Attributes:
             delete (List[str]):
             add (List[str]):
      """
 
     delete: List[str]
@@ -64,14 +64,14 @@
         d = src_dict.copy()
         delete = cast(List[str], d.pop("delete"))
 
 
         add = cast(List[str], d.pop("add"))
 
 
-        patch_databases = cls(
+        patch_user_databases = cls(
             delete=delete,
             add=add,
         )
 
-        return patch_databases
+        return patch_user_databases
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/patch_user.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/patch_user.py`

 * *Files 21% similar despite different names*

```diff
@@ -17,39 +17,39 @@
 
 from ..types import (
     UNSET,
     Unset,
 )
 
 if TYPE_CHECKING:
-  from ..models.patch_databases import PatchDatabases
+  from ..models.patch_user_databases import PatchUserDatabases
 
 
 
 
 
 T = TypeVar("T", bound="PatchUser")
 
 
 @_attrs_define
 class PatchUser:
     """ 
         Attributes:
             role_id (Union[Unset, str]):
-            databases (Union[Unset, PatchDatabases]):
+            databases (Union[Unset, PatchUserDatabases]):
             db_username (Union[Unset, str]):
      """
 
     role_id: Union[Unset, str] = UNSET
-    databases: Union[Unset, 'PatchDatabases'] = UNSET
+    databases: Union[Unset, 'PatchUserDatabases'] = UNSET
     db_username: Union[Unset, str] = UNSET
 
 
     def to_dict(self) -> Dict[str, Any]:
-        from ..models.patch_databases import PatchDatabases
+        from ..models.patch_user_databases import PatchUserDatabases
         role_id = self.role_id
 
         databases: Union[Unset, Dict[str, Any]] = UNSET
         if not isinstance(self.databases, Unset):
             databases = self.databases.to_dict()
 
         db_username = self.db_username
@@ -67,24 +67,24 @@
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
-        from ..models.patch_databases import PatchDatabases
+        from ..models.patch_user_databases import PatchUserDatabases
         d = src_dict.copy()
         role_id = d.pop("roleID", UNSET)
 
         _databases = d.pop("databases", UNSET)
-        databases: Union[Unset, PatchDatabases]
+        databases: Union[Unset, PatchUserDatabases]
         if isinstance(_databases,  Unset):
             databases = UNSET
         else:
-            databases = PatchDatabases.from_dict(_databases)
+            databases = PatchUserDatabases.from_dict(_databases)
 
 
 
 
         db_username = d.pop("dbUsername", UNSET)
 
         patch_user = cls(
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/platform.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/user_role.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="Platform")
+T = TypeVar("T", bound="UserRole")
 
 
 @_attrs_define
-class Platform:
+class UserRole:
     """ 
         Attributes:
             id (str):
             name (str):
      """
 
     id: str
@@ -52,14 +52,14 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         name = d.pop("name")
 
-        platform = cls(
+        user_role = cls(
             id=id,
             name=name,
         )
 
-        return platform
+        return user_role
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/profile.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,19 +28,19 @@
   from ..models.user_database import UserDatabase
   from ..models.user_role import UserRole
 
 
 
 
 
-T = TypeVar("T", bound="Profile")
+T = TypeVar("T", bound="User")
 
 
 @_attrs_define
-class Profile:
+class User:
     """ 
         Attributes:
             email (str):
             id (str):
             created_at (datetime.datetime):
             created_by (str):
             status (UserStatus):
@@ -175,23 +175,23 @@
 
 
             databases.append(databases_item)
 
 
         db_username = d.pop("dbUsername", UNSET)
 
-        profile = cls(
+        user = cls(
             email=email,
             id=id,
             created_at=created_at,
             created_by=created_by,
             status=status,
             roles=roles,
             is_deletable=is_deletable,
             first_name=first_name,
             last_name=last_name,
             databases=databases,
             db_username=db_username,
         )
 
-        return profile
+        return user
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/region.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/region.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/scale_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/scale_cluster.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/update_allowed_ip.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/update_allowed_ip.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/update_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/update_cluster.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/update_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/user_database.py`

 * *Files 24% similar despite different names*

```diff
@@ -14,44 +14,52 @@
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="UpdateDatabase")
+T = TypeVar("T", bound="UserDatabase")
 
 
 @_attrs_define
-class UpdateDatabase:
+class UserDatabase:
     """ 
         Attributes:
+            id (str):
             name (str):
      """
 
+    id: str
     name: str
 
 
     def to_dict(self) -> Dict[str, Any]:
+        id = self.id
+
         name = self.name
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update({
+            "id": id,
             "name": name,
         })
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
+        id = d.pop("id")
+
         name = d.pop("name")
 
-        update_database = cls(
+        user_database = cls(
+            id=id,
             name=name,
         )
 
-        return update_database
+        return user_database
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/update_profile.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/update_profile.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/upload_file.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/upload_file.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/usage_cluster.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/usage_cluster.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/user_database.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/extension_instance.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,19 +14,19 @@
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="UserDatabase")
+T = TypeVar("T", bound="ExtensionInstance")
 
 
 @_attrs_define
-class UserDatabase:
+class ExtensionInstance:
     """ 
         Attributes:
             id (str):
             name (str):
      """
 
     id: str
@@ -52,14 +52,14 @@
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
         name = d.pop("name")
 
-        user_database = cls(
+        extension_instance = cls(
             id=id,
             name=name,
         )
 
-        return user_database
+        return extension_instance
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/models/user_role.py` & `saas_api-0.2.0/exasol/saas/client/openapi/models/extension_parameter_value.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,52 +14,52 @@
 from attrs import field as _attrs_field
 
 from ..types import (
     UNSET,
     Unset,
 )
 
-T = TypeVar("T", bound="UserRole")
+T = TypeVar("T", bound="ExtensionParameterValue")
 
 
 @_attrs_define
-class UserRole:
+class ExtensionParameterValue:
     """ 
         Attributes:
             id (str):
-            name (str):
+            value (str):
      """
 
     id: str
-    name: str
+    value: str
 
 
     def to_dict(self) -> Dict[str, Any]:
         id = self.id
 
-        name = self.name
+        value = self.value
 
 
         field_dict: Dict[str, Any] = {}
         field_dict.update({
             "id": id,
-            "name": name,
+            "value": value,
         })
 
         return field_dict
 
 
 
     @classmethod
     def from_dict(cls: Type[T], src_dict: Dict[str, Any]) -> T:
         d = src_dict.copy()
         id = d.pop("id")
 
-        name = d.pop("name")
+        value = d.pop("value")
 
-        user_role = cls(
+        extension_parameter_value = cls(
             id=id,
-            name=name,
+            value=value,
         )
 
-        return user_role
+        return extension_parameter_value
```

### Comparing `saas_api-0.1.0/exasol/saas/client/openapi/types.py` & `saas_api-0.2.0/exasol/saas/client/openapi/types.py`

 * *Files identical despite different names*

### Comparing `saas_api-0.1.0/pyproject.toml` & `saas_api-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "saas-api"
-version = "0.1.0"
+version = "0.2.0"
 description = "API enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services"
 packages = [ {include = "exasol"}, ]
 authors = [ "Christoph Kuhnke <christoph.kuhnke@exasol.com>" ]
 maintainers = [ "Christoph Kuhnke <christoph.kuhnke@exasol.com>" ]
 classifiers = [
    "Programming Language :: Python :: 3",
    "Development Status :: 3 - Alpha",
```

### Comparing `saas_api-0.1.0/setup.py` & `saas_api-0.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 packages = \
 ['exasol',
  'exasol.saas.client',
  'exasol.saas.client.openapi',
  'exasol.saas.client.openapi.api',
  'exasol.saas.client.openapi.api.clusters',
  'exasol.saas.client.openapi.api.databases',
+ 'exasol.saas.client.openapi.api.extensions',
  'exasol.saas.client.openapi.api.files',
  'exasol.saas.client.openapi.api.platform',
  'exasol.saas.client.openapi.api.profile',
  'exasol.saas.client.openapi.api.security',
  'exasol.saas.client.openapi.api.usage',
  'exasol.saas.client.openapi.api.users',
  'exasol.saas.client.openapi.models']
@@ -25,15 +26,15 @@
  'types-requests>=2.31.0.6,<3.0.0.0']
 
 entry_points = \
 {'console_scripts': ['tbx = exasol.toolbox.tools.tbx:CLI']}
 
 setup_kwargs = {
     'name': 'saas-api',
-    'version': '0.1.0',
+    'version': '0.2.0',
     'description': 'API enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services',
     'long_description': '# SaaS API for Python\n\nAPI enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services.\n\nThe model layer of this API is generated from the OpenAPI specification in JSON format of the SaaS API https://cloud.exasol.com/openapi.json using [openapi-python-client](https://github.com/openapi-generators/openapi-python-client).\n\nA GitHub action will check each morning if the generated model layer is outdated.\n\nSee\n* [User Guide](doc/user_guide/user-guide.md)\n* [Developer Guide](doc/developer_guide/developer_guide.md)\n',
     'author': 'Christoph Kuhnke',
     'author_email': 'christoph.kuhnke@exasol.com',
     'maintainer': 'Christoph Kuhnke',
     'maintainer_email': 'christoph.kuhnke@exasol.com',
     'url': 'None',
```

### Comparing `saas_api-0.1.0/PKG-INFO` & `saas_api-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: saas-api
-Version: 0.1.0
+Version: 0.2.0
 Summary: API enabling Python applications connecting to Exasol database SaaS instances and using their SaaS services
 License: MIT
 Author: Christoph Kuhnke
 Author-email: christoph.kuhnke@exasol.com
 Maintainer: Christoph Kuhnke
 Maintainer-email: christoph.kuhnke@exasol.com
 Requires-Python: >=3.8.0,<4.0
```

