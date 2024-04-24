# Comparing `tmp/dolphie-4.3.5.tar.gz` & `tmp/dolphie-5.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dolphie-4.3.5.tar", max compression
+gzip compressed data, was "dolphie-5.0.0.tar", max compression
```

## Comparing `dolphie-4.3.5.tar` & `dolphie-5.0.0.tar`

### file list

```diff
@@ -1,28 +1,35 @@
--rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-4.3.5/LICENSE
--rw-r--r--   0        0        0    10412 2024-03-02 09:52:23.105106 dolphie-4.3.5/README.md
--rw-r--r--   0        0        0     5425 2024-02-29 04:17:53.317177 dolphie-4.3.5/dolphie/DataTypes.py
--rw-r--r--   0        0        0     7998 2024-04-07 22:58:19.683385 dolphie-4.3.5/dolphie/Dolphie.css
--rw-r--r--   0        0        0    22016 2024-03-02 09:47:47.243202 dolphie-4.3.5/dolphie/Modules/ArgumentParser.py
--rw-r--r--   0        0        0     6770 2024-03-02 06:56:36.204962 dolphie-4.3.5/dolphie/Modules/Functions.py
--rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-4.3.5/dolphie/Modules/ManualException.py
--rw-r--r--   0        0        0    26287 2024-02-27 06:42:42.249716 dolphie-4.3.5/dolphie/Modules/MetricManager.py
--rw-r--r--   0        0        0     7446 2024-03-11 10:37:06.615356 dolphie-4.3.5/dolphie/Modules/MySQL.py
--rw-r--r--   0        0        0    17039 2024-03-12 05:51:44.344342 dolphie-4.3.5/dolphie/Modules/Queries.py
--rw-r--r--   0        0        0    23820 2024-03-02 06:25:14.219098 dolphie-4.3.5/dolphie/Modules/TabManager.py
--rw-r--r--   0        0        0     9270 2024-02-27 06:42:42.250655 dolphie-4.3.5/dolphie/Panels/dashboard_panel.py
--rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-4.3.5/dolphie/Panels/ddl_panel.py
--rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-4.3.5/dolphie/Panels/innodb_trx_locks_panel.py
--rw-r--r--   0        0        0     6877 2024-03-02 10:45:55.398930 dolphie-4.3.5/dolphie/Panels/metadata_locks_panel.py
--rw-r--r--   0        0        0     9179 2024-04-07 22:50:40.254587 dolphie-4.3.5/dolphie/Panels/processlist_panel.py
--rw-r--r--   0        0        0    25774 2024-02-27 06:28:11.313610 dolphie-4.3.5/dolphie/Panels/replication_panel.py
--rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-4.3.5/dolphie/Widgets/command_screen.py
--rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-4.3.5/dolphie/Widgets/event_log_screen.py
--rw-r--r--   0        0        0    13960 2024-03-15 01:09:17.039272 dolphie-4.3.5/dolphie/Widgets/host_setup.py
--rw-r--r--   0        0        0    11456 2024-03-28 20:01:57.993852 dolphie-4.3.5/dolphie/Widgets/modal.py
--rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-4.3.5/dolphie/Widgets/spinner.py
--rw-r--r--   0        0        0     5926 2024-03-12 06:05:29.747155 dolphie-4.3.5/dolphie/Widgets/thread_screen.py
--rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-4.3.5/dolphie/Widgets/topbar.py
--rw-r--r--   0        0        0    11982 2024-03-28 19:49:45.553457 dolphie-4.3.5/dolphie/__init__.py
--rwxr-xr-x   0        0        0    66820 2024-03-28 19:49:45.554130 dolphie-4.3.5/dolphie/app.py
--rw-r--r--   0        0        0      645 2024-04-07 23:24:53.185954 dolphie-4.3.5/pyproject.toml
--rw-r--r--   0        0        0    11471 1970-01-01 00:00:00.000000 dolphie-4.3.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2022-09-02 19:06:44.751434 dolphie-5.0.0/LICENSE
+-rw-r--r--   0        0        0    10612 2024-04-24 08:27:31.216200 dolphie-5.0.0/README.md
+-rw-r--r--   0        0        0     7743 2024-04-24 08:27:31.216691 dolphie-5.0.0/dolphie/DataTypes.py
+-rw-r--r--   0        0        0     8998 2024-04-24 08:27:31.216991 dolphie-5.0.0/dolphie/Dolphie.css
+-rw-r--r--   0        0        0    21812 2024-04-24 08:27:31.217321 dolphie-5.0.0/dolphie/Modules/ArgumentParser.py
+-rw-r--r--   0        0        0     6769 2024-04-24 08:27:31.217923 dolphie-5.0.0/dolphie/Modules/Functions.py
+-rw-r--r--   0        0        0      975 2024-02-26 06:55:52.585216 dolphie-5.0.0/dolphie/Modules/ManualException.py
+-rw-r--r--   0        0        0    38471 2024-04-24 08:27:31.218418 dolphie-5.0.0/dolphie/Modules/MetricManager.py
+-rw-r--r--   0        0        0     8308 2024-04-24 08:27:31.218829 dolphie-5.0.0/dolphie/Modules/MySQL.py
+-rw-r--r--   0        0        0    19600 2024-04-24 08:27:31.219258 dolphie-5.0.0/dolphie/Modules/Queries.py
+-rw-r--r--   0        0        0    25493 2024-04-24 08:27:31.219824 dolphie-5.0.0/dolphie/Modules/TabManager.py
+-rw-r--r--   0        0        0     9247 2024-04-24 08:27:31.220351 dolphie-5.0.0/dolphie/Panels/dashboard_panel.py
+-rw-r--r--   0        0        0     1559 2024-02-26 06:55:52.588164 dolphie-5.0.0/dolphie/Panels/ddl_panel.py
+-rw-r--r--   0        0        0     2893 2024-02-26 06:55:52.588611 dolphie-5.0.0/dolphie/Panels/innodb_trx_locks_panel.py
+-rw-r--r--   0        0        0     7360 2024-04-24 08:27:31.220949 dolphie-5.0.0/dolphie/Panels/metadata_locks_panel.py
+-rw-r--r--   0        0        0     9809 2024-04-24 08:27:31.221435 dolphie-5.0.0/dolphie/Panels/processlist_panel.py
+-rw-r--r--   0        0        0     3925 2024-04-24 08:27:31.221888 dolphie-5.0.0/dolphie/Panels/proxysql_command_stats_panel.py
+-rw-r--r--   0        0        0     5766 2024-04-24 08:27:31.222346 dolphie-5.0.0/dolphie/Panels/proxysql_dashboard_panel.py
+-rw-r--r--   0        0        0     4949 2024-04-24 08:27:31.222954 dolphie-5.0.0/dolphie/Panels/proxysql_hostgroup_summary_panel.py
+-rw-r--r--   0        0        0     4086 2024-04-24 08:27:31.223282 dolphie-5.0.0/dolphie/Panels/proxysql_mysql_query_rules_panel.py
+-rw-r--r--   0        0        0     6839 2024-04-24 08:27:31.223666 dolphie-5.0.0/dolphie/Panels/proxysql_processlist_panel.py
+-rw-r--r--   0        0        0    25774 2024-04-09 22:54:28.708150 dolphie-5.0.0/dolphie/Panels/replication_panel.py
+-rw-r--r--   0        0        0     1050 2024-02-12 13:50:32.934971 dolphie-5.0.0/dolphie/Widgets/command_screen.py
+-rw-r--r--   0        0        0     6319 2024-02-26 06:55:52.590441 dolphie-5.0.0/dolphie/Widgets/event_log_screen.py
+-rw-r--r--   0        0        0     9392 2024-04-24 08:27:31.224044 dolphie-5.0.0/dolphie/Widgets/help.py
+-rw-r--r--   0        0        0    13960 2024-03-15 01:09:17.039272 dolphie-5.0.0/dolphie/Widgets/host_setup.py
+-rw-r--r--   0        0        0    12034 2024-04-24 08:27:31.224413 dolphie-5.0.0/dolphie/Widgets/modal.py
+-rw-r--r--   0        0        0     3873 2024-04-24 08:27:31.224676 dolphie-5.0.0/dolphie/Widgets/proxysql_thread_screen.py
+-rw-r--r--   0        0        0      563 2024-02-26 06:55:52.591220 dolphie-5.0.0/dolphie/Widgets/spinner.py
+-rw-r--r--   0        0        0     5997 2024-04-24 08:27:31.225002 dolphie-5.0.0/dolphie/Widgets/thread_screen.py
+-rw-r--r--   0        0        0     1125 2024-02-12 13:50:32.936036 dolphie-5.0.0/dolphie/Widgets/topbar.py
+-rw-r--r--   0        0        0    13475 2024-04-24 08:27:31.225358 dolphie-5.0.0/dolphie/__init__.py
+-rwxr-xr-x   0        0        0    79079 2024-04-24 08:27:31.225932 dolphie-5.0.0/dolphie/app.py
+-rw-r--r--   0        0        0      679 2024-04-24 08:27:31.227560 dolphie-5.0.0/pyproject.toml
+-rw-r--r--   0        0        0    11680 1970-01-01 00:00:00.000000 dolphie-5.0.0/PKG-INFO
```

### Comparing `dolphie-4.3.5/LICENSE` & `dolphie-5.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/README.md` & `dolphie-5.0.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # Dolphie
 <p align="center">
   <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
-  Echolocate your MySQL health with real-time monitoring in the terminal<br><br>
+  Your single pane of glass for real-time analytics into MySQL & ProxySQL<br><br>
   <img src="https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-97f8-3b7ef5096eae" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/1d94502a-9abf-4436-a7d0-cb2b08c105c1" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83" width="30">
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/charlesthompson">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee">
@@ -63,44 +63,44 @@
 $ docker run -dit --name dolphie ghcr.io/charles-001/dolphie:latest
 $ docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-pass
 ```
 
 ## Usage
 ```
 positional arguments:
-  uri                   Use a URI string for credentials - format: mysql://user:password@host:port (port is optional with default 3306)
+  uri                   Use a URI string for credentials (mysql/proxysql) - format: mysql://user:password@host:port (port is optional with default 3306, or 6032 for ProxySQL)
 
 options:
   --help                show this help message and exit
   --host-setup          Start Dolphie by showing the Host Setup modal instead of automatically connecting
-  -u , --user           Username for MySQL
-  -p , --password       Password for MySQL
-  -h , --host           Hostname/IP address for MySQL
-  -P , --port           Port for MySQL (Socket has precendence)
-  -S , --socket         Socket file for MySQL
+  -u , --user           Username
+  -p , --password       Password
+  -h , --host           Hostname/IP address
+  -P , --port           Port(Socket has precendence)
+  -S , --socket         Socket file
   --config-file         Dolphie's config file to use. Options are read from these files in the given order: /etc/dolphie.cnf, ~/.dolphie.cnf
   --mycnf-file          MySQL config file path to use. This should use [client] section [default: ~/.my.cnf]
   -f , --host-cache-file
                         Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format ip=hostname [default: ~/dolphie_host_cache]
   -q , --host-setup-file
                         Specify location of file that stores the available hosts to use in host setup modal [default: ~/dolphie_hosts]
   -l , --login-path     Specify login path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supercedes config file [default: client]
   -r , --refresh_interval
                         How much time to wait in seconds between each refresh [default: 1]
   -H , --heartbeat-table
-                        If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it has for replication lag instead of Seconds_Behind_Master from SHOW REPLICA STATUS
+                        (MySQL only) If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it has for replication lag instead of Seconds_Behind_Master from SHOW REPLICA STATUS
   --ssl-mode            Desired security state of the connection to the host. Supports: REQUIRED/VERIFY_CA/VERIFY_IDENTITY [default: OFF]
   --ssl-ca              Path to the file that contains a CA (certificate authority)
   --ssl-cert            Path to the file that contains a certificate
   --ssl-key             Path to the file that contains a private key for the certificate
-  --panels              What panels to display on startup separated by a comma. Supports: dashboard,processlist,graphs,replication,metadata_locks,ddl [default: dashboard,processlist]
+  --panels              What panels to display on startup separated by a comma. Supports:  dashboard,processlist,graphs,replication,metadata_locks,ddl,proxysql_hostgroup_summary,proxysql_mysql_query_rules,proxysql_command_stats [default: dashboard,processlist]
   --graph-marker        What marker to use for graphs (available options: https://tinyurl.com/dolphie-markers) [default: braille]
   --pypi-repository     What PyPi repository to use when checking for a new version. If not specified, it will use Dolphie's PyPi repository
   --hostgroup           This is used for creating tabs and connecting to them for hosts you specify in Dolphie's config file under a hostgroup section. As an example, you'll have a section called [cluster1] then below it you will list each host on a new line in the format key=host (keys have no meaning). Hosts support optional port (default is whatever port parameter is) in the format host:port. You can also name the tabs by suffixing ~tab_name to the host (i.e. 1=host~tab_name)
-  --show-trxs-only      Start with only showing threads that have an active transaction
+  --show-trxs-only      (MySQL only) Start with only showing threads that have an active transaction
   --additional-columns  Start with additional columns in Processlist panel
   --debug-options       Display options that are set and what they're set by (command-line, dolphie config, etc) then exit
   -V, --version         Display version and exit
 
 MySQL my.cnf file supports these options under [client] section:
 	host
 	user
@@ -149,15 +149,18 @@
 	(str) hostgroup
 	(bool) show_trxs_only
 	(bool) show_additional_query_columns
 ```
 
 ## Supported MySQL versions
 - MySQL/Percona Server 5.6/5.7/8.0+
-- RDS/Aurora
+- RDS & Aurora + Azure
+
+## Supported ProxySQL versions
+- ProxySQL 2.6+ (could work on previous versions but not tested)
 
 ## Grants required
 #### Least privilege
 1. PROCESS (only if you switch to using processlist via `P` command)
 2. SELECT to `performance_schema` + `pt-heartbeat table` (if used)
 3. REPLICATION CLIENT/REPLICATION SLAVE
 4. BACKUP_ADMIN (MySQL 8 only)
```

#### html2text {}

```diff
@@ -1,11 +1,11 @@
 # Dolphie
  [https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-
                           4f9c-ada5-a153cdcf4070.png]
-    Echolocate your MySQL health with real-time monitoring in the terminal
+    Your single pane of glass for real-time analytics into MySQL & ProxySQL
 
   [https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-
   97f8-3b7ef5096eae][https://github.com/charles-001/dolphie/assets/13244625/
  1d94502a-9abf-4436-a7d0-cb2b08c105c1][https://github.com/charles-001/dolphie/
              assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83]
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ![Untitled](https://github.com/charles-001/dolphie/assets/13244625/d1292ddc-
@@ -23,98 +23,99 @@
 curl -sSL https://install.python-poetry.org | python3 - $ poetry install ```
 #### Using Homebrew If you are a [Homebrew](https://brew.sh/) user, you can
 install [dolphie](https://formulae.brew.sh/formula/dolphie) via ```sh $ brew
 install dolphie ``` #### Using Docker ```sh $ docker pull ghcr.io/charles-001/
 dolphie:latest $ docker run -dit --name dolphie ghcr.io/charles-001/dolphie:
 latest $ docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-
 pass ``` ## Usage ``` positional arguments: uri Use a URI string for
-credentials - format: mysql://user:password@host:port (port is optional with
-default 3306) options: --help show this help message and exit --host-setup
-Start Dolphie by showing the Host Setup modal instead of automatically
-connecting -u , --user Username for MySQL -p , --password Password for MySQL -
-h , --host Hostname/IP address for MySQL -P , --port Port for MySQL (Socket has
-precendence) -S , --socket Socket file for MySQL --config-file Dolphie's config
-file to use. Options are read from these files in the given order: /etc/
-dolphie.cnf, ~/.dolphie.cnf --mycnf-file MySQL config file path to use. This
-should use [client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve
-IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on
-its own line using format ip=hostname [default: ~/dolphie_host_cache] -q , --
-host-setup-file Specify location of file that stores the available hosts to use
-in host setup modal [default: ~/dolphie_hosts] -l , --login-path Specify login
+credentials (mysql/proxysql) - format: mysql://user:password@host:port (port is
+optional with default 3306, or 6032 for ProxySQL) options: --help show this
+help message and exit --host-setup Start Dolphie by showing the Host Setup
+modal instead of automatically connecting -u , --user Username -p , --password
+Password -h , --host Hostname/IP address -P , --port Port(Socket has
+precendence) -S , --socket Socket file --config-file Dolphie's config file to
+use. Options are read from these files in the given order: /etc/dolphie.cnf,
+~/.dolphie.cnf --mycnf-file MySQL config file path to use. This should use
+[client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve IPs to
+hostnames when your DNS is unable to. Each IP/hostname pair should be on its
+own line using format ip=hostname [default: ~/dolphie_host_cache] -q , --host-
+setup-file Specify location of file that stores the available hosts to use in
+host setup modal [default: ~/dolphie_hosts] -l , --login-path Specify login
 path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login
 credentials. Supercedes config file [default: client] -r , --refresh_interval
 How much time to wait in seconds between each refresh [default: 1] -H , --
-heartbeat-table If your hosts use pt-heartbeat, specify table in format
-db.table to use the timestamp it has for replication lag instead of
+heartbeat-table (MySQL only) If your hosts use pt-heartbeat, specify table in
+format db.table to use the timestamp it has for replication lag instead of
 Seconds_Behind_Master from SHOW REPLICA STATUS --ssl-mode Desired security
 state of the connection to the host. Supports: REQUIRED/VERIFY_CA/
 VERIFY_IDENTITY [default: OFF] --ssl-ca Path to the file that contains a CA
 (certificate authority) --ssl-cert Path to the file that contains a certificate
 --ssl-key Path to the file that contains a private key for the certificate --
 panels What panels to display on startup separated by a comma. Supports:
-dashboard,processlist,graphs,replication,metadata_locks,ddl [default:
-dashboard,processlist] --graph-marker What marker to use for graphs (available
-options: https://tinyurl.com/dolphie-markers) [default: braille] --pypi-
-repository What PyPi repository to use when checking for a new version. If not
-specified, it will use Dolphie's PyPi repository --hostgroup This is used for
-creating tabs and connecting to them for hosts you specify in Dolphie's config
-file under a hostgroup section. As an example, you'll have a section called
-[cluster1] then below it you will list each host on a new line in the format
-key=host (keys have no meaning). Hosts support optional port (default is
+dashboard,processlist,graphs,replication,metadata_locks,ddl,proxysql_hostgroup_summary,proxysql_mysql_query_rules,proxysql_command_stats
+[default: dashboard,processlist] --graph-marker What marker to use for graphs
+(available options: https://tinyurl.com/dolphie-markers) [default: braille] --
+pypi-repository What PyPi repository to use when checking for a new version. If
+not specified, it will use Dolphie's PyPi repository --hostgroup This is used
+for creating tabs and connecting to them for hosts you specify in Dolphie's
+config file under a hostgroup section. As an example, you'll have a section
+called [cluster1] then below it you will list each host on a new line in the
+format key=host (keys have no meaning). Hosts support optional port (default is
 whatever port parameter is) in the format host:port. You can also name the tabs
 by suffixing ~tab_name to the host (i.e. 1=host~tab_name) --show-trxs-only
-Start with only showing threads that have an active transaction --additional-
-columns Start with additional columns in Processlist panel --debug-options
-Display options that are set and what they're set by (command-line, dolphie
-config, etc) then exit -V, --version Display version and exit MySQL my.cnf file
-supports these options under [client] section: host user password port socket
-ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca ssl_cert ssl_key Login path
-file supports these options: host user password port socket Environment
-variables support these options: DOLPHIE_USER DOLPHIE_PASSWORD DOLPHIE_HOST
-DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config supports these options under
-[dolphie] section: (bool) host_setup (str) user (str) password (str) host (int)
-port (str) socket (str) ssl_mode (str) ssl_ca (str) ssl_cert (str) ssl_key
-(str) mycnf_file (str) login_path (str) host_cache_file (str) host_setup_file
-(int) refresh_interval (str) heartbeat_table (str) startup_panels (str)
-graph_marker (str) pypi_repository (str) hostgroup (bool) show_trxs_only (bool)
-show_additional_query_columns ``` ## Supported MySQL versions - MySQL/Percona
-Server 5.6/5.7/8.0+ - RDS/Aurora ## Grants required #### Least privilege 1.
-PROCESS (only if you switch to using processlist via `P` command) 2. SELECT to
-`performance_schema` + `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/
-REPLICATION SLAVE 4. BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS
-(only if you switch to using processlist via `P` command) 2. Global SELECT
-access (good for explaining queries, listing all databases, etc) 4. REPLICATION
-CLIENT/REPLICATION SLAVE 5. SUPER (required if you want to kill queries) 6.
-BACKUP_ADMIN (MySQL 8 only) ## Features - Tabs docked at the top to seamlessly
-switch between connected hosts - Hostgroups to make it easy for connecting to
-multiple hosts at once - Dolphie uses panels to present groups of data. They
-can all be turned on/off to have a view of your database server that you prefer
-- Graphs for many metrics that can give you great insight into how your
-database is performing - Sparkline to show queries per second in a live view -
-2 options for finding replica lag in this order of precedence: - `pt-heartbeat
-table` (specified by `--heartbeat-table`) - `SHOW SLAVE STATUS` - Keeps a
-history of the servers you connect to that provides autocompletion for
-hostnames in the Host Setup modal - Host cache file. This provides users a way
-to specify hostnames for IPs when their network's DNS can't resolve them. An
-example use case for this is when you connect to your work's VPN and DNS isn't
-available to resolve IPs. In my opinion, it's a lot easier to look at hostnames
-than IPs! - Supports encrypted login credentials via `mysql_config_editor` -
-Automatic conversion of large numbers & bytes to human-readable - Notifies when
-new version is available - Many commands at your fingertips with autocompletion
-for their input ## Hostgroups Hostgroups are a way to easily connect to
-multiple hosts at once. To set this up, you will create a section in Dolphie's
-config file with the name you want the hostgroup to be and list each host on a
-new line in the format `key=host` (keys have no meaning). Hosts support
-optional port (default is whatever `port` parameter is) in the format `host:
-port`. You can also name the tabs by suffixing `~tab_name` to the host. Once
-ready, you will use the parameter `hostgroup` or `Host Setup` modal to see it
-in action! Note: Colors can be used in the tab name by using the format `
-[color]text[/color]` (i.e. `[red]production[/red]`). You can also use emojis
-supported by Rich (can see them by running `python -m rich.emoji`) by using the
-format `:emoji:` (i.e. `:ghost:`). Rich supports the normal emoji shortcodes.
-Example: ```ini [cluster1] 1=host1 2=host2:3307 3=host3:3308~[red]production[/
-red] :ghost: ``` ## Things to note Order of precedence for methods that pass
-options to Dolphie: 1. Command-line 2. Environment variables 3. Dolphie's
-config (set by `--config-file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5.
-~/.my.cnf (set by `--mycnf-file`) ## Feedback I welcome all questions, bug
-reports, and requests. If you enjoy Dolphie, please let me know! I'd love to
-hear from you :smiley:
+(MySQL only) Start with only showing threads that have an active transaction --
+additional-columns Start with additional columns in Processlist panel --debug-
+options Display options that are set and what they're set by (command-line,
+dolphie config, etc) then exit -V, --version Display version and exit MySQL
+my.cnf file supports these options under [client] section: host user password
+port socket ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca ssl_cert ssl_key
+Login path file supports these options: host user password port socket
+Environment variables support these options: DOLPHIE_USER DOLPHIE_PASSWORD
+DOLPHIE_HOST DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config supports these
+options under [dolphie] section: (bool) host_setup (str) user (str) password
+(str) host (int) port (str) socket (str) ssl_mode (str) ssl_ca (str) ssl_cert
+(str) ssl_key (str) mycnf_file (str) login_path (str) host_cache_file (str)
+host_setup_file (int) refresh_interval (str) heartbeat_table (str)
+startup_panels (str) graph_marker (str) pypi_repository (str) hostgroup (bool)
+show_trxs_only (bool) show_additional_query_columns ``` ## Supported MySQL
+versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS & Aurora + Azure ##
+Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
+but not tested) ## Grants required #### Least privilege 1. PROCESS (only if you
+switch to using processlist via `P` command) 2. SELECT to `performance_schema`
++ `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/REPLICATION SLAVE 4.
+BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS (only if you switch to
+using processlist via `P` command) 2. Global SELECT access (good for explaining
+queries, listing all databases, etc) 4. REPLICATION CLIENT/REPLICATION SLAVE 5.
+SUPER (required if you want to kill queries) 6. BACKUP_ADMIN (MySQL 8 only) ##
+Features - Tabs docked at the top to seamlessly switch between connected hosts
+- Hostgroups to make it easy for connecting to multiple hosts at once - Dolphie
+uses panels to present groups of data. They can all be turned on/off to have a
+view of your database server that you prefer - Graphs for many metrics that can
+give you great insight into how your database is performing - Sparkline to show
+queries per second in a live view - 2 options for finding replica lag in this
+order of precedence: - `pt-heartbeat table` (specified by `--heartbeat-table`)
+- `SHOW SLAVE STATUS` - Keeps a history of the servers you connect to that
+provides autocompletion for hostnames in the Host Setup modal - Host cache
+file. This provides users a way to specify hostnames for IPs when their
+network's DNS can't resolve them. An example use case for this is when you
+connect to your work's VPN and DNS isn't available to resolve IPs. In my
+opinion, it's a lot easier to look at hostnames than IPs! - Supports encrypted
+login credentials via `mysql_config_editor` - Automatic conversion of large
+numbers & bytes to human-readable - Notifies when new version is available -
+Many commands at your fingertips with autocompletion for their input ##
+Hostgroups Hostgroups are a way to easily connect to multiple hosts at once. To
+set this up, you will create a section in Dolphie's config file with the name
+you want the hostgroup to be and list each host on a new line in the format
+`key=host` (keys have no meaning). Hosts support optional port (default is
+whatever `port` parameter is) in the format `host:port`. You can also name the
+tabs by suffixing `~tab_name` to the host. Once ready, you will use the
+parameter `hostgroup` or `Host Setup` modal to see it in action! Note: Colors
+can be used in the tab name by using the format `[color]text[/color]` (i.e. `
+[red]production[/red]`). You can also use emojis supported by Rich (can see
+them by running `python -m rich.emoji`) by using the format `:emoji:` (i.e. `:
+ghost:`). Rich supports the normal emoji shortcodes. Example: ```ini [cluster1]
+1=host1 2=host2:3307 3=host3:3308~[red]production[/red] :ghost: ``` ## Things
+to note Order of precedence for methods that pass options to Dolphie: 1.
+Command-line 2. Environment variables 3. Dolphie's config (set by `--config-
+file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5. ~/.my.cnf (set by `--mycnf-
+file`) ## Feedback I welcome all questions, bug reports, and requests. If you
+enjoy Dolphie, please let me know! I'd love to hear from you :smiley:
```

### Comparing `dolphie-4.3.5/dolphie/DataTypes.py` & `dolphie-5.0.0/dolphie/DataTypes.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,36 @@
 from dataclasses import dataclass
 from typing import Dict, List
 
 from dolphie.Modules.Functions import format_query, format_time
-from dolphie.Modules.MySQL import Database
 from rich.table import Table
 
 
 @dataclass
+class ConnectionSource:
+    mysql = "mysql"
+    proxysql = "proxysql"
+    mariadb = "mariadb"
+    aws_rds = "aws_rds"
+    azure_mysql = "azure_mysql"
+
+
+@dataclass
 class ConnectionStatus:
     connecting = "CONNECTING"
     disconnected = "DISCONNECTED"
     read_write = "R/W"
     read_only = "RO"
 
 
 @dataclass
 class Replica:
     thread_id: int
     host: str
-    connection: Database = None
+    connection: str = None
     table: Table = None
     replication_status: Dict[str, str] = None
     lag_source: str = None
     lag: int = None
     previous_sbm: int = 0
     mysql_version: str = None
 
@@ -64,17 +72,19 @@
 
 class Panels:
     def __init__(self):
         self.dashboard = Panel("dashboard")
         self.processlist = Panel("processlist")
         self.graphs = Panel("graphs")
         self.replication = Panel("replication")
-        # self.innodb_trx_locks = Panel("innodb_trx_locks")
         self.metadata_locks = Panel("metadata_locks")
         self.ddl = Panel("ddl")
+        self.proxysql_hostgroup_summary = Panel("proxysql_hostgroup_summary")
+        self.proxysql_mysql_query_rules = Panel("proxysql_mysql_query_rules")
+        self.proxysql_command_stats = Panel("proxysql_command_stats")
 
     def get_panel(self, panel_name: str) -> Panel:
         return self.__dict__.get(panel_name, None)
 
     def get_all_panels(self) -> List[Panel]:
         return [panel for panel in self.__dict__.values() if isinstance(panel, Panel)]
 
@@ -89,15 +99,14 @@
 class ProcesslistThread:
     def __init__(self, thread_data: Dict[str, str]):
         self.id = str(thread_data.get("id", ""))
         self.mysql_thread_id = thread_data.get("mysql_thread_id")
         self.user = thread_data.get("user", "")
         self.host = thread_data.get("host", "")
         self.db = thread_data.get("db", "")
-        self.query = thread_data.get("query", "")
         self.time = int(thread_data.get("time", 0))
         self.protocol = self._get_formatted_string(thread_data.get("connection_type", ""))
         self.formatted_query = self._get_formatted_query(thread_data.get("query", ""))
         self.formatted_time = self._get_formatted_time()
         self.command = self._get_formatted_command(thread_data.get("command", ""))
         self.state = self._get_formatted_string(thread_data.get("state", ""))
         self.trx_state = self._get_formatted_string(thread_data.get("trx_state", ""))
@@ -109,31 +118,82 @@
 
     def _get_formatted_time(self) -> str:
         thread_color = self._get_time_color()
         return f"[{thread_color}]{format_time(self.time)}[/{thread_color}]" if thread_color else format_time(self.time)
 
     def _get_time_color(self) -> str:
         thread_color = ""
-        if "Group replication" not in self.query:  # Don't color GR threads
-            if "SELECT /*!40001 SQL_NO_CACHE */ *" in self.query:
+        if "Group replication" not in self.formatted_query.code:  # Don't color GR threads
+            if "SELECT /*!40001 SQL_NO_CACHE */ *" in self.formatted_query.code:
                 thread_color = "purple"
-            elif self.query:
+            elif self.formatted_query.code:
                 if self.time >= 10:
                     thread_color = "red"
                 elif self.time >= 5:
                     thread_color = "yellow"
                 else:
                     thread_color = "green"
         return thread_color
 
     def _get_formatted_command(self, command: str):
         return "[red]Killed[/red]" if command == "Killed" else command
 
     def _get_formatted_trx_time(self, trx_time: str):
         return format_time(int(trx_time)) if trx_time else "[dark_gray]N/A"
+
+    def _get_formatted_query(self, query: str):
+        return format_query(query)
+
+    def _get_formatted_string(self, string: str):
+        if not string:
+            return "[dark_gray]N/A"
+
+        return string
+
+    def _get_formatted_number(self, number):
+        if not number or number == "0":
+            return "[dark_gray]0"
+
+        return number
+
+
+class ProxySQLProcesslistThread:
+    def __init__(self, thread_data: Dict[str, str]):
+        self.id = str(thread_data.get("id", ""))
+        self.hostgroup = thread_data.get("hostgroup")
+        self.user = thread_data.get("user", "")
+        self.frontend_host = self._get_formatted_string(thread_data.get("frontend_host", ""))
+        self.host = self._get_formatted_string(thread_data.get("backend_host", ""))
+        self.db = thread_data.get("db", "")
+        self.time = int(thread_data.get("time", 0)) / 1000  # Convert to seconds since ProxySQL returns milliseconds
+        self.formatted_query = self._get_formatted_query(thread_data.get("query", "").strip(" \t\n\r"))
+        self.formatted_time = self._get_formatted_time()
+        self.command = self._get_formatted_command(thread_data.get("command", ""))
+        self.extended_info = thread_data.get("extended_info", "")
+
+    def _get_formatted_time(self) -> str:
+        thread_color = self._get_time_color()
+        return f"[{thread_color}]{format_time(self.time)}[/{thread_color}]" if thread_color else format_time(self.time)
+
+    def _get_time_color(self) -> str:
+        thread_color = ""
+        if self.formatted_query.code:
+            if self.time >= 10:
+                thread_color = "red"
+            elif self.time >= 5:
+                thread_color = "yellow"
+            else:
+                thread_color = "green"
+        return thread_color
+
+    def _get_formatted_command(self, command: str):
+        return "[red]Killed[/red]" if command == "Killed" else command
+
+    def _get_formatted_trx_time(self, trx_time: str):
+        return format_time(int(trx_time)) if trx_time else "[dark_gray]N/A"
 
     def _get_formatted_query(self, query: str):
         return format_query(query)
 
     def _get_formatted_string(self, string: str):
         if not string:
             return "[dark_gray]N/A"
```

### Comparing `dolphie-4.3.5/dolphie/Dolphie.css` & `dolphie-5.0.0/dolphie/Dolphie.css`

 * *Files 4% similar despite different names*

```diff
@@ -33,14 +33,15 @@
 }
 DataTable > .datatable--odd-row {
     background: #131a2c;
 }
 DataTable > .datatable--even-row {
     background: #0f1525;
 }
+
 LoadingIndicator {
     color: #8fb0ee;
     height: auto;
     content-align: center middle;
 }
 ModalScreen {
     background: #0d1015 70%;
@@ -96,28 +97,14 @@
     content-align: center top;
     background: #0f1525;
     border: tall #1b233a;
     height: 11;
     width: auto;
 }
 
-.innodb_trx_locks {
-    height: auto;
-    background: #0f1525;
-    border: tall #1b233a;
-    margin-bottom: 1;
-}
-.innodb_trx_locks > Label {
-    width: 100%;
-    text-style: bold;
-    color: #bbc8e8;
-    content-align: center middle;
-    margin-bottom: 1;
-}
-
 .metadata_locks {
     height: auto;
     background: #0f1525;
     border: tall #1b233a;
     margin-bottom: 1;
 }
 .metadata_locks > Label {
@@ -228,14 +215,77 @@
 .ddl > Label {
     width: 100%;
     color: #bbc8e8;
     text-style: bold;
     content-align: center middle;
 }
 
+.proxysql_hostgroup_summary_datatable {
+    overflow-x: auto;
+}
+.proxysql_hostgroup_summary {
+    height: auto;
+    background: #0f1525;
+    border: tall #1b233a;
+    margin-bottom: 1;
+}
+.proxysql_hostgroup_summary > Container {
+    height: auto;
+    width: auto;
+}
+.proxysql_hostgroup_summary > Label {
+    width: 100%;
+    color: #bbc8e8;
+    text-style: bold;
+    content-align: center middle;
+    margin-bottom: 1;
+}
+
+.proxysql_mysql_query_rules_datatable {
+    overflow-x: auto;
+}
+.proxysql_mysql_query_rules {
+    height: auto;
+    background: #0f1525;
+    border: tall #1b233a;
+    margin-bottom: 1;
+}
+.proxysql_mysql_query_rules > Container {
+    height: auto;
+    width: auto;
+}
+.proxysql_mysql_query_rules > Label {
+    width: 100%;
+    color: #bbc8e8;
+    text-style: bold;
+    content-align: center middle;
+    margin-bottom: 1;
+}
+
+.proxysql_command_stats {
+    overflow-x: auto;
+}
+.proxysql_command_stats {
+    height: auto;
+    background: #0f1525;
+    border: tall #1b233a;
+    margin-bottom: 1;
+}
+.proxysql_command_stats > Container {
+    height: auto;
+    width: auto;
+}
+.proxysql_command_stats > Label {
+    width: 100%;
+    color: #bbc8e8;
+    text-style: bold;
+    content-align: center middle;
+    margin-bottom: 1;
+}
+
 .pad_bottom_1 {
     padding-bottom: 1;
 }
 
 
 TabPane {
     padding: 0;
@@ -285,14 +335,15 @@
     text-style: bold;
 }
 
 .panel_container {
     height: auto;
 }
 .button_container {
+    height: auto;
     width: 100%;
     align-horizontal: center;
 }
 .switch_container {
     align: center top;
     margin: 1 0 1 0;
     height: auto;
```

### Comparing `dolphie-4.3.5/dolphie/Modules/ArgumentParser.py` & `dolphie-5.0.0/dolphie/Modules/ArgumentParser.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,49 +125,49 @@
     def _add_options(self):
         self.parser.add_argument(
             "uri",
             metavar="uri",
             type=str,
             nargs="?",
             help=(
-                "Use a URI string for credentials - format: mysql://user:password@host:port (port is optional with"
-                f" default {self.config.port})"
+                "Use a URI string for credentials (mysql/proxysql) - format: mysql://user:password@host:port"
+                f" (port is optional with default {self.config.port}, or 6032 for ProxySQL)"
             ),
         )
 
         self.parser.add_argument(
             "--host-setup",
             dest="host_setup",
             action="store_true",
             help="Start Dolphie by showing the Host Setup modal instead of automatically connecting",
         )
-        self.parser.add_argument("-u", "--user", dest="user", type=str, help="Username for MySQL", metavar="")
-        self.parser.add_argument("-p", "--password", dest="password", type=str, help="Password for MySQL", metavar="")
+        self.parser.add_argument("-u", "--user", dest="user", type=str, help="Username", metavar="")
+        self.parser.add_argument("-p", "--password", dest="password", type=str, help="Password", metavar="")
         self.parser.add_argument(
             "-h",
             "--host",
             dest="host",
             type=str,
-            help="Hostname/IP address for MySQL",
+            help="Hostname/IP address",
             metavar="",
         )
         self.parser.add_argument(
             "-P",
             "--port",
             dest="port",
             type=int,
-            help="Port for MySQL (socket has precendence)",
+            help="Port (socket has precendence)",
             metavar="",
         )
         self.parser.add_argument(
             "-S",
             "--socket",
             dest="socket",
             type=str,
-            help="Socket file for MySQL",
+            help="Socket file",
             metavar="",
         )
         self.parser.add_argument(
             "--config-file",
             dest="config_file",
             type=str,
             help=(
@@ -229,15 +229,15 @@
         )
         self.parser.add_argument(
             "-H",
             "--heartbeat-table",
             dest="heartbeat_table",
             type=str,
             help=(
-                "If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it "
+                "(MySQL only) If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it "
                 "has for replication lag instead of Seconds_Behind_Master from SHOW REPLICA STATUS"
             ),
             metavar="",
         )
         self.parser.add_argument(
             "--ssl-mode",
             dest="ssl_mode",
@@ -270,15 +270,15 @@
             metavar="",
         )
         self.parser.add_argument(
             "--panels",
             dest="startup_panels",
             type=str,
             help=(
-                "What panels to display on startup separated by a comma. Supports:"
+                "What panels to display on startup separated by a comma. Supports: "
                 f" {','.join(self.panels.all())} [default: {self.config.startup_panels}]"
             ),
             metavar="",
         )
         self.parser.add_argument(
             "--graph-marker",
             dest="graph_marker",
@@ -313,31 +313,22 @@
             ),
             metavar="",
         )
         self.parser.add_argument(
             "--show-trxs-only",
             dest="show_trxs_only",
             action="store_true",
-            help="Start with only showing threads that have an active transaction",
+            help="(MySQL only) Start with only showing threads that have an active transaction",
         )
         self.parser.add_argument(
             "--additional-columns",
             dest="show_additional_query_columns",
             action="store_true",
             help="Start with additional columns in Processlist panel",
         )
-        # self.parser.add_argument(
-        #     "--historical-trx-locks",
-        #     dest="historical_trx_locks",
-        #     action="store_true",
-        #     help=(
-        #         "Always run the InnoDB TRX Locks query so it can save historical data to its graph instead of only "
-        #         "when the panel is open. This query can be expensive in some environments"
-        #     ),
-        # )
         self.parser.add_argument(
             "--debug-options",
             dest="debug_options",
             action="store_true",
             help="Display options that are set and what they're set by (command-line, dolphie config, etc) then exit",
         )
         self.parser.add_argument(
@@ -476,21 +467,26 @@
                 self.set_config_value("command-line", option, options[option])
 
         # Lastly, parse URI if specified
         if options["uri"]:
             try:
                 parsed = urlparse(options["uri"])
 
-                if parsed.scheme != "mysql":
-                    self.exit("Invalid URI scheme: Only 'mysql' is supported (see --help for more information)")
+                if parsed.scheme == "mysql":
+                    self.config.port = parsed.port or 3306
+                elif parsed.scheme == "proxysql":
+                    self.config.port = parsed.port or 6032
+                else:
+                    self.exit(
+                        "Invalid URI scheme: Only 'mysql' or 'proxysql' are supported (see --help for more information)"
+                    )
 
                 self.config.user = parsed.username
                 self.config.password = parsed.password
                 self.config.host = parsed.hostname
-                self.config.port = parsed.port or 3306
             except Exception as e:
                 self.exit(f"Invalid URI: {e} (see --help for more information)")
 
         # Sanity check for hostgroup
         if self.config.hostgroup:
             if self.config.hostgroup not in hostgroups:
                 self.exit(
```

### Comparing `dolphie-4.3.5/dolphie/Modules/Functions.py` & `dolphie-5.0.0/dolphie/Modules/Functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -87,19 +87,17 @@
         Generic.Output: nord4,
         Generic.Traceback: nord11,
         Error: nord11,
     }
 
 
 def format_query(query: str, minify: bool = True) -> Syntax:
-    formatted_query = ""
-    if query:
-        query = markup_escape(re.sub(r"\s+", " ", query)) if minify else query
+    query = markup_escape(re.sub(r"\s+", " ", query)) if minify else query
 
-        formatted_query = Syntax(code=query, lexer="sql", word_wrap=True, theme=NordModifiedTheme)
+    formatted_query = Syntax(code=query, lexer="sql", word_wrap=True, theme=NordModifiedTheme)
 
     return formatted_query
 
 
 def format_bytes(bytes_value, color=True):
     units = ["B", "KB", "MB", "GB", "TB"]
     unit_index = 0
@@ -109,15 +107,17 @@
         unit_index += 1
 
     formatted_value = f"{bytes_value:.2f}"
 
     if formatted_value.endswith(".00"):
         formatted_value = formatted_value[:-3]  # Remove ".00" from the end
 
-    if color:
+    if bytes_value == 0:
+        return "0"
+    elif color:
         return f"{formatted_value}[highlight]{units[unit_index]}[/highlight]"
     else:
         return f"{formatted_value}{units[unit_index]}"
 
 
 def format_time(time: int, picoseconds=False):
     if time is None:
```

### Comparing `dolphie-4.3.5/dolphie/Modules/ManualException.py` & `dolphie-5.0.0/dolphie/Modules/ManualException.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Modules/MetricManager.py` & `dolphie-5.0.0/dolphie/Modules/MetricManager.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass, field
 from datetime import datetime
 from typing import Dict, List, Union
 
 import plotext as plt
+from dolphie.DataTypes import ConnectionSource
 from dolphie.Modules.Functions import format_bytes, format_number, format_time
 from rich.text import Text
 from textual.widgets import Static
 
 
 class Graph(Static):
     def __init__(self, *args, **kwargs) -> None:
@@ -65,55 +66,69 @@
                     x,
                     y,
                     marker=self.marker,
                     label=self.metric_instance.Innodb_checkpoint_age.label,
                     color=self.metric_instance.Innodb_checkpoint_age.color,
                 )
                 max_y_value = self.metric_instance.checkpoint_age_max
-        elif isinstance(self.metric_instance, RedoLogMetrics) and "graph_redo_log_bar" in self.id:
-            if self.metric_instance.Innodb_lsn_current.values:
-                x = [0]
-                y = [
-                    round(
-                        sum(self.metric_instance.Innodb_lsn_current.values)
-                        * (3600 / len(self.metric_instance.Innodb_lsn_current.values))
+        elif isinstance(self.metric_instance, RedoLogMetrics):
+            if "graph_redo_log_bar" in self.id:
+                if self.metric_instance.Innodb_lsn_current.values:
+                    x = [0]
+                    y = [
+                        round(
+                            sum(self.metric_instance.Innodb_lsn_current.values)
+                            * (3600 / len(self.metric_instance.Innodb_lsn_current.values))
+                        )
+                    ]
+
+                    plt.hline(self.metric_instance.redo_log_size, (252, 121, 121))
+                    plt.text(
+                        "Log Size",
+                        y=self.metric_instance.redo_log_size,
+                        x=0,
+                        alignment="center",
+                        color=(233, 233, 233),
+                        style="bold",
                     )
-                ]
 
-                plt.hline(self.metric_instance.redo_log_size, (252, 121, 121))
-                plt.text(
-                    "Log Size",
-                    y=self.metric_instance.redo_log_size,
-                    x=0,
-                    alignment="center",
-                    color=(233, 233, 233),
-                    style="bold",
-                )
-
-                bar_color = (46, 124, 175)
-                if y[0] >= self.metric_instance.redo_log_size:
-                    bar_color = (252, 121, 121)
+                    bar_color = (46, 124, 175)
+                    if y[0] >= self.metric_instance.redo_log_size:
+                        bar_color = (252, 121, 121)
+
+                    plt.text(
+                        format_bytes(y[0], color=False) + "/hr",
+                        y=y[0],
+                        x=0,
+                        alignment="center",
+                        color=(233, 233, 233),
+                        style="bold",
+                        background=bar_color,
+                    )
 
-                plt.text(
-                    format_bytes(y[0], color=False) + "/hr",
-                    y=y[0],
-                    x=0,
-                    alignment="center",
-                    color=(233, 233, 233),
-                    style="bold",
-                    background=bar_color,
-                )
+                    plt.bar(
+                        x,
+                        y,
+                        marker="hd",
+                        color=bar_color,
+                    )
+                    max_y_value = max(self.metric_instance.redo_log_size, max(y))
+            else:
+                x = self.metric_instance.datetimes
+                y = self.metric_instance.Innodb_lsn_current.values
 
-                plt.bar(
-                    x,
-                    y,
-                    marker="hd",
-                    color=bar_color,
-                )
-                max_y_value = max(self.metric_instance.redo_log_size, max(y))
+                if y:
+                    plt.plot(
+                        x,
+                        y,
+                        marker=self.marker,
+                        label=self.metric_instance.Innodb_lsn_current.label,
+                        color=self.metric_instance.Innodb_lsn_current.color,
+                    )
+                    max_y_value = max(max_y_value, max(y))
         elif isinstance(self.metric_instance, RedoLogActiveCountMetrics):
             x = self.metric_instance.datetimes
             y = self.metric_instance.Active_redo_log_count.values
 
             if y:
                 plt.hline(1, (10, 14, 27))
                 plt.hline(34, (252, 121, 121))
@@ -130,15 +145,14 @@
                     x,
                     y,
                     marker=self.marker,
                     label=self.metric_instance.Active_redo_log_count.label,
                     color=self.metric_instance.Active_redo_log_count.color,
                 )
                 max_y_value = 32
-
         else:
             for metric_data in self.metric_instance.__dict__.values():
                 if isinstance(metric_data, MetricData) and metric_data.visible:
                     x = self.metric_instance.datetimes
                     y = metric_data.values
 
                     if y:
@@ -166,47 +180,54 @@
 
 
 def get_number_format_function(data, color=False):
     data_formatters = {
         ReplicationLagMetrics: lambda val: format_time(val),
         CheckpointMetrics: lambda val: format_bytes(val, color=color),
         RedoLogMetrics: lambda val: format_bytes(val, color=color),
-        AdaptiveHashIndexHitRatioMetrics: lambda val: f"{round(val)}%",
+        AdaptiveHashIndexHitRatio: lambda val: f"{round(val)}%",
+        ProxySQLMultiplexEfficiency: lambda val: f"{round(val)}%",
         DiskIOMetrics: lambda val: format_bytes(val, color=color),
+        ProxySQLQueriesDataNetwork: lambda val: format_bytes(val, color=color),
     }
 
     return data_formatters.get(type(data), lambda val: format_number(val, color=color))
 
 
 @dataclass
 class MetricSource:
     global_status: str = "global_status"
     innodb_metrics: str = "innodb_metrics"
     disk_io_metrics: str = "disk_io_metrics"
+    proxysql_select_command_stats: str = "proxysql_select_command_stats"
+    proxysql_total_command_stats: str = "proxysql_total_command_stats"
     none: str = "none"
 
 
 @dataclass
 class MetricColor:
     gray: tuple = (172, 207, 231)
     blue: tuple = (68, 180, 255)
     green: tuple = (84, 239, 174)
     red: tuple = (255, 73, 112)
     yellow: tuple = (252, 213, 121)
+    purple: tuple = (191, 121, 252)
+    orange: tuple = (252, 121, 121)
 
 
 @dataclass
 class MetricData:
     label: str
     color: tuple
     visible: bool = True
     save_history: bool = True
     per_second_calculation: bool = True
     last_value: int = None
     graphable: bool = True
+    create_switch: bool = True
     values: List[int] = field(default_factory=list)
 
 
 @dataclass
 class DMLMetrics:
     Queries: MetricData
     Com_select: MetricData
@@ -214,167 +235,299 @@
     Com_update: MetricData
     Com_delete: MetricData
     Com_replace: MetricData
     Com_commit: MetricData
     Com_rollback: MetricData
     graphs: List[str]
     tab_name: str = "dml"
+    graph_tab_name = "DML"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(
+        default_factory=lambda: [ConnectionSource.mysql, ConnectionSource.proxysql]
+    )
 
 
 @dataclass
 class ReplicationLagMetrics:
     lag: MetricData
     graphs: List[str]
     tab_name: str = "replication_lag"
+    graph_tab_name = "Replication"
     metric_source: MetricSource = MetricSource.none
-
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class CheckpointMetrics:
     Innodb_checkpoint_age: MetricData
     graphs: List[str]
     tab_name: str = "checkpoint"
+    graph_tab_name = "Checkpoint"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
     checkpoint_age_max: int = 0
     checkpoint_age_sync_flush: int = 0
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class BufferPoolRequestsMetrics:
     Innodb_buffer_pool_read_requests: MetricData
     Innodb_buffer_pool_write_requests: MetricData
     Innodb_buffer_pool_reads: MetricData
     graphs: List[str]
     tab_name: str = "buffer_pool_requests"
+    graph_tab_name = "BP Requests"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class AdaptiveHashIndexMetrics:
     adaptive_hash_searches: MetricData
     adaptive_hash_searches_btree: MetricData
     graphs: List[str]
     tab_name: str = "adaptive_hash_index"
+    graph_tab_name = "AHI"
     metric_source: MetricSource = MetricSource.innodb_metrics
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
-class AdaptiveHashIndexHitRatioMetrics:
+class AdaptiveHashIndexHitRatio:
     hit_ratio: MetricData
     graphs: List[str]
     smoothed_hit_ratio: float = None
     tab_name: str = "adaptive_hash_index"
+    graph_tab_name = "AHI"
     metric_source: MetricSource = MetricSource.none
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class RedoLogMetrics:
     Innodb_lsn_current: MetricData
     graphs: List[str]
     tab_name: str = "redo_log"
+    graph_tab_name = "Redo Log"
     redo_log_size: int = 0
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class RedoLogActiveCountMetrics:
     Active_redo_log_count: MetricData
     graphs: List[str]
     tab_name: str = "redo_log"
+    graph_tab_name = "Redo Log"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class TableCacheMetrics:
     Table_open_cache_hits: MetricData
     Table_open_cache_misses: MetricData
     Table_open_cache_overflows: MetricData
     graphs: List[str]
     tab_name: str = "table_cache"
+    graph_tab_name = "Table Cache"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class ThreadMetrics:
     Threads_connected: MetricData
     Threads_running: MetricData
     graphs: List[str]
     tab_name: str = "threads"
+    graph_tab_name = "Threads"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class TemporaryObjectMetrics:
     Created_tmp_tables: MetricData
     Created_tmp_disk_tables: MetricData
     Created_tmp_files: MetricData
     graphs: List[str]
     tab_name: str = "temporary_objects"
+    graph_tab_name = "Temp Objects"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class AbortedConnectionsMetrics:
     Aborted_clients: MetricData
     Aborted_connects: MetricData
     graphs: List[str]
     tab_name: str = "aborted_connections"
+    graph_tab_name = "Aborted Connections"
     metric_source: MetricSource = MetricSource.global_status
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class DiskIOMetrics:
     io_read: MetricData
     io_write: MetricData
     graphs: List[str]
     tab_name: str = "disk_io"
+    graph_tab_name = "Disk I/O"
     metric_source: MetricSource = MetricSource.disk_io_metrics
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
 
 
 @dataclass
 class LocksMetrics:
-    # innodb_trx_lock_count: MetricData
     metadata_lock_count: MetricData
     graphs: List[str]
     tab_name: str = "locks"
+    graph_tab_name = "Locks"
     metric_source: MetricSource = MetricSource.none
     datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.mysql])
+
+
+@dataclass
+class ProxySQLConnectionsMetrics:
+    Client_Connections_non_idle: MetricData
+    Client_Connections_aborted: MetricData
+    Client_Connections_connected: MetricData
+    Client_Connections_created: MetricData
+    Server_Connections_aborted: MetricData
+    Server_Connections_connected: MetricData
+    Server_Connections_created: MetricData
+    Access_Denied_Wrong_Password: MetricData
+    graphs: List[str]
+    tab_name: str = "proxysql_connections"
+    graph_tab_name = "Connections"
+    metric_source: MetricSource = MetricSource.global_status
+    datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.proxysql])
+
+
+@dataclass
+class ProxySQLQueriesDataNetwork:
+    Queries_backends_bytes_recv: MetricData
+    Queries_backends_bytes_sent: MetricData
+    Queries_frontends_bytes_recv: MetricData
+    Queries_frontends_bytes_sent: MetricData
+    graphs: List[str]
+    tab_name: str = "proxysql_queries_data_network"
+    graph_tab_name = "Query Data Rates"
+    metric_source: MetricSource = MetricSource.global_status
+    datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.proxysql])
+
+
+@dataclass
+class ProxySQLActiveTRX:
+    Active_Transactions: MetricData
+    graphs: List[str]
+    tab_name: str = "proxysql_active_trx"
+    graph_tab_name = "Active TRX"
+    metric_source: MetricSource = MetricSource.global_status
+    datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.proxysql])
+
+
+@dataclass
+class ProxySQLMultiplexEfficiency:
+    proxysql_multiplex_efficiency_ratio: MetricData
+    graphs: List[str]
+    tab_name: str = "proxysql_multiplex_efficiency"
+    graph_tab_name = "Multiplex Efficiency"
+    metric_source: MetricSource = MetricSource.global_status
+    datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.proxysql])
+
+
+@dataclass
+class ProxySQLSELECTCommandStats:
+    cnt_100us: MetricData
+    cnt_500us: MetricData
+    cnt_1ms: MetricData
+    cnt_5ms: MetricData
+    cnt_10ms: MetricData
+    cnt_50ms: MetricData
+    cnt_100ms: MetricData
+    cnt_500ms: MetricData
+    cnt_1s: MetricData
+    cnt_5s: MetricData
+    cnt_10s: MetricData
+    cnt_INFs: MetricData
+    graphs: List[str]
+    tab_name: str = "proxysql_select_command_stats"
+    graph_tab_name = "SELECT Command Stats"
+    metric_source: MetricSource = MetricSource.proxysql_select_command_stats
+    datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.proxysql])
+
+
+@dataclass
+class ProxySQLTotalCommandStats:
+    cnt_100us: MetricData
+    cnt_500us: MetricData
+    cnt_1ms: MetricData
+    cnt_5ms: MetricData
+    cnt_10ms: MetricData
+    cnt_50ms: MetricData
+    cnt_100ms: MetricData
+    cnt_500ms: MetricData
+    cnt_1s: MetricData
+    cnt_5s: MetricData
+    cnt_10s: MetricData
+    cnt_INFs: MetricData
+    graphs: List[str]
+    tab_name: str = "proxysql_total_command_stats"
+    graph_tab_name = "Total Command Stats"
+    metric_source: MetricSource = MetricSource.proxysql_total_command_stats
+    datetimes: List[str] = field(default_factory=list)
+    connection_source: List[ConnectionSource] = field(default_factory=lambda: [ConnectionSource.proxysql])
 
 
 @dataclass
 class MetricInstances:
     dml: DMLMetrics
-    replication_lag: ReplicationLagMetrics
     checkpoint: CheckpointMetrics
     buffer_pool_requests: BufferPoolRequestsMetrics
     adaptive_hash_index: AdaptiveHashIndexMetrics
-    adaptive_hash_index_hit_ratio: AdaptiveHashIndexHitRatioMetrics
-    redo_log: RedoLogMetrics
+    adaptive_hash_index_hit_ratio: AdaptiveHashIndexHitRatio
     redo_log_active_count: RedoLogActiveCountMetrics
+    redo_log: RedoLogMetrics
     table_cache: TableCacheMetrics
     threads: ThreadMetrics
     temporary_objects: TemporaryObjectMetrics
     aborted_connections: AbortedConnectionsMetrics
     disk_io: DiskIOMetrics
     locks: LocksMetrics
+    replication_lag: ReplicationLagMetrics
+    proxysql_active_trx: ProxySQLActiveTRX
+    proxysql_multiplex_efficiency: ProxySQLMultiplexEfficiency
+    proxysql_connections: ProxySQLConnectionsMetrics
+    proxysql_queries_data_network: ProxySQLQueriesDataNetwork
+    proxysql_select_command_stats: ProxySQLSELECTCommandStats
+    proxysql_total_command_stats: ProxySQLTotalCommandStats
 
 
 class MetricManager:
     def __init__(self):
         self.reset()
 
     def reset(self):
@@ -401,56 +554,64 @@
                 ),
                 Com_rollback=MetricData(
                     label="ROLLBACK", color=MetricColor.red, visible=False, save_history=False, graphable=False
                 ),
             ),
             replication_lag=ReplicationLagMetrics(
                 graphs=["graph_replication_lag"],
-                lag=MetricData(label="Lag", color=MetricColor.blue, per_second_calculation=False),
+                lag=MetricData(label="Lag", color=MetricColor.blue, per_second_calculation=False, create_switch=False),
             ),
             checkpoint=CheckpointMetrics(
                 graphs=["graph_checkpoint"],
                 Innodb_checkpoint_age=MetricData(
-                    label="Uncheckpointed", color=MetricColor.blue, per_second_calculation=False
+                    label="Uncheckpointed", color=MetricColor.blue, per_second_calculation=False, create_switch=False
                 ),
             ),
             buffer_pool_requests=BufferPoolRequestsMetrics(
                 graphs=["graph_buffer_pool_requests"],
                 Innodb_buffer_pool_read_requests=MetricData(label="Read Requests", color=MetricColor.blue),
                 Innodb_buffer_pool_write_requests=MetricData(label="Write Requests", color=MetricColor.green),
                 Innodb_buffer_pool_reads=MetricData(label="Disk Reads", color=MetricColor.red),
             ),
             adaptive_hash_index=AdaptiveHashIndexMetrics(
                 graphs=["graph_adaptive_hash_index"],
                 adaptive_hash_searches=MetricData(label="Hit", color=MetricColor.green),
                 adaptive_hash_searches_btree=MetricData(label="Miss", color=MetricColor.red),
             ),
-            adaptive_hash_index_hit_ratio=AdaptiveHashIndexHitRatioMetrics(
+            adaptive_hash_index_hit_ratio=AdaptiveHashIndexHitRatio(
                 graphs=["graph_adaptive_hash_index_hit_ratio"],
-                hit_ratio=MetricData(label="Hit Ratio", color=MetricColor.green, per_second_calculation=False),
+                hit_ratio=MetricData(
+                    label="Hit Ratio", color=MetricColor.green, per_second_calculation=False, create_switch=False
+                ),
             ),
             redo_log=RedoLogMetrics(
-                graphs=["graph_redo_log", "graph_redo_log_bar"],
-                Innodb_lsn_current=MetricData(label="Data Written", color=MetricColor.blue),
+                graphs=["graph_redo_log_data_written", "graph_redo_log_bar"],
+                Innodb_lsn_current=MetricData(label="Data Written", color=MetricColor.blue, create_switch=False),
             ),
             redo_log_active_count=RedoLogActiveCountMetrics(
                 graphs=["graph_redo_log_active_count"],
                 Active_redo_log_count=MetricData(
-                    label="Active Count", color=MetricColor.blue, per_second_calculation=False, visible=False
+                    label="Active Count",
+                    color=MetricColor.blue,
+                    per_second_calculation=False,
+                    visible=False,
+                    create_switch=False,
                 ),
             ),
             table_cache=TableCacheMetrics(
                 graphs=["graph_table_cache"],
                 Table_open_cache_hits=MetricData(label="Hit", color=MetricColor.green),
                 Table_open_cache_misses=MetricData(label="Miss", color=MetricColor.red),
                 Table_open_cache_overflows=MetricData(label="Overflow", color=MetricColor.yellow),
             ),
             threads=ThreadMetrics(
                 graphs=["graph_threads"],
-                Threads_connected=MetricData(label="Connected", color=MetricColor.green, per_second_calculation=False),
+                Threads_connected=MetricData(
+                    label="Connected", color=MetricColor.green, per_second_calculation=False, visible=False
+                ),
                 Threads_running=MetricData(label="Running", color=MetricColor.blue, per_second_calculation=False),
             ),
             temporary_objects=TemporaryObjectMetrics(
                 graphs=["graph_temporary_objects"],
                 Created_tmp_tables=MetricData(label="Tables", color=MetricColor.blue),
                 Created_tmp_disk_tables=MetricData(label="Disk", color=MetricColor.red),
                 Created_tmp_files=MetricData(label="Files", color=MetricColor.yellow),
@@ -463,53 +624,121 @@
             disk_io=DiskIOMetrics(
                 graphs=["graph_disk_io"],
                 io_read=MetricData(label="Read", color=MetricColor.blue),
                 io_write=MetricData(label="Write", color=MetricColor.green),
             ),
             locks=LocksMetrics(
                 graphs=["graph_locks"],
-                # innodb_trx_lock_count=MetricData(
-                #     label="InnoDB TRX", color=MetricColor.blue, per_second_calculation=False
-                # ),
                 metadata_lock_count=MetricData(label="Metadata", color=MetricColor.red, per_second_calculation=False),
             ),
+            proxysql_connections=ProxySQLConnectionsMetrics(
+                graphs=["graph_proxysql_connections"],
+                Client_Connections_aborted=MetricData(label="FE (aborted)", color=MetricColor.gray),
+                Client_Connections_connected=MetricData(
+                    label="FE (connected)", color=MetricColor.green, per_second_calculation=False, visible=False
+                ),
+                Client_Connections_created=MetricData(label="FE (created)", color=MetricColor.yellow),
+                Server_Connections_aborted=MetricData(label="BE (aborted)", color=MetricColor.red),
+                Server_Connections_connected=MetricData(
+                    label="BE (connected)", color=MetricColor.green, per_second_calculation=False, visible=False
+                ),
+                Server_Connections_created=MetricData(label="BE (created)", color=MetricColor.blue),
+                Access_Denied_Wrong_Password=MetricData(label="Wrong Password", color=MetricColor.purple),
+                Client_Connections_non_idle=MetricData(
+                    label="FE (non-idle)", color=MetricColor.green, per_second_calculation=False, visible=True
+                ),
+            ),
+            proxysql_queries_data_network=ProxySQLQueriesDataNetwork(
+                graphs=["graph_proxysql_queries_data_network"],
+                Queries_backends_bytes_recv=MetricData(label="BE Recv", color=MetricColor.blue),
+                Queries_backends_bytes_sent=MetricData(label="BE Sent", color=MetricColor.green),
+                Queries_frontends_bytes_recv=MetricData(label="FE Recv", color=MetricColor.purple),
+                Queries_frontends_bytes_sent=MetricData(label="FE Sent", color=MetricColor.yellow),
+            ),
+            proxysql_active_trx=ProxySQLActiveTRX(
+                graphs=["graph_proxysql_active_trx"],
+                Active_Transactions=MetricData(
+                    label="Active TRX", color=MetricColor.blue, per_second_calculation=False, create_switch=False
+                ),
+            ),
+            proxysql_multiplex_efficiency=ProxySQLMultiplexEfficiency(
+                graphs=["graph_proxysql_multiplex_efficiency"],
+                proxysql_multiplex_efficiency_ratio=MetricData(
+                    label="Multiplex Efficiency",
+                    color=MetricColor.blue,
+                    per_second_calculation=False,
+                    create_switch=False,
+                ),
+            ),
+            proxysql_select_command_stats=ProxySQLSELECTCommandStats(
+                graphs=["graph_proxysql_select_command_stats"],
+                cnt_100us=MetricData(label="100us", color=MetricColor.gray, visible=False),
+                cnt_500us=MetricData(label="500us", color=MetricColor.blue, visible=False),
+                cnt_1ms=MetricData(label="1ms", color=MetricColor.green, visible=False),
+                cnt_5ms=MetricData(label="5ms", color=MetricColor.green, visible=False),
+                cnt_10ms=MetricData(label="10ms", color=MetricColor.green),
+                cnt_50ms=MetricData(label="50ms", color=MetricColor.yellow),
+                cnt_100ms=MetricData(label="100ms", color=MetricColor.yellow),
+                cnt_500ms=MetricData(label="500ms", color=MetricColor.orange),
+                cnt_1s=MetricData(label="1s", color=MetricColor.orange),
+                cnt_5s=MetricData(label="5s", color=MetricColor.red),
+                cnt_10s=MetricData(label="10s", color=MetricColor.purple),
+                cnt_INFs=MetricData(label="10s+", color=MetricColor.purple),
+            ),
+            proxysql_total_command_stats=ProxySQLTotalCommandStats(
+                graphs=["graph_proxysql_total_command_stats"],
+                cnt_100us=MetricData(label="100us", color=MetricColor.gray, visible=False),
+                cnt_500us=MetricData(label="500us", color=MetricColor.blue, visible=False),
+                cnt_1ms=MetricData(label="1ms", color=MetricColor.green, visible=False),
+                cnt_5ms=MetricData(label="5ms", color=MetricColor.green, visible=False),
+                cnt_10ms=MetricData(label="10ms", color=MetricColor.green),
+                cnt_50ms=MetricData(label="50ms", color=MetricColor.yellow),
+                cnt_100ms=MetricData(label="100ms", color=MetricColor.yellow),
+                cnt_500ms=MetricData(label="500ms", color=MetricColor.orange),
+                cnt_1s=MetricData(label="1s", color=MetricColor.orange),
+                cnt_5s=MetricData(label="5s", color=MetricColor.red),
+                cnt_10s=MetricData(label="10s", color=MetricColor.purple),
+                cnt_INFs=MetricData(label="10s+", color=MetricColor.purple),
+            ),
         )
 
     def refresh_data(
         self,
         worker_start_time: datetime,
         polling_latency: float,
-        global_variables: Dict[str, Union[int, str]],
-        global_status: Dict[str, int],
-        innodb_metrics: Dict[str, int],
-        disk_io_metrics: Dict[str, int],
-        # innodb_trx_lock_metrics: Dict[str, int],
-        metadata_lock_metrics: Dict[str, int],
-        replication_status: Dict[str, Union[int, str]],
-        replication_lag: int,  # this can be from SHOW SLAVE Status/heartbeat table
+        global_variables: Dict[str, Union[int, str]] = {},
+        global_status: Dict[str, int] = {},
+        innodb_metrics: Dict[str, int] = {},
+        proxysql_command_stats: Dict[str, int] = {},
+        disk_io_metrics: Dict[str, int] = {},
+        metadata_lock_metrics: Dict[str, int] = {},
+        replication_status: Dict[str, Union[int, str]] = {},
+        replication_lag: int = 0,  # this can be from SHOW SLAVE Status/heartbeat table
     ):
         self.worker_start_time = worker_start_time
         self.polling_latency = polling_latency
         self.global_variables = global_variables
         self.global_status = global_status
         self.innodb_metrics = innodb_metrics
         self.disk_io_metrics = disk_io_metrics
-        # self.innodb_trx_lock_metrics = innodb_trx_lock_metrics
         self.metadata_lock_metrics = metadata_lock_metrics
         self.replication_status = replication_status
         self.replication_lag = replication_lag
+        self.proxysql_total_command_stats = {}
+        self.proxysql_select_command_stats = {}
 
         # Support MySQL 8.0.30+ redo log size variable
         innodb_redo_log_capacity = self.global_variables.get("innodb_redo_log_capacity", 0)
         innodb_log_file_size = round(
             self.global_variables.get("innodb_log_file_size", 0)
             * self.global_variables.get("innodb_log_files_in_group", 1)
         )
         self.redo_log_size = max(innodb_redo_log_capacity, innodb_log_file_size)
 
+        self.update_proxysql_command_stats(proxysql_command_stats)
         self.update_metrics_per_second_values()
 
         self.update_metrics_replication_lag()
         self.update_metrics_checkpoint()
         self.update_metrics_adaptive_hash_index_hit_ratio()
         self.update_metrics_locks()
 
@@ -519,48 +748,82 @@
 
     def add_metric(self, metric_data: MetricData, value: int):
         if metric_data.save_history:
             metric_data.values.append(value)
         else:
             metric_data.values = [value]
 
-    def update_metrics_per_second_values(self):
-        for metric_instance in self.metrics.__dict__.values():
-            added = False
+    def get_metric_source_data(self, metric_source):
+        if metric_source == MetricSource.global_status:
+            metric_source_data = self.global_status
+        elif metric_source == MetricSource.innodb_metrics:
+            metric_source_data = self.innodb_metrics
+        elif metric_source == MetricSource.disk_io_metrics:
+            metric_source_data = self.disk_io_metrics
+        elif metric_source == MetricSource.proxysql_select_command_stats:
+            metric_source_data = self.proxysql_select_command_stats
+        elif metric_source == MetricSource.proxysql_total_command_stats:
+            metric_source_data = self.proxysql_total_command_stats
+        else:
+            metric_source_data = None
 
-            metric_source = None  # Initialize as None
+        return metric_source_data
 
-            if metric_instance.metric_source == MetricSource.global_status:
-                metric_source = self.global_status
-            elif metric_instance.metric_source == MetricSource.innodb_metrics:
-                metric_source = self.innodb_metrics
-            elif metric_instance.metric_source == MetricSource.disk_io_metrics:
-                metric_source = self.disk_io_metrics
+    def update_metrics_per_second_values(self):
+        for metric_instance in self.metrics.__dict__.values():
+            metrics_updated = False
 
-            if metric_source is None:
+            metric_source_data = self.get_metric_source_data(metric_instance.metric_source)
+            if metric_source_data is None:
                 continue  # Skip if there's no metric source
 
             for metric_name, metric_data in metric_instance.__dict__.items():
                 if isinstance(metric_data, MetricData):
+                    current_metric_source_value = metric_source_data.get(metric_name, 0)
+
                     if metric_data.last_value is None:
-                        metric_data.last_value = metric_source.get(metric_name, 0)
+                        metric_data.last_value = current_metric_source_value
                     else:
                         if metric_data.per_second_calculation:
-                            metric_status_per_sec = self.get_metric_calculate_per_sec(
-                                metric_name, metric_source, format=False
-                            )
+                            metric_diff = current_metric_source_value - metric_data.last_value
+                            metric_status_per_sec = round(metric_diff / self.polling_latency)
                         else:
-                            metric_status_per_sec = metric_source.get(metric_name, 0)
+                            metric_status_per_sec = current_metric_source_value
 
                         self.add_metric(metric_data, metric_status_per_sec)
-                        added = True
+                        metrics_updated = True
 
-            if added:
+            if metrics_updated:
                 metric_instance.datetimes.append(self.worker_start_time.strftime("%d/%m/%y %H:%M:%S"))
 
+    def update_metrics_last_value(self):
+        # We set the last value for specific metrics that need it so they can get per second values
+        for metric_instance in self.metrics.__dict__.values():
+            metric_source_data = self.get_metric_source_data(metric_instance.metric_source)
+
+            for metric_name, metric_data in metric_instance.__dict__.items():
+                if isinstance(metric_data, MetricData) and metric_data.per_second_calculation:
+                    metric_data.last_value = metric_source_data.get(metric_name, 0)
+
+    def update_proxysql_command_stats(self, proxysql_command_stats):
+        for row in proxysql_command_stats:
+            # Convert all values to integers if they are a number for SELECT command
+            if row["Command"] == "SELECT":
+                self.proxysql_select_command_stats = {
+                    key: int(value) if value.isdigit() else value for key, value in row.items()
+                }
+
+            for key, value in row.items():
+                if key.startswith("cnt_") and value.isdigit():
+                    # If the key exists, add to it; otherwise, initialize with the integer value
+                    if key in self.proxysql_total_command_stats:
+                        self.proxysql_total_command_stats[key] += int(value)
+                    else:
+                        self.proxysql_total_command_stats[key] = int(value)
+
     def update_metrics_replication_lag(self):
         if self.replication_status:
             metric_instance = self.metrics.replication_lag
             self.add_metric(metric_instance.lag, self.replication_lag)
             metric_instance.datetimes.append(self.worker_start_time.strftime("%d/%m/%y %H:%M:%S"))
 
     def update_metrics_adaptive_hash_index_hit_ratio(self):
@@ -576,40 +839,26 @@
 
         metric_instance = self.metrics.checkpoint
         metric_instance.checkpoint_age_max = max_checkpoint_age_bytes
         metric_instance.checkpoint_age_sync_flush = checkpoint_age_sync_flush_bytes
 
     def update_metrics_locks(self):
         metric_instance = self.metrics.locks
-        # self.add_metric(metric_instance.innodb_trx_lock_count, len(self.innodb_trx_lock_metrics))
         self.add_metric(metric_instance.metadata_lock_count, len(self.metadata_lock_metrics))
         metric_instance.datetimes.append(self.worker_start_time.strftime("%d/%m/%y %H:%M:%S"))
 
-    def get_metric_calculate_per_sec(self, metric_name, metric_source=None, format=True):
-        if not metric_source:
-            metric_source = self.global_status
-
-        for metric_instance in self.metrics.__dict__.values():
-            if hasattr(metric_instance, metric_name):
-                metric_data: MetricData = getattr(metric_instance, metric_name)
-
-                metric_diff = metric_source.get(metric_name, 0) - metric_data.last_value
-                metric_per_sec = round(metric_diff / self.polling_latency)
-
-                if format:
-                    return format_number(metric_per_sec)
-                else:
-                    return metric_per_sec
-
     def get_metric_checkpoint_age(self, format):
         checkpoint_age_bytes = round(self.global_status.get("Innodb_checkpoint_age", 0))
         max_checkpoint_age_bytes = self.redo_log_size
 
-        if checkpoint_age_bytes + max_checkpoint_age_bytes == 0:
-            return "N/A"
+        if checkpoint_age_bytes == 0:
+            if format:
+                return "N/A"
+            else:
+                return self.redo_log_size, 0, 0
 
         checkpoint_age_sync_flush_bytes = round(max_checkpoint_age_bytes * 0.825)
         checkpoint_age_ratio = round(checkpoint_age_bytes / max_checkpoint_age_bytes * 100, 2)
 
         if format:
             if checkpoint_age_ratio >= 80:
                 color_code = "red"
@@ -654,21 +903,7 @@
         if smoothed_hit_ratio is None:
             smoothed_hit_ratio = hit_ratio
         else:
             smoothed_hit_ratio = (1 - smoothing_factor) * smoothed_hit_ratio + smoothing_factor * hit_ratio
         self.metrics.adaptive_hash_index_hit_ratio.smoothed_hit_ratio = smoothed_hit_ratio
 
         return smoothed_hit_ratio
-
-    def update_metrics_last_value(self):
-        # We set the last value for specific metrics that need it so they can get per second values
-        for metric_instance in self.metrics.__dict__.values():
-            if metric_instance.metric_source == MetricSource.global_status:
-                metrics_data = self.global_status
-            elif metric_instance.metric_source == MetricSource.innodb_metrics:
-                metrics_data = self.innodb_metrics
-            elif metric_instance.metric_source == MetricSource.disk_io_metrics:
-                metrics_data = self.disk_io_metrics
-
-            for metric_name, metric_data in metric_instance.__dict__.items():
-                if isinstance(metric_data, MetricData) and metric_data.per_second_calculation:
-                    metric_data.last_value = metrics_data.get(metric_name, 0)
```

### Comparing `dolphie-4.3.5/dolphie/Modules/MySQL.py` & `dolphie-5.0.0/dolphie/Modules/MySQL.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import time
 from ssl import SSLError
 
 import pymysql
+from dolphie.DataTypes import ConnectionSource
 from dolphie.Modules.ManualException import ManualException
-from dolphie.Modules.Queries import MySQLQueries
+from dolphie.Modules.Queries import MySQLQueries, ProxySQLQueries
 from textual.app import App
 
 
 class Database:
     def __init__(
         self,
         app: App,
@@ -31,14 +32,15 @@
         self.port = port
         self.ssl = ssl
         self.save_connection_id = save_connection_id
 
         self.max_reconnect_attempts: int = 3
         self.running_query: bool = False
         self.using_ssl: str = None
+        self.source: ConnectionSource = None
 
         if auto_connect:
             self.connect()
 
     def connect(self):
         try:
             self.connection = pymysql.connect(
@@ -51,20 +53,32 @@
                 ssl=self.ssl,
                 autocommit=True,
                 connect_timeout=5,
                 program_name="Dolphie",
             )
             self.cursor = self.connection.cursor(pymysql.cursors.DictCursor)
 
+            # If the query is successful, then the connection is to ProxySQL
+            try:
+                self.cursor.execute("SELECT @@admin-version")
+                self.source = ConnectionSource.proxysql
+            except Exception:
+                self.source = ConnectionSource.mysql
+
             # Get connection ID for processlist filtering
             if self.save_connection_id:
-                self.connection_id = self.fetch_value_from_field("SELECT CONNECTION_ID()")
+                self.connection_id = self.connection.thread_id()
 
             # Determine if SSL is being used
-            self.using_ssl = "ON" if self.fetch_value_from_field("SHOW STATUS LIKE 'Ssl_cipher'", "Value") else "OFF"
+            self.using_ssl = (
+                "ON"
+                if self.source == ConnectionSource.mysql
+                and self.fetch_value_from_field("SHOW STATUS LIKE 'Ssl_cipher'", "Value")
+                else "OFF"
+            )
         except pymysql.Error as e:
             if len(e.args) == 1:
                 raise ManualException(e.args[0])
             else:
                 raise ManualException(e.args[1])
         except FileNotFoundError:  # Catch SSL file path errors
             raise ManualException("SSL certificate file path isn't valid!")
@@ -93,15 +107,16 @@
                 timeout=10,
             )
             return None
 
         error_message = None
 
         # Prefix all queries with dolphie so they can be identified in the processlist from other people
-        query = "/* dolphie */ " + query
+        if self.source != ConnectionSource.proxysql:
+            query = "/* dolphie */ " + query
 
         for _ in range(self.max_reconnect_attempts):
             self.running_query = True
 
             try:
                 rows = self.cursor.execute(query, values)
                 self.running_query = False
@@ -163,15 +178,18 @@
             )
 
     def _process_row(self, row):
         processed_row = {}
 
         for field, value in row.items():
             if isinstance(value, (bytes, bytearray)):
-                processed_row[field] = value.decode()
+                try:
+                    processed_row[field] = value.decode()
+                except UnicodeDecodeError:
+                    processed_row[field] = "/* Dolphie can't decode query with utf-8 */"
             else:
                 processed_row[field] = value
 
         return processed_row
 
     def fetchall(self):
         if not self.is_connected():
@@ -215,18 +233,22 @@
 
     def fetch_status_and_variables(self, command):
         if not self.is_connected():
             return None
 
         command_data = {}
 
-        self.execute(getattr(MySQLQueries, command))
+        if self.source == ConnectionSource.proxysql:
+            self.execute(getattr(ProxySQLQueries, command))
+        else:
+            self.execute(getattr(MySQLQueries, command))
+
         data = self.fetchall()
 
-        if command in {"status", "variables"}:
+        if command in {"status", "variables", "mysql_stats"}:
             for row in data:
                 variable = row["Variable_name"]
                 value = row["Value"]
 
                 converted_value = int(value) if value.isnumeric() else value
 
                 command_data[variable] = converted_value
```

### Comparing `dolphie-4.3.5/dolphie/Modules/Queries.py` & `dolphie-5.0.0/dolphie/Modules/Queries.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,112 @@
 from dataclasses import dataclass
 
 
 @dataclass
+class ProxySQLQueries:
+
+    processlist: str = """/* dolphie */
+        SELECT
+            SessionID AS id,
+            user AS user,
+            db AS db,
+            cli_host AS frontend_host,
+            hostgroup AS hostgroup,
+            srv_host AS backend_host,
+            command AS command,
+            time_ms AS time,
+            IFNULL(info, "") AS query,
+            IFNULL(extended_info, "") AS extended_info
+        FROM
+            stats_mysql_processlist
+        WHERE
+            $1
+    """
+    mysql_stats: str = """
+        SELECT
+            Variable_Name as Variable_name,
+            Variable_Value as Value
+        FROM
+            stats_mysql_global
+    """
+    connection_pool_data: str = """
+        SELECT
+            SUM(Latency_us) / COUNT(*) AS avg_latency,
+            SUM(ConnUsed) AS connection_pool_connections
+        FROM
+            stats_mysql_connection_pool
+    """
+    user_stats: str = """
+        SELECT DISTINCT
+            su.username,
+            frontend_connections,
+            frontend_max_connections,
+            default_hostgroup,
+            default_schema,
+            use_ssl
+        FROM
+            stats_mysql_users su JOIN
+            runtime_mysql_users ru ON su.username = ru.username
+        WHERE
+            frontend_connections > 0
+        ORDER BY
+            frontend_connections DESC
+    """
+    hostgroup_summary: str = """
+        SELECT
+            *
+        FROM
+            stats_mysql_connection_pool LEFT JOIN
+            runtime_mysql_servers ON hostgroup = hostgroup_id AND srv_host = hostname AND srv_port = port
+        ORDER BY
+            hostgroup
+    """
+    query_rules_summary: str = """
+        SELECT
+            *,
+            hits AS hits_s
+        FROM
+            stats_mysql_query_rules
+            JOIN runtime_mysql_query_rules USING (rule_id)
+        WHERE
+            active = 1
+        ORDER BY
+            hits DESC
+    """
+    command_stats: str = """
+        SELECT
+            *,
+            Total_cnt AS Total_cnt_s
+        FROM
+            stats_mysql_commands_counters
+        WHERE
+            Total_cnt != 0
+        ORDER BY
+            Total_cnt DESC
+    """
+    memory_metrics: str = """
+        SELECT
+            *
+        FROM
+            stats_memory_metrics
+        ORDER BY
+            CAST(Variable_Value AS DECIMAL) DESC;
+    """
+    query_errors: str = """
+        SELECT
+            *
+        FROM
+            stats_mysql_errors
+        ORDER BY
+            count_star DESC
+    """
+    variables: str = "SHOW GLOBAL VARIABLES"
+
+
+@dataclass
 class MySQLQueries:
     pl_query: str = """
         SELECT
             id,
             IFNULL(User, "")                    AS user,
             IFNULL(Host, "")                    AS host,
             IFNULL(db, "")                      AS db,
```

### Comparing `dolphie-4.3.5/dolphie/Panels/dashboard_panel.py` & `dolphie-5.0.0/dolphie/Panels/dashboard_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,21 +39,21 @@
 
     replicas = 0
     if dolphie.replica_manager.available_replicas:
         replicas = len(dolphie.replica_manager.available_replicas)
 
     table_information.add_column()
     table_information.add_column(min_width=25, max_width=27)
-    table_information.add_row("[label]Version", f"{dolphie.host_distro} {dolphie.mysql_version}")
+    table_information.add_row("[label]Version", f"{dolphie.host_distro} {dolphie.host_version}")
     table_information.add_row(
         "[label]", "%s (%s)" % (global_variables["version_compile_os"], global_variables["version_compile_machine"])
     )
     table_information.add_row("[label]Type", f"{host_type} [label]SSL[/label] {dolphie.main_db_connection.using_ssl}")
     table_information.add_row("[label]Uptime", str(timedelta(seconds=global_status["Uptime"])))
-    table_information.add_row("[label]Runtime", f"{runtime} [label]Latency[/label] {dolphie.refresh_latency}s")
+    table_information.add_row("[label]Runtime", f"{runtime} [dark_gray]({dolphie.refresh_latency}s)")
     table_information.add_row("[label]Replicas", "%s" % replicas)
     table_information.add_row(
         "[label]Threads",
         "[label]con[/label] %s[highlight]/[/highlight][label]run[/label]"
         " %s[highlight]/[/highlight][label]cac[/label] %s"
         % (
             format_number(global_status["Threads_connected"]),
@@ -66,15 +66,15 @@
         "[label]open[/label] %s[highlight]/[/highlight][label]opened[/label] %s"
         % (
             format_number(global_status["Open_tables"]),
             format_number(global_status["Opened_tables"]),
         ),
     )
 
-    tab.dashboard_host_information.update(table_information)
+    tab.dashboard_section_1.update(table_information)
 
     ###########
     # InnoDB  #
     ###########
     table_innodb = Table(show_header=False, box=None, title="InnoDB", title_style=table_title_style)
 
     table_innodb.add_column()
@@ -120,15 +120,15 @@
         format_bytes(
             dolphie.global_variables["innodb_buffer_pool_size"] - dolphie.global_status["Innodb_buffer_pool_bytes_data"]
         ),
     )
     table_innodb.add_row("[label]BP Dirty", format_bytes(global_status["Innodb_buffer_pool_bytes_dirty"]))
     table_innodb.add_row("[label]History List", format_number(history_list_length))
 
-    tab.dashboard_innodb.update(table_innodb)
+    tab.dashboard_section_2.update(table_innodb)
 
     ##############
     # Binary Log #
     ##############
     table_primary = Table(show_header=False, box=None, title="Binary Log", title_style=table_title_style)
 
     if not binlog_status:
@@ -187,24 +187,24 @@
 
         table_primary.add_row("[label]Compression", binlog_compression)
 
         # Save some global_variables to be used in next refresh
         if dolphie.binlog_status:
             dolphie.previous_binlog_position = dolphie.binlog_status["Position"]
 
-    tab.dashboard_binary_log.update(table_primary)
+    tab.dashboard_section_3.update(table_primary)
 
     ###############
     # Replication #
     ###############
     if dolphie.replication_status and not dolphie.panels.replication.visible:
-        tab.dashboard_replication.display = True
-        tab.dashboard_replication.update(replication_panel.create_replication_table(tab, dashboard_table=True))
+        tab.dashboard_section_5.display = True
+        tab.dashboard_section_5.update(replication_panel.create_replication_table(tab, dashboard_table=True))
     else:
-        tab.dashboard_replication.display = False
+        tab.dashboard_section_5.display = False
     ###############
     # Statistics #
     ###############
     table_stats = Table(show_header=False, box=None, title="Statistics/s", title_style=table_title_style)
 
     table_stats.add_column()
     table_stats.add_column(min_width=6)
@@ -226,8 +226,8 @@
         metric_data: MetricData = getattr(metrics, metric_name)
 
         if metric_data.values:
             table_stats.add_row(f"[label]{label}", format_number(metric_data.values[-1]))
         else:
             table_stats.add_row(f"[label]{label}", "0")
 
-    tab.dashboard_statistics.update(table_stats)
+    tab.dashboard_section_4.update(table_stats)
```

### Comparing `dolphie-4.3.5/dolphie/Panels/ddl_panel.py` & `dolphie-5.0.0/dolphie/Panels/ddl_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Panels/innodb_trx_locks_panel.py` & `dolphie-5.0.0/dolphie/Panels/innodb_trx_locks_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Panels/metadata_locks_panel.py` & `dolphie-5.0.0/dolphie/Panels/metadata_locks_panel.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,14 +20,16 @@
         "THREAD_SOURCE": {"name": "Thread Source", "width": 15},
         "PROCESSLIST_ID": {"name": "Process ID", "width": 13},
         "PROCESSLIST_USER": {"name": "User", "width": 20},
         "PROCESSLIST_TIME": {"name": "Age", "width": 8},
         "PROCESSLIST_INFO": {"name": "Query", "width": None},
     }
 
+    # Refresh optimization
+    query_length_max = 300
     metadata_locks_datatable = tab.metadata_locks_datatable
 
     if not metadata_locks_datatable.columns:
         for column_key, column_data in columns.items():
             column_name = column_data["name"]
             metadata_locks_datatable.add_column(column_name, key=column_name, width=column_data["width"])
 
@@ -64,21 +66,29 @@
                 # If the column is the query, we need to compare the code of the Syntax object
                 update_width = False
                 if column_key == "PROCESSLIST_INFO":
                     update_width = True
 
                     if isinstance(thread_value, Syntax):
                         temp_thread_value = thread_value.code
+
+                        # Only show the first {query_length_max} characters of the query
+                        thread_value = format_query(thread_value.code[:query_length_max])
+
                     if isinstance(datatable_value, Syntax):
                         temp_datatable_value = datatable_value.code
 
                 # Update the datatable if values differ
                 if temp_thread_value != temp_datatable_value:
                     metadata_locks_datatable.update_cell(lock_id, column_name, thread_value, update_width=update_width)
             else:
+                # Only show the first {query_length_max} characters of the query
+                if column_name == "Query" and isinstance(thread_value, Syntax):
+                    thread_value = format_query(thread_value.code[:query_length_max])
+
                 # Create an array of values to append to the datatable
                 row_values.append(thread_value)
 
         # Add a new row to the datatable
         if row_values:
             metadata_locks_datatable.add_row(*row_values, key=lock_id, height=row_height)
```

### Comparing `dolphie-4.3.5/dolphie/Panels/processlist_panel.py` & `dolphie-5.0.0/dolphie/Panels/processlist_panel.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from typing import Dict
 
 from dolphie.DataTypes import ProcesslistThread
-from dolphie.Modules.Functions import format_number
+from dolphie.Modules.Functions import format_number, format_query
 from dolphie.Modules.Queries import MySQLQueries
 from dolphie.Modules.TabManager import Tab
 from rich.syntax import Syntax
 from textual.widgets import DataTable
 
 
 def create_panel(tab: Tab) -> DataTable:
@@ -14,15 +14,15 @@
     if not dolphie.performance_schema_enabled and dolphie.use_performance_schema:
         dolphie.app.notify(
             "Performance Schema is not enabled on this host, using Information Schema instead for processlist"
         )
         dolphie.use_performance_schema = False
 
     columns = [
-        {"name": "Process ID", "field": "id", "width": 11, "format_number": False},
+        {"name": "Process ID", "field": "id", "width": None, "format_number": False},
         {"name": "Protocol", "field": "protocol", "width": 8, "format_number": False},
         {"name": "Username", "field": "user", "width": 20, "format_number": False},
     ]
 
     if dolphie.show_additional_query_columns:
         columns.extend(
             [
@@ -53,14 +53,16 @@
         [
             {"name": "Age", "field": "formatted_time", "width": 9, "format_number": False},
             {"name": "Query", "field": "formatted_query", "width": None, "format_number": False},
             {"name": "time_seconds", "field": "time", "width": 0, "format_number": False},
         ]
     )
 
+    # Refresh optimization
+    query_length_max = 300
     processlist_datatable = tab.processlist_datatable
 
     # Clear table if columns change
     if len(processlist_datatable.columns) != len(columns):
         processlist_datatable.clear(columns=True)
 
     # Add columns to the datatable if it is empty
@@ -80,31 +82,42 @@
             column_format_number = column_data["format_number"]
             column_value = getattr(thread, column_field)
 
             thread_value = format_number(column_value) if column_format_number else column_value
             if thread_id in processlist_datatable.rows:
                 datatable_value = processlist_datatable.get_row(thread_id)[column_id]
 
-                # Store the code of the Syntax object if it's a query
+                # Initialize temp values for possible Syntax object comparison below
                 temp_thread_value = thread_value
                 temp_datatable_value = datatable_value
 
                 # If the column is the query, we need to compare the code of the Syntax object
                 update_width = False
                 if column_field == "formatted_query":
                     update_width = True
                     if isinstance(thread_value, Syntax):
                         temp_thread_value = thread_value.code
+
+                        # Only show the first {query_length_max} characters of the query
+                        thread_value = format_query(thread_value.code[:query_length_max])
                     if isinstance(datatable_value, Syntax):
                         temp_datatable_value = datatable_value.code
 
                 # Update the datatable if values differ
-                if temp_thread_value != temp_datatable_value or column_field == "formatted_time":
+                if (
+                    temp_thread_value != temp_datatable_value
+                    or column_field == "formatted_time"
+                    or column_field == "time"
+                ):
                     processlist_datatable.update_cell(thread_id, column_name, thread_value, update_width=update_width)
             else:
+                # Only show the first {query_length_max} characters of the query
+                if column_field == "formatted_query" and isinstance(thread_value, Syntax):
+                    thread_value = format_query(thread_value.code[:query_length_max])
+
                 # Create an array of values to append to the datatable
                 row_values.append(thread_value)
 
         # Add a new row to the datatable
         if row_values:
             processlist_datatable.add_row(*row_values, key=thread_id)
```

### Comparing `dolphie-4.3.5/dolphie/Panels/replication_panel.py` & `dolphie-5.0.0/dolphie/Panels/replication_panel.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Widgets/command_screen.py` & `dolphie-5.0.0/dolphie/Widgets/command_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Widgets/event_log_screen.py` & `dolphie-5.0.0/dolphie/Widgets/event_log_screen.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Widgets/host_setup.py` & `dolphie-5.0.0/dolphie/Widgets/host_setup.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Widgets/modal.py` & `dolphie-5.0.0/dolphie/Widgets/modal.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import re
 
-from dolphie.DataTypes import HotkeyCommands
+from dolphie.DataTypes import ConnectionSource, HotkeyCommands
 from textual.app import ComposeResult
 from textual.binding import Binding
 from textual.containers import Horizontal, Vertical
 from textual.screen import ModalScreen
 from textual.widgets import (
     Button,
     Checkbox,
@@ -57,18 +57,21 @@
             width: 100%;
         }
     """
     BINDINGS = [
         Binding("escape", "app.pop_screen", "", show=False),
     ]
 
-    def __init__(self, command, message, processlist_data=None, host_cache_data=None):
+    def __init__(
+        self, command, message, connection_source: ConnectionSource = None, processlist_data=None, host_cache_data=None
+    ):
         super().__init__()
         self.command = command
         self.message = message
+        self.connection_source = connection_source
         self.processlist_data = processlist_data
         self.host_cache_data = host_cache_data
 
         self.dropdown_items = []
         if processlist_data:
             sorted_keys = sorted(processlist_data.keys(), key=lambda x: int(x))
             self.dropdown_items = [DropdownItem(thread_id) for thread_id in sorted_keys]
@@ -77,14 +80,15 @@
         with Vertical():
             with Vertical():
                 yield Label(self.message)
                 with RadioSet(id="filter_radio_buttons"):
                     yield RadioButton("User", id="user")
                     yield RadioButton("Host/IP", id="host")
                     yield RadioButton("Database", id="db")
+                    yield RadioButton("Hostgroup", id="hostgroup")
                     yield RadioButton("Query Text", id="query_text")
                     yield RadioButton("Query Time", id="query_time")
                 with Vertical(id="kill_container"):
                     with RadioSet(id="kill_radio_buttons"):
                         yield RadioButton("Username", id="username")
                         yield RadioButton("Host/IP", id="host")
                         yield RadioButton("Time range", id="time_range")
@@ -108,14 +112,17 @@
         kill_container.display = False
 
         if self.command == HotkeyCommands.thread_filter:
             filter_radio_buttons.display = True
             filter_radio_buttons.focus()
 
             input.placeholder = "Select an option from above"
+
+            if self.connection_source != ConnectionSource.proxysql:
+                self.query_one("#filter_radio_buttons #hostgroup", RadioButton).display = False
         elif self.command == HotkeyCommands.thread_kill_by_parameter:
             sleeping_queries_checkbox = self.query_one("#sleeping_queries", Checkbox)
             sleeping_queries_checkbox.toggle()
 
             kill_container.display = True
 
             kill_radio_buttons = self.query_one("#kill_radio_buttons", RadioSet)
@@ -165,14 +172,17 @@
             elif event.pressed.id == "query_text":
                 modal_input.placeholder = "Partial query text"
             elif event.pressed.id == "query_time":
                 modal_input.placeholder = "Minimum query time (in seconds)"
             elif event.pressed.id == "user":
                 self.create_dropdown_items("user")
                 modal_input.placeholder = "Username"
+            elif event.pressed.id == "hostgroup":
+                self.create_dropdown_items("hostgroup")
+                modal_input.placeholder = "Hostgroup"
         elif self.command == HotkeyCommands.thread_kill_by_parameter:
             if event.pressed.id == "username":
                 self.create_dropdown_items("user")
                 modal_input.placeholder = "Username"
             elif event.pressed.id == "host":
                 self.create_dropdown_items("host")
                 modal_input.placeholder = "Hostname or IP address"
@@ -192,28 +202,29 @@
             return
 
         if self.command == HotkeyCommands.thread_filter:
             filter_options = {
                 "user": "User",
                 "db": "Database",
                 "host": "Host",
+                "hostgroup": "Hostgroup",
                 "query_time": "Query time",
                 "query_text": "Query text",
             }
 
             for rb_id, label in filter_options.items():
                 if self.query_one(f"#filter_radio_buttons #{rb_id}", RadioButton).value:
                     filter_id = rb_id
                     filter_label = label
                     break
 
             if filter_label:
-                if filter_id == "query_time":
+                if filter_id in ["query_time", "hostgroup"]:
                     if not modal_input.isdigit():
-                        self.update_error_response("Query time must be an integer")
+                        self.update_error_response("Value must be an integer")
                     else:
                         self.dismiss([filter_label, int(modal_input)])
                 elif filter_id == "query_text":
                     self.dismiss([filter_label, modal_input])
                 else:
                     if filter_id == "host":
                         value = next((ip for ip, addr in self.host_cache_data.items() if modal_input == addr), None)
@@ -259,15 +270,15 @@
                 self.dismiss([rb.id, modal_input, checkbox_sleeping_queries, lower_limit, upper_limit])
             else:
                 self.update_error_response("Please select a kill option")
         elif self.command in [HotkeyCommands.thread_kill_by_id, HotkeyCommands.show_thread]:
             value = next((thread_id for thread_id in self.processlist_data.keys() if modal_input == thread_id), None)
 
             if not value:
-                self.update_error_response(f"Thread ID [b red]{modal_input}[/b red] does not exist")
+                self.update_error_response(f"Process ID [bold red]{modal_input}[/bold red] does not exist")
             else:
                 self.dismiss(modal_input)
         elif self.command == HotkeyCommands.refresh_interval:
             if not modal_input.isnumeric():
                 self.update_error_response("Input must be an integer")
                 return
```

### Comparing `dolphie-4.3.5/dolphie/Widgets/spinner.py` & `dolphie-5.0.0/dolphie/Widgets/spinner.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/Widgets/thread_screen.py` & `dolphie-5.0.0/dolphie/Widgets/thread_screen.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
         height: auto;
     }
     ThreadScreen #thread_container {
         margin-top: 1;
         height: auto;
         layout: horizontal;
     }
-    ThreadScreen Label {
+    ThreadScreen .title {
         width: 100%;
         content-align: center middle;
         color: #bbc8e8;
         text-style: bold;
     }
     ThreadScreen Center {
         height: auto;
@@ -140,31 +140,31 @@
             self.query_one("#query_container").display = False
 
     def compose(self) -> ComposeResult:
         yield TopBar(connection_status=self.connection_status, app_version=self.app_version, host=self.host)
 
         with Container(id="thread_container", classes="container"):
             with Container():
-                yield Label("Thread Details")
+                yield Label("Process Details", classes="title")
                 yield ScrollableContainer(Static(id="thread_table"), classes="table")
             with Container():
-                yield Label("Thread Attributes")
+                yield Label("Process Attributes", classes="title")
                 yield ScrollableContainer(Static(id="user_thread_attributes_table"), classes="table")
 
         with Container(id="query_container", classes="container"):
             yield Rule(line_style="heavy")
-            yield Label("Query Details")
+            yield Label("Query Details", classes="title")
             yield Center(Static(id="query", shrink=True, classes="table"))
 
             yield DataTable(show_cursor=False, id="explain_table", classes="table")
             yield Label("", id="explain_failure")
 
         with Container(id="transaction_history_container", classes="container"):
             yield Rule(line_style="heavy")
-            yield Label("Transaction History", id="transaction_history_label")
+            yield Label("Transaction History", id="transaction_history_label", classes="title")
             yield Center(
                 Static(id="transaction_history_table", shrink=True, classes="table"),
                 id="transaction_history_table_center",
             )
 
     @on(events.Key)
     def on_keypress(self, event: events.Key):
```

### Comparing `dolphie-4.3.5/dolphie/Widgets/topbar.py` & `dolphie-5.0.0/dolphie/Widgets/topbar.py`

 * *Files identical despite different names*

### Comparing `dolphie-4.3.5/dolphie/__init__.py` & `dolphie-5.0.0/dolphie/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import socket
 from datetime import datetime
 
 import dolphie.DataTypes as DataTypes
 import dolphie.Modules.MetricManager as MetricManager
 from dolphie.Modules.ArgumentParser import Config
 from dolphie.Modules.Functions import load_host_cache_file
-from dolphie.Modules.MySQL import Database
+from dolphie.Modules.MySQL import ConnectionSource, Database
 from dolphie.Modules.Queries import MySQLQueries
 from packaging.version import parse as parse_version
 from textual.app import App
 from textual.widgets import Switch
 
 
 class Dolphie:
@@ -34,45 +34,35 @@
         self.refresh_interval = config.refresh_interval
         self.show_trxs_only = config.show_trxs_only
         self.show_additional_query_columns = config.show_additional_query_columns
         self.heartbeat_table = config.heartbeat_table
         self.host_setup_available_hosts = config.host_setup_available_hosts
         self.startup_panels = config.startup_panels
         self.graph_marker = config.graph_marker
-        # self.historical_trx_locks = config.historical_trx_locks
         self.hostgroup = config.hostgroup
         self.hostgroup_hosts = config.hostgroup_hosts
 
         self.reset_runtime_variables()
 
         # Set the default panels based on startup_panels to be visible
         self.panels = DataTypes.Panels()
         for panel in self.panels.all():
             setattr(getattr(self.panels, panel), "visible", False)
+
         for panel in self.startup_panels:
-            setattr(getattr(self.panels, panel), "visible", True)
+            if panel in self.panels.all():
+                setattr(getattr(self.panels, panel), "visible", True)
 
         self.show_idle_threads: bool = False
         self.sort_by_time_descending: bool = True
 
     def reset_runtime_variables(self):
         self.metric_manager = MetricManager.MetricManager()
         self.replica_manager = DataTypes.ReplicaManager()
 
-        # Set the graph switches to what they're currently selected to since we reset metric_manager
-        switches = self.app.query(f".switch_container_{self.tab_id} Switch")
-        for switch in switches:
-            switch: Switch
-            metric_instance_name = switch.name
-            metric = switch.id
-
-            metric_instance = getattr(self.metric_manager.metrics, metric_instance_name)
-            metric_data: MetricManager.MetricData = getattr(metric_instance, metric)
-            metric_data.visible = switch.value
-
         self.dolphie_start_time: datetime = datetime.now()
         self.worker_start_time: datetime = datetime.now()
         self.worker_previous_start_time: datetime = datetime.now()
         self.completed_first_loop: bool = False
         self.polling_latency: float = 0
         self.refresh_latency: str = "0"
         self.connection_status: DataTypes.ConnectionStatus = None
@@ -91,33 +81,38 @@
         self.global_status: dict = {}
         self.binlog_status: dict = {}
         self.replication_status: dict = {}
         self.replication_applier_status: dict = {}
         self.replica_lag_source: str = None
         self.replica_lag: int = None
         self.active_redo_logs: int = None
-        self.mysql_host: str = f"{self.host}:{self.port}"
+        self.host_with_port: str = f"{self.host}:{self.port}"
         self.binlog_transaction_compression_percentage: int = None
         self.host_cache: dict = {}
+        self.proxysql_hostgroup_summary: dict = {}
+        self.proxysql_mysql_query_rules: dict = {}
+        self.proxysql_per_second_data: dict = {}
+        self.proxysql_command_stats: dict = {}
+        self.proxysql_process_execution_time: float = 0
 
         self.user_filter = None
         self.db_filter = None
         self.host_filter = None
+        self.hostgroup_filter = None
         self.query_time_filter = None
         self.query_filter = None
 
         # Types of hosts
+        self.connection_source: ConnectionSource = ConnectionSource.mysql
+        self.connection_source_alt: ConnectionSource = ConnectionSource.mysql  # rds, azure, etc
         self.galera_cluster: bool = False
         self.group_replication: bool = False
         self.innodb_cluster: bool = False
         self.innodb_cluster_read_replica: bool = False
         self.replicaset: bool = False
-        self.aws_rds: bool = False
-        self.azure: bool = False
-        self.mariadb: bool = False
 
         # These are for group replication in replication panel
         self.is_group_replication_primary: bool = False
         self.group_replication_members: dict = {}
         self.group_replication_data: dict = {}
 
         # Main connection is used for Textual's worker thread so it can run asynchronous
@@ -134,70 +129,87 @@
         self.main_db_connection = Database(**db_connection_args)
         # Secondary connection is for ad-hoc commands that are not a part of the worker thread
         self.secondary_db_connection = Database(**db_connection_args, save_connection_id=False)
 
         self.performance_schema_enabled: bool = False
         self.use_performance_schema: bool = True
         self.server_uuid: str = None
-        self.mysql_version: str = None
+        self.host_version: str = None
         self.host_distro: str = None
 
         self.host_cache_from_file = load_host_cache_file(self.host_cache_file)
 
+        self.update_switches_after_reset()
+
     def db_connect(self):
         self.main_db_connection.connect()
         self.secondary_db_connection.connect()
 
+        version = self.main_db_connection.fetch_value_from_field("SELECT @@version")
+        version_split = version.split(".")
+        self.host_version = "%s.%s.%s" % (
+            version_split[0],
+            version_split[1],
+            version_split[2].split("-")[0],
+        )
+
+        self.connection_source = self.main_db_connection.source
+        self.connection_source_alt = self.connection_source
+        if self.connection_source == ConnectionSource.proxysql:
+            self.host_distro = "ProxySQL"
+            self.host_with_port = f"{self.host}:{self.port}"
+        elif self.connection_source == ConnectionSource.mysql:
+            self.setup_connection_mysql()
+
+        # Add host to host setup file if it doesn't exist
+        self.add_host_to_host_cache_file()
+
+    def setup_connection_mysql(self):
         global_variables = self.main_db_connection.fetch_status_and_variables("variables")
 
         basedir = global_variables.get("basedir")
         aurora_version = global_variables.get("aurora_version")
         version = global_variables.get("version").lower()
         version_comment = global_variables.get("version_comment").lower()
         version_split = version.split(".")
-        self.mysql_version = "%s.%s.%s" % (
-            version_split[0],
-            version_split[1],
-            version_split[2].split("-")[0],
-        )
 
         # Get proper host version and fork
         if "percona xtradb cluster" in version_comment:
             self.host_distro = "Percona XtraDB Cluster"
         elif "percona server" in version_comment:
             self.host_distro = "Percona Server"
         elif "mariadb cluster" in version_comment:
             self.host_distro = "MariaDB Cluster"
-            self.mariadb = True
+            self.connection_source_alt == ConnectionSource.mariadb
         elif "mariadb" in version_comment or "mariadb" in version:
             self.host_distro = "MariaDB"
-            self.mariadb = True
+            self.connection_source_alt == ConnectionSource.mariadb
         elif aurora_version:
             self.host_distro = "Amazon Aurora"
-            self.aws_rds = True
+            self.connection_source_alt == ConnectionSource.aws_rds
         elif "rdsdb" in basedir:
             self.host_distro = "Amazon RDS"
-            self.aws_rds = True
+            self.connection_source_alt == ConnectionSource.aws_rds
         elif global_variables.get("aad_auth_only"):
             self.host_distro = "Azure MySQL"
-            self.azure = True
+            self.connection_source_alt == ConnectionSource.azure_mysql
         else:
             self.host_distro = "MySQL"
 
         # For RDS and Azure, we will use the host specified to connect with since hostname isn't related to the endpoint
-        if self.aws_rds:
-            self.mysql_host = f"{self.host.split('.rds.amazonaws.com')[0]}:{self.port}"
-        elif self.azure:
-            self.mysql_host = f"{self.host.split('.mysql.database.azure.com')[0]}:{self.port}"
+        if self.connection_source_alt == ConnectionSource.aws_rds:
+            self.host_with_port = f"{self.host.split('.rds.amazonaws.com')[0]}:{self.port}"
+        elif self.connection_source_alt == ConnectionSource.azure_mysql:
+            self.host_with_port = f"{self.host.split('.mysql.database.azure.com')[0]}:{self.port}"
         else:
-            self.mysql_host = f"{global_variables.get('hostname')}:{self.port}"
+            self.host_with_port = f"{global_variables.get('hostname')}:{self.port}"
 
         major_version = int(version_split[0])
         self.server_uuid = global_variables.get("server_uuid")
-        if "MariaDB" in self.host_distro and major_version >= 10:
+        if self.connection_source_alt == ConnectionSource.mariadb and major_version >= 10:
             self.server_uuid = global_variables.get("server_id")
 
         if global_variables.get("performance_schema") == "ON":
             self.performance_schema_enabled = True
 
         # Check to see if the host is in a Galera cluster
         galera_matches = any(key.startswith("wsrep_") for key in global_variables.keys())
@@ -224,30 +236,30 @@
             if instance_type == "read-replica":
                 self.innodb_cluster = False  # It doesn't work like an actual member in a cluster so set it to False
                 self.innodb_cluster_read_replica = True
 
         if not self.innodb_cluster and global_variables.get("group_replication_group_name"):
             self.group_replication = True
 
-        # Add host to host setup file if it doesn't exist
+    def add_host_to_host_cache_file(self):
         with open(self.host_setup_file, "a+") as file:
             file.seek(0)
             lines = file.readlines()
 
             if self.port != 3306:
                 host = f"{self.host}:{self.port}\n"
             else:
                 host = f"{self.host}\n"
 
             if host not in lines:
                 file.write(host)
                 self.host_setup_available_hosts.append(host[:-1])  # remove the \n
 
     def is_mysql_version_at_least(self, target, use_version=None):
-        version = self.mysql_version
+        version = self.host_version
         if use_version:
             version = use_version
 
         parsed_source = parse_version(version)
         parsed_target = parse_version(target)
 
         return parsed_source >= parsed_target
@@ -270,23 +282,38 @@
 
         return hostname
 
     def massage_metrics_data(self):
         if self.is_mysql_version_at_least("8.0"):
             # If we're using MySQL 8, we need to fetch the checkpoint age from the performance schema if it's not
             # available in global status
-            # On Azure MySQL there is no BACKUP_ADMIN privilege so we can't fetch the checkpoint age
-            if not self.global_status.get("Innodb_checkpoint_age") and not self.azure:
+            # On Azure/Aurora MySQL there is no BACKUP_ADMIN privilege so we can't fetch the checkpoint age from them
+            if (
+                not self.global_status.get("Innodb_checkpoint_age")
+                and self.connection_source_alt == ConnectionSource.mysql
+            ):
                 self.global_status["Innodb_checkpoint_age"] = self.main_db_connection.fetch_value_from_field(
                     MySQLQueries.checkpoint_age, "checkpoint_age"
                 )
 
             if self.is_mysql_version_at_least("8.0.30"):
                 active_redo_logs_count = self.main_db_connection.fetch_value_from_field(
                     MySQLQueries.active_redo_logs, "count"
                 )
                 self.global_status["Active_redo_log_count"] = active_redo_logs_count
 
         # If the server doesn't support Innodb_lsn_current, use Innodb_os_log_written instead
         # which has less precision, but it's good enough
         if not self.global_status.get("Innodb_lsn_current"):
             self.global_status["Innodb_lsn_current"] = self.global_status["Innodb_os_log_written"]
+
+    def update_switches_after_reset(self):
+        # Set the graph switches to what they're currently selected to after a reset
+        switches = self.app.query(f".switch_container_{self.tab_id} Switch")
+        for switch in switches:
+            switch: Switch
+            metric_instance_name = switch.name
+            metric = switch.id
+
+            metric_instance = getattr(self.metric_manager.metrics, metric_instance_name)
+            metric_data: MetricManager.MetricData = getattr(metric_instance, metric)
+            metric_data.visible = switch.value
```

### Comparing `dolphie-4.3.5/dolphie/app.py` & `dolphie-5.0.0/dolphie/app.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,48 +11,62 @@
 from datetime import datetime, timedelta
 from functools import partial
 from importlib import metadata
 
 import dolphie.Modules.MetricManager as MetricManager
 import requests
 from dolphie import Dolphie
-from dolphie.DataTypes import ConnectionStatus, HotkeyCommands, ProcesslistThread
+from dolphie.DataTypes import (
+    ConnectionSource,
+    ConnectionStatus,
+    HotkeyCommands,
+    ProcesslistThread,
+    ProxySQLProcesslistThread,
+)
 from dolphie.Modules.ArgumentParser import ArgumentParser, Config
 from dolphie.Modules.Functions import (
+    format_bytes,
     format_number,
     format_query,
     format_sys_table_memory,
 )
 from dolphie.Modules.ManualException import ManualException
-from dolphie.Modules.Queries import MySQLQueries
+from dolphie.Modules.Queries import MySQLQueries, ProxySQLQueries
 from dolphie.Modules.TabManager import Tab, TabManager
 from dolphie.Panels import (
     dashboard_panel,
     ddl_panel,
     metadata_locks_panel,
     processlist_panel,
+    proxysql_command_stats_panel,
+    proxysql_dashboard_panel,
+    proxysql_hostgroup_summary_panel,
+    proxysql_mysql_query_rules_panel,
+    proxysql_processlist_panel,
     replication_panel,
 )
 from dolphie.Widgets.command_screen import CommandScreen
 from dolphie.Widgets.event_log_screen import EventLog
+from dolphie.Widgets.help import HelpScreen
 from dolphie.Widgets.modal import CommandModal
+from dolphie.Widgets.proxysql_thread_screen import ProxySQLThreadScreen
 from dolphie.Widgets.thread_screen import ThreadScreen
 from dolphie.Widgets.topbar import TopBar
 from packaging.version import parse as parse_version
 from rich import box
 from rich.align import Align
 from rich.console import Group
 from rich.style import Style
 from rich.table import Table
 from rich.theme import Theme
 from rich.traceback import Traceback
 from sqlparse import format as sqlformat
 from textual import events, on, work
 from textual.app import App
-from textual.widgets import Switch, TabbedContent
+from textual.widgets import Switch, TabbedContent, TabPane
 from textual.worker import Worker, WorkerState, get_current_worker
 
 try:
     __package_name__ = metadata.metadata(__package__ or __name__)["Name"]
     __version__ = metadata.version(__package__ or __name__)
 except Exception:
     __package_name__ = "Dolphie"
@@ -81,15 +95,15 @@
                 "dark_gray": "#969aad",
                 "highlight": "#91abec",
                 "label": "#c5c7d2",
                 "b label": "b #c5c7d2",
                 "light_blue": "#bbc8e8",
                 "b white": "b #e9e9e9",
                 "b highlight": "b #91abec",
-                "b red": "b #fd8383",
+                "bold red": "b #fd8383",
                 "b light_blue": "b #bbc8e8",
                 "panel_border": "#6171a6",
                 "table_border": "#333f62",
             }
         )
         self.console.push_theme(theme)
         self.console.set_window_title(self.TITLE)
@@ -102,124 +116,31 @@
         tab.worker = get_current_worker()
         tab.worker.name = tab_id
         tab.worker_running = True
 
         dolphie = tab.dolphie
         try:
             if not dolphie.main_db_connection.is_connected():
-                self.tab_manager.rename_tab(tab)  # this will use dolphie.host instead of mysql_host
+                self.tab_manager.rename_tab(tab)  # this will use dolphie.host instead of host_with_port
                 self.tab_manager.update_topbar(tab=tab, connection_status=ConnectionStatus.connecting)
                 tab.loading_indicator.display = True
 
                 dolphie.db_connect()
                 self.tab_manager.rename_tab(tab)
 
             dolphie.worker_start_time = datetime.now()
             dolphie.polling_latency = (dolphie.worker_start_time - dolphie.worker_previous_start_time).total_seconds()
             dolphie.refresh_latency = round(dolphie.polling_latency - dolphie.refresh_interval, 2)
             dolphie.worker_previous_start_time = dolphie.worker_start_time
 
-            dolphie.global_variables = dolphie.main_db_connection.fetch_status_and_variables("variables")
-            dolphie.global_status = dolphie.main_db_connection.fetch_status_and_variables("status")
-            dolphie.innodb_metrics = dolphie.main_db_connection.fetch_status_and_variables("innodb_metrics")
-
-            if dolphie.performance_schema_enabled and dolphie.is_mysql_version_at_least("5.7"):
-                find_replicas_query = MySQLQueries.ps_find_replicas
-            else:
-                find_replicas_query = MySQLQueries.pl_find_replicas
-
-            dolphie.main_db_connection.execute(find_replicas_query)
-            available_replicas = dolphie.main_db_connection.fetchall()
-            # We update the replica ports used if the number of replicas have changed
-            if len(available_replicas) != len(dolphie.replica_manager.available_replicas):
-                dolphie.replica_manager.ports = {}
-
-                dolphie.main_db_connection.execute(MySQLQueries.get_replicas)
-                replica_data = dolphie.main_db_connection.fetchall()
-                for row in replica_data:
-                    dolphie.replica_manager.ports[row["Slave_UUID"]] = row["Port"]
-
-                dolphie.replica_manager.available_replicas = available_replicas
-
-            dolphie.main_db_connection.execute(MySQLQueries.ps_disk_io)
-            dolphie.disk_io_metrics = dolphie.main_db_connection.fetchone()
-
-            dolphie.previous_replica_sbm = dolphie.replica_lag
-            dolphie.replica_lag_source, dolphie.replica_lag, dolphie.replication_status = (
-                replication_panel.fetch_replication_data(tab)
-            )
-
-            # If using MySQL 8, fetch the replication applier status data
-            if (
-                dolphie.is_mysql_version_at_least("8.0")
-                and dolphie.panels.replication.visible
-                and dolphie.global_variables.get("slave_parallel_workers", 0) > 1
-            ):
-                dolphie.main_db_connection.execute(MySQLQueries.replication_applier_status)
-                dolphie.replication_applier_status = dolphie.main_db_connection.fetchall()
-
-            dolphie.massage_metrics_data()
-
-            if dolphie.group_replication or dolphie.innodb_cluster:
-                if dolphie.is_mysql_version_at_least("8.0.13"):
-                    dolphie.main_db_connection.execute(MySQLQueries.group_replication_get_write_concurrency)
-                    dolphie.group_replication_data = dolphie.main_db_connection.fetchone()
-
-                dolphie.main_db_connection.execute(MySQLQueries.get_group_replication_members)
-                dolphie.group_replication_members = dolphie.main_db_connection.fetchall()
-                for member_role_data in dolphie.group_replication_members:
-                    if (
-                        member_role_data.get("MEMBER_ID") == dolphie.server_uuid
-                        and member_role_data.get("MEMBER_ROLE") == "PRIMARY"
-                    ):
-                        dolphie.is_group_replication_primary = True
-                        break
-
-            if dolphie.panels.dashboard.visible:
-                dolphie.main_db_connection.execute(MySQLQueries.binlog_status)
-                dolphie.binlog_status = dolphie.main_db_connection.fetchone()
-
-                # This can cause MySQL to crash: https://perconadev.atlassian.net/browse/PS-9066
-                # if dolphie.global_variables.get("binlog_transaction_compression") == "ON":
-                #     dolphie.main_db_connection.execute(MySQLQueries.get_binlog_transaction_compression_percentage)
-                #     dolphie.binlog_transaction_compression_percentage = dolphie.main_db_connection.fetchone().get(
-                #         "compression_percentage"
-                #     )
-
-            if dolphie.panels.processlist.visible:
-                dolphie.processlist_threads = processlist_panel.fetch_data(tab)
-
-            if dolphie.is_mysql_version_at_least("5.7"):
-                if dolphie.panels.metadata_locks.visible:
-                    dolphie.metadata_locks = metadata_locks_panel.fetch_data(tab)
-                else:
-                    # Reset this data so the graph doesn't show old data
-                    dolphie.metadata_locks = {}
-
-                # This can cause MySQL to crash: https://bugs.mysql.com/bug.php?id=112035
-                # if dolphie.panels.innodb_trx_locks.visible or dolphie.historical_trx_locks:
-                #     dolphie.main_db_connection.execute(MySQLQueries.locks_query)
-                #     dolphie.lock_transactions = dolphie.main_db_connection.fetchall()
-
-                if dolphie.panels.ddl.visible:
-                    dolphie.main_db_connection.execute(MySQLQueries.ddls)
-                    dolphie.ddl = dolphie.main_db_connection.fetchall()
-
-            dolphie.metric_manager.refresh_data(
-                worker_start_time=dolphie.worker_start_time,
-                polling_latency=dolphie.polling_latency,
-                global_variables=dolphie.global_variables,
-                global_status=dolphie.global_status,
-                innodb_metrics=dolphie.innodb_metrics,
-                disk_io_metrics=dolphie.disk_io_metrics,
-                # innodb_trx_lock_metrics=dolphie.lock_transactions,
-                metadata_lock_metrics=dolphie.metadata_locks,
-                replication_status=dolphie.replication_status,
-                replication_lag=dolphie.replica_lag,
-            )
+            if dolphie.connection_source == ConnectionSource.mysql:
+                self.process_mysql_data(tab)
+            elif dolphie.connection_source == ConnectionSource.proxysql:
+                self.process_proxysql_data(tab)
+                dolphie.proxysql_process_execution_time = (datetime.now() - dolphie.worker_start_time).total_seconds()
         except ManualException as exception:
             # This will set up the worker state change function below to trigger the
             # host setup modal with the error
             tab.worker_cancel_error = exception
 
             await self.tab_manager.disconnect_tab(tab)
 
@@ -240,27 +161,63 @@
 
                 # Skip this if the conditions are right
                 if len(self.screen_stack) > 1 or dolphie.pause_refresh or not dolphie.main_db_connection.is_connected():
                     tab.worker_timer = self.set_timer(dolphie.refresh_interval, partial(self.run_worker_main, tab.id))
 
                     return
 
-                self.refresh_screen(tab)
+                # If the main container isn't displayed, it means we just connected
+                if not tab.main_container.display:
+                    tab.main_container.display = True
+                    tab.sparkline.display = True
+
+                    # Hide all graph tabs so we can show the ones we want
+                    tabs = tab.metric_graph_tabs.query(TabPane)
+                    for graph_tab in tabs:
+                        tab.metric_graph_tabs.hide_tab(graph_tab.id)
+
+                    # Show the tabs that are for the current connection source
+                    for metric_instance in dolphie.metric_manager.metrics.__dict__.values():
+                        if dolphie.connection_source in metric_instance.connection_source:
+                            tab.metric_graph_tabs.show_tab(f"graph_tab_{metric_instance.tab_name}_{tab.id}")
+
+                refresh_interval = dolphie.refresh_interval
+                if dolphie.connection_source == ConnectionSource.mysql:
+                    self.refresh_screen_mysql(tab)
+                elif dolphie.connection_source == ConnectionSource.proxysql:
+                    self.refresh_screen_proxysql(tab)
+
+                    # If we have a lot of client connections, increase the refresh interval based on the
+                    # proxysql process execution time. René asked for this to be added to reduce load on ProxySQL
+                    client_connections = dolphie.global_status.get("Client_Connections_connected", 0)
+                    if client_connections > 30000:
+                        percentage = 0.60
+                    elif client_connections > 20000:
+                        percentage = 0.50
+                    elif client_connections > 10000:
+                        percentage = 0.40
+                    else:
+                        percentage = 0
+
+                    if percentage:
+                        refresh_interval = dolphie.refresh_interval + (
+                            dolphie.proxysql_process_execution_time * percentage
+                        )
 
-                tab.worker_timer = self.set_timer(dolphie.refresh_interval, partial(self.run_worker_main, tab.id))
+                tab.worker_timer = self.set_timer(refresh_interval, partial(self.run_worker_main, tab.id))
             elif event.state == WorkerState.CANCELLED:
                 # Only show the modal if there's a worker cancel error
                 if tab.worker_cancel_error:
                     if self.tab_manager.active_tab.id != tab.id or self.loading_hostgroups:
                         self.notify(
                             (
                                 f"[b light_blue]{dolphie.host}:{dolphie.port}[/b light_blue]: "
                                 f"{tab.worker_cancel_error.reason}"
                             ),
-                            title="MySQL Connection Error",
+                            title="Connection Error",
                             severity="error",
                             timeout=10,
                         )
 
                     if not self.loading_hostgroups:
                         self.tab_manager.switch_tab(tab.id)
 
@@ -310,27 +267,206 @@
                 tab.replicas_worker_running = False
             else:
                 tab.replicas_container.display = False
         else:
             # If we're not displaying the replication panel, close all replica connections
             dolphie.replica_manager.remove_all()
 
-    def refresh_screen(self, tab: Tab):
+    def process_mysql_data(self, tab: Tab):
+        dolphie = tab.dolphie
+
+        dolphie.global_variables = dolphie.main_db_connection.fetch_status_and_variables("variables")
+        dolphie.global_status = dolphie.main_db_connection.fetch_status_and_variables("status")
+        dolphie.innodb_metrics = dolphie.main_db_connection.fetch_status_and_variables("innodb_metrics")
+
+        if dolphie.performance_schema_enabled and dolphie.is_mysql_version_at_least("5.7"):
+            find_replicas_query = MySQLQueries.ps_find_replicas
+        else:
+            find_replicas_query = MySQLQueries.pl_find_replicas
+
+        dolphie.main_db_connection.execute(find_replicas_query)
+        available_replicas = dolphie.main_db_connection.fetchall()
+        # We update the replica ports used if the number of replicas have changed
+        if len(available_replicas) != len(dolphie.replica_manager.available_replicas):
+            dolphie.replica_manager.ports = {}
+
+            dolphie.main_db_connection.execute(MySQLQueries.get_replicas)
+            replica_data = dolphie.main_db_connection.fetchall()
+            for row in replica_data:
+                dolphie.replica_manager.ports[row["Slave_UUID"]] = row["Port"]
+
+            dolphie.replica_manager.available_replicas = available_replicas
+
+        dolphie.main_db_connection.execute(MySQLQueries.ps_disk_io)
+        dolphie.disk_io_metrics = dolphie.main_db_connection.fetchone()
+
+        dolphie.previous_replica_sbm = dolphie.replica_lag
+        dolphie.replica_lag_source, dolphie.replica_lag, dolphie.replication_status = (
+            replication_panel.fetch_replication_data(tab)
+        )
+
+        # If using MySQL 8, fetch the replication applier status data
+        if (
+            dolphie.is_mysql_version_at_least("8.0")
+            and dolphie.panels.replication.visible
+            and dolphie.global_variables.get("slave_parallel_workers", 0) > 1
+        ):
+            dolphie.main_db_connection.execute(MySQLQueries.replication_applier_status)
+            dolphie.replication_applier_status = dolphie.main_db_connection.fetchall()
+
+        dolphie.massage_metrics_data()
+
+        if dolphie.group_replication or dolphie.innodb_cluster:
+            if dolphie.is_mysql_version_at_least("8.0.13"):
+                dolphie.main_db_connection.execute(MySQLQueries.group_replication_get_write_concurrency)
+                dolphie.group_replication_data = dolphie.main_db_connection.fetchone()
+
+            dolphie.main_db_connection.execute(MySQLQueries.get_group_replication_members)
+            dolphie.group_replication_members = dolphie.main_db_connection.fetchall()
+            for member_role_data in dolphie.group_replication_members:
+                if (
+                    member_role_data.get("MEMBER_ID") == dolphie.server_uuid
+                    and member_role_data.get("MEMBER_ROLE") == "PRIMARY"
+                ):
+                    dolphie.is_group_replication_primary = True
+                    break
+
+        if dolphie.panels.dashboard.visible:
+            dolphie.main_db_connection.execute(MySQLQueries.binlog_status)
+            dolphie.binlog_status = dolphie.main_db_connection.fetchone()
+
+            # This can cause MySQL to crash: https://perconadev.atlassian.net/browse/PS-9066
+            # if dolphie.global_variables.get("binlog_transaction_compression") == "ON":
+            #     dolphie.main_db_connection.execute(MySQLQueries.get_binlog_transaction_compression_percentage)
+            #     dolphie.binlog_transaction_compression_percentage = dolphie.main_db_connection.fetchone().get(
+            #         "compression_percentage"
+            #     )
+
+        if dolphie.panels.processlist.visible:
+            dolphie.processlist_threads = processlist_panel.fetch_data(tab)
+
+        if dolphie.is_mysql_version_at_least("5.7"):
+            if dolphie.panels.metadata_locks.visible:
+                dolphie.metadata_locks = metadata_locks_panel.fetch_data(tab)
+            else:
+                # Reset this data so the graph doesn't show old data
+                dolphie.metadata_locks = {}
+
+            if dolphie.panels.ddl.visible:
+                dolphie.main_db_connection.execute(MySQLQueries.ddls)
+                dolphie.ddl = dolphie.main_db_connection.fetchall()
+
+        dolphie.metric_manager.refresh_data(
+            worker_start_time=dolphie.worker_start_time,
+            polling_latency=dolphie.polling_latency,
+            global_variables=dolphie.global_variables,
+            global_status=dolphie.global_status,
+            innodb_metrics=dolphie.innodb_metrics,
+            disk_io_metrics=dolphie.disk_io_metrics,
+            metadata_lock_metrics=dolphie.metadata_locks,
+            replication_status=dolphie.replication_status,
+            replication_lag=dolphie.replica_lag,
+        )
+
+    def process_proxysql_data(self, tab: Tab):
+        dolphie = tab.dolphie
+
+        dolphie.global_variables = dolphie.main_db_connection.fetch_status_and_variables("variables")
+        dolphie.global_status = dolphie.main_db_connection.fetch_status_and_variables("mysql_stats")
+
+        dolphie.main_db_connection.execute(ProxySQLQueries.command_stats)
+        dolphie.proxysql_command_stats = dolphie.main_db_connection.fetchall()
+
+        # Here, we're going to format the command stats to match the global status keys of
+        # MySQL and get total count of queries
+        total_queries_count = 0
+        for row in dolphie.proxysql_command_stats:
+            total_cnt = int(row["Total_cnt"])
+            total_queries_count += total_cnt
+
+            dolphie.global_status[f"Com_{row['Command'].lower()}"] = total_cnt
+
+        # Add the total queries to the global status
+        dolphie.global_status["Queries"] = total_queries_count
+
+        dolphie.main_db_connection.execute(ProxySQLQueries.connection_pool_data)
+        data = dolphie.main_db_connection.fetchone()
+        dolphie.global_status["proxysql_backend_host_average_latency"] = int(data.get("avg_latency", 0))
+        dolphie.global_status["proxysql_multiplex_efficiency_ratio"] = round(
+            100
+            - (
+                (
+                    int(data.get("connection_pool_connections", 0))
+                    / dolphie.global_status.get("Client_Connections_connected", 0)
+                )
+                * 100
+            ),
+            2,
+        )
+
+        if dolphie.panels.proxysql_hostgroup_summary.visible:
+            dolphie.main_db_connection.execute(ProxySQLQueries.hostgroup_summary)
+            dolphie.proxysql_hostgroup_summary = dolphie.main_db_connection.fetchall()
+
+        if dolphie.panels.processlist.visible:
+            dolphie.processlist_threads = proxysql_processlist_panel.fetch_data(tab)
+
+        if dolphie.panels.proxysql_mysql_query_rules.visible:
+            dolphie.main_db_connection.execute(ProxySQLQueries.query_rules_summary)
+            dolphie.proxysql_mysql_query_rules = dolphie.main_db_connection.fetchall()
+
+        dolphie.metric_manager.refresh_data(
+            worker_start_time=dolphie.worker_start_time,
+            polling_latency=dolphie.polling_latency,
+            global_variables=dolphie.global_variables,
+            global_status=dolphie.global_status,
+            proxysql_command_stats=dolphie.proxysql_command_stats,
+        )
+
+    def refresh_screen_proxysql(self, tab: Tab):
+        dolphie = tab.dolphie
+
+        if tab.loading_indicator.display:
+            tab.loading_indicator.display = False
+            self.tab_manager.update_topbar(tab=tab, connection_status="ONLINE")
+
+        # Loop each panel and refresh it
+        for panel in dolphie.panels.get_all_panels():
+            if panel.visible:
+                # Skip the graphs panel since it's handled separately
+                if panel.name == dolphie.panels.graphs.name:
+                    continue
+
+                self.refresh_panel(tab, panel.name)
+
+                if panel.name == dolphie.panels.dashboard.name and dolphie.metric_manager.metrics.dml.Queries.values:
+                    # Update the sparkline for queries per second
+                    tab.sparkline.data = dolphie.metric_manager.metrics.dml.Queries.values
+                    tab.sparkline.refresh()
+
+        if dolphie.panels.graphs.visible:
+            # Refresh the graph(s) for the selected tab
+            self.update_graphs(tab.metric_graph_tabs.get_pane(tab.metric_graph_tabs.active).name)
+
+        # We take a snapshot of the processlist to be used for commands
+        # since the data can change after a key is pressed
+        dolphie.processlist_threads_snapshot = dolphie.processlist_threads.copy()
+
+        # This denotes that we've gone through the first loop of the worker thread
+        dolphie.completed_first_loop = True
+
+    def refresh_screen_mysql(self, tab: Tab):
         dolphie = tab.dolphie
 
         if tab.loading_indicator.display:
             tab.loading_indicator.display = False
 
             self.layout_graphs(tab)
             self.tab_manager.update_topbar(tab=tab, connection_status=dolphie.connection_status)
 
-        if not tab.main_container.display:
-            tab.main_container.display = True
-            tab.sparkline.display = True
-
         # Loop each panel and refresh it
         for panel in dolphie.panels.get_all_panels():
             if panel.visible:
                 # Skip the graphs panel since it's handled separately
                 if panel.name == dolphie.panels.graphs.name:
                     continue
 
@@ -357,19 +493,22 @@
 
         # This denotes that we've gone through the first loop of the worker thread
         dolphie.completed_first_loop = True
 
     def monitor_read_only_change(self, tab: Tab):
         dolphie = tab.dolphie
 
+        if dolphie.connection_source == ConnectionSource.proxysql:
+            return
+
         current_ro_status = dolphie.global_variables.get("read_only")
         formatted_ro_status = ConnectionStatus.read_only if current_ro_status == "ON" else ConnectionStatus.read_write
         status = "read-only" if current_ro_status == "ON" else "read/write"
 
-        message = f"Host [light_blue]{dolphie.mysql_host}[/light_blue] is now [b highlight]{status}[/b highlight]"
+        message = f"Host [light_blue]{dolphie.host_with_port}[/light_blue] is now [b highlight]{status}[/b highlight]"
 
         if current_ro_status == "ON" and not dolphie.replication_status and not dolphie.group_replication:
             message += " ([yellow]SHOULD BE READ/WRITE?[/yellow])"
         elif current_ro_status == "ON" and dolphie.group_replication and dolphie.is_group_replication_primary:
             message += " ([yellow]SHOULD BE READ/WRITE?[/yellow])"
 
         if (
@@ -443,17 +582,20 @@
 
     def update_stats_label(self, tab_metric_instance_name):
         stat_data = {}
 
         for metric_instance in self.tab_manager.active_tab.dolphie.metric_manager.metrics.__dict__.values():
             if metric_instance.tab_name == tab_metric_instance_name:
                 number_format_func = MetricManager.get_number_format_function(metric_instance, color=True)
-                for metric_data in metric_instance.__dict__.values():
+                for metric_name, metric_data in metric_instance.__dict__.items():
                     if isinstance(metric_data, MetricManager.MetricData) and metric_data.values and metric_data.visible:
-                        stat_data[metric_data.label] = number_format_func(metric_data.values[-1])
+                        if f"graph_{metric_name}" in metric_instance.graphs:
+                            stat_data[metric_data.label] = round(metric_data.values[-1])
+                        else:
+                            stat_data[metric_data.label] = number_format_func(metric_data.values[-1])
 
         formatted_stat_data = "  ".join(
             f"[b light_blue]{label}[/b light_blue] {value}" for label, value in stat_data.items()
         )
         getattr(self.tab_manager.active_tab, tab_metric_instance_name).update(formatted_stat_data)
 
     def toggle_panel(self, panel_name):
@@ -467,73 +609,107 @@
         if panel_name not in [self.tab_manager.active_tab.dolphie.panels.graphs.name]:
             self.refresh_panel(self.tab_manager.active_tab, panel_name, toggled=True)
 
         panel.display = new_display_status
 
     def refresh_panel(self, tab: Tab, panel_name: str, toggled: bool = False):
         panel_mapping = {
-            tab.dolphie.panels.replication.name: replication_panel,
-            tab.dolphie.panels.dashboard.name: dashboard_panel,
-            tab.dolphie.panels.processlist.name: processlist_panel,
-            # tab.dolphie.panels.innodb_trx_locks.name: innodb_trx_locks_panel,
-            tab.dolphie.panels.metadata_locks.name: metadata_locks_panel,
-            tab.dolphie.panels.ddl.name: ddl_panel,
+            tab.dolphie.panels.replication.name: {ConnectionSource.mysql: replication_panel},
+            tab.dolphie.panels.dashboard.name: {
+                ConnectionSource.mysql: dashboard_panel,
+                ConnectionSource.proxysql: proxysql_dashboard_panel,
+            },
+            tab.dolphie.panels.processlist.name: {
+                ConnectionSource.mysql: processlist_panel,
+                ConnectionSource.proxysql: proxysql_processlist_panel,
+            },
+            tab.dolphie.panels.metadata_locks.name: {ConnectionSource.mysql: metadata_locks_panel},
+            tab.dolphie.panels.ddl.name: {ConnectionSource.mysql: ddl_panel},
+            tab.dolphie.panels.proxysql_hostgroup_summary.name: {
+                ConnectionSource.proxysql: proxysql_hostgroup_summary_panel
+            },
+            tab.dolphie.panels.proxysql_mysql_query_rules.name: {
+                ConnectionSource.proxysql: proxysql_mysql_query_rules_panel
+            },
+            tab.dolphie.panels.proxysql_command_stats.name: {ConnectionSource.proxysql: proxysql_command_stats_panel},
         }
-        for panel_map_name, panel_map_obj in panel_mapping.items():
+
+        if tab.dolphie.connection_source == ConnectionSource.mysql:
+            if toggled or not tab.dolphie.completed_first_loop:
+                # Update the sizes of the panels depending if replication container is visible or not
+                if tab.dolphie.replication_status and not tab.dolphie.panels.replication.visible:
+                    tab.dashboard_section_1.styles.width = "25vw"
+                    tab.dashboard_section_2.styles.width = "17vw"
+                    tab.dashboard_section_3.styles.width = "21vw"
+                    tab.dashboard_section_4.styles.width = "12vw"
+                    tab.dashboard_section_5.styles.width = "25vw"
+
+                    tab.dashboard_section_5.display = True
+                else:
+                    tab.dashboard_section_1.styles.width = "32vw"
+                    tab.dashboard_section_2.styles.width = "24vw"
+                    tab.dashboard_section_3.styles.width = "27vw"
+                    tab.dashboard_section_4.styles.width = "17vw"
+                    tab.dashboard_section_5.styles.width = "0"
+
+                    tab.dashboard_section_5.display = False
+
+                tab.dashboard_section_1.styles.max_width = "45"
+                tab.dashboard_section_2.styles.max_width = "32"
+                tab.dashboard_section_3.styles.max_width = "38"
+                tab.dashboard_section_4.styles.max_width = "22"
+                tab.dashboard_section_5.styles.max_width = "55"
+
+        elif tab.dolphie.connection_source == ConnectionSource.proxysql:
+            tab.dashboard_section_1.styles.width = "24vw"
+            tab.dashboard_section_2.styles.width = "20vw"
+            tab.dashboard_section_3.styles.width = "22vw"
+            tab.dashboard_section_4.styles.width = "13vw"
+
+            tab.dashboard_section_5.display = False
+
+            tab.dashboard_section_1.styles.max_width = "35"
+            tab.dashboard_section_2.styles.max_width = "28"
+            tab.dashboard_section_3.styles.max_width = "25"
+            tab.dashboard_section_4.styles.max_width = "25"
+
+        for panel_map_name, panel_map_connection_sources in panel_mapping.items():
+            panel_map_obj = panel_map_connection_sources.get(tab.dolphie.connection_source)
+
+            if not panel_map_obj:
+                tab.get_panel_widget(panel_map_name).display = False
+                continue
+
             if panel_name == panel_map_name:
                 panel_map_obj.create_panel(tab)
+
             if panel_name == tab.dolphie.panels.replication.name and toggled and tab.dolphie.replication_status:
                 # When replication panel status is changed, we need to refresh the dashboard panel as well since
                 # it adds/removes it from there
                 dashboard_panel.create_panel(tab)
 
-        if toggled or not tab.dolphie.completed_first_loop:
-            # Update the sizes of the panels depending if replication container is visible or not
-            if tab.dolphie.replication_status and not tab.dolphie.panels.replication.visible:
-                tab.dashboard_host_information.styles.width = "25vw"
-                tab.dashboard_binary_log.styles.width = "21vw"
-                tab.dashboard_innodb.styles.width = "17vw"
-                tab.dashboard_replication.styles.width = "25vw"
-                tab.dashboard_statistics.styles.width = "12vw"
-
-                tab.dashboard_replication.display = True
-            else:
-                tab.dashboard_host_information.styles.width = "32vw"
-                tab.dashboard_binary_log.styles.width = "27vw"
-                tab.dashboard_innodb.styles.width = "24vw"
-                tab.dashboard_replication.styles.width = "0"
-                tab.dashboard_statistics.styles.width = "17vw"
-
-                tab.dashboard_replication.display = False
-
-            tab.dashboard_host_information.styles.max_width = "45"
-            tab.dashboard_binary_log.styles.max_width = "38"
-            tab.dashboard_innodb.styles.max_width = "32"
-            tab.dashboard_replication.styles.max_width = "55"
-            tab.dashboard_statistics.styles.max_width = "22"
-
     def layout_graphs(self, tab: Tab):
         # These variables are dynamically created
         if tab.dolphie.is_mysql_version_at_least("8.0.30"):
-            tab.graph_redo_log.styles.width = "55%"
+            tab.graph_redo_log_data_written.styles.width = "55%"
             tab.graph_redo_log_bar.styles.width = "12%"
             tab.graph_redo_log_active_count.styles.width = "33%"
             tab.graph_redo_log_active_count.display = True
             tab.dolphie.metric_manager.metrics.redo_log_active_count.Active_redo_log_count.visible = True
         else:
-            tab.graph_redo_log.styles.width = "88%"
+            tab.graph_redo_log_data_written.styles.width = "88%"
             tab.graph_redo_log_bar.styles.width = "12%"
             tab.graph_redo_log_active_count.display = False
 
         tab.graph_adaptive_hash_index.styles.width = "50%"
         tab.graph_adaptive_hash_index_hit_ratio.styles.width = "50%"
 
     @on(Switch.Changed)
     def switch_changed(self, event: Switch.Changed):
-        if len(self.screen_stack) > 1:
+        if len(self.screen_stack) > 1 or not self.tab_manager.active_tab:
             return
 
         metric_instance_name = event.switch.name
         metric = event.switch.id
 
         metric_instance = getattr(self.tab_manager.active_tab.dolphie.metric_manager.metrics, metric_instance_name)
         metric_data: MetricManager.MetricData = getattr(metric_instance, metric)
@@ -594,60 +770,68 @@
             self.toggle_panel(dolphie.panels.dashboard.name)
         elif key == "2":
             self.tab_manager.active_tab.processlist_datatable.clear()
             self.toggle_panel(dolphie.panels.processlist.name)
 
             tab.processlist_title.update("Processlist ([highlight]0[/highlight])")
         elif key == "3":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.toggle_panel(dolphie.panels.proxysql_hostgroup_summary.name)
+                dolphie.proxysql_per_second_data = {}
+                self.tab_manager.active_tab.proxysql_hostgroup_summary_datatable.clear()
+
+                return
+
             self.toggle_panel(dolphie.panels.replication.name)
 
             tab.replicas_container.display = False
             if not dolphie.panels.replication.visible:
                 for member in dolphie.app.query(f".replica_container_{dolphie.tab_id}"):
                     member.remove()
             else:
                 if dolphie.replica_manager.available_replicas:
                     tab.replicas_container.display = True
                     tab.replicas_title.update(
                         f"[b]Loading [highlight]{len(dolphie.replica_manager.available_replicas)}[/highlight]"
                         " replicas...\n"
                     )
                     tab.replicas_loading_indicator.display = True
-
         elif key == "4":
             self.toggle_panel(dolphie.panels.graphs.name)
             self.app.update_graphs("dml")
-        # elif key == "5":
-        #     if not dolphie.is_mysql_version_at_least("5.7"):
-        #         self.notify("InnoDB Transaction Locks panel requires MySQL 5.7+")
-        #         return
-
-        #     self.toggle_panel(dolphie.panels.innodb_trx_locks.name)
-        #     self.tab_manager.active_tab.innodb_trx_locks_datatable.clear()
         elif key == "5":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.toggle_panel(dolphie.panels.proxysql_mysql_query_rules.name)
+                return
+
             if not dolphie.is_mysql_version_at_least("5.7") or not dolphie.performance_schema_enabled:
                 self.notify("Metadata Locks panel requires MySQL 5.7+ with Performance Schema enabled")
                 return
 
             query = (
                 "SELECT enabled FROM performance_schema.setup_instruments WHERE name = 'wait/lock/metadata/sql/mdl';"
             )
+
             dolphie.secondary_db_connection.execute(query)
             row = dolphie.secondary_db_connection.fetchone()
             if row and row.get("enabled") == "NO":
                 self.notify(
                     "Metadata Locks panel requires Performance Schema to have"
                     " [highlight]wait/lock/metadata/sql/mdl[/highlight] enabled"
                 )
                 return
 
             self.toggle_panel(dolphie.panels.metadata_locks.name)
             self.tab_manager.active_tab.metadata_locks_datatable.clear()
             tab.metadata_locks_title.update("Metadata Locks ([highlight]0[/highlight])")
         elif key == "6":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.toggle_panel(dolphie.panels.proxysql_command_stats.name)
+                return
+
             if not dolphie.is_mysql_version_at_least("5.7") or not dolphie.performance_schema_enabled:
                 self.notify("DDL panel requires MySQL 5.7+ with Performance Schema enabled")
                 return
 
             query = "SELECT enabled FROM performance_schema.setup_instruments WHERE name LIKE 'stage/innodb/alter%';"
             dolphie.secondary_db_connection.execute(query)
             data = dolphie.secondary_db_connection.fetchall()
@@ -706,46 +890,56 @@
                 dolphie.show_additional_query_columns = True
                 self.notify("Processlist will now show additional columns")
 
         elif key == "c":
             dolphie.user_filter = ""
             dolphie.db_filter = ""
             dolphie.host_filter = ""
+            dolphie.hostgroup_filter = ""
             dolphie.query_time_filter = ""
             dolphie.query_filter = ""
 
             self.notify("Cleared all filters", severity="success")
 
         elif key == "d":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.notify(f"Command [highlight]{key}[/highlight] is only available for MySQL connections")
+                return
+
             self.run_command_in_worker(key=key, dolphie=dolphie)
 
         elif key == "D":
             await self.tab_manager.disconnect_tab(tab)
 
         elif key == "e":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.run_command_in_worker(key=key, dolphie=dolphie)
+                return
+
             if dolphie.is_mysql_version_at_least("8.0") and dolphie.performance_schema_enabled:
                 self.app.push_screen(
                     EventLog(
                         dolphie.connection_status,
                         dolphie.app_version,
-                        dolphie.mysql_host,
+                        dolphie.host_with_port,
                         dolphie.secondary_db_connection,
                     )
                 )
             else:
                 self.notify("Error log command requires MySQL 8+ with Performance Schema enabled")
 
         elif key == "f":
 
             def command_get_input(filter_data):
                 filter_name, filter_value = filter_data[0], filter_data[1]
                 filters_mapping = {
                     "User": "user_filter",
                     "Database": "db_filter",
                     "Host": "host_filter",
+                    "Hostgroup": "hostgroup_filter",
                     "Query time": "query_time_filter",
                     "Query text": "query_filter",
                 }
 
                 attribute = filters_mapping.get(filter_name)
                 if attribute:
                     setattr(dolphie, attribute, int(filter_value) if attribute == "query_time_filter" else filter_value)
@@ -758,14 +952,15 @@
 
             self.app.push_screen(
                 CommandModal(
                     command=HotkeyCommands.thread_filter,
                     message="Select which field you'd like to filter by",
                     processlist_data=dolphie.processlist_threads_snapshot,
                     host_cache_data=dolphie.host_cache,
+                    connection_source=dolphie.connection_source,
                 ),
                 command_get_input,
             )
 
         elif key == "i":
             if dolphie.show_idle_threads:
                 dolphie.show_idle_threads = False
@@ -782,55 +977,71 @@
 
             def command_get_input(data):
                 self.run_command_in_worker(key=key, dolphie=dolphie, additional_data=data)
 
             self.app.push_screen(
                 CommandModal(
                     command=HotkeyCommands.thread_kill_by_id,
-                    message="Kill Thread",
+                    message="Kill Process",
                     processlist_data=dolphie.processlist_threads_snapshot,
                 ),
                 command_get_input,
             )
 
         elif key == "K":
 
             def command_get_input(data):
                 self.run_command_in_worker(key=key, dolphie=dolphie, additional_data=data)
 
             self.app.push_screen(
                 CommandModal(
                     command=HotkeyCommands.thread_kill_by_parameter,
-                    message="Kill threads based around parameters",
+                    message="Kill processes based around parameters",
                     processlist_data=dolphie.processlist_threads_snapshot,
                 ),
                 command_get_input,
             )
 
         elif key == "l":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.notify(f"Command [highlight]{key}[/highlight] is only available for MySQL connections")
+                return
+
             self.run_command_in_worker(key=key, dolphie=dolphie)
 
         elif key == "o":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.notify(f"Command [highlight]{key}[/highlight] is only available for MySQL connections")
+                return
+
             self.run_command_in_worker(key=key, dolphie=dolphie)
 
         elif key == "m":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.run_command_in_worker(key=key, dolphie=dolphie)
+                return
+
             if not dolphie.is_mysql_version_at_least("5.7") or not dolphie.performance_schema_enabled:
                 self.notify("Memory usage command requires MySQL 5.7+ with Performance Schema enabled")
             else:
                 self.run_command_in_worker(key=key, dolphie=dolphie)
 
         elif key == "p":
             if not dolphie.pause_refresh:
                 dolphie.pause_refresh = True
                 self.notify(f"Refresh is paused! Press [b highlight]{key}[/b highlight] again to resume")
             else:
                 dolphie.pause_refresh = False
                 self.notify("Refreshing has resumed", severity="success")
 
         if key == "P":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.notify(f"Command [highlight]{key}[/highlight] is only available for MySQL connections")
+                return
+
             if dolphie.use_performance_schema:
                 dolphie.use_performance_schema = False
                 self.notify("Switched to using [b highlight]Processlist")
             else:
                 if dolphie.performance_schema_enabled:
                     dolphie.use_performance_schema = True
                     self.notify("Switched to using [b highlight]Performance Schema")
@@ -855,53 +1066,99 @@
                 command_get_input,
             )
 
         elif key == "R":
             dolphie.metric_manager.reset()
 
             self.update_graphs(tab.metric_graph_tabs.get_pane(tab.metric_graph_tabs.active).name)
+            dolphie.update_switches_after_reset()
             self.notify("Metrics have been reset", severity="success")
 
         elif key == "s":
             if dolphie.sort_by_time_descending:
                 dolphie.sort_by_time_descending = False
                 self.notify("Processlist will now sort threads by time in ascending order")
             else:
                 dolphie.sort_by_time_descending = True
                 self.notify("Processlist will now sort threads by time in descending order")
 
         elif key == "t":
 
-            def command_get_input(data):
-                self.run_command_in_worker(key=key, dolphie=dolphie, additional_data=data)
+            if dolphie.connection_source == ConnectionSource.proxysql:
+
+                def command_get_input(data):
+                    thread_table = Table(box=None, show_header=False)
+                    thread_table.add_column("")
+                    thread_table.add_column("", overflow="fold")
+
+                    thread_id = data
+                    thread_data: ProxySQLProcesslistThread = dolphie.processlist_threads_snapshot.get(thread_id)
+                    if not thread_data:
+                        self.notify(f"Thread ID [highlight]{thread_id}[/highlight] was not found", severity="error")
+                        return
+
+                    thread_table.add_row("[label]Process ID", thread_id)
+                    thread_table.add_row("[label]Hostgroup", thread_data.hostgroup)
+                    thread_table.add_row("[label]User", thread_data.user)
+                    thread_table.add_row("[label]Frontend Host", thread_data.frontend_host)
+                    thread_table.add_row("[label]Backend Host", thread_data.host)
+                    thread_table.add_row("[label]Database", thread_data.db)
+                    thread_table.add_row("[label]Command", thread_data.command)
+                    thread_table.add_row("[label]Time", str(timedelta(seconds=thread_data.time)).zfill(8))
+
+                    formatted_query = None
+                    if thread_data.formatted_query.code:
+                        query = sqlformat(thread_data.formatted_query.code, reindent_aligned=True)
+                        formatted_query = format_query(query, minify=False)
+
+                    self.app.push_screen(
+                        ProxySQLThreadScreen(
+                            connection_status=dolphie.connection_status,
+                            app_version=dolphie.app_version,
+                            host=dolphie.host_with_port,
+                            thread_table=thread_table,
+                            query=formatted_query,
+                            extended_info=thread_data.extended_info,
+                        )
+                    )
+
+            else:
+
+                def command_get_input(data):
+                    self.run_command_in_worker(key=key, dolphie=dolphie, additional_data=data)
 
             self.app.push_screen(
                 CommandModal(
                     command=HotkeyCommands.show_thread,
-                    message="Thread Details",
+                    message="Process Details",
                     processlist_data=dolphie.processlist_threads_snapshot,
                 ),
                 command_get_input,
             )
 
         elif key == "T":
+            if dolphie.connection_source == ConnectionSource.proxysql:
+                self.notify(f"Command [highlight]{key}[/highlight] is only available for MySQL connections")
+                return
+
             if dolphie.show_trxs_only:
                 dolphie.show_trxs_only = False
                 dolphie.show_idle_threads = False
                 self.notify("Processlist will now no longer only show threads that have an active transaction")
             else:
                 dolphie.show_trxs_only = True
                 dolphie.show_idle_threads = True
                 self.notify("Processlist will now only show threads that have an active transaction")
 
         elif key == "u":
-            if not dolphie.performance_schema_enabled:
+            if not dolphie.performance_schema_enabled and dolphie.connection_source != ConnectionSource.proxysql:
                 self.notify("User statistics command requires Performance Schema to be enabled")
-            else:
-                self.run_command_in_worker(key=key, dolphie=dolphie)
+                return
+
+            self.run_command_in_worker(key=key, dolphie=dolphie)
 
         elif key == "v":
 
             def command_get_input(input_variable):
                 table_grid = Table.grid()
                 table_counter = 1
                 variable_counter = 1
@@ -948,15 +1205,17 @@
 
                 # Add the data into a single tuple for add_row
                 if display_global_variables:
                     table_grid.add_row(*all_tables)
                     screen_data = Align.center(table_grid)
 
                     self.app.push_screen(
-                        CommandScreen(dolphie.connection_status, dolphie.app_version, dolphie.mysql_host, screen_data)
+                        CommandScreen(
+                            dolphie.connection_status, dolphie.app_version, dolphie.host_with_port, screen_data
+                        )
                     )
                 else:
                     if input_variable:
                         self.notify("No variable(s) found that match [b highlight]%s[/b highlight]" % input_variable)
 
             self.app.push_screen(
                 CommandModal(HotkeyCommands.variable_search, message="Specify a variable to wildcard search"),
@@ -986,137 +1245,37 @@
                 )
             else:
                 screen_data = Group(
                     Align.center("[b light_blue]Host Cache[/b light_blue]\n"), "There are currently no hosts resolved"
                 )
 
         elif key == "question_mark":
-            keys = {
-                "1": "Show/hide Dashboard",
-                "2": "Show/hide Processlist",
-                "3": "Show/hide Replication/Replicas",
-                "4": "Show/hide Graph Metrics",
-                # "5": "Show/hide InnoDB Transaction Locks",
-                "5": "Show/hide Metadata Locks",
-                "6": "Show/hide DDLs",
-                "`": "Open Host Setup",
-                "+": "Create a new tab",
-                "-": "Remove the current tab",
-                "=": "Rename the current tab",
-                "a": "Toggle additional processlist columns",
-                "c": "Clear all filters set",
-                "d": "Display all databases",
-                "D": "Disconnect from the tab's host",
-                "e": "Display error log from Performance Schema",
-                "f": "Filter processlist by a supported option",
-                "i": "Toggle displaying idle threads",
-                "k": "Kill a thread by its ID",
-                "K": "Kill a thread by a supported option",
-                "l": "Display the most recent deadlock",
-                "o": "Display output from SHOW ENGINE INNODB STATUS",
-                "m": "Display memory usage",
-                "p": "Pause refreshing of panels",
-                "P": "Switch between using Information Schema/Performance Schema for processlist panel",
-                "q": "Quit",
-                "r": "Set the refresh interval",
-                "R": "Reset all metrics",
-                "t": "Display details of a thread along with an EXPLAIN of its query",
-                "T": "Transaction view - toggle displaying threads that only have an active transaction",
-                "s": "Toggle sorting for Age in descending/ascending order",
-                "u": "List active connected users and their statistics",
-                "v": "Variable wildcard search sourced from SHOW GLOBAL VARIABLES",
-                "z": "Display all entries in the host cache",
-                "space": "Force a manual refresh of all panels except replicas",
-                "ctrl+a": "Switch to the previous tab",
-                "ctrl+d": "Switch to the next tab",
-            }
-
-            table_keys = Table(
-                box=box.SIMPLE_HEAVY,
-                show_edge=False,
-                style="table_border",
-                title="Commands",
-                title_style="bold #bbc8e8",
-                header_style="bold",
-            )
-            table_keys.add_column("Key", justify="center", style="b highlight")
-            table_keys.add_column("Description")
-
-            for key, description in keys.items():
-                table_keys.add_row(key, description)
-
-            datapoints = {
-                "Read Only": "If the host is in read-only mode",
-                "Read Hit": "The percentage of how many reads are from InnoDB buffer pool compared to from disk",
-                "Lag": ("Retrieves metric from: Default -> SHOW SLAVE STATUS, HB -> Heartbeat table"),
-                "Chkpt Age": (
-                    "This depicts how close InnoDB is before it starts to furiously flush dirty data to disk "
-                    "(Lower is better)"
-                ),
-                "AHI Hit": (
-                    "The percentage of how many lookups there are from Adapative Hash Index compared to it not"
-                    " being used"
-                ),
-                "Diff": "This is the size difference of the binary log between each refresh interval",
-                "Cache Hit": "The percentage of how many binary log lookups are from cache instead of from disk",
-                "History List": "History list length (number of un-purged row changes in InnoDB's undo logs)",
-                "QPS": "Queries per second from Com_queries in SHOW GLOBAL STATUS",
-                "Latency": "How much time it takes to receive data from the host for each refresh interval",
-                "Threads": "Con = Connected, Run = Running, Cac = Cached from SHOW GLOBAL STATUS",
-                "Speed": "How many seconds were taken off of replication lag from the last refresh interval",
-                "Tickets": "Relates to innodb_concurrency_tickets variable",
-                "R-Lock/Mod": "Relates to how many rows are locked/modified for the thread's transaction",
-                "GR": "Group Replication",
-            }
-
-            table_terminology = Table(
-                box=box.SIMPLE_HEAVY,
-                show_edge=False,
-                style="table_border",
-                title="Terminology",
-                title_style="bold #bbc8e8",
-                header_style="bold",
-            )
-            table_terminology.add_column("Datapoint", style="highlight")
-            table_terminology.add_column("Description")
-            for datapoint, description in sorted(datapoints.items()):
-                table_terminology.add_row(datapoint, description)
-
-            screen_data = Group(
-                Align.center(table_keys),
-                "",
-                Align.center(table_terminology),
-                "",
-                Align.center(
-                    "[light_blue][b]Note[/b]: Textual puts your terminal in application mode which disables selecting"
-                    " text.\nTo see how to select text on your terminal, visit: https://tinyurl.com/dolphie-copy-text"
-                ),
-            )
+            self.app.push_screen(HelpScreen(dolphie.connection_source))
 
         if screen_data:
             self.app.push_screen(
-                CommandScreen(dolphie.connection_status, dolphie.app_version, dolphie.mysql_host, screen_data)
+                CommandScreen(dolphie.connection_status, dolphie.app_version, dolphie.host_with_port, screen_data)
             )
 
     @work(thread=True)
     def run_command_in_worker(self, key: str, dolphie: Dolphie, additional_data=None):
         tab = self.tab_manager.active_tab
 
         # These are the screens to display we use for the commands
         def show_command_screen():
             self.app.push_screen(
-                CommandScreen(dolphie.connection_status, dolphie.app_version, dolphie.mysql_host, screen_data)
+                CommandScreen(dolphie.connection_status, dolphie.app_version, dolphie.host_with_port, screen_data)
             )
 
         def show_thread_screen():
             self.app.push_screen(
                 ThreadScreen(
                     connection_status=dolphie.connection_status,
                     app_version=dolphie.app_version,
-                    host=dolphie.mysql_host,
+                    host=dolphie.host_with_port,
                     thread_table=thread_table,
                     user_thread_attributes_table=user_thread_attributes_table,
                     query=formatted_query,
                     explain_data=explain_data,
                     explain_failure=explain_failure,
                     transaction_history_table=transaction_history_table,
                 )
@@ -1169,35 +1328,72 @@
                 screen_data = Group(
                     Align.center("[b light_blue]Databases[/b light_blue] ([b highlight]%s[/b highlight])\n" % db_count),
                     Align.center(table_grid),
                 )
 
                 self.call_from_thread(show_command_screen)
 
-            if key == "k":
+            elif key == "e":
+                header_style = Style(bold=True)
+                table = Table(box=box.SIMPLE_HEAVY, style="table_border", show_edge=False)
+                table.add_column("Hostgroup", header_style=header_style)
+                table.add_column("Backend Host", max_width=35, header_style=header_style)
+                table.add_column("Username", header_style=header_style)
+                table.add_column("Schema", header_style=header_style)
+                table.add_column("First Seen", header_style=header_style)
+                table.add_column("Last Seen", header_style=header_style)
+                table.add_column("Count", header_style=header_style)
+                table.add_column("Error", header_style=header_style, overflow="fold")
+
+                dolphie.secondary_db_connection.execute(ProxySQLQueries.query_errors)
+                data = dolphie.secondary_db_connection.fetchall()
+
+                for row in data:
+                    table.add_row(
+                        row.get("hostgroup"),
+                        f"{dolphie.get_hostname(row.get('hostname'))}:{row.get('port')}",
+                        row.get("username"),
+                        row.get("schemaname"),
+                        str(datetime.fromtimestamp(int(row.get("first_seen", 0)))),
+                        str(datetime.fromtimestamp(int(row.get("last_seen", 0)))),
+                        format_number(int(row.get("count_star", 0))),
+                        "[b][highlight]%s[/b][/highlight]: %s" % (row.get("errno", 0), row.get("last_error")),
+                    )
+
+                screen_data = Group(
+                    Align.center(f"[b light_blue]Query Errors ([highlight]{table.row_count}[/highlight])\n"),
+                    Align.center(table),
+                )
+
+                self.call_from_thread(show_command_screen)
+            elif key == "k":
                 thread_id = additional_data
                 try:
-                    if dolphie.aws_rds:
+                    if dolphie.connection_source_alt == ConnectionSource.aws_rds:
                         dolphie.secondary_db_connection.execute("CALL mysql.rds_kill(%s)" % thread_id)
-                    elif dolphie.azure:
+                    elif dolphie.connection_source_alt == ConnectionSource.azure_mysql:
                         dolphie.secondary_db_connection.execute("CALL mysql.az_kill(%s)" % thread_id)
+                    elif dolphie.connection_source == ConnectionSource.proxysql:
+                        dolphie.secondary_db_connection.execute("KILL CONNECTION %s" % thread_id)
                     else:
                         dolphie.secondary_db_connection.execute("KILL %s" % thread_id)
 
-                    self.notify("Killed Thread ID [b highlight]%s[/b highlight]" % thread_id, severity="success")
+                    self.notify("Killed Process ID [b highlight]%s[/b highlight]" % thread_id, severity="success")
                 except ManualException as e:
-                    self.notify(e.reason, title="Error killing Thread ID", severity="error")
+                    self.notify(e.reason, title="Error killing Process ID", severity="error")
 
-            if key == "K":
+            elif key == "K":
 
                 def execute_kill(thread_id):
-                    if dolphie.aws_rds:
+                    if dolphie.connection_source_alt == ConnectionSource.aws_rds:
                         query = "CALL mysql.rds_kill(%s)"
-                    elif dolphie.azure:
+                    elif dolphie.connection_source_alt == ConnectionSource.azure_mysql:
                         query = "CALL mysql.az_kill(%s)"
+                    elif dolphie.connection_source == ConnectionSource.proxysql:
+                        query = "KILL CONNECTION %s"
                     else:
                         query = "KILL %s"
 
                     dolphie.secondary_db_connection.execute(query % thread_id)
 
                 kill_type, kill_value, include_sleeping_queries, lower_limit, upper_limit = additional_data
                 db_field = {"username": "user", "host": "host", "time_range": "time"}.get(kill_type)
@@ -1220,20 +1416,20 @@
                                 if lower_limit <= thread.time <= upper_limit:
                                     execute_kill(thread_id)
                                     threads_killed += 1
                             elif getattr(thread, db_field) == kill_value:
                                 execute_kill(thread_id)
                                 threads_killed += 1
                     except ManualException as e:
-                        self.notify(e.reason, title=f"Error Killing Thread ID {thread_id}", severity="error")
+                        self.notify(e.reason, title=f"Error Killing Process ID {thread_id}", severity="error")
 
                 if threads_killed:
-                    self.notify(f"Killed [highlight]{threads_killed}[/highlight] threads")
+                    self.notify(f"Killed [highlight]{threads_killed}[/highlight] processes")
                 else:
-                    self.notify("No threads were killed")
+                    self.notify("No processes were killed")
 
             elif key == "l":
                 deadlock = ""
                 output = re.search(
                     r"------------------------\nLATEST\sDETECTED\sDEADLOCK\n------------------------"
                     "\n(.*?)------------\nTRANSACTIONS",
                     dolphie.secondary_db_connection.fetch_value_from_field(MySQLQueries.innodb_status, "Status"),
@@ -1253,60 +1449,77 @@
                 screen_data = dolphie.secondary_db_connection.fetch_value_from_field(
                     MySQLQueries.innodb_status, "Status"
                 )
 
                 self.call_from_thread(show_command_screen)
 
             elif key == "m":
-                table_grid = Table.grid()
-                table1 = Table(box=box.SIMPLE_HEAVY, style="table_border")
-
                 header_style = Style(bold=True)
-                table1.add_column("User", header_style=header_style)
-                table1.add_column("Current", header_style=header_style)
-                table1.add_column("Total", header_style=header_style)
 
-                dolphie.secondary_db_connection.execute(MySQLQueries.memory_by_user)
-                data = dolphie.secondary_db_connection.fetchall()
-                for row in data:
-                    table1.add_row(
-                        row["user"],
-                        format_sys_table_memory(row["current_allocated"]),
-                        format_sys_table_memory(row["total_allocated"]),
-                    )
+                if dolphie.connection_source == ConnectionSource.proxysql:
+                    table = Table(box=box.SIMPLE_HEAVY, style="table_border", show_edge=False)
+                    table.add_column("Variable", header_style=header_style)
+                    table.add_column("Value", header_style=header_style)
 
-                table2 = Table(box=box.SIMPLE_HEAVY, style="table_border")
-                table2.add_column("Code Area", header_style=header_style)
-                table2.add_column("Current", header_style=header_style)
+                    dolphie.secondary_db_connection.execute(ProxySQLQueries.memory_metrics)
+                    data = dolphie.secondary_db_connection.fetchall()
 
-                dolphie.secondary_db_connection.execute(MySQLQueries.memory_by_code_area)
-                data = dolphie.secondary_db_connection.fetchall()
-                for row in data:
-                    table2.add_row(row["code_area"], format_sys_table_memory(row["current_allocated"]))
+                    for row in data:
+                        if row["Variable_Name"]:
+                            table.add_row(f"{row['Variable_Name']}", f"{format_bytes(int(row['Variable_Value']))}")
 
-                table3 = Table(box=box.SIMPLE_HEAVY, style="table_border")
-                table3.add_column("Host", header_style=header_style)
-                table3.add_column("Current", header_style=header_style)
-                table3.add_column("Total", header_style=header_style)
+                    screen_data = Group(Align.center("[b light_blue]Memory Usage[/b light_blue]"), Align.center(table))
 
-                dolphie.secondary_db_connection.execute(MySQLQueries.memory_by_host)
-                data = dolphie.secondary_db_connection.fetchall()
-                for row in data:
-                    table3.add_row(
-                        dolphie.get_hostname(row["host"]),
-                        format_sys_table_memory(row["current_allocated"]),
-                        format_sys_table_memory(row["total_allocated"]),
-                    )
+                    self.call_from_thread(show_command_screen)
+                else:
+                    table_grid = Table.grid()
+                    table1 = Table(box=box.SIMPLE_HEAVY, style="table_border")
+
+                    table1.add_column("User", header_style=header_style)
+                    table1.add_column("Current", header_style=header_style)
+                    table1.add_column("Total", header_style=header_style)
+
+                    dolphie.secondary_db_connection.execute(MySQLQueries.memory_by_user)
+                    data = dolphie.secondary_db_connection.fetchall()
+                    for row in data:
+                        table1.add_row(
+                            row["user"],
+                            format_sys_table_memory(row["current_allocated"]),
+                            format_sys_table_memory(row["total_allocated"]),
+                        )
 
-                table_grid.add_row("", Align.center("[b light_blue]Memory Allocation"), "")
-                table_grid.add_row(table1, table3, table2)
+                    table2 = Table(box=box.SIMPLE_HEAVY, style="table_border")
+                    table2.add_column("Code Area", header_style=header_style)
+                    table2.add_column("Current", header_style=header_style)
+
+                    dolphie.secondary_db_connection.execute(MySQLQueries.memory_by_code_area)
+                    data = dolphie.secondary_db_connection.fetchall()
+                    for row in data:
+                        table2.add_row(row["code_area"], format_sys_table_memory(row["current_allocated"]))
+
+                    table3 = Table(box=box.SIMPLE_HEAVY, style="table_border")
+                    table3.add_column("Host", header_style=header_style)
+                    table3.add_column("Current", header_style=header_style)
+                    table3.add_column("Total", header_style=header_style)
+
+                    dolphie.secondary_db_connection.execute(MySQLQueries.memory_by_host)
+                    data = dolphie.secondary_db_connection.fetchall()
+                    for row in data:
+                        table3.add_row(
+                            dolphie.get_hostname(row["host"]),
+                            format_sys_table_memory(row["current_allocated"]),
+                            format_sys_table_memory(row["total_allocated"]),
+                        )
 
-                screen_data = Align.center(table_grid)
+                    table_grid.add_row("", Align.center("[b light_blue]Memory Allocation"), "")
+                    table_grid.add_row(table1, table3, table2)
 
-                self.call_from_thread(show_command_screen)
+                    screen_data = Align.center(table_grid)
+
+                    self.call_from_thread(show_command_screen)
             elif key == "t":
                 formatted_query = ""
                 explain_failure = ""
                 explain_data = ""
 
                 thread_table = Table(box=None, show_header=False)
                 thread_table.add_column("")
@@ -1332,16 +1545,16 @@
                     thread_table.add_row("[label]Tickets", thread_data.trx_concurrency_tickets)
 
                 thread_table.add_row("", "")
                 thread_table.add_row("[label]TRX Time", thread_data.trx_time)
                 thread_table.add_row("[label]TRX State", thread_data.trx_state)
                 thread_table.add_row("[label]TRX Operation", thread_data.trx_operation_state)
 
-                if thread_data.query:
-                    query = sqlformat(thread_data.query, reindent_aligned=True)
+                if thread_data.formatted_query.code:
+                    query = sqlformat(thread_data.formatted_query.code, reindent_aligned=True)
                     query_db = thread_data.db
 
                     formatted_query = format_query(query, minify=False)
 
                     if query_db:
                         try:
                             dolphie.secondary_db_connection.execute("USE %s" % query_db)
@@ -1400,58 +1613,99 @@
                             transaction_history_table.add_row(
                                 query["start_time"].strftime("%Y-%m-%d %H:%M:%S"), trx_history_formatted_query
                             )
 
                 self.call_from_thread(show_thread_screen)
 
             elif key == "u":
-                if dolphie.is_mysql_version_at_least("5.7"):
-                    dolphie.secondary_db_connection.execute(MySQLQueries.ps_user_statisitics)
-                else:
-                    dolphie.secondary_db_connection.execute(MySQLQueries.ps_user_statisitics_56)
+                if dolphie.connection_source == ConnectionSource.proxysql:
+                    title = "Frontend Users"
 
-                users = dolphie.secondary_db_connection.fetchall()
+                    dolphie.secondary_db_connection.execute(ProxySQLQueries.user_stats)
+                    users = dolphie.secondary_db_connection.fetchall()
 
-                columns = {
-                    "User": {"field": "user", "format_number": False},
-                    "Active": {"field": "current_connections", "format_number": True},
-                    "Total": {"field": "total_connections", "format_number": True},
-                    "Rows Read": {"field": "rows_examined", "format_number": True},
-                    "Rows Sent": {"field": "rows_sent", "format_number": True},
-                    "Rows Updated": {"field": "rows_affected", "format_number": True},
-                    "Tmp Tables": {"field": "created_tmp_tables", "format_number": True},
-                    "Tmp Disk Tables": {"field": "created_tmp_disk_tables", "format_number": True},
-                    "Plugin": {"field": "plugin", "format_number": False},
-                    "Password Expire": {"field": "password_expires_in", "format_number": False},
-                }
+                    columns = {
+                        "User": {"field": "username", "format_number": False},
+                        "Active": {"field": "frontend_connections", "format_number": True},
+                        "Max": {"field": "frontend_max_connections", "format_number": True},
+                        "Default HG": {"field": "default_hostgroup", "format_number": False},
+                        "Default Schema": {"field": "default_schema", "format_number": False},
+                        "SSL": {"field": "use_ssl", "format_number": False},
+                    }
+
+                    table = Table(
+                        header_style="b",
+                        box=box.SIMPLE_HEAVY,
+                        show_edge=False,
+                        style="table_border",
+                    )
+                    for column, data in columns.items():
+                        table.add_column(column, no_wrap=True)
 
-                table = Table(
-                    header_style="b",
-                    box=box.SIMPLE_HEAVY,
-                    show_edge=False,
-                    style="table_border",
-                )
-                for column, data in columns.items():
-                    table.add_column(column, no_wrap=True)
+                    for user in users:
+                        row_values = []
+
+                        for column, data in columns.items():
+                            value = user.get(data["field"], "N/A")
+
+                            if data["format_number"]:
+                                row_values.append(format_number(value) if value else "0")
+                            elif column == "SSL":
+                                row_values.append("ON" if value == "1" else "OFF")
+                            else:
+                                row_values.append(value or "")
 
-                for user in users:
-                    row_values = []
+                        table.add_row(*row_values)
+                else:
+                    title = "Users"
+
+                    if dolphie.is_mysql_version_at_least("5.7"):
+                        dolphie.secondary_db_connection.execute(MySQLQueries.ps_user_statisitics)
+                    else:
+                        dolphie.secondary_db_connection.execute(MySQLQueries.ps_user_statisitics_56)
 
+                    users = dolphie.secondary_db_connection.fetchall()
+
+                    columns = {
+                        "User": {"field": "user", "format_number": False},
+                        "Active": {"field": "current_connections", "format_number": True},
+                        "Total": {"field": "total_connections", "format_number": True},
+                        "Rows Read": {"field": "rows_examined", "format_number": True},
+                        "Rows Sent": {"field": "rows_sent", "format_number": True},
+                        "Rows Updated": {"field": "rows_affected", "format_number": True},
+                        "Tmp Tables": {"field": "created_tmp_tables", "format_number": True},
+                        "Tmp Disk Tables": {"field": "created_tmp_disk_tables", "format_number": True},
+                        "Plugin": {"field": "plugin", "format_number": False},
+                        "Password Expire": {"field": "password_expires_in", "format_number": False},
+                    }
+
+                    table = Table(
+                        header_style="b",
+                        box=box.SIMPLE_HEAVY,
+                        show_edge=False,
+                        style="table_border",
+                    )
                     for column, data in columns.items():
-                        value = user.get(data["field"], "N/A")
+                        table.add_column(column, no_wrap=True)
 
-                        if data["format_number"]:
-                            row_values.append(format_number(value) if value else "0")
-                        else:
-                            row_values.append(value or "")
+                    for user in users:
+                        row_values = []
+
+                        for column, data in columns.items():
+                            value = user.get(data.get("field"), "N/A")
+
+                            if data["format_number"]:
+                                row_values.append(format_number(value) if value else "0")
+                            else:
+                                row_values.append(value or "")
 
-                    table.add_row(*row_values)
+                        table.add_row(*row_values)
 
                 screen_data = Group(
-                    Align.center(f"[b light_blue]Users Connected ([highlight]{len(users)}[/highlight])\n"),
+                    Align.center(f"[b light_blue]{title} Connected ([highlight]{len(users)}[/highlight])\n"),
                     Align.center(table),
                 )
 
                 self.call_from_thread(show_command_screen)
         except ManualException as e:
             self.notify(e.reason, title=f"Error running command '{key}'", severity="error", timeout=10)
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dolphie-4.3.5/pyproject.toml` & `dolphie-5.0.0/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [tool.poetry]
 name = "dolphie"
-version = "4.3.5"
+version = "5.0.0"
 license = "GPL-3.0-or-later"
-description = "Echolocate your MySQL health with real-time monitoring in the terminal"
+description = "Your single pane of glass for real-time analytics into MySQL & ProxySQL"
 authors = ["Charles Thompson <01charles.t@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 rich = "^13.7.1"
 pymysql = "^1.1.0"
 myloginpath = "^0.0.4"
 packaging = "^24.0"
 requests = "^2.31.0"
 sqlparse = "^0.4.4"
-textual = "^0.56.2"
+textual = {extras = ["syntax"], version = "^0.57.1"}
 textual-autocomplete = "^2.1.0b0"
 charset-normalizer = "^3.3.2"
 plotext = "^5.2.8"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `dolphie-4.3.5/PKG-INFO` & `dolphie-5.0.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: dolphie
-Version: 4.3.5
-Summary: Echolocate your MySQL health with real-time monitoring in the terminal
+Version: 5.0.0
+Summary: Your single pane of glass for real-time analytics into MySQL & ProxySQL
 License: GPL-3.0-or-later
 Author: Charles Thompson
 Author-email: 01charles.t@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -16,22 +16,22 @@
 Requires-Dist: myloginpath (>=0.0.4,<0.0.5)
 Requires-Dist: packaging (>=24.0,<25.0)
 Requires-Dist: plotext (>=5.2.8,<6.0.0)
 Requires-Dist: pymysql (>=1.1.0,<2.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: rich (>=13.7.1,<14.0.0)
 Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
-Requires-Dist: textual (>=0.56.2,<0.57.0)
 Requires-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0)
+Requires-Dist: textual[syntax] (>=0.57.1,<0.58.0)
 Description-Content-Type: text/markdown
 
 # Dolphie
 <p align="center">
   <img src="https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-4f9c-ada5-a153cdcf4070.png" width="120"><br>
-  Echolocate your MySQL health with real-time monitoring in the terminal<br><br>
+  Your single pane of glass for real-time analytics into MySQL & ProxySQL<br><br>
   <img src="https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-97f8-3b7ef5096eae" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/1d94502a-9abf-4436-a7d0-cb2b08c105c1" width="30">
   <img src="https://github.com/charles-001/dolphie/assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83" width="30">
 </p>
 <p align="center">
   <a href="https://www.buymeacoffee.com/charlesthompson">
     <img src="https://www.buymeacoffee.com/assets/img/custom_images/orange_img.png" alt="Buy Me A Coffee">
@@ -89,44 +89,44 @@
 $ docker run -dit --name dolphie ghcr.io/charles-001/dolphie:latest
 $ docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-pass
 ```
 
 ## Usage
 ```
 positional arguments:
-  uri                   Use a URI string for credentials - format: mysql://user:password@host:port (port is optional with default 3306)
+  uri                   Use a URI string for credentials (mysql/proxysql) - format: mysql://user:password@host:port (port is optional with default 3306, or 6032 for ProxySQL)
 
 options:
   --help                show this help message and exit
   --host-setup          Start Dolphie by showing the Host Setup modal instead of automatically connecting
-  -u , --user           Username for MySQL
-  -p , --password       Password for MySQL
-  -h , --host           Hostname/IP address for MySQL
-  -P , --port           Port for MySQL (Socket has precendence)
-  -S , --socket         Socket file for MySQL
+  -u , --user           Username
+  -p , --password       Password
+  -h , --host           Hostname/IP address
+  -P , --port           Port(Socket has precendence)
+  -S , --socket         Socket file
   --config-file         Dolphie's config file to use. Options are read from these files in the given order: /etc/dolphie.cnf, ~/.dolphie.cnf
   --mycnf-file          MySQL config file path to use. This should use [client] section [default: ~/.my.cnf]
   -f , --host-cache-file
                         Resolve IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on its own line using format ip=hostname [default: ~/dolphie_host_cache]
   -q , --host-setup-file
                         Specify location of file that stores the available hosts to use in host setup modal [default: ~/dolphie_hosts]
   -l , --login-path     Specify login path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login credentials. Supercedes config file [default: client]
   -r , --refresh_interval
                         How much time to wait in seconds between each refresh [default: 1]
   -H , --heartbeat-table
-                        If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it has for replication lag instead of Seconds_Behind_Master from SHOW REPLICA STATUS
+                        (MySQL only) If your hosts use pt-heartbeat, specify table in format db.table to use the timestamp it has for replication lag instead of Seconds_Behind_Master from SHOW REPLICA STATUS
   --ssl-mode            Desired security state of the connection to the host. Supports: REQUIRED/VERIFY_CA/VERIFY_IDENTITY [default: OFF]
   --ssl-ca              Path to the file that contains a CA (certificate authority)
   --ssl-cert            Path to the file that contains a certificate
   --ssl-key             Path to the file that contains a private key for the certificate
-  --panels              What panels to display on startup separated by a comma. Supports: dashboard,processlist,graphs,replication,metadata_locks,ddl [default: dashboard,processlist]
+  --panels              What panels to display on startup separated by a comma. Supports:  dashboard,processlist,graphs,replication,metadata_locks,ddl,proxysql_hostgroup_summary,proxysql_mysql_query_rules,proxysql_command_stats [default: dashboard,processlist]
   --graph-marker        What marker to use for graphs (available options: https://tinyurl.com/dolphie-markers) [default: braille]
   --pypi-repository     What PyPi repository to use when checking for a new version. If not specified, it will use Dolphie's PyPi repository
   --hostgroup           This is used for creating tabs and connecting to them for hosts you specify in Dolphie's config file under a hostgroup section. As an example, you'll have a section called [cluster1] then below it you will list each host on a new line in the format key=host (keys have no meaning). Hosts support optional port (default is whatever port parameter is) in the format host:port. You can also name the tabs by suffixing ~tab_name to the host (i.e. 1=host~tab_name)
-  --show-trxs-only      Start with only showing threads that have an active transaction
+  --show-trxs-only      (MySQL only) Start with only showing threads that have an active transaction
   --additional-columns  Start with additional columns in Processlist panel
   --debug-options       Display options that are set and what they're set by (command-line, dolphie config, etc) then exit
   -V, --version         Display version and exit
 
 MySQL my.cnf file supports these options under [client] section:
 	host
 	user
@@ -175,15 +175,18 @@
 	(str) hostgroup
 	(bool) show_trxs_only
 	(bool) show_additional_query_columns
 ```
 
 ## Supported MySQL versions
 - MySQL/Percona Server 5.6/5.7/8.0+
-- RDS/Aurora
+- RDS & Aurora + Azure
+
+## Supported ProxySQL versions
+- ProxySQL 2.6+ (could work on previous versions but not tested)
 
 ## Grants required
 #### Least privilege
 1. PROCESS (only if you switch to using processlist via `P` command)
 2. SELECT to `performance_schema` + `pt-heartbeat table` (if used)
 3. REPLICATION CLIENT/REPLICATION SLAVE
 4. BACKUP_ADMIN (MySQL 8 only)
```

#### html2text {}

```diff
@@ -1,25 +1,24 @@
-Metadata-Version: 2.1 Name: dolphie Version: 4.3.5 Summary: Echolocate your
-MySQL health with real-time monitoring in the terminal License: GPL-3.0-or-
-later Author: Charles Thompson Author-email: 01charles.t@gmail.com Requires-
-Python: >=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General Public
-License v3 or later (GPLv3+) Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
-Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11 Requires-Dist: charset-
-normalizer (>=3.3.2,<4.0.0) Requires-Dist: myloginpath (>=0.0.4,<0.0.5)
-Requires-Dist: packaging (>=24.0,<25.0) Requires-Dist: plotext (>=5.2.8,<6.0.0)
-Requires-Dist: pymysql (>=1.1.0,<2.0.0) Requires-Dist: requests
-(>=2.31.0,<3.0.0) Requires-Dist: rich (>=13.7.1,<14.0.0) Requires-Dist:
-sqlparse (>=0.4.4,<0.5.0) Requires-Dist: textual (>=0.56.2,<0.57.0) Requires-
-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0) Description-Content-Type: text/
-markdown # Dolphie
+Metadata-Version: 2.1 Name: dolphie Version: 5.0.0 Summary: Your single pane of
+glass for real-time analytics into MySQL & ProxySQL License: GPL-3.0-or-later
+Author: Charles Thompson Author-email: 01charles.t@gmail.com Requires-Python:
+>=3.8,<4.0 Classifier: License :: OSI Approved :: GNU General Public License v3
+or later (GPLv3+) Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.8 Classifier: Programming Language ::
+Python :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
+Programming Language :: Python :: 3.11 Requires-Dist: charset-normalizer
+(>=3.3.2,<4.0.0) Requires-Dist: myloginpath (>=0.0.4,<0.0.5) Requires-Dist:
+packaging (>=24.0,<25.0) Requires-Dist: plotext (>=5.2.8,<6.0.0) Requires-Dist:
+pymysql (>=1.1.0,<2.0.0) Requires-Dist: requests (>=2.31.0,<3.0.0) Requires-
+Dist: rich (>=13.7.1,<14.0.0) Requires-Dist: sqlparse (>=0.4.4,<0.5.0)
+Requires-Dist: textual-autocomplete (>=2.1.0b0,<3.0.0) Requires-Dist: textual
+[syntax] (>=0.57.1,<0.58.0) Description-Content-Type: text/markdown # Dolphie
  [https://user-images.githubusercontent.com/13244625/187600748-19d2ad15-42e8-
                           4f9c-ada5-a153cdcf4070.png]
-    Echolocate your MySQL health with real-time monitoring in the terminal
+    Your single pane of glass for real-time analytics into MySQL & ProxySQL
 
   [https://github.com/charles-001/dolphie/assets/13244625/88a41290-f52c-4b8e-
   97f8-3b7ef5096eae][https://github.com/charles-001/dolphie/assets/13244625/
  1d94502a-9abf-4436-a7d0-cb2b08c105c1][https://github.com/charles-001/dolphie/
              assets/13244625/9b1aadc8-cabb-4256-92f9-fe4d04451b83]
                                _[_B_u_y_ _M_e_ _A_ _C_o_f_f_e_e_]
 ![Untitled](https://github.com/charles-001/dolphie/assets/13244625/d1292ddc-
@@ -37,98 +36,99 @@
 curl -sSL https://install.python-poetry.org | python3 - $ poetry install ```
 #### Using Homebrew If you are a [Homebrew](https://brew.sh/) user, you can
 install [dolphie](https://formulae.brew.sh/formula/dolphie) via ```sh $ brew
 install dolphie ``` #### Using Docker ```sh $ docker pull ghcr.io/charles-001/
 dolphie:latest $ docker run -dit --name dolphie ghcr.io/charles-001/dolphie:
 latest $ docker exec -it dolphie dolphie -h host.docker.internal -u root --ask-
 pass ``` ## Usage ``` positional arguments: uri Use a URI string for
-credentials - format: mysql://user:password@host:port (port is optional with
-default 3306) options: --help show this help message and exit --host-setup
-Start Dolphie by showing the Host Setup modal instead of automatically
-connecting -u , --user Username for MySQL -p , --password Password for MySQL -
-h , --host Hostname/IP address for MySQL -P , --port Port for MySQL (Socket has
-precendence) -S , --socket Socket file for MySQL --config-file Dolphie's config
-file to use. Options are read from these files in the given order: /etc/
-dolphie.cnf, ~/.dolphie.cnf --mycnf-file MySQL config file path to use. This
-should use [client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve
-IPs to hostnames when your DNS is unable to. Each IP/hostname pair should be on
-its own line using format ip=hostname [default: ~/dolphie_host_cache] -q , --
-host-setup-file Specify location of file that stores the available hosts to use
-in host setup modal [default: ~/dolphie_hosts] -l , --login-path Specify login
+credentials (mysql/proxysql) - format: mysql://user:password@host:port (port is
+optional with default 3306, or 6032 for ProxySQL) options: --help show this
+help message and exit --host-setup Start Dolphie by showing the Host Setup
+modal instead of automatically connecting -u , --user Username -p , --password
+Password -h , --host Hostname/IP address -P , --port Port(Socket has
+precendence) -S , --socket Socket file --config-file Dolphie's config file to
+use. Options are read from these files in the given order: /etc/dolphie.cnf,
+~/.dolphie.cnf --mycnf-file MySQL config file path to use. This should use
+[client] section [default: ~/.my.cnf] -f , --host-cache-file Resolve IPs to
+hostnames when your DNS is unable to. Each IP/hostname pair should be on its
+own line using format ip=hostname [default: ~/dolphie_host_cache] -q , --host-
+setup-file Specify location of file that stores the available hosts to use in
+host setup modal [default: ~/dolphie_hosts] -l , --login-path Specify login
 path to use with mysql_config_editor's file ~/.mylogin.cnf for encrypted login
 credentials. Supercedes config file [default: client] -r , --refresh_interval
 How much time to wait in seconds between each refresh [default: 1] -H , --
-heartbeat-table If your hosts use pt-heartbeat, specify table in format
-db.table to use the timestamp it has for replication lag instead of
+heartbeat-table (MySQL only) If your hosts use pt-heartbeat, specify table in
+format db.table to use the timestamp it has for replication lag instead of
 Seconds_Behind_Master from SHOW REPLICA STATUS --ssl-mode Desired security
 state of the connection to the host. Supports: REQUIRED/VERIFY_CA/
 VERIFY_IDENTITY [default: OFF] --ssl-ca Path to the file that contains a CA
 (certificate authority) --ssl-cert Path to the file that contains a certificate
 --ssl-key Path to the file that contains a private key for the certificate --
 panels What panels to display on startup separated by a comma. Supports:
-dashboard,processlist,graphs,replication,metadata_locks,ddl [default:
-dashboard,processlist] --graph-marker What marker to use for graphs (available
-options: https://tinyurl.com/dolphie-markers) [default: braille] --pypi-
-repository What PyPi repository to use when checking for a new version. If not
-specified, it will use Dolphie's PyPi repository --hostgroup This is used for
-creating tabs and connecting to them for hosts you specify in Dolphie's config
-file under a hostgroup section. As an example, you'll have a section called
-[cluster1] then below it you will list each host on a new line in the format
-key=host (keys have no meaning). Hosts support optional port (default is
+dashboard,processlist,graphs,replication,metadata_locks,ddl,proxysql_hostgroup_summary,proxysql_mysql_query_rules,proxysql_command_stats
+[default: dashboard,processlist] --graph-marker What marker to use for graphs
+(available options: https://tinyurl.com/dolphie-markers) [default: braille] --
+pypi-repository What PyPi repository to use when checking for a new version. If
+not specified, it will use Dolphie's PyPi repository --hostgroup This is used
+for creating tabs and connecting to them for hosts you specify in Dolphie's
+config file under a hostgroup section. As an example, you'll have a section
+called [cluster1] then below it you will list each host on a new line in the
+format key=host (keys have no meaning). Hosts support optional port (default is
 whatever port parameter is) in the format host:port. You can also name the tabs
 by suffixing ~tab_name to the host (i.e. 1=host~tab_name) --show-trxs-only
-Start with only showing threads that have an active transaction --additional-
-columns Start with additional columns in Processlist panel --debug-options
-Display options that are set and what they're set by (command-line, dolphie
-config, etc) then exit -V, --version Display version and exit MySQL my.cnf file
-supports these options under [client] section: host user password port socket
-ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca ssl_cert ssl_key Login path
-file supports these options: host user password port socket Environment
-variables support these options: DOLPHIE_USER DOLPHIE_PASSWORD DOLPHIE_HOST
-DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config supports these options under
-[dolphie] section: (bool) host_setup (str) user (str) password (str) host (int)
-port (str) socket (str) ssl_mode (str) ssl_ca (str) ssl_cert (str) ssl_key
-(str) mycnf_file (str) login_path (str) host_cache_file (str) host_setup_file
-(int) refresh_interval (str) heartbeat_table (str) startup_panels (str)
-graph_marker (str) pypi_repository (str) hostgroup (bool) show_trxs_only (bool)
-show_additional_query_columns ``` ## Supported MySQL versions - MySQL/Percona
-Server 5.6/5.7/8.0+ - RDS/Aurora ## Grants required #### Least privilege 1.
-PROCESS (only if you switch to using processlist via `P` command) 2. SELECT to
-`performance_schema` + `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/
-REPLICATION SLAVE 4. BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS
-(only if you switch to using processlist via `P` command) 2. Global SELECT
-access (good for explaining queries, listing all databases, etc) 4. REPLICATION
-CLIENT/REPLICATION SLAVE 5. SUPER (required if you want to kill queries) 6.
-BACKUP_ADMIN (MySQL 8 only) ## Features - Tabs docked at the top to seamlessly
-switch between connected hosts - Hostgroups to make it easy for connecting to
-multiple hosts at once - Dolphie uses panels to present groups of data. They
-can all be turned on/off to have a view of your database server that you prefer
-- Graphs for many metrics that can give you great insight into how your
-database is performing - Sparkline to show queries per second in a live view -
-2 options for finding replica lag in this order of precedence: - `pt-heartbeat
-table` (specified by `--heartbeat-table`) - `SHOW SLAVE STATUS` - Keeps a
-history of the servers you connect to that provides autocompletion for
-hostnames in the Host Setup modal - Host cache file. This provides users a way
-to specify hostnames for IPs when their network's DNS can't resolve them. An
-example use case for this is when you connect to your work's VPN and DNS isn't
-available to resolve IPs. In my opinion, it's a lot easier to look at hostnames
-than IPs! - Supports encrypted login credentials via `mysql_config_editor` -
-Automatic conversion of large numbers & bytes to human-readable - Notifies when
-new version is available - Many commands at your fingertips with autocompletion
-for their input ## Hostgroups Hostgroups are a way to easily connect to
-multiple hosts at once. To set this up, you will create a section in Dolphie's
-config file with the name you want the hostgroup to be and list each host on a
-new line in the format `key=host` (keys have no meaning). Hosts support
-optional port (default is whatever `port` parameter is) in the format `host:
-port`. You can also name the tabs by suffixing `~tab_name` to the host. Once
-ready, you will use the parameter `hostgroup` or `Host Setup` modal to see it
-in action! Note: Colors can be used in the tab name by using the format `
-[color]text[/color]` (i.e. `[red]production[/red]`). You can also use emojis
-supported by Rich (can see them by running `python -m rich.emoji`) by using the
-format `:emoji:` (i.e. `:ghost:`). Rich supports the normal emoji shortcodes.
-Example: ```ini [cluster1] 1=host1 2=host2:3307 3=host3:3308~[red]production[/
-red] :ghost: ``` ## Things to note Order of precedence for methods that pass
-options to Dolphie: 1. Command-line 2. Environment variables 3. Dolphie's
-config (set by `--config-file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5.
-~/.my.cnf (set by `--mycnf-file`) ## Feedback I welcome all questions, bug
-reports, and requests. If you enjoy Dolphie, please let me know! I'd love to
-hear from you :smiley:
+(MySQL only) Start with only showing threads that have an active transaction --
+additional-columns Start with additional columns in Processlist panel --debug-
+options Display options that are set and what they're set by (command-line,
+dolphie config, etc) then exit -V, --version Display version and exit MySQL
+my.cnf file supports these options under [client] section: host user password
+port socket ssl_mode REQUIRED/VERIFY_CA/VERIFY_IDENTITY ssl_ca ssl_cert ssl_key
+Login path file supports these options: host user password port socket
+Environment variables support these options: DOLPHIE_USER DOLPHIE_PASSWORD
+DOLPHIE_HOST DOLPHIE_PORT DOLPHIE_SOCKET Dolphie's config supports these
+options under [dolphie] section: (bool) host_setup (str) user (str) password
+(str) host (int) port (str) socket (str) ssl_mode (str) ssl_ca (str) ssl_cert
+(str) ssl_key (str) mycnf_file (str) login_path (str) host_cache_file (str)
+host_setup_file (int) refresh_interval (str) heartbeat_table (str)
+startup_panels (str) graph_marker (str) pypi_repository (str) hostgroup (bool)
+show_trxs_only (bool) show_additional_query_columns ``` ## Supported MySQL
+versions - MySQL/Percona Server 5.6/5.7/8.0+ - RDS & Aurora + Azure ##
+Supported ProxySQL versions - ProxySQL 2.6+ (could work on previous versions
+but not tested) ## Grants required #### Least privilege 1. PROCESS (only if you
+switch to using processlist via `P` command) 2. SELECT to `performance_schema`
++ `pt-heartbeat table` (if used) 3. REPLICATION CLIENT/REPLICATION SLAVE 4.
+BACKUP_ADMIN (MySQL 8 only) #### Recommended 1. PROCESS (only if you switch to
+using processlist via `P` command) 2. Global SELECT access (good for explaining
+queries, listing all databases, etc) 4. REPLICATION CLIENT/REPLICATION SLAVE 5.
+SUPER (required if you want to kill queries) 6. BACKUP_ADMIN (MySQL 8 only) ##
+Features - Tabs docked at the top to seamlessly switch between connected hosts
+- Hostgroups to make it easy for connecting to multiple hosts at once - Dolphie
+uses panels to present groups of data. They can all be turned on/off to have a
+view of your database server that you prefer - Graphs for many metrics that can
+give you great insight into how your database is performing - Sparkline to show
+queries per second in a live view - 2 options for finding replica lag in this
+order of precedence: - `pt-heartbeat table` (specified by `--heartbeat-table`)
+- `SHOW SLAVE STATUS` - Keeps a history of the servers you connect to that
+provides autocompletion for hostnames in the Host Setup modal - Host cache
+file. This provides users a way to specify hostnames for IPs when their
+network's DNS can't resolve them. An example use case for this is when you
+connect to your work's VPN and DNS isn't available to resolve IPs. In my
+opinion, it's a lot easier to look at hostnames than IPs! - Supports encrypted
+login credentials via `mysql_config_editor` - Automatic conversion of large
+numbers & bytes to human-readable - Notifies when new version is available -
+Many commands at your fingertips with autocompletion for their input ##
+Hostgroups Hostgroups are a way to easily connect to multiple hosts at once. To
+set this up, you will create a section in Dolphie's config file with the name
+you want the hostgroup to be and list each host on a new line in the format
+`key=host` (keys have no meaning). Hosts support optional port (default is
+whatever `port` parameter is) in the format `host:port`. You can also name the
+tabs by suffixing `~tab_name` to the host. Once ready, you will use the
+parameter `hostgroup` or `Host Setup` modal to see it in action! Note: Colors
+can be used in the tab name by using the format `[color]text[/color]` (i.e. `
+[red]production[/red]`). You can also use emojis supported by Rich (can see
+them by running `python -m rich.emoji`) by using the format `:emoji:` (i.e. `:
+ghost:`). Rich supports the normal emoji shortcodes. Example: ```ini [cluster1]
+1=host1 2=host2:3307 3=host3:3308~[red]production[/red] :ghost: ``` ## Things
+to note Order of precedence for methods that pass options to Dolphie: 1.
+Command-line 2. Environment variables 3. Dolphie's config (set by `--config-
+file`) 4. ~/.mylogin.cnf (`mysql_config_editor`) 5. ~/.my.cnf (set by `--mycnf-
+file`) ## Feedback I welcome all questions, bug reports, and requests. If you
+enjoy Dolphie, please let me know! I'd love to hear from you :smiley:
```

