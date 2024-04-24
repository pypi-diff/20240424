# Comparing `tmp/napalm_s350-0.5.0.tar.gz` & `tmp/napalm_s350-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napalm_s350-0.5.0.tar", last modified: Tue Apr 23 07:07:54 2024, max compression
+gzip compressed data, was "napalm_s350-0.5.1.tar", last modified: Wed Apr 24 15:37:21 2024, max compression
```

## Comparing `napalm_s350-0.5.0.tar` & `napalm_s350-0.5.1.tar`

### file list

```diff
@@ -1,21 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7368 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350/
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24138 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/s350.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350/utils/textfsm_templates/
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/napalm_s350/utils/textfsm_templates/hosts.tpl
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/napalm_s350.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8435 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-23 07:07:54.000000 napalm_s350-0.5.0/napalm_s350.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-23 07:07:54.305477 napalm_s350-0.5.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-23 07:07:46.000000 napalm_s350-0.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:37:21.448786 napalm_s350-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-24 15:37:12.000000 napalm_s350-0.5.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 15:37:12.000000 napalm_s350-0.5.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-04-24 15:37:21.448786 napalm_s350-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8231 2024-04-24 15:37:12.000000 napalm_s350-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:37:21.448786 napalm_s350-0.5.1/napalm_s350/
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 15:37:12.000000 napalm_s350-0.5.1/napalm_s350/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24577 2024-04-24 15:37:12.000000 napalm_s350-0.5.1/napalm_s350/s350.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:37:21.448786 napalm_s350-0.5.1/napalm_s350.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9298 2024-04-24 15:37:21.000000 napalm_s350-0.5.1/napalm_s350.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 15:37:21.000000 napalm_s350-0.5.1/napalm_s350.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:37:21.000000 napalm_s350-0.5.1/napalm_s350.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 15:37:21.000000 napalm_s350-0.5.1/napalm_s350.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 15:37:21.000000 napalm_s350-0.5.1/napalm_s350.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 15:37:12.000000 napalm_s350-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-24 15:37:21.448786 napalm_s350-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-04-24 15:37:12.000000 napalm_s350-0.5.1/setup.py
```

### Comparing `napalm_s350-0.5.0/LICENSE` & `napalm_s350-0.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `napalm_s350-0.5.0/PKG-INFO` & `napalm_s350-0.5.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-s350
-Version: 0.5.0
+Version: 0.5.1
 Summary: NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)
 Home-page: https://github.com/napalm-automation-community/napalm-s350
 Author: Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher
 Author-email: j@jasper.la, qaxi@seznam.cz, mail@phill93.de
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 License-File: LICENSE
 Requires-Dist: napalm>=4.0.0
 Requires-Dist: netmiko>=4.0.0
 Requires-Dist: netaddr>=1.2.1
 
 # Napalm-s350
 
-NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
+NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG250, SG3xx, SG5xx, CBS35x).
 
 ## Status
 
 Master: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
 Develop: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=develop)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
@@ -67,75 +67,91 @@
 Debug
 ```bash
 napalm --user USER --password PASSWORD --vendor s350 --debug HOSTNAME
 ```
 
 ## Supported devices
 
-This driver initially targets the Cisco SG350 device though other, similar, devices may
+This driver initially targets the Cisco SG350 device though other, similar, devices are
 be supported.
 
-| function                  | SG300 | SG500 | SG350 | SG550 | stack SG500 | stack SG550 | CBS350 |
-| :---                      | :---: | :---: | :---: | :---: | :---:       | :---:       | :---:  |
-| **Send commands**                                                                              |
-| cli                       | x     | x     | x     | x     | x           | x           | x      |
-| **Config manipulation**                                                                        |
-|get_config                 | x     | x     | x     | x     |             |             | x      |
-|get_config (filtered)      | x     | x     | x     | x     |             |             | x      |
-|get_config (sanitized)     | x     | x     | x     | x     |             |             | x      |
-|load_merge_candidate       |       |       |       |       |             |             |        |
-|load_replace_candidate     |       |       |       |       |             |             |        |
-|compare_config             |       |       |       |       |             |             |        |
-|commit_config              |       |       |       |       |             |             |        |
-|confirm_commit             |       |       |       |       |             |             |        |
-|has_pending_commit         |       |       |       |       |             |             |        |
-|rollback                   |       |       |       |       |             |             |        |
-|discard_config             |       |       |       |       |             |             |        |
-|compliance_report          |       |       |       |       |             |             |        |
-|load_template              |       |       |       |       |             |             |        |
-| **Get information**                                                                            |
-|get_arp_table              | x     | x     | x     | x     |             |             | x      |
-|get_arp_table (with vrf)   | NS    | NS    | NS    | NS    |             |             | NS     |
-|get_bgp_config             |       |       |       |       |             |             |        |
-|get_bgp_neighbors          |       |       |       |       |             |             |        |
-|get_bgp_neighbors_detail   |       |       |       |       |             |             |        |
-|get_environment            |       |       |       |       |             |             |        |
-|get_facts                  | x     | x     | x     | x     |             |             | x      |
-|get_firewall_policies      |       |       |       |       |             |             |        |
-|get_interfaces             | x     | x     | x     | x     |             |             | x      |
-|get_interfaces_counters    |       |       |       |       |             |             |        |
-|get_interfaces_ip          | x 4   | x 4   | x 4   | x 4   |             |             | x 4    |
-|get_ipv6_neighbors_table   |       |       |       |       |             |             |        |
-|get_lldp_neighbors         | x     | x     | x     | x     |             |             | x      |
-|get_lldp_neighbors_detail  | x     | x     | x     | x     |             |             | x      |
-|get_mac_address_table      |       |       |       |       |             |             |        |
-|get_network_instances      |       |       |       |       |             |             |        |
-|get_ntp_peers              |       |       |       |       |             |             |        |
-|get_ntp_servers            | x     | x     | x     | x     |             |             | x      |
-|get_ntp_stats              |       |       |       |       |             |             |        |
-|get_optics                 |       |       |       |       |             |             |        |
-|get_probes_config          |       |       |       |       |             |             |        |
-|get_probes_results         |       |       |       |       |             |             |        |
-|get_route_to               |       |       |       |       |             |             |        |
-|get_snmp_information       |       |       |       |       |             |             |        |
-|get_users                  |       |       |       |       |             |             |        |
-|get_vlans                  | x     | x     | x     | x     |             |             | x      |
-| **Other actions**                                                                              |
-|is_alive                   |       |       |       |       |             |             |        |
-|ping                       |       |       |       |       |             |             |        |
-|traceroute                 |       |       |       |       |             |             |        |
+| function                  | SG250 | SG300 | SG500 | SG350 | SG550 | stack SG500 | stack SG550 | CBS350 |
+| :---                      | :---: | :---: | :---: | :---: | :---: | :---:       | :---:       | :---:  |
+| **Send commands**                                                                                      |
+| cli                       | x     | x     | x     | x     | x     | x           | x           | x      |
+| **Config manipulation**                                                                                |
+|get_config                 | x     | x     | x     | x     | x     |             |             | x      |
+|get_config (filtered)      | x     | x     | x     | x     | x     |             |             | x      |
+|get_config (sanitized)     | x     | x     | x     | x     | x     |             |             | x      |
+|load_merge_candidate       |       |       |       |       |       |             |             |        |
+|load_replace_candidate     |       |       |       |       |       |             |             |        |
+|compare_config             |       |       |       |       |       |             |             |        |
+|commit_config              |       |       |       |       |       |             |             |        |
+|confirm_commit             |       |       |       |       |       |             |             |        |
+|has_pending_commit         |       |       |       |       |       |             |             |        |
+|rollback                   |       |       |       |       |       |             |             |        |
+|discard_config             |       |       |       |       |       |             |             |        |
+|compliance_report          |       |       |       |       |       |             |             |        |
+|load_template              |       |       |       |       |       |             |             |        |
+| **Get information**                                                                                    |
+|get_arp_table              | x     | x     | x     | x     | x     |             |             | x      |
+|get_arp_table (with vrf)   | NS    | NS    | NS    | NS    | NS    |             |             | NS     |
+|get_bgp_config             |       |       |       |       |       |             |             |        |
+|get_bgp_neighbors          |       |       |       |       |       |             |             |        |
+|get_bgp_neighbors_detail   |       |       |       |       |       |             |             |        |
+|get_environment            |       |       |       |       |       |             |             |        |
+|get_facts                  | x     | x     | x     | x     | x     |             |             | x      |
+|get_firewall_policies      |       |       |       |       |       |             |             |        |
+|get_interfaces             | x     | x     | x     | x     | x     |             |             | x      |
+|get_interfaces_counters    |       |       |       |       |       |             |             |        |
+|get_interfaces_ip          | x 4   | x 4   | x 4   | x 4   | x 4   |             |             | x 4    |
+|get_ipv6_neighbors_table   |       |       |       |       |       |             |             |        |
+|get_lldp_neighbors         | x     | x     | x     | x     | x     |             |             | x      |
+|get_lldp_neighbors_detail  | x     | x     | x     | x     | x     |             |             | x      |
+|get_mac_address_table      |       |       |       |       |       |             |             |        |
+|get_network_instances      |       |       |       |       |       |             |             |        |
+|get_ntp_peers              |       |       |       |       |       |             |             |        |
+|get_ntp_servers            | x     | x     | x     | x     | x     |             |             | x      |
+|get_ntp_stats              |       |       |       |       |       |             |             |        |
+|get_optics                 |       |       |       |       |       |             |             |        |
+|get_probes_config          |       |       |       |       |       |             |             |        |
+|get_probes_results         |       |       |       |       |       |             |             |        |
+|get_route_to               |       |       |       |       |       |             |             |        |
+|get_snmp_information       |       |       |       |       |       |             |             |        |
+|get_users                  |       |       |       |       |       |             |             |        |
+|get_vlans                  | x     | x     | x     | x     | x     |             |             | x      |
+| **Other actions**                                                                                      |
+|is_alive                   | x     | x     | x     | x     | x     | x           | x           | x      |
+|ping                       |       |       |       |       |       |             |             |        |
+|traceroute                 |       |       |       |       |       |             |             |        |
 
 
 NS - not supported - devices do not have support for that feature
 4  - IPv4 only ...
 
 ## Want to add new device support?
 
 To be sure we can support new device we use test files.
 
+### Fetch command output tool
+There is tool for getting necessary infromatin form running switch
+```
+cd test/unit
+
+# DEVICE_TYPE as PID: in "show inventory" output
+# INTERFACE an inteface
+# LLDP_INTERFACE inteface for getting LLDP inforation
+./fetch_command_output.sh -u USER -p PASSWORD -t DEVICE_TYPE -v s350 \
+    -d SWITCH_IP_or_FQDN -i INTERFACE -l LLDP_INTERFACE 
+```
+
+Output files from that tool are in "test/unit/command_output/$DEVICE_TYPE"
+
+### By hand
+
 We need text output of those commands, to add new device:
 ```
 show arp
 show startup-config
 show version
 show system
 show inventory
```

### Comparing `napalm_s350-0.5.0/README.md` & `napalm_s350-0.5.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # Napalm-s350
 
-NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
+NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG250, SG3xx, SG5xx, CBS35x).
 
 ## Status
 
 Master: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
 Develop: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=develop)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
@@ -41,75 +41,91 @@
 Debug
 ```bash
 napalm --user USER --password PASSWORD --vendor s350 --debug HOSTNAME
 ```
 
 ## Supported devices
 
-This driver initially targets the Cisco SG350 device though other, similar, devices may
+This driver initially targets the Cisco SG350 device though other, similar, devices are
 be supported.
 
-| function                  | SG300 | SG500 | SG350 | SG550 | stack SG500 | stack SG550 | CBS350 |
-| :---                      | :---: | :---: | :---: | :---: | :---:       | :---:       | :---:  |
-| **Send commands**                                                                              |
-| cli                       | x     | x     | x     | x     | x           | x           | x      |
-| **Config manipulation**                                                                        |
-|get_config                 | x     | x     | x     | x     |             |             | x      |
-|get_config (filtered)      | x     | x     | x     | x     |             |             | x      |
-|get_config (sanitized)     | x     | x     | x     | x     |             |             | x      |
-|load_merge_candidate       |       |       |       |       |             |             |        |
-|load_replace_candidate     |       |       |       |       |             |             |        |
-|compare_config             |       |       |       |       |             |             |        |
-|commit_config              |       |       |       |       |             |             |        |
-|confirm_commit             |       |       |       |       |             |             |        |
-|has_pending_commit         |       |       |       |       |             |             |        |
-|rollback                   |       |       |       |       |             |             |        |
-|discard_config             |       |       |       |       |             |             |        |
-|compliance_report          |       |       |       |       |             |             |        |
-|load_template              |       |       |       |       |             |             |        |
-| **Get information**                                                                            |
-|get_arp_table              | x     | x     | x     | x     |             |             | x      |
-|get_arp_table (with vrf)   | NS    | NS    | NS    | NS    |             |             | NS     |
-|get_bgp_config             |       |       |       |       |             |             |        |
-|get_bgp_neighbors          |       |       |       |       |             |             |        |
-|get_bgp_neighbors_detail   |       |       |       |       |             |             |        |
-|get_environment            |       |       |       |       |             |             |        |
-|get_facts                  | x     | x     | x     | x     |             |             | x      |
-|get_firewall_policies      |       |       |       |       |             |             |        |
-|get_interfaces             | x     | x     | x     | x     |             |             | x      |
-|get_interfaces_counters    |       |       |       |       |             |             |        |
-|get_interfaces_ip          | x 4   | x 4   | x 4   | x 4   |             |             | x 4    |
-|get_ipv6_neighbors_table   |       |       |       |       |             |             |        |
-|get_lldp_neighbors         | x     | x     | x     | x     |             |             | x      |
-|get_lldp_neighbors_detail  | x     | x     | x     | x     |             |             | x      |
-|get_mac_address_table      |       |       |       |       |             |             |        |
-|get_network_instances      |       |       |       |       |             |             |        |
-|get_ntp_peers              |       |       |       |       |             |             |        |
-|get_ntp_servers            | x     | x     | x     | x     |             |             | x      |
-|get_ntp_stats              |       |       |       |       |             |             |        |
-|get_optics                 |       |       |       |       |             |             |        |
-|get_probes_config          |       |       |       |       |             |             |        |
-|get_probes_results         |       |       |       |       |             |             |        |
-|get_route_to               |       |       |       |       |             |             |        |
-|get_snmp_information       |       |       |       |       |             |             |        |
-|get_users                  |       |       |       |       |             |             |        |
-|get_vlans                  | x     | x     | x     | x     |             |             | x      |
-| **Other actions**                                                                              |
-|is_alive                   |       |       |       |       |             |             |        |
-|ping                       |       |       |       |       |             |             |        |
-|traceroute                 |       |       |       |       |             |             |        |
+| function                  | SG250 | SG300 | SG500 | SG350 | SG550 | stack SG500 | stack SG550 | CBS350 |
+| :---                      | :---: | :---: | :---: | :---: | :---: | :---:       | :---:       | :---:  |
+| **Send commands**                                                                                      |
+| cli                       | x     | x     | x     | x     | x     | x           | x           | x      |
+| **Config manipulation**                                                                                |
+|get_config                 | x     | x     | x     | x     | x     |             |             | x      |
+|get_config (filtered)      | x     | x     | x     | x     | x     |             |             | x      |
+|get_config (sanitized)     | x     | x     | x     | x     | x     |             |             | x      |
+|load_merge_candidate       |       |       |       |       |       |             |             |        |
+|load_replace_candidate     |       |       |       |       |       |             |             |        |
+|compare_config             |       |       |       |       |       |             |             |        |
+|commit_config              |       |       |       |       |       |             |             |        |
+|confirm_commit             |       |       |       |       |       |             |             |        |
+|has_pending_commit         |       |       |       |       |       |             |             |        |
+|rollback                   |       |       |       |       |       |             |             |        |
+|discard_config             |       |       |       |       |       |             |             |        |
+|compliance_report          |       |       |       |       |       |             |             |        |
+|load_template              |       |       |       |       |       |             |             |        |
+| **Get information**                                                                                    |
+|get_arp_table              | x     | x     | x     | x     | x     |             |             | x      |
+|get_arp_table (with vrf)   | NS    | NS    | NS    | NS    | NS    |             |             | NS     |
+|get_bgp_config             |       |       |       |       |       |             |             |        |
+|get_bgp_neighbors          |       |       |       |       |       |             |             |        |
+|get_bgp_neighbors_detail   |       |       |       |       |       |             |             |        |
+|get_environment            |       |       |       |       |       |             |             |        |
+|get_facts                  | x     | x     | x     | x     | x     |             |             | x      |
+|get_firewall_policies      |       |       |       |       |       |             |             |        |
+|get_interfaces             | x     | x     | x     | x     | x     |             |             | x      |
+|get_interfaces_counters    |       |       |       |       |       |             |             |        |
+|get_interfaces_ip          | x 4   | x 4   | x 4   | x 4   | x 4   |             |             | x 4    |
+|get_ipv6_neighbors_table   |       |       |       |       |       |             |             |        |
+|get_lldp_neighbors         | x     | x     | x     | x     | x     |             |             | x      |
+|get_lldp_neighbors_detail  | x     | x     | x     | x     | x     |             |             | x      |
+|get_mac_address_table      |       |       |       |       |       |             |             |        |
+|get_network_instances      |       |       |       |       |       |             |             |        |
+|get_ntp_peers              |       |       |       |       |       |             |             |        |
+|get_ntp_servers            | x     | x     | x     | x     | x     |             |             | x      |
+|get_ntp_stats              |       |       |       |       |       |             |             |        |
+|get_optics                 |       |       |       |       |       |             |             |        |
+|get_probes_config          |       |       |       |       |       |             |             |        |
+|get_probes_results         |       |       |       |       |       |             |             |        |
+|get_route_to               |       |       |       |       |       |             |             |        |
+|get_snmp_information       |       |       |       |       |       |             |             |        |
+|get_users                  |       |       |       |       |       |             |             |        |
+|get_vlans                  | x     | x     | x     | x     | x     |             |             | x      |
+| **Other actions**                                                                                      |
+|is_alive                   | x     | x     | x     | x     | x     | x           | x           | x      |
+|ping                       |       |       |       |       |       |             |             |        |
+|traceroute                 |       |       |       |       |       |             |             |        |
 
 
 NS - not supported - devices do not have support for that feature
 4  - IPv4 only ...
 
 ## Want to add new device support?
 
 To be sure we can support new device we use test files.
 
+### Fetch command output tool
+There is tool for getting necessary infromatin form running switch
+```
+cd test/unit
+
+# DEVICE_TYPE as PID: in "show inventory" output
+# INTERFACE an inteface
+# LLDP_INTERFACE inteface for getting LLDP inforation
+./fetch_command_output.sh -u USER -p PASSWORD -t DEVICE_TYPE -v s350 \
+    -d SWITCH_IP_or_FQDN -i INTERFACE -l LLDP_INTERFACE 
+```
+
+Output files from that tool are in "test/unit/command_output/$DEVICE_TYPE"
+
+### By hand
+
 We need text output of those commands, to add new device:
 ```
 show arp
 show startup-config
 show version
 show system
 show inventory
```

### Comparing `napalm_s350-0.5.0/napalm_s350/__init__.py` & `napalm_s350-0.5.1/napalm_s350/__init__.py`

 * *Files identical despite different names*

### Comparing `napalm_s350-0.5.0/napalm_s350/s350.py` & `napalm_s350-0.5.1/napalm_s350/s350.py`

 * *Files 3% similar despite different names*

```diff
@@ -96,19 +96,19 @@
         """Wrapper for self.device.send.command().
 
         If command is a list will iterate through commands until valid command.
         """
         try:
             if isinstance(command, list):
                 for cmd in command:
-                    output = self.device.send_command(cmd)
+                    output = self.device.send_command(cmd, read_timeout=self.timeout)
                     if "% Invalid" not in output:
                         break
             else:
-                output = self.device.send_command(command)
+                output = self.device.send_command(command, read_timeout=self.timeout)
             return output.strip()
         except (socket.error, EOFError) as e:
             raise ConnectionClosedException(str(e))
 
     def _parse_uptime(self, uptime_str):
         """Parse an uptime string into number of seconds"""
         uptime_str = uptime_str.strip()
@@ -241,21 +241,36 @@
             )
 
         # uptime
         uptime_str = self._get_facts_uptime(show_sys)
         uptime = self._parse_uptime(uptime_str)
 
         # serial_number and model
+        # take first device
         inventory = self._get_facts_parse_inventory(show_inv)["1"]
         serial_number = inventory["sn"]
         model = inventory["pid"]
 
         # fqdn
-        domainname = napalm.base.helpers.textfsm_extractor(self, "hosts", show_hosts)[0]
-        domainname = domainname["domain_name"]
+        # take first domain name
+        domainname = "Unknown"
+        atDTh = False
+        atDT = False
+        for line in show_hosts.splitlines():
+            if line.startswith("Default Domain Table"):
+                atDTh = True
+                continue
+            if atDTh and line.startswith("--------"):
+                atDT = True
+                continue
+            if atDT:
+                fields = line.split(" ")
+                domainname = fields[0]
+                break
+
         if domainname == "Domain":
             domainname = "Unknown"
         if domainname != "Unknown" and hostname != "Unknown":
             fqdn = "{0}.{1}".format(hostname, domainname)
 
         # interface_list
```

### Comparing `napalm_s350-0.5.0/napalm_s350.egg-info/PKG-INFO` & `napalm_s350-0.5.1/napalm_s350.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napalm-s350
-Version: 0.5.0
+Version: 0.5.1
 Summary: NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)
 Home-page: https://github.com/napalm-automation-community/napalm-s350
 Author: Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher
 Author-email: j@jasper.la, qaxi@seznam.cz, mail@phill93.de
 License: Apache 2.0
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: Apache Software License
@@ -22,15 +22,15 @@
 License-File: LICENSE
 Requires-Dist: napalm>=4.0.0
 Requires-Dist: netmiko>=4.0.0
 Requires-Dist: netaddr>=1.2.1
 
 # Napalm-s350
 
-NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx, CBS35x).
+NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG250, SG3xx, SG5xx, CBS35x).
 
 ## Status
 
 Master: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=master)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
 Develop: [![Thorough Test](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml/badge.svg?branch=develop)](https://github.com/napalm-automation-community/napalm-s350/actions/workflows/ThoroughTest.yml)
 
@@ -67,75 +67,91 @@
 Debug
 ```bash
 napalm --user USER --password PASSWORD --vendor s350 --debug HOSTNAME
 ```
 
 ## Supported devices
 
-This driver initially targets the Cisco SG350 device though other, similar, devices may
+This driver initially targets the Cisco SG350 device though other, similar, devices are
 be supported.
 
-| function                  | SG300 | SG500 | SG350 | SG550 | stack SG500 | stack SG550 | CBS350 |
-| :---                      | :---: | :---: | :---: | :---: | :---:       | :---:       | :---:  |
-| **Send commands**                                                                              |
-| cli                       | x     | x     | x     | x     | x           | x           | x      |
-| **Config manipulation**                                                                        |
-|get_config                 | x     | x     | x     | x     |             |             | x      |
-|get_config (filtered)      | x     | x     | x     | x     |             |             | x      |
-|get_config (sanitized)     | x     | x     | x     | x     |             |             | x      |
-|load_merge_candidate       |       |       |       |       |             |             |        |
-|load_replace_candidate     |       |       |       |       |             |             |        |
-|compare_config             |       |       |       |       |             |             |        |
-|commit_config              |       |       |       |       |             |             |        |
-|confirm_commit             |       |       |       |       |             |             |        |
-|has_pending_commit         |       |       |       |       |             |             |        |
-|rollback                   |       |       |       |       |             |             |        |
-|discard_config             |       |       |       |       |             |             |        |
-|compliance_report          |       |       |       |       |             |             |        |
-|load_template              |       |       |       |       |             |             |        |
-| **Get information**                                                                            |
-|get_arp_table              | x     | x     | x     | x     |             |             | x      |
-|get_arp_table (with vrf)   | NS    | NS    | NS    | NS    |             |             | NS     |
-|get_bgp_config             |       |       |       |       |             |             |        |
-|get_bgp_neighbors          |       |       |       |       |             |             |        |
-|get_bgp_neighbors_detail   |       |       |       |       |             |             |        |
-|get_environment            |       |       |       |       |             |             |        |
-|get_facts                  | x     | x     | x     | x     |             |             | x      |
-|get_firewall_policies      |       |       |       |       |             |             |        |
-|get_interfaces             | x     | x     | x     | x     |             |             | x      |
-|get_interfaces_counters    |       |       |       |       |             |             |        |
-|get_interfaces_ip          | x 4   | x 4   | x 4   | x 4   |             |             | x 4    |
-|get_ipv6_neighbors_table   |       |       |       |       |             |             |        |
-|get_lldp_neighbors         | x     | x     | x     | x     |             |             | x      |
-|get_lldp_neighbors_detail  | x     | x     | x     | x     |             |             | x      |
-|get_mac_address_table      |       |       |       |       |             |             |        |
-|get_network_instances      |       |       |       |       |             |             |        |
-|get_ntp_peers              |       |       |       |       |             |             |        |
-|get_ntp_servers            | x     | x     | x     | x     |             |             | x      |
-|get_ntp_stats              |       |       |       |       |             |             |        |
-|get_optics                 |       |       |       |       |             |             |        |
-|get_probes_config          |       |       |       |       |             |             |        |
-|get_probes_results         |       |       |       |       |             |             |        |
-|get_route_to               |       |       |       |       |             |             |        |
-|get_snmp_information       |       |       |       |       |             |             |        |
-|get_users                  |       |       |       |       |             |             |        |
-|get_vlans                  | x     | x     | x     | x     |             |             | x      |
-| **Other actions**                                                                              |
-|is_alive                   |       |       |       |       |             |             |        |
-|ping                       |       |       |       |       |             |             |        |
-|traceroute                 |       |       |       |       |             |             |        |
+| function                  | SG250 | SG300 | SG500 | SG350 | SG550 | stack SG500 | stack SG550 | CBS350 |
+| :---                      | :---: | :---: | :---: | :---: | :---: | :---:       | :---:       | :---:  |
+| **Send commands**                                                                                      |
+| cli                       | x     | x     | x     | x     | x     | x           | x           | x      |
+| **Config manipulation**                                                                                |
+|get_config                 | x     | x     | x     | x     | x     |             |             | x      |
+|get_config (filtered)      | x     | x     | x     | x     | x     |             |             | x      |
+|get_config (sanitized)     | x     | x     | x     | x     | x     |             |             | x      |
+|load_merge_candidate       |       |       |       |       |       |             |             |        |
+|load_replace_candidate     |       |       |       |       |       |             |             |        |
+|compare_config             |       |       |       |       |       |             |             |        |
+|commit_config              |       |       |       |       |       |             |             |        |
+|confirm_commit             |       |       |       |       |       |             |             |        |
+|has_pending_commit         |       |       |       |       |       |             |             |        |
+|rollback                   |       |       |       |       |       |             |             |        |
+|discard_config             |       |       |       |       |       |             |             |        |
+|compliance_report          |       |       |       |       |       |             |             |        |
+|load_template              |       |       |       |       |       |             |             |        |
+| **Get information**                                                                                    |
+|get_arp_table              | x     | x     | x     | x     | x     |             |             | x      |
+|get_arp_table (with vrf)   | NS    | NS    | NS    | NS    | NS    |             |             | NS     |
+|get_bgp_config             |       |       |       |       |       |             |             |        |
+|get_bgp_neighbors          |       |       |       |       |       |             |             |        |
+|get_bgp_neighbors_detail   |       |       |       |       |       |             |             |        |
+|get_environment            |       |       |       |       |       |             |             |        |
+|get_facts                  | x     | x     | x     | x     | x     |             |             | x      |
+|get_firewall_policies      |       |       |       |       |       |             |             |        |
+|get_interfaces             | x     | x     | x     | x     | x     |             |             | x      |
+|get_interfaces_counters    |       |       |       |       |       |             |             |        |
+|get_interfaces_ip          | x 4   | x 4   | x 4   | x 4   | x 4   |             |             | x 4    |
+|get_ipv6_neighbors_table   |       |       |       |       |       |             |             |        |
+|get_lldp_neighbors         | x     | x     | x     | x     | x     |             |             | x      |
+|get_lldp_neighbors_detail  | x     | x     | x     | x     | x     |             |             | x      |
+|get_mac_address_table      |       |       |       |       |       |             |             |        |
+|get_network_instances      |       |       |       |       |       |             |             |        |
+|get_ntp_peers              |       |       |       |       |       |             |             |        |
+|get_ntp_servers            | x     | x     | x     | x     | x     |             |             | x      |
+|get_ntp_stats              |       |       |       |       |       |             |             |        |
+|get_optics                 |       |       |       |       |       |             |             |        |
+|get_probes_config          |       |       |       |       |       |             |             |        |
+|get_probes_results         |       |       |       |       |       |             |             |        |
+|get_route_to               |       |       |       |       |       |             |             |        |
+|get_snmp_information       |       |       |       |       |       |             |             |        |
+|get_users                  |       |       |       |       |       |             |             |        |
+|get_vlans                  | x     | x     | x     | x     | x     |             |             | x      |
+| **Other actions**                                                                                      |
+|is_alive                   | x     | x     | x     | x     | x     | x           | x           | x      |
+|ping                       |       |       |       |       |       |             |             |        |
+|traceroute                 |       |       |       |       |       |             |             |        |
 
 
 NS - not supported - devices do not have support for that feature
 4  - IPv4 only ...
 
 ## Want to add new device support?
 
 To be sure we can support new device we use test files.
 
+### Fetch command output tool
+There is tool for getting necessary infromatin form running switch
+```
+cd test/unit
+
+# DEVICE_TYPE as PID: in "show inventory" output
+# INTERFACE an inteface
+# LLDP_INTERFACE inteface for getting LLDP inforation
+./fetch_command_output.sh -u USER -p PASSWORD -t DEVICE_TYPE -v s350 \
+    -d SWITCH_IP_or_FQDN -i INTERFACE -l LLDP_INTERFACE 
+```
+
+Output files from that tool are in "test/unit/command_output/$DEVICE_TYPE"
+
+### By hand
+
 We need text output of those commands, to add new device:
 ```
 show arp
 show startup-config
 show version
 show system
 show inventory
```

### Comparing `napalm_s350-0.5.0/setup.py` & `napalm_s350-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     reqs = [r for r in fs.read().splitlines() if (len(r) > 0 and not r.startswith("#"))]
 
 with open("README.md", "r") as fs:
     long_description = fs.read()
 
 setup(
     name="napalm-s350",
-    version="0.5.0",
+    version="0.5.1",
     packages=find_packages(exclude=("test*",)),
     author="Jasper Lievisse Adriaanse, Petr Klíma, Daniel Bacher",
     author_email="j@jasper.la, qaxi@seznam.cz, mail@phill93.de",
     description="NAPALM driver for Cisco SMB switches (SF3xx, SF5xx, SG3xx, SG5xx)",
     license="Apache 2.0",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

