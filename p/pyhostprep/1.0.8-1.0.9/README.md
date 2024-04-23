# Comparing `tmp/pyhostprep-1.0.8.tar.gz` & `tmp/pyhostprep-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyhostprep-1.0.8.tar", last modified: Tue Mar 26 15:58:43 2024, max compression
+gzip compressed data, was "pyhostprep-1.0.9.tar", last modified: Wed Mar 27 20:54:59 2024, max compression
```

## Comparing `pyhostprep-1.0.8.tar` & `pyhostprep-1.0.9.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-26 15:58:43.775993 pyhostprep-1.0.8/
--rw-r--r--   0 michael    (501) staff       (20)    10141 2024-01-29 21:18:06.000000 pyhostprep-1.0.8/LICENSE.txt
--rw-r--r--   0 michael    (501) staff       (20)     1194 2024-03-26 15:58:43.775793 pyhostprep-1.0.8/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)      383 2024-03-26 15:58:12.000000 pyhostprep-1.0.8/README.md
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-26 15:58:43.744672 pyhostprep-1.0.8/pyhostprep/
--rw-r--r--   0 michael    (501) staff       (20)      395 2024-03-26 15:58:12.000000 pyhostprep-1.0.8/pyhostprep/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     4207 2024-03-11 15:33:20.000000 pyhostprep-1.0.8/pyhostprep/bundlemgr.py
--rw-r--r--   0 michael    (501) staff       (20)     2305 2023-09-20 17:59:26.000000 pyhostprep-1.0.8/pyhostprep/bundles.py
--rw-r--r--   0 michael    (501) staff       (20)     5669 2023-11-17 23:00:14.000000 pyhostprep-1.0.8/pyhostprep/cli.py
--rw-r--r--   0 michael    (501) staff       (20)     1819 2023-09-01 19:46:47.000000 pyhostprep-1.0.8/pyhostprep/command.py
--rw-r--r--   0 michael    (501) staff       (20)      486 2024-03-11 14:41:44.000000 pyhostprep-1.0.8/pyhostprep/constants.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-26 15:58:43.693262 pyhostprep-1.0.8/pyhostprep/data/
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-26 15:58:43.751595 pyhostprep-1.0.8/pyhostprep/data/config/
--rw-r--r--   0 michael    (501) staff       (20)       52 2023-08-21 21:09:49.000000 pyhostprep-1.0.8/pyhostprep/data/config/91-couchbase.conf
--rw-r--r--   0 michael    (501) staff       (20)     1011 2023-08-21 21:09:49.000000 pyhostprep-1.0.8/pyhostprep/data/config/disable-thp
--rw-r--r--   0 michael    (501) staff       (20)     6920 2023-12-01 07:15:45.000000 pyhostprep-1.0.8/pyhostprep/data/config/packages.json
--rw-r--r--   0 michael    (501) staff       (20)      949 2023-09-20 19:11:59.000000 pyhostprep-1.0.8/pyhostprep/data/config/sync_gateway_2.json
--rw-r--r--   0 michael    (501) staff       (20)      872 2023-09-20 19:02:13.000000 pyhostprep-1.0.8/pyhostprep/data/config/sync_gateway_3.json
--rw-r--r--   0 michael    (501) staff       (20)       63 2023-08-21 21:09:49.000000 pyhostprep-1.0.8/pyhostprep/data/config/tuned.conf
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-26 15:58:43.766104 pyhostprep-1.0.8/pyhostprep/data/playbooks/
--rw-r--r--   0 michael    (501) staff       (20)     1104 2023-12-16 00:05:21.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/base_sw_amzn.yaml
--rw-r--r--   0 michael    (501) staff       (20)      472 2023-12-16 00:03:11.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/base_sw_apt.yaml
--rw-r--r--   0 michael    (501) staff       (20)      872 2023-12-16 00:03:59.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/base_sw_yum.yaml
--rw-r--r--   0 michael    (501) staff       (20)      366 2023-12-16 00:09:17.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/base_sw_zypper.yaml
--rw-r--r--   0 michael    (501) staff       (20)     1900 2023-10-26 18:08:22.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/configure_cbdata.yaml
--rw-r--r--   0 michael    (501) staff       (20)     1183 2023-10-26 15:42:18.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/configure_swap.yaml
--rw-r--r--   0 michael    (501) staff       (20)      211 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/configure_swappiness.yaml
--rw-r--r--   0 michael    (501) staff       (20)      317 2023-09-20 19:50:57.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_firewall_dep.yaml
--rw-r--r--   0 michael    (501) staff       (20)      232 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_firewalld_rhel.yaml
--rw-r--r--   0 michael    (501) staff       (20)      566 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_thp_amzn.yaml
--rw-r--r--   0 michael    (501) staff       (20)      389 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_thp_deb.yaml
--rw-r--r--   0 michael    (501) staff       (20)      745 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_thp_rhel.yaml
--rw-r--r--   0 michael    (501) staff       (20)      575 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_thp_sles.yaml
--rw-r--r--   0 michael    (501) staff       (20)      228 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/enable_chrony_dep.yaml
--rw-r--r--   0 michael    (501) staff       (20)      229 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/enable_chrony_rhel.yaml
--rw-r--r--   0 michael    (501) staff       (20)      510 2023-10-11 18:19:38.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/enable_sgw.yaml
--rw-r--r--   0 michael    (501) staff       (20)      186 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/install_cbs_apt.yaml
--rw-r--r--   0 michael    (501) staff       (20)      247 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/install_cbs_sles.yaml
--rw-r--r--   0 michael    (501) staff       (20)      488 2023-08-21 20:56:07.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/install_cbs_yum.yaml
--rw-r--r--   0 michael    (501) staff       (20)      676 2023-12-16 00:09:17.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/install_libcouchbase_apt.yaml
--rw-r--r--   0 michael    (501) staff       (20)      532 2023-12-16 00:09:17.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/install_libcouchbase_yum.yaml
--rw-r--r--   0 michael    (501) staff       (20)      178 2023-09-20 15:30:00.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/install_sgw_deb.yaml
--rw-r--r--   0 michael    (501) staff       (20)      234 2023-09-20 15:26:54.000000 pyhostprep-1.0.8/pyhostprep/data/playbooks/install_sgw_rpm.yaml
--rw-r--r--   0 michael    (501) staff       (20)     7056 2023-09-06 20:54:59.000000 pyhostprep-1.0.8/pyhostprep/ebsnvme.py
--rw-r--r--   0 michael    (501) staff       (20)     1105 2023-09-07 21:30:13.000000 pyhostprep-1.0.8/pyhostprep/exception.py
--rw-r--r--   0 michael    (501) staff       (20)     4417 2023-11-17 23:09:48.000000 pyhostprep-1.0.8/pyhostprep/gateway.py
--rw-r--r--   0 michael    (501) staff       (20)     2603 2023-10-11 21:39:40.000000 pyhostprep-1.0.8/pyhostprep/hostinfo.py
--rw-r--r--   0 michael    (501) staff       (20)     1280 2024-03-15 19:53:17.000000 pyhostprep-1.0.8/pyhostprep/network.py
--rw-r--r--   0 michael    (501) staff       (20)     2219 2023-11-17 22:30:00.000000 pyhostprep-1.0.8/pyhostprep/osinfo.py
--rw-r--r--   0 michael    (501) staff       (20)     7800 2023-10-11 19:24:09.000000 pyhostprep-1.0.8/pyhostprep/rest.py
--rw-r--r--   0 michael    (501) staff       (20)     2830 2023-08-21 20:48:25.000000 pyhostprep-1.0.8/pyhostprep/retry.py
--rw-r--r--   0 michael    (501) staff       (20)    17426 2024-03-26 15:54:24.000000 pyhostprep-1.0.8/pyhostprep/server.py
--rw-r--r--   0 michael    (501) staff       (20)     7621 2024-03-11 14:41:44.000000 pyhostprep-1.0.8/pyhostprep/software.py
--rw-r--r--   0 michael    (501) staff       (20)     1704 2023-09-07 00:52:04.000000 pyhostprep-1.0.8/pyhostprep/storage.py
--rw-r--r--   0 michael    (501) staff       (20)     1102 2023-09-07 13:08:46.000000 pyhostprep-1.0.8/pyhostprep/storagemgr.py
--rw-r--r--   0 michael    (501) staff       (20)     4819 2024-03-15 19:30:42.000000 pyhostprep-1.0.8/pyhostprep/swmgr.py
--rw-r--r--   0 michael    (501) staff       (20)     1970 2024-03-20 23:11:01.000000 pyhostprep-1.0.8/pyhostprep/util.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-26 15:58:43.746101 pyhostprep-1.0.8/pyhostprep.egg-info/
--rw-r--r--   0 michael    (501) staff       (20)     1194 2024-03-26 15:58:43.000000 pyhostprep-1.0.8/pyhostprep.egg-info/PKG-INFO
--rw-r--r--   0 michael    (501) staff       (20)     2152 2024-03-26 15:58:43.000000 pyhostprep-1.0.8/pyhostprep.egg-info/SOURCES.txt
--rw-r--r--   0 michael    (501) staff       (20)        1 2024-03-26 15:58:43.000000 pyhostprep-1.0.8/pyhostprep.egg-info/dependency_links.txt
--rw-r--r--   0 michael    (501) staff       (20)      126 2024-03-26 15:58:43.000000 pyhostprep-1.0.8/pyhostprep.egg-info/entry_points.txt
--rw-r--r--   0 michael    (501) staff       (20)      260 2024-03-26 15:58:43.000000 pyhostprep-1.0.8/pyhostprep.egg-info/requires.txt
--rw-r--r--   0 michael    (501) staff       (20)       11 2024-03-26 15:58:43.000000 pyhostprep-1.0.8/pyhostprep.egg-info/top_level.txt
--rw-r--r--   0 michael    (501) staff       (20)       38 2024-03-26 15:58:43.776053 pyhostprep-1.0.8/setup.cfg
--rw-r--r--   0 michael    (501) staff       (20)     1905 2023-11-15 19:45:03.000000 pyhostprep-1.0.8/setup.py
-drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-26 15:58:43.775444 pyhostprep-1.0.8/tests/
--rw-r--r--   0 michael    (501) staff       (20)        0 2023-08-21 20:52:13.000000 pyhostprep-1.0.8/tests/__init__.py
--rw-r--r--   0 michael    (501) staff       (20)     6417 2023-11-15 19:24:08.000000 pyhostprep-1.0.8/tests/common.py
--rwxr-xr-x   0 michael    (501) staff       (20)     1359 2023-08-21 20:52:13.000000 pyhostprep-1.0.8/tests/journalctl3.py
--rwxr-xr-x   0 michael    (501) staff       (20)   302133 2023-08-21 20:52:13.000000 pyhostprep-1.0.8/tests/systemctl3.py
--rwxr-xr-x   0 michael    (501) staff       (20)     2617 2023-08-25 14:53:42.000000 pyhostprep-1.0.8/tests/test_1.py
--rw-r--r--   0 michael    (501) staff       (20)      617 2023-08-21 20:52:13.000000 pyhostprep-1.0.8/tests/test_2.py
--rw-r--r--   0 michael    (501) staff       (20)      663 2023-08-21 20:52:13.000000 pyhostprep-1.0.8/tests/test_3.py
--rwxr-xr-x   0 michael    (501) staff       (20)     4333 2023-08-25 15:05:29.000000 pyhostprep-1.0.8/tests/test_m.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-27 20:54:59.169799 pyhostprep-1.0.9/
+-rw-r--r--   0 michael    (501) staff       (20)    10141 2024-01-29 21:18:06.000000 pyhostprep-1.0.9/LICENSE.txt
+-rw-r--r--   0 michael    (501) staff       (20)     1194 2024-03-27 20:54:59.169664 pyhostprep-1.0.9/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)      383 2024-03-27 20:54:26.000000 pyhostprep-1.0.9/README.md
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-27 20:54:59.147563 pyhostprep-1.0.9/pyhostprep/
+-rw-r--r--   0 michael    (501) staff       (20)      395 2024-03-27 20:54:26.000000 pyhostprep-1.0.9/pyhostprep/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     4207 2024-03-11 15:33:20.000000 pyhostprep-1.0.9/pyhostprep/bundlemgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     2305 2023-09-20 17:59:26.000000 pyhostprep-1.0.9/pyhostprep/bundles.py
+-rw-r--r--   0 michael    (501) staff       (20)     5669 2023-11-17 23:00:14.000000 pyhostprep-1.0.9/pyhostprep/cli.py
+-rw-r--r--   0 michael    (501) staff       (20)     1819 2023-09-01 19:46:47.000000 pyhostprep-1.0.9/pyhostprep/command.py
+-rw-r--r--   0 michael    (501) staff       (20)      486 2024-03-11 14:41:44.000000 pyhostprep-1.0.9/pyhostprep/constants.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-27 20:54:59.137966 pyhostprep-1.0.9/pyhostprep/data/
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-27 20:54:59.150822 pyhostprep-1.0.9/pyhostprep/data/config/
+-rw-r--r--   0 michael    (501) staff       (20)       52 2023-08-21 21:09:49.000000 pyhostprep-1.0.9/pyhostprep/data/config/91-couchbase.conf
+-rw-r--r--   0 michael    (501) staff       (20)     1011 2023-08-21 21:09:49.000000 pyhostprep-1.0.9/pyhostprep/data/config/disable-thp
+-rw-r--r--   0 michael    (501) staff       (20)     6920 2023-12-01 07:15:45.000000 pyhostprep-1.0.9/pyhostprep/data/config/packages.json
+-rw-r--r--   0 michael    (501) staff       (20)      949 2023-09-20 19:11:59.000000 pyhostprep-1.0.9/pyhostprep/data/config/sync_gateway_2.json
+-rw-r--r--   0 michael    (501) staff       (20)      872 2023-09-20 19:02:13.000000 pyhostprep-1.0.9/pyhostprep/data/config/sync_gateway_3.json
+-rw-r--r--   0 michael    (501) staff       (20)       63 2023-08-21 21:09:49.000000 pyhostprep-1.0.9/pyhostprep/data/config/tuned.conf
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-27 20:54:59.163685 pyhostprep-1.0.9/pyhostprep/data/playbooks/
+-rw-r--r--   0 michael    (501) staff       (20)     1104 2023-12-16 00:05:21.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/base_sw_amzn.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      472 2023-12-16 00:03:11.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/base_sw_apt.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      872 2023-12-16 00:03:59.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/base_sw_yum.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      366 2023-12-16 00:09:17.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/base_sw_zypper.yaml
+-rw-r--r--   0 michael    (501) staff       (20)     1900 2023-10-26 18:08:22.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/configure_cbdata.yaml
+-rw-r--r--   0 michael    (501) staff       (20)     1183 2023-10-26 15:42:18.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/configure_swap.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      211 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/configure_swappiness.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      317 2023-09-20 19:50:57.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_firewall_dep.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      232 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_firewalld_rhel.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      566 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_thp_amzn.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      389 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_thp_deb.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      745 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_thp_rhel.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      575 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_thp_sles.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      228 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/enable_chrony_dep.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      229 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/enable_chrony_rhel.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      510 2023-10-11 18:19:38.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/enable_sgw.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      186 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/install_cbs_apt.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      247 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/install_cbs_sles.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      488 2023-08-21 20:56:07.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/install_cbs_yum.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      676 2023-12-16 00:09:17.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/install_libcouchbase_apt.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      532 2023-12-16 00:09:17.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/install_libcouchbase_yum.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      178 2023-09-20 15:30:00.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/install_sgw_deb.yaml
+-rw-r--r--   0 michael    (501) staff       (20)      234 2023-09-20 15:26:54.000000 pyhostprep-1.0.9/pyhostprep/data/playbooks/install_sgw_rpm.yaml
+-rw-r--r--   0 michael    (501) staff       (20)     7056 2023-09-06 20:54:59.000000 pyhostprep-1.0.9/pyhostprep/ebsnvme.py
+-rw-r--r--   0 michael    (501) staff       (20)     1105 2023-09-07 21:30:13.000000 pyhostprep-1.0.9/pyhostprep/exception.py
+-rw-r--r--   0 michael    (501) staff       (20)     4417 2023-11-17 23:09:48.000000 pyhostprep-1.0.9/pyhostprep/gateway.py
+-rw-r--r--   0 michael    (501) staff       (20)     2603 2023-10-11 21:39:40.000000 pyhostprep-1.0.9/pyhostprep/hostinfo.py
+-rw-r--r--   0 michael    (501) staff       (20)     1280 2024-03-15 19:53:17.000000 pyhostprep-1.0.9/pyhostprep/network.py
+-rw-r--r--   0 michael    (501) staff       (20)     2219 2023-11-17 22:30:00.000000 pyhostprep-1.0.9/pyhostprep/osinfo.py
+-rw-r--r--   0 michael    (501) staff       (20)     7800 2023-10-11 19:24:09.000000 pyhostprep-1.0.9/pyhostprep/rest.py
+-rw-r--r--   0 michael    (501) staff       (20)     2830 2023-08-21 20:48:25.000000 pyhostprep-1.0.9/pyhostprep/retry.py
+-rw-r--r--   0 michael    (501) staff       (20)    17426 2024-03-26 21:38:36.000000 pyhostprep-1.0.9/pyhostprep/server.py
+-rw-r--r--   0 michael    (501) staff       (20)     7621 2024-03-11 14:41:44.000000 pyhostprep-1.0.9/pyhostprep/software.py
+-rw-r--r--   0 michael    (501) staff       (20)     1704 2023-09-07 00:52:04.000000 pyhostprep-1.0.9/pyhostprep/storage.py
+-rw-r--r--   0 michael    (501) staff       (20)     1102 2023-09-07 13:08:46.000000 pyhostprep-1.0.9/pyhostprep/storagemgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     4819 2024-03-15 19:30:42.000000 pyhostprep-1.0.9/pyhostprep/swmgr.py
+-rw-r--r--   0 michael    (501) staff       (20)     1970 2024-03-20 23:11:01.000000 pyhostprep-1.0.9/pyhostprep/util.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-27 20:54:59.148634 pyhostprep-1.0.9/pyhostprep.egg-info/
+-rw-r--r--   0 michael    (501) staff       (20)     1194 2024-03-27 20:54:59.000000 pyhostprep-1.0.9/pyhostprep.egg-info/PKG-INFO
+-rw-r--r--   0 michael    (501) staff       (20)     2152 2024-03-27 20:54:59.000000 pyhostprep-1.0.9/pyhostprep.egg-info/SOURCES.txt
+-rw-r--r--   0 michael    (501) staff       (20)        1 2024-03-27 20:54:59.000000 pyhostprep-1.0.9/pyhostprep.egg-info/dependency_links.txt
+-rw-r--r--   0 michael    (501) staff       (20)      126 2024-03-27 20:54:59.000000 pyhostprep-1.0.9/pyhostprep.egg-info/entry_points.txt
+-rw-r--r--   0 michael    (501) staff       (20)      260 2024-03-27 20:54:59.000000 pyhostprep-1.0.9/pyhostprep.egg-info/requires.txt
+-rw-r--r--   0 michael    (501) staff       (20)       11 2024-03-27 20:54:59.000000 pyhostprep-1.0.9/pyhostprep.egg-info/top_level.txt
+-rw-r--r--   0 michael    (501) staff       (20)       38 2024-03-27 20:54:59.169841 pyhostprep-1.0.9/setup.cfg
+-rw-r--r--   0 michael    (501) staff       (20)     1905 2024-03-27 20:54:18.000000 pyhostprep-1.0.9/setup.py
+drwxr-xr-x   0 michael    (501) staff       (20)        0 2024-03-27 20:54:59.169305 pyhostprep-1.0.9/tests/
+-rw-r--r--   0 michael    (501) staff       (20)        0 2023-08-21 20:52:13.000000 pyhostprep-1.0.9/tests/__init__.py
+-rw-r--r--   0 michael    (501) staff       (20)     6417 2023-11-15 19:24:08.000000 pyhostprep-1.0.9/tests/common.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     1359 2023-08-21 20:52:13.000000 pyhostprep-1.0.9/tests/journalctl3.py
+-rwxr-xr-x   0 michael    (501) staff       (20)   302133 2023-08-21 20:52:13.000000 pyhostprep-1.0.9/tests/systemctl3.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     2617 2023-08-25 14:53:42.000000 pyhostprep-1.0.9/tests/test_1.py
+-rw-r--r--   0 michael    (501) staff       (20)      617 2023-08-21 20:52:13.000000 pyhostprep-1.0.9/tests/test_2.py
+-rw-r--r--   0 michael    (501) staff       (20)      663 2023-08-21 20:52:13.000000 pyhostprep-1.0.9/tests/test_3.py
+-rwxr-xr-x   0 michael    (501) staff       (20)     4333 2023-08-25 15:05:29.000000 pyhostprep-1.0.9/tests/test_m.py
```

### Comparing `pyhostprep-1.0.8/LICENSE.txt` & `pyhostprep-1.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/PKG-INFO` & `pyhostprep-1.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhostprep
-Version: 1.0.8
+Version: 1.0.9
 Summary: Couchbase Host Automation Library
 Home-page: https://github.com/mminichino/host-prep-lib
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: Apache License 2.0
 Keywords: couchbase,devops,automation
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# host-prep-lib 1.0.8
+# host-prep-lib 1.0.9
 
 Automation for preparing a host to run Couchbase software.
 
 Note: This package is not officially supported by Couchbase.
 
 ## Quick Start
```

### Comparing `pyhostprep-1.0.8/pyhostprep/bundlemgr.py` & `pyhostprep-1.0.9/pyhostprep/bundlemgr.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/bundles.py` & `pyhostprep-1.0.9/pyhostprep/bundles.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/cli.py` & `pyhostprep-1.0.9/pyhostprep/cli.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/command.py` & `pyhostprep-1.0.9/pyhostprep/command.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/config/disable-thp` & `pyhostprep-1.0.9/pyhostprep/data/config/disable-thp`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/config/packages.json` & `pyhostprep-1.0.9/pyhostprep/data/config/packages.json`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/config/sync_gateway_2.json` & `pyhostprep-1.0.9/pyhostprep/data/config/sync_gateway_2.json`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/config/sync_gateway_3.json` & `pyhostprep-1.0.9/pyhostprep/data/config/sync_gateway_3.json`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/base_sw_amzn.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/base_sw_amzn.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/base_sw_yum.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/base_sw_yum.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/configure_cbdata.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/configure_cbdata.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/configure_swap.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/configure_swap.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_thp_amzn.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_thp_amzn.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_thp_rhel.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_thp_rhel.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/disable_thp_sles.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/disable_thp_sles.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/install_libcouchbase_apt.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/install_libcouchbase_apt.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/data/playbooks/install_libcouchbase_yum.yaml` & `pyhostprep-1.0.9/pyhostprep/data/playbooks/install_libcouchbase_yum.yaml`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/ebsnvme.py` & `pyhostprep-1.0.9/pyhostprep/ebsnvme.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/exception.py` & `pyhostprep-1.0.9/pyhostprep/exception.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/gateway.py` & `pyhostprep-1.0.9/pyhostprep/gateway.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/hostinfo.py` & `pyhostprep-1.0.9/pyhostprep/hostinfo.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/network.py` & `pyhostprep-1.0.9/pyhostprep/network.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/osinfo.py` & `pyhostprep-1.0.9/pyhostprep/osinfo.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/rest.py` & `pyhostprep-1.0.9/pyhostprep/rest.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/retry.py` & `pyhostprep-1.0.9/pyhostprep/retry.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/server.py` & `pyhostprep-1.0.9/pyhostprep/server.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/software.py` & `pyhostprep-1.0.9/pyhostprep/software.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/storage.py` & `pyhostprep-1.0.9/pyhostprep/storage.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/storagemgr.py` & `pyhostprep-1.0.9/pyhostprep/storagemgr.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/swmgr.py` & `pyhostprep-1.0.9/pyhostprep/swmgr.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep/util.py` & `pyhostprep-1.0.9/pyhostprep/util.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/pyhostprep.egg-info/PKG-INFO` & `pyhostprep-1.0.9/pyhostprep.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyhostprep
-Version: 1.0.8
+Version: 1.0.9
 Summary: Couchbase Host Automation Library
 Home-page: https://github.com/mminichino/host-prep-lib
 Author: Michael Minichino
 Author-email: info@unix.us.com
 License: Apache License 2.0
 Keywords: couchbase,devops,automation
 Classifier: Development Status :: 4 - Beta
@@ -16,15 +16,15 @@
 Classifier: Topic :: Database
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
-# host-prep-lib 1.0.8
+# host-prep-lib 1.0.9
 
 Automation for preparing a host to run Couchbase software.
 
 Note: This package is not officially supported by Couchbase.
 
 ## Quick Start
```

### Comparing `pyhostprep-1.0.8/pyhostprep.egg-info/SOURCES.txt` & `pyhostprep-1.0.9/pyhostprep.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/setup.py` & `pyhostprep-1.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,20 @@
         "pytest-asyncio>=0.16.0",
         "pytest-rerunfailures>=10.3",
         "pytest-mock>=3.6.1",
         "docker>=5.0.3",
         "ansible>=6.7.0",
         "ansible-runner>=2.3.3",
         "requests>=2.31.0",
-        "urllib3==1.26.16",
+        "urllib3>=1.26.18",
         "overrides>=7.4.0",
         "bumpversion>=0.6.0",
         "psutil>=5.9.5",
         "cbcmgr>=2.1.5",
-        "Jinja2>=3.0.3"
+        "Jinja2>=3.1.3"
     ],
     author_email='info@unix.us.com',
     description='Couchbase Host Automation Library',
     long_description=long_description,
     long_description_content_type='text/markdown',
     keywords=["couchbase", "devops", "automation"],
     classifiers=[
```

### Comparing `pyhostprep-1.0.8/tests/common.py` & `pyhostprep-1.0.9/tests/common.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/tests/journalctl3.py` & `pyhostprep-1.0.9/tests/journalctl3.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/tests/systemctl3.py` & `pyhostprep-1.0.9/tests/systemctl3.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/tests/test_1.py` & `pyhostprep-1.0.9/tests/test_1.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/tests/test_2.py` & `pyhostprep-1.0.9/tests/test_2.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/tests/test_3.py` & `pyhostprep-1.0.9/tests/test_3.py`

 * *Files identical despite different names*

### Comparing `pyhostprep-1.0.8/tests/test_m.py` & `pyhostprep-1.0.9/tests/test_m.py`

 * *Files identical despite different names*

