# Comparing `tmp/pulumi_linode-4.9.0a1700248892.tar.gz` & `tmp/pulumi_linode-4.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_linode-4.9.0a1700248892.tar", last modified: Fri Nov 17 19:25:22 2023, max compression
+gzip compressed data, was "pulumi_linode-4.9.1.tar", last modified: Mon Dec  4 18:14:02 2023, max compression
```

## Comparing `pulumi_linode-4.9.0a1700248892.tar` & `pulumi_linode-4.9.1.tar`

### file list

```diff
@@ -1,101 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 19:25:22.221087 pulumi_linode-4.9.0a1700248892/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-11-17 19:25:22.221087 pulumi_linode-4.9.0a1700248892/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 19:25:22.221087 pulumi_linode-4.9.0a1700248892/pulumi_linode/
--rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   290134 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     8081 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    16532 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/account_settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 19:25:22.221087 pulumi_linode-4.9.0a1700248892/pulumi_linode/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    12684 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/database_access_controls.py
--rw-r--r--   0 runner    (1001) docker     (127)    44527 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)    50181 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)    40821 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/domain.py
--rw-r--r--   0 runner    (1001) docker     (127)    33929 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    35787 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    13586 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/firewall_device.py
--rw-r--r--   0 runner    (1001) docker     (127)     8323 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account.py
--rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account_login.py
--rw-r--r--   0 runner    (1001) docker     (127)     4827 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account_logins.py
--rw-r--r--   0 runner    (1001) docker     (127)     5353 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     8865 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_engines.py
--rw-r--r--   0 runner    (1001) docker     (127)    15050 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_mysql.py
--rw-r--r--   0 runner    (1001) docker     (127)     7983 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_mysql_backups.py
--rw-r--r--   0 runner    (1001) docker     (127)    16312 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_postgresql.py
--rw-r--r--   0 runner    (1001) docker     (127)     6046 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_databases.py
--rw-r--r--   0 runner    (1001) docker     (127)     9608 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_domain.py
--rw-r--r--   0 runner    (1001) docker     (127)     8745 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_domain_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3780 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_domain_zonefile.py
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)     8313 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_firewalls.py
--rw-r--r--   0 runner    (1001) docker     (127)     8365 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_image.py
--rw-r--r--   0 runner    (1001) docker     (127)     7884 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_images.py
--rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_backups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_networking.py
--rw-r--r--   0 runner    (1001) docker     (127)     7625 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     6616 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     6734 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instances.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (127)     5950 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     6106 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_kernels.py
--rw-r--r--   0 runner    (1001) docker     (127)     4729 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_linode_object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)     7224 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_lke_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7190 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_networking_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     7111 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    13058 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     6893 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (127)     6638 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_nodebalancers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_object_storage_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     8249 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     5317 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_region.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_regions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     6285 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_sshkeys.py
--rw-r--r--   0 runner    (1001) docker     (127)     9856 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_stack_script.py
--rw-r--r--   0 runner    (1001) docker     (127)     8084 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_stack_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)    14159 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     6380 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vlans.py
--rw-r--r--   0 runner    (1001) docker     (127)     6953 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_volume.py
--rw-r--r--   0 runner    (1001) docker     (127)     5478 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_volumes.py
--rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     5617 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpc_subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)     5404 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpc_subnets.py
--rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpcs.py
--rw-r--r--   0 runner    (1001) docker     (127)    34342 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/image.py
--rw-r--r--   0 runner    (1001) docker     (127)   117154 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/instance.py
--rw-r--r--   0 runner    (1001) docker     (127)    33871 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/instance_disk.py
--rw-r--r--   0 runner    (1001) docker     (127)    20651 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/instance_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     8713 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/instance_shared_ips.py
--rw-r--r--   0 runner    (1001) docker     (127)    15042 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/ipv6_range.py
--rw-r--r--   0 runner    (1001) docker     (127)    26054 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/lke_cluster.py
--rw-r--r--   0 runner    (1001) docker     (127)    24174 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/node_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)    57023 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/node_balancer_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    21278 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/node_balancer_node.py
--rw-r--r--   0 runner    (1001) docker     (127)    31602 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/object_storage_bucket.py
--rw-r--r--   0 runner    (1001) docker     (127)    14371 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/object_storage_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    52151 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/object_storage_object.py
--rw-r--r--   0 runner    (1001) docker     (127)   367947 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    20702 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    11351 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/rdns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9506 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/ssh_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    31276 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/stack_script.py
--rw-r--r--   0 runner    (1001) docker     (127)    17518 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/token.py
--rw-r--r--   0 runner    (1001) docker     (127)    41796 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    24339 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/volume.py
--rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/vpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    13121 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode/vpc_subnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-17 19:25:22.221087 pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-11-17 19:25:22.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2998 2023-11-17 19:25:22.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-17 19:25:22.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2023-11-17 19:25:22.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-17 19:25:22.000000 pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      679 2023-11-17 19:25:11.000000 pulumi_linode-4.9.0a1700248892/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-17 19:25:22.221087 pulumi_linode-4.9.0a1700248892/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:14:02.151434 pulumi_linode-4.9.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2023-12-04 18:14:02.151434 pulumi_linode-4.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:14:02.147433 pulumi_linode-4.9.1/pulumi_linode/
+-rw-r--r--   0 runner    (1001) docker     (127)     7725 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   290134 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8081 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16532 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/account_settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:14:02.151434 pulumi_linode-4.9.1/pulumi_linode/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/config/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3426 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12684 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/database_access_controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44527 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50181 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40821 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33929 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35787 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13586 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/firewall_device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8323 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4954 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_account_login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4827 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_account_logins.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5353 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_account_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8865 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_database_backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_database_engines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15050 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_database_mysql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7983 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_database_mysql_backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16312 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_database_postgresql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6046 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_databases.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9608 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8745 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_domain_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3780 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_domain_zonefile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8313 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_firewalls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8365 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_image.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7884 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4124 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_instance_backups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3942 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_instance_networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7625 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_instance_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6616 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_instance_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6734 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_instances.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5950 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6106 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4729 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_linode_object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7224 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_lke_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7190 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_networking_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7111 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13058 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6893 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_nodebalancers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4871 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_object_storage_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8249 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5317 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_region.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_regions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6285 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_sshkeys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9856 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8084 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_stack_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14159 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6380 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_vlans.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6953 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5478 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_volumes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4684 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5617 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_vpc_subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5404 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_vpc_subnets.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/get_vpcs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34342 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)   117154 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33871 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/instance_disk.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20651 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/instance_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8713 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/instance_shared_ips.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15042 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/ipv6_range.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26054 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/lke_cluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24174 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/node_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    57023 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/node_balancer_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21278 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/node_balancer_node.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31602 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/object_storage_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14371 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/object_storage_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52151 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/object_storage_object.py
+-rw-r--r--   0 runner    (1001) docker     (127)   367947 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20702 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    11351 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/rdns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9506 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/ssh_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    31276 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/stack_script.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17518 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41796 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24339 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/volume.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11797 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/vpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13121 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pulumi_linode/vpc_subnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-04 18:14:02.151434 pulumi_linode-4.9.1/pulumi_linode.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2817 2023-12-04 18:14:02.000000 pulumi_linode-4.9.1/pulumi_linode.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3032 2023-12-04 18:14:02.000000 pulumi_linode-4.9.1/pulumi_linode.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-04 18:14:02.000000 pulumi_linode-4.9.1/pulumi_linode.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2023-12-04 18:14:02.000000 pulumi_linode-4.9.1/pulumi_linode.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-04 18:14:02.000000 pulumi_linode-4.9.1/pulumi_linode.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2023-12-04 18:13:49.000000 pulumi_linode-4.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-04 18:14:02.151434 pulumi_linode-4.9.1/setup.cfg
```

### Comparing `pulumi_linode-4.9.0a1700248892/PKG-INFO` & `pulumi_linode-4.9.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_linode
-Version: 4.9.0a1700248892
+Version: 4.9.1
 Summary: A Pulumi package for creating and managing linode cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi,linode
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_linode-4.9.0a1700248892/README.md` & `pulumi_linode-4.9.1/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/__init__.py` & `pulumi_linode-4.9.1/pulumi_linode/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/_inputs.py` & `pulumi_linode-4.9.1/pulumi_linode/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/_utilities.py` & `pulumi_linode-4.9.1/pulumi_linode/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/account_settings.py` & `pulumi_linode-4.9.1/pulumi_linode/account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/config/vars.py` & `pulumi_linode-4.9.1/pulumi_linode/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/database_access_controls.py` & `pulumi_linode-4.9.1/pulumi_linode/database_access_controls.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/database_mysql.py` & `pulumi_linode-4.9.1/pulumi_linode/database_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/database_postgresql.py` & `pulumi_linode-4.9.1/pulumi_linode/database_postgresql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/domain.py` & `pulumi_linode-4.9.1/pulumi_linode/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/domain_record.py` & `pulumi_linode-4.9.1/pulumi_linode/domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/firewall.py` & `pulumi_linode-4.9.1/pulumi_linode/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/firewall_device.py` & `pulumi_linode-4.9.1/pulumi_linode/firewall_device.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account.py` & `pulumi_linode-4.9.1/pulumi_linode/get_account.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account_login.py` & `pulumi_linode-4.9.1/pulumi_linode/get_account_login.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account_logins.py` & `pulumi_linode-4.9.1/pulumi_linode/get_account_logins.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_account_settings.py` & `pulumi_linode-4.9.1/pulumi_linode/get_account_settings.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_backups.py` & `pulumi_linode-4.9.1/pulumi_linode/get_database_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_engines.py` & `pulumi_linode-4.9.1/pulumi_linode/get_database_engines.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_mysql.py` & `pulumi_linode-4.9.1/pulumi_linode/get_database_mysql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_mysql_backups.py` & `pulumi_linode-4.9.1/pulumi_linode/get_database_mysql_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_database_postgresql.py` & `pulumi_linode-4.9.1/pulumi_linode/get_database_postgresql.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_databases.py` & `pulumi_linode-4.9.1/pulumi_linode/get_databases.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_domain.py` & `pulumi_linode-4.9.1/pulumi_linode/get_domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_domain_record.py` & `pulumi_linode-4.9.1/pulumi_linode/get_domain_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_domain_zonefile.py` & `pulumi_linode-4.9.1/pulumi_linode/get_domain_zonefile.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_firewall.py` & `pulumi_linode-4.9.1/pulumi_linode/get_firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_firewalls.py` & `pulumi_linode-4.9.1/pulumi_linode/get_firewalls.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_image.py` & `pulumi_linode-4.9.1/pulumi_linode/get_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_images.py` & `pulumi_linode-4.9.1/pulumi_linode/get_images.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_backups.py` & `pulumi_linode-4.9.1/pulumi_linode/get_instance_backups.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_networking.py` & `pulumi_linode-4.9.1/pulumi_linode/get_instance_networking.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_type.py` & `pulumi_linode-4.9.1/pulumi_linode/get_instance_type.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instance_types.py` & `pulumi_linode-4.9.1/pulumi_linode/get_instance_types.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_instances.py` & `pulumi_linode-4.9.1/pulumi_linode/get_instances.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_ipv6_range.py` & `pulumi_linode-4.9.1/pulumi_linode/get_ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_kernel.py` & `pulumi_linode-4.9.1/pulumi_linode/get_kernel.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_kernels.py` & `pulumi_linode-4.9.1/pulumi_linode/get_kernels.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_linode_object_storage_bucket.py` & `pulumi_linode-4.9.1/pulumi_linode/get_linode_object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_lke_cluster.py` & `pulumi_linode-4.9.1/pulumi_linode/get_lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_lke_versions.py` & `pulumi_linode-4.9.1/pulumi_linode/get_lke_versions.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_networking_ip.py` & `pulumi_linode-4.9.1/pulumi_linode/get_networking_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_node_balancer.py` & `pulumi_linode-4.9.1/pulumi_linode/get_node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_node_balancer_config.py` & `pulumi_linode-4.9.1/pulumi_linode/get_node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_node_balancer_node.py` & `pulumi_linode-4.9.1/pulumi_linode/get_node_balancer_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_nodebalancers.py` & `pulumi_linode-4.9.1/pulumi_linode/get_nodebalancers.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_object_storage_cluster.py` & `pulumi_linode-4.9.1/pulumi_linode/get_object_storage_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_profile.py` & `pulumi_linode-4.9.1/pulumi_linode/get_profile.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_region.py` & `pulumi_linode-4.9.1/pulumi_linode/get_region.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_regions.py` & `pulumi_linode-4.9.1/pulumi_linode/get_regions.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_ssh_key.py` & `pulumi_linode-4.9.1/pulumi_linode/get_ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_sshkeys.py` & `pulumi_linode-4.9.1/pulumi_linode/get_sshkeys.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_stack_script.py` & `pulumi_linode-4.9.1/pulumi_linode/get_stack_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_stack_scripts.py` & `pulumi_linode-4.9.1/pulumi_linode/get_stack_scripts.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_user.py` & `pulumi_linode-4.9.1/pulumi_linode/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_users.py` & `pulumi_linode-4.9.1/pulumi_linode/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vlans.py` & `pulumi_linode-4.9.1/pulumi_linode/get_vlans.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_volume.py` & `pulumi_linode-4.9.1/pulumi_linode/get_volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_volumes.py` & `pulumi_linode-4.9.1/pulumi_linode/get_volumes.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpc.py` & `pulumi_linode-4.9.1/pulumi_linode/get_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpc_subnet.py` & `pulumi_linode-4.9.1/pulumi_linode/get_vpc_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpc_subnets.py` & `pulumi_linode-4.9.1/pulumi_linode/get_vpc_subnets.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/get_vpcs.py` & `pulumi_linode-4.9.1/pulumi_linode/get_vpcs.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/image.py` & `pulumi_linode-4.9.1/pulumi_linode/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/instance.py` & `pulumi_linode-4.9.1/pulumi_linode/instance.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/instance_disk.py` & `pulumi_linode-4.9.1/pulumi_linode/instance_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/instance_ip.py` & `pulumi_linode-4.9.1/pulumi_linode/instance_ip.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/instance_shared_ips.py` & `pulumi_linode-4.9.1/pulumi_linode/instance_shared_ips.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/ipv6_range.py` & `pulumi_linode-4.9.1/pulumi_linode/ipv6_range.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/lke_cluster.py` & `pulumi_linode-4.9.1/pulumi_linode/lke_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/node_balancer.py` & `pulumi_linode-4.9.1/pulumi_linode/node_balancer.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/node_balancer_config.py` & `pulumi_linode-4.9.1/pulumi_linode/node_balancer_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/node_balancer_node.py` & `pulumi_linode-4.9.1/pulumi_linode/node_balancer_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/object_storage_bucket.py` & `pulumi_linode-4.9.1/pulumi_linode/object_storage_bucket.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/object_storage_key.py` & `pulumi_linode-4.9.1/pulumi_linode/object_storage_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/object_storage_object.py` & `pulumi_linode-4.9.1/pulumi_linode/object_storage_object.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/outputs.py` & `pulumi_linode-4.9.1/pulumi_linode/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/provider.py` & `pulumi_linode-4.9.1/pulumi_linode/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/rdns.py` & `pulumi_linode-4.9.1/pulumi_linode/rdns.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/ssh_key.py` & `pulumi_linode-4.9.1/pulumi_linode/ssh_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/stack_script.py` & `pulumi_linode-4.9.1/pulumi_linode/stack_script.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/token.py` & `pulumi_linode-4.9.1/pulumi_linode/token.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/user.py` & `pulumi_linode-4.9.1/pulumi_linode/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -510,15 +510,15 @@
                 permissions="read_write",
             )],
             restricted=True,
             username="cooluser123")
         ```
         ## Global Grants
 
-        * `account-access` - (optional) The level of access this User has to Account-level actions, like billing information. (`read_only`, `read_write`)
+        * `account_access` - (optional) The level of access this User has to Account-level actions, like billing information. (`read_only`, `read_write`)
 
         * `add_domains` - (optional) If true, this User may add Domains.
 
         * `add_databases` - (optional) If true, this User may add Databases.
 
         * `add_firewalls` - (optional) If true, this User may add Firewalls.
 
@@ -600,15 +600,15 @@
                 permissions="read_write",
             )],
             restricted=True,
             username="cooluser123")
         ```
         ## Global Grants
 
-        * `account-access` - (optional) The level of access this User has to Account-level actions, like billing information. (`read_only`, `read_write`)
+        * `account_access` - (optional) The level of access this User has to Account-level actions, like billing information. (`read_only`, `read_write`)
 
         * `add_domains` - (optional) If true, this User may add Domains.
 
         * `add_databases` - (optional) If true, this User may add Databases.
 
         * `add_firewalls` - (optional) If true, this User may add Firewalls.
```

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/volume.py` & `pulumi_linode-4.9.1/pulumi_linode/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/vpc.py` & `pulumi_linode-4.9.1/pulumi_linode/vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode/vpc_subnet.py` & `pulumi_linode-4.9.1/pulumi_linode/vpc_subnet.py`

 * *Files identical despite different names*

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/PKG-INFO` & `pulumi_linode-4.9.1/pulumi_linode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-linode
-Version: 4.9.0a1700248892
+Version: 4.9.1
 Summary: A Pulumi package for creating and managing linode cloud resources.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.io
 Project-URL: Repository, https://github.com/pulumi/pulumi-linode
 Keywords: pulumi,linode
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_linode-4.9.0a1700248892/pulumi_linode.egg-info/SOURCES.txt` & `pulumi_linode-4.9.1/pulumi_linode.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -88,8 +88,9 @@
 pulumi_linode/vpc_subnet.py
 pulumi_linode.egg-info/PKG-INFO
 pulumi_linode.egg-info/SOURCES.txt
 pulumi_linode.egg-info/dependency_links.txt
 pulumi_linode.egg-info/requires.txt
 pulumi_linode.egg-info/top_level.txt
 pulumi_linode/config/__init__.py
+pulumi_linode/config/__init__.pyi
 pulumi_linode/config/vars.py
```

