# Comparing `tmp/perun.proxy.utils-2.7.1.tar.gz` & `tmp/perun.proxy.utils-2.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perun.proxy.utils-2.7.1.tar", last modified: Tue Apr 23 22:07:58 2024, max compression
+gzip compressed data, was "perun.proxy.utils-2.7.2.tar", last modified: Tue Apr 23 22:13:57 2024, max compression
```

## Comparing `perun.proxy.utils-2.7.1.tar` & `perun.proxy.utils-2.7.2.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:07:58.644190 perun.proxy.utils-2.7.1/
--rw-rw-rw-   0     1001 root         (0)     1560 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/LICENSE
--rw-r--r--   0     1001 root         (0)     7768 2024-04-23 22:07:58.644190 perun.proxy.utils-2.7.1/PKG-INFO
--rw-rw-rw-   0     1001 root         (0)     6763 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/README.md
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:07:58.636190 perun.proxy.utils-2.7.1/perun/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:07:58.636190 perun.proxy.utils-2.7.1/perun/proxy/
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:07:58.640190 perun.proxy.utils-2.7.1/perun/proxy/utils/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/__init__.py
--rw-rw-rw-   0     1001 root         (0)     1077 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/metadata_expiration.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:07:58.644190 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/
--rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/__init__.py
--rw-rw-rw-   0     1001 root         (0)      811 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_custom_command.py
--rw-rw-rw-   0     1001 root         (0)     1516 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_dockers.py
--rw-rw-rw-   0     1001 root         (0)      591 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_exabgp_propagation.py
--rw-rw-rw-   0     1001 root         (0)     2435 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_ldap.py
--rw-rw-rw-   0     1001 root         (0)      238 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_ldap_syncrepl.py
--rw-rw-rw-   0     1001 root         (0)    72116 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_mongodb.py
--rw-rw-rw-   0     1001 root         (0)      244 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_nginx.py
--rw-rw-rw-   0     1001 root         (0)    10260 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_oidc_login.py
--rw-rw-rw-   0     1001 root         (0)     5934 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_pgsql.py
--rwxrwxrwx   0     1001 root         (0)     1519 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_php_syntax.py
--rw-rw-rw-   0     1001 root         (0)     4627 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_privacyidea.py
--rw-rw-rw-   0     1001 root         (0)     1757 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_rpc_status.py
--rwxrwxrwx   0     1001 root         (0)    19494 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_saml.py
--rw-rw-rw-   0     1001 root         (0)     3199 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_user_logins.py
--rwxrwxrwx   0     1001 root         (0)      945 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/webserver_availability.py
--rw-rw-rw-   0     1001 root         (0)     7850 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/oracle2postgresql.py
--rwxrwxrwx   0     1001 root         (0)     2652 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/print_docker_versions.py
--rw-rw-rw-   0     1001 root         (0)     2988 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/run_probes.py
--rw-rw-rw-   0     1001 root         (0)     3215 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/run_version_script.py
--rw-rw-rw-   0     1001 root         (0)     2392 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/separate_oidc_logs.py
--rwxrwxrwx   0     1001 root         (0)     2786 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/separate_ssp_logs.py
--rw-rw-rw-   0     1001 root         (0)     4597 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/perun/proxy/utils/sync_usable_token_types.py
-drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:07:58.640190 perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/
--rw-r--r--   0     1001 root         (0)     7768 2024-04-23 22:07:58.000000 perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/PKG-INFO
--rw-r--r--   0     1001 root         (0)     1340 2024-04-23 22:07:58.000000 perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/SOURCES.txt
--rw-r--r--   0     1001 root         (0)        1 2024-04-23 22:07:58.000000 perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/dependency_links.txt
--rw-r--r--   0     1001 root         (0)     1510 2024-04-23 22:07:58.000000 perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/entry_points.txt
--rw-r--r--   0     1001 root         (0)      332 2024-04-23 22:07:58.000000 perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/requires.txt
--rw-r--r--   0     1001 root         (0)        6 2024-04-23 22:07:58.000000 perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/top_level.txt
--rw-rw-rw-   0     1001 root         (0)      171 2024-04-23 22:07:58.644190 perun.proxy.utils-2.7.1/setup.cfg
--rw-rw-rw-   0     1001 root         (0)     2903 2024-04-23 22:07:20.000000 perun.proxy.utils-2.7.1/setup.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:13:57.673622 perun.proxy.utils-2.7.2/
+-rw-rw-rw-   0     1001 root         (0)     1560 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/LICENSE
+-rw-r--r--   0     1001 root         (0)     7768 2024-04-23 22:13:57.673622 perun.proxy.utils-2.7.2/PKG-INFO
+-rw-rw-rw-   0     1001 root         (0)     6763 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/README.md
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:13:57.669622 perun.proxy.utils-2.7.2/perun/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:13:57.669622 perun.proxy.utils-2.7.2/perun/proxy/
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:13:57.669622 perun.proxy.utils-2.7.2/perun/proxy/utils/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/__init__.py
+-rw-rw-rw-   0     1001 root         (0)     1077 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/metadata_expiration.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:13:57.673622 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/
+-rw-rw-rw-   0     1001 root         (0)        0 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/__init__.py
+-rw-rw-rw-   0     1001 root         (0)      811 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_custom_command.py
+-rw-rw-rw-   0     1001 root         (0)     1516 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_dockers.py
+-rw-rw-rw-   0     1001 root         (0)      591 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_exabgp_propagation.py
+-rw-rw-rw-   0     1001 root         (0)     2435 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_ldap.py
+-rw-rw-rw-   0     1001 root         (0)      238 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_ldap_syncrepl.py
+-rw-rw-rw-   0     1001 root         (0)    72116 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_mongodb.py
+-rw-rw-rw-   0     1001 root         (0)      244 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_nginx.py
+-rw-rw-rw-   0     1001 root         (0)    10260 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_oidc_login.py
+-rw-rw-rw-   0     1001 root         (0)     5934 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_pgsql.py
+-rwxrwxrwx   0     1001 root         (0)     1519 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_php_syntax.py
+-rw-rw-rw-   0     1001 root         (0)     4627 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_privacyidea.py
+-rw-rw-rw-   0     1001 root         (0)     1757 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_rpc_status.py
+-rwxrwxrwx   0     1001 root         (0)    19494 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_saml.py
+-rw-rw-rw-   0     1001 root         (0)     3199 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_user_logins.py
+-rwxrwxrwx   0     1001 root         (0)      945 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/webserver_availability.py
+-rw-rw-rw-   0     1001 root         (0)     7850 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/oracle2postgresql.py
+-rwxrwxrwx   0     1001 root         (0)     2652 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/print_docker_versions.py
+-rw-rw-rw-   0     1001 root         (0)     2988 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/run_probes.py
+-rw-rw-rw-   0     1001 root         (0)     3215 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/run_version_script.py
+-rw-rw-rw-   0     1001 root         (0)     2392 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/separate_oidc_logs.py
+-rwxrwxrwx   0     1001 root         (0)     2786 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/separate_ssp_logs.py
+-rw-rw-rw-   0     1001 root         (0)     4597 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/perun/proxy/utils/sync_usable_token_types.py
+drwxr-xr-x   0     1001 root         (0)        0 2024-04-23 22:13:57.669622 perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/
+-rw-r--r--   0     1001 root         (0)     7768 2024-04-23 22:13:57.000000 perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/PKG-INFO
+-rw-r--r--   0     1001 root         (0)     1340 2024-04-23 22:13:57.000000 perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/SOURCES.txt
+-rw-r--r--   0     1001 root         (0)        1 2024-04-23 22:13:57.000000 perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/dependency_links.txt
+-rw-r--r--   0     1001 root         (0)     1510 2024-04-23 22:13:57.000000 perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/entry_points.txt
+-rw-r--r--   0     1001 root         (0)      332 2024-04-23 22:13:57.000000 perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/requires.txt
+-rw-r--r--   0     1001 root         (0)        6 2024-04-23 22:13:57.000000 perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/top_level.txt
+-rw-rw-rw-   0     1001 root         (0)      171 2024-04-23 22:13:57.673622 perun.proxy.utils-2.7.2/setup.cfg
+-rw-rw-rw-   0     1001 root         (0)     2903 2024-04-23 22:13:19.000000 perun.proxy.utils-2.7.2/setup.py
```

### Comparing `perun.proxy.utils-2.7.1/LICENSE` & `perun.proxy.utils-2.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/PKG-INFO` & `perun.proxy.utils-2.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 2.7.1
+Version: 2.7.2
 Summary: Utilities and monitoring probes for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/perun-proxy-utils.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pymongo~=4.3
```

### Comparing `perun.proxy.utils-2.7.1/README.md` & `perun.proxy.utils-2.7.2/README.md`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/metadata_expiration.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/metadata_expiration.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_custom_command.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_custom_command.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_dockers.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_dockers.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_exabgp_propagation.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_exabgp_propagation.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_ldap.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_ldap.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_mongodb.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_mongodb.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_oidc_login.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_oidc_login.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_pgsql.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_pgsql.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_php_syntax.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_php_syntax.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_privacyidea.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_privacyidea.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_rpc_status.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_rpc_status.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_saml.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_saml.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/check_user_logins.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/check_user_logins.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/nagios/webserver_availability.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/nagios/webserver_availability.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/oracle2postgresql.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/oracle2postgresql.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     """
     Import append-only attributes from Oracle DB to Postgresql.
     For all IDs returned from the Oracle SQL, insert a predefined value into an attribute.
     Currently, for all alumni insert alum into eduPersonAffiliation.
     """
 
     def __init__(self, full_sync):
-        self.table_for_imported_attributes = "AttributeFromSQLUnique"
+        self.table_for_imported_attributes = "attributefromsqlunique"
         self.imported_table_name = "w_exp_passwd_all"
         self.__get_config()
         self.full_sync = full_sync
         self.oracle_engine = self.__get_oracle_engine()
         self.postgresql_engine = self.__get_postgresql_engine()
         self.__create_tables_if_they_dont_exist()
```

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/print_docker_versions.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/print_docker_versions.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/run_probes.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/run_probes.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/run_version_script.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/run_version_script.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/separate_oidc_logs.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/separate_oidc_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/separate_ssp_logs.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/separate_ssp_logs.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun/proxy/utils/sync_usable_token_types.py` & `perun.proxy.utils-2.7.2/perun/proxy/utils/sync_usable_token_types.py`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/PKG-INFO` & `perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perun.proxy.utils
-Version: 2.7.1
+Version: 2.7.2
 Summary: Utilities and monitoring probes for Perun ProxyIdP
 Home-page: https://gitlab.ics.muni.cz/perun/perun-proxyidp/perun-proxy-utils.git
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: setuptools
 Requires-Dist: pymongo~=4.3
```

### Comparing `perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/SOURCES.txt` & `perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/perun.proxy.utils.egg-info/entry_points.txt` & `perun.proxy.utils-2.7.2/perun.proxy.utils.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `perun.proxy.utils-2.7.1/setup.py` & `perun.proxy.utils-2.7.2/setup.py`

 * *Files identical despite different names*

