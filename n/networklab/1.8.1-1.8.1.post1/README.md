# Comparing `tmp/networklab-1.8.1.tar.gz` & `tmp/networklab-1.8.1.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "networklab-1.8.1.tar", last modified: Mon Apr  8 09:30:57 2024, max compression
+gzip compressed data, was "networklab-1.8.1.post1.tar", last modified: Wed Apr 24 08:33:48 2024, max compression
```

## Comparing `networklab-1.8.1.tar` & `networklab-1.8.1.post1.tar`

### file list

```diff
@@ -1,741 +1,741 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.480151 networklab-1.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-08 09:30:50.000000 networklab-1.8.1/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-08 09:30:50.000000 networklab-1.8.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-08 09:30:57.480151 networklab-1.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-08 09:30:50.000000 networklab-1.8.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-08 09:30:50.000000 networklab-1.8.1/netlab
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.364151 networklab-1.8.1/netsim/
--rwxr-xr-x   0 runner    (1001) docker     (127)      420 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.364151 networklab-1.8.1/netsim/ansible/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/collect-configs.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/create-config.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/display-neighbors.ansible
--rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/initial-config.ansible
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/reload-config.ansible
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.368151 networklab-1.8.1/netsim/ansible/tasks/
--rw-r--r--   0 runner    (1001) docker     (127)      975 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/create-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      451 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/create-custom-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.368151 networklab-1.8.1/netsim/ansible/tasks/deploy-config/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/linux-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/missing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-config/vyos.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-custom-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/deploy-module.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/fetch-config/
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/arcos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/asa.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/ios.yml
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fetch-config/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/frr/
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/frr/deploy-config.yml
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/frr/mpls-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/initial-config.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.372151 networklab-1.8.1/netsim/ansible/tasks/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/linux/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/linux/initial-clab.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/tasks/nxos/
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/nxos/initial.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/tasks/readiness-check/
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/eos-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/iosxr-clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/readiness-check/vsrx.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/tasks/vmx/
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/vmx/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/tasks/wait-for-ready.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.376151 networklab-1.8.1/netsim/ansible/templates/bfd/
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bfd/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/bgp/
--rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/asa.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/eos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/ios.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     8178 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1492 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/bgp/vyos.macro.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/dhcp/
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/dnsmasq.j2
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/eos.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/ios.server.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/dhcp/linux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/eigrp/
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/eigrp/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/eigrp/nxos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.384151 networklab-1.8.1/netsim/ansible/templates/evpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/frr.evpn-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1853 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/evpn/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.388151 networklab-1.8.1/netsim/ansible/templates/gateway/
--rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/gateway/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.392151 networklab-1.8.1/netsim/ansible/templates/initial/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arubacx.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/arubacx.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/csr.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/dellos10.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/eos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/ios.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/ios.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/junos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/junos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.392151 networklab-1.8.1/netsim/ansible/templates/initial/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux/ubuntu.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux/vanilla.j2
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux-clab.j2
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/linux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/nxos.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros7.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/routeros7.vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4983 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2782 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/vyos.vlan.j2
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/initial/vyos.vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.396151 networklab-1.8.1/netsim/ansible/templates/isis/
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/asa.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/isis/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/missing.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.400151 networklab-1.8.1/netsim/ansible/templates/mpls/
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/arubacx.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.6pe.j2
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
--rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/junos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros7.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/srlinux.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/vyos.ldp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.408151 networklab-1.8.1/netsim/ansible/templates/ospf/
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arcos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/junos.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/none.j2
--rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/sros.md-cli.j2
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/sros.openconfig.j2
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.408151 networklab-1.8.1/netsim/ansible/templates/sr/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/sr/sros.openconfig.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.408151 networklab-1.8.1/netsim/ansible/templates/srv6/
--rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/srv6/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.412151 networklab-1.8.1/netsim/ansible/templates/vlan/
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1913 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vmx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vptx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vsrx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.420151 networklab-1.8.1/netsim/ansible/templates/vrf/
--rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/cumulus_nvue.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/eos.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.frr-config.j2
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/frr.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv3.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/junos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/junos.ospf-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/nxos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
--rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1323 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp.j2
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.424151 networklab-1.8.1/netsim/ansible/templates/vxlan/
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/csr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/dellos10.j2
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/ansible/templates/vxlan/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.424151 networklab-1.8.1/netsim/api/
--rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.424151 networklab-1.8.1/netsim/augment/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/addressing.py
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/components.py
--rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/links.py
--rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/main.py
--rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/topology.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/augment/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/cli/
--rwxr-xr-x   0 runner    (1001) docker     (127)    10608 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/alias.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/cli/clab_actions/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab_actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab_actions/build.py
--rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/clab_actions/tarball.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/collect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/down.py
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/empty.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/external_commands.py
--rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)     3667 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/install.py
--rw-r--r--   0 runner    (1001) docker     (127)    11030 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/restart.py
--rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show-usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/cli/show_commands/
--rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/images.py
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/module_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/show_commands/reports.py
--rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/test.py
--rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/up.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/usage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/usage.txt
--rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/validate.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/cli/version.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.432151 networklab-1.8.1/netsim/daemons/
--rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/daemons/bird.yml
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/daemons/dnsmasq.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.436151 networklab-1.8.1/netsim/data/
--rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/filemaps.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/global_vars.py
--rw-r--r--   0 runner    (1001) docker     (127)    30638 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/types.py
--rw-r--r--   0 runner    (1001) docker     (127)    28960 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/data/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.436151 networklab-1.8.1/netsim/defaults/
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/addressing.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/automation.yml
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/hints.yml
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/multilab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/paths.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/defaults/ports.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.440151 networklab-1.8.1/netsim/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/arubacx.py
--rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/arubacx.yml
--rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/asav.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/asav.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/csr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/cumulus.yml
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/cumulus_nvue.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/dellos10.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/eos.py
--rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/eos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/fortios.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/frr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/iosv.py
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/iosv.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/iosxr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/junos.py
--rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/junos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/linux.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/linux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/none.yml
--rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/nxos.yml
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/routeros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/routeros7.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/srlinux.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/sros.yml
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/unknown.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/unknown.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vmx.py
--rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vmx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vptx.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vptx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2310 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vsrx.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vsrx.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/devices/vyos.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.360151 networklab-1.8.1/netsim/extra/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.440151 networklab-1.8.1/netsim/extra/bgp.domain/
--rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.domain/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.domain/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.440151 networklab-1.8.1/netsim/extra/bgp.originate/
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.originate/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.originate/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.444151 networklab-1.8.1/netsim/extra/bgp.policy/
--rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/_route_map_aoscx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/_route_map_ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/simple-attributes.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.policy/srlinux.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/bgp.session/
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/_sample_bfd_template.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/bird.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/default-originate.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/junos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/nxos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/routeros7.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/sros.j2
--rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/topology.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/bgp.session/vyos.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/ebgp.multihop/
--rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/arubacx.j2
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/cumulus.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
--rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/eos.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/frr.j2
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/ios.j2
--rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.multihop/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/ebgp.utils/
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/ebgp.utils/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/fabric/
--rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/fabric/defaults.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/fabric/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/multilab/
--rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/multilab/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/none/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/none/none.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.448151 networklab-1.8.1/netsim/extra/proxy-arp/
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/proxy-arp/plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/proxy-arp/srlinux.j2
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/extra/proxy-arp/sros.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/
--rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/ansible.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/containerlab.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/grpc.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/arubacx.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/asav/
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/asav/day0-config
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/asav.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/csr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/dellos10.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/eos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/eos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/iosv.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/iosv.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/iosxr.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/nxos.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/nxos.xml.j2
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/routeros7.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/vptx/
--rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx/juniper.conf
--rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx/make-config.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx/run.sh
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vptx.xml.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.452151 networklab-1.8.1/netsim/install/libvirt/vsrx/
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vsrx/juniper.conf
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt/vsrx.txt
--rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/libvirt.sh
--rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/install/ubuntu.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.460151 networklab-1.8.1/netsim/modules/
--rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/_dataplane.py
--rw-r--r--   0 runner    (1001) docker     (127)    14999 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/_routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bfd.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bfd.yml
--rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/bgp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/dhcp.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/dhcp.yml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/eigrp.py
--rw-r--r--   0 runner    (1001) docker     (127)      329 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/eigrp.yml
--rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/evpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/evpn.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/gateway.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/gateway.yml
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/initial.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/isis.py
--rw-r--r--   0 runner    (1001) docker     (127)      963 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/isis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/mpls.py
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/mpls.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4674 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/ospf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1261 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/ospf.yml
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/sr.py
--rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/sr.yml
--rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/srv6.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/srv6.yml
--rw-r--r--   0 runner    (1001) docker     (127)    60006 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vlan.yml
--rw-r--r--   0 runner    (1001) docker     (127)    20374 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vrf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vrf.yml
--rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vxlan.py
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/modules/vxlan.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/outputs/
--rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/ansible.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/d2.py
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/d2.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/devices.py
--rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/format.py
--rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/graph.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/graph.yml
--rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/json.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/none.py
--rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/outputs/yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/providers/
--rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/clab.py
--rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/external.py
--rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/external.yml
--rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/libvirt.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/virtualbox.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/providers/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/ansible.cfg.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.364151 networklab-1.8.1/netsim/templates/provider/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/clab.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/cumulus/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/cumulus/hosts.j2
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/cumulus/interfaces.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/frr/
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/frr/daemons.j2
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/frr/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/clab/linux/
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/clab/linux/hosts.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.464151 networklab-1.8.1/netsim/templates/provider/external/
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/external/external.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/templates/provider/libvirt/
--rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/arubacx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/asav-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/csr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/define-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/dellos10-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/fortios-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/forwarded-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/iosv-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/iosxr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-bridge.j2
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
--rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/none-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/routeros-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/routeros7-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vptx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vsrx-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/libvirt/vyos-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/templates/provider/virtualbox/
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/Vagrantfile.j2
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/arcos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/cumulus-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/eos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/frr-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/linux-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/nxos-domain.j2
--rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/virtualbox-network.j2
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
--rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/provider/virtualbox/vsrx-domain.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/templates/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/clab.yml
--rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/grpc.yml
--rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/libvirt.yml
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/templates/tests/virtualbox.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.472151 networklab-1.8.1/netsim/tools/
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/graphite.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/graphite.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/netsim/tools/suzieq/
--rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/suzieq/suzieq-cfg.yml
--rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/tools/suzieq.yml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/topology-defaults.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/netsim/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/bgp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/callback.py
--rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/log.py
--rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/read.py
--rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/sort.py
--rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/strings.py
--rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/templates.py
--rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/utils/versioning.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/netsim/validate/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/validate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/validate/frr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-08 09:30:50.000000 networklab-1.8.1/netsim/validate/linux.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.480151 networklab-1.8.1/networklab.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4289 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24814 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-08 09:30:57.000000 networklab-1.8.1/networklab.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-08 09:30:50.000000 networklab-1.8.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 09:30:57.480151 networklab-1.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-08 09:30:50.000000 networklab-1.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 09:30:57.476151 networklab-1.8.1/tests/
--rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-04-08 09:30:50.000000 networklab-1.8.1/tests/test_transformation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1153 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      288 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      221 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netlab
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.494491 networklab-1.8.1.post1/netsim/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      426 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.498491 networklab-1.8.1.post1/netsim/ansible/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1199 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/collect-configs.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      861 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/create-config.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)      295 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/display-neighbors.ansible
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2876 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/initial-config.ansible
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/reload-config.ansible
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.498491 networklab-1.8.1.post1/netsim/ansible/tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/create-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/create-custom-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      163 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      204 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/missing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3328 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/vyos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-custom-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/deploy-module.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/arcos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/asa.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      308 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      346 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/fortinet.fortios.fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/ios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/
+-rw-r--r--   0 runner    (1001) docker     (127)     2645 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2494 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.502491 networklab-1.8.1.post1/netsim/ansible/tasks/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/frr/deploy-config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/frr/mpls-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/initial-config.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/linux/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/linux/initial-clab.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/nxos/
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/nxos/initial.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/eos-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/iosxr-clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/vsrx.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/tasks/vmx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/vmx/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/tasks/wait-for-ready.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.506491 networklab-1.8.1.post1/netsim/ansible/templates/bfd/
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bfd/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.510491 networklab-1.8.1.post1/netsim/ansible/templates/bgp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1363 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3040 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1830 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2308 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1696 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     8174 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1636 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.macro.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.514491 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/dnsmasq.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      646 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.server.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1162 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/dhcp/linux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.514491 networklab-1.8.1.post1/netsim/ansible/templates/eigrp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/eigrp/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      862 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/eigrp/nxos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.514491 networklab-1.8.1.post1/netsim/ansible/templates/evpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1143 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2035 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1631 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1677 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2883 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/evpn/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.518491 networklab-1.8.1.post1/netsim/ansible/templates/gateway/
+-rw-r--r--   0 runner    (1001) docker     (127)     1346 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1244 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      951 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/gateway/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.522491 networklab-1.8.1.post1/netsim/ansible/templates/initial/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      480 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/csr.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4070 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1839 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      269 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/eos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.522491 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      686 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3792 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/ubuntu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/vanilla.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux-clab.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/linux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/nxos.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1571 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     3479 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5008 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1434 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2941 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.vlan.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.526491 networklab-1.8.1.post1/netsim/ansible/templates/isis/
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/asa.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1241 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1628 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1428 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/isis/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/missing.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.530491 networklab-1.8.1.post1/netsim/ansible/templates/mpls/
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      203 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/arubacx.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/arubacx.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      272 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      208 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.6pe.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      326 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      151 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros7.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      408 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/routeros7.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      777 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/srlinux.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1424 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      780 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.mplsvpn.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.ldp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.534491 networklab-1.8.1.post1/netsim/ansible/templates/ospf/
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arcos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      198 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1170 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1228 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      194 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/junos.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/none.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      152 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      478 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1900 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.md-cli.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.openconfig.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      957 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      869 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.538491 networklab-1.8.1.post1/netsim/ansible/templates/sr/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1127 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2144 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.openconfig.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.538491 networklab-1.8.1.post1/netsim/ansible/templates/srv6/
+-rw-r--r--   0 runner    (1001) docker     (127)     4092 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/srv6/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.538491 networklab-1.8.1.post1/netsim/ansible/templates/vlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1730 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      949 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1938 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vmx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vptx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vsrx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.546491 networklab-1.8.1.post1/netsim/ansible/templates/vrf/
+-rw-r--r--   0 runner    (1001) docker     (127)     1381 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      920 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/cumulus_nvue.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2119 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.frr-config.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1262 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      699 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv3.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2355 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.ospf-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1423 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      173 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1540 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      182 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      185 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      463 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.ospfv2-vrf.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1272 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1408 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.550491 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      608 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/csr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1062 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      458 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/dellos10.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2234 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/ansible/templates/vxlan/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.550491 networklab-1.8.1.post1/netsim/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      956 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.550491 networklab-1.8.1.post1/netsim/augment/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13278 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/addressing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/components.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5897 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24713 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42721 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3598 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14678 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11670 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3665 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/topology.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/augment/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.554491 networklab-1.8.1.post1/netsim/cli/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10608 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/alias.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)      891 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.554491 networklab-1.8.1.post1/netsim/cli/clab_actions/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab_actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3896 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab_actions/build.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3661 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/clab_actions/tarball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2669 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/collect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7048 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6716 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/down.py
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/empty.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7964 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/external_commands.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1585 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3671 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2349 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2026 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/install.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11727 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1332 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/restart.py
+-rw-r--r--   0 runner    (1001) docker     (127)      843 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show-usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3214 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/cli/show_commands/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1613 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2693 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1505 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/images.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/module_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3289 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3409 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4528 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/show_commands/reports.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8258 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4380 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/up.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/usage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2287 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/usage.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    31711 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/validate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/cli/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/daemons/
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/daemons/bird.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/daemons/dnsmasq.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3076 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/filemaps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/global_vars.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30700 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28964 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/data/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.558491 networklab-1.8.1.post1/netsim/defaults/
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/addressing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3141 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/automation.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/hints.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/multilab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3810 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/paths.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/defaults/ports.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.562491 networklab-1.8.1.post1/netsim/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      850 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/arubacx.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/arubacx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      946 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/asav.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/asav.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/csr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/cumulus.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/cumulus_nvue.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1233 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/dellos10.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2644 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/eos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2033 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/eos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/fortios.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1738 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/frr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      932 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/iosv.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/iosv.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1138 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/iosxr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/junos.py
+-rw-r--r--   0 runner    (1001) docker     (127)      669 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/junos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      562 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/linux.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/none.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/nxos.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/routeros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/routeros7.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/srlinux.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1857 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/sros.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/unknown.py
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/unknown.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vmx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      430 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vmx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vptx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vptx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2983 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vsrx.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vsrx.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/devices/vyos.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.490491 networklab-1.8.1.post1/netsim/extra/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.562491 networklab-1.8.1.post1/netsim/extra/bgp.domain/
+-rw-r--r--   0 runner    (1001) docker     (127)       77 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.domain/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3282 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.domain/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.566491 networklab-1.8.1.post1/netsim/extra/bgp.originate/
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.originate/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1670 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.originate/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.566491 networklab-1.8.1.post1/netsim/extra/bgp.policy/
+-rw-r--r--   0 runner    (1001) docker     (127)     2737 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_aoscx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1438 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1570 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1604 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/simple-attributes.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.policy/srlinux.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/bgp.session/
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/_sample_bfd_template.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1732 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/bird.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/default-originate.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2797 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2827 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2588 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/junos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/nxos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5344 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/routeros7.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2651 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     2218 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/sros.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      264 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/topology.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2877 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/bgp.session/vyos.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/
+-rw-r--r--   0 runner    (1001) docker     (127)      690 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/arubacx.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/cumulus.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      689 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/eos.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/frr.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ios.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     6450 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      937 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.multihop/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/ebgp.utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/ebgp.utils/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/fabric/
+-rw-r--r--   0 runner    (1001) docker     (127)      340 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/fabric/defaults.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9454 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/fabric/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/multilab/
+-rw-r--r--   0 runner    (1001) docker     (127)     2989 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/multilab/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.570491 networklab-1.8.1.post1/netsim/extra/none/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/none/none.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/extra/proxy-arp/
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/proxy-arp/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/proxy-arp/srlinux.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/extra/proxy-arp/sros.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/install/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/ansible.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3699 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/containerlab.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1063 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/grpc.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/install/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/arubacx.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.574491 networklab-1.8.1.post1/netsim/install/libvirt/asav/
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/asav/day0-config
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/asav.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1219 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/csr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/dellos10.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2214 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/eos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/eos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1665 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/iosv.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2911 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/iosv.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/iosxr.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1524 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/nxos.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/nxos.xml.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/routeros7.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.578491 networklab-1.8.1.post1/netsim/install/libvirt/vptx/
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx/juniper.conf
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1089 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx/make-config.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)      210 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx/run.sh
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1982 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vptx.xml.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.578491 networklab-1.8.1.post1/netsim/install/libvirt/vsrx/
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vsrx/juniper.conf
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt/vsrx.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3267 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/libvirt.sh
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2319 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/install/ubuntu.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.582491 networklab-1.8.1.post1/netsim/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)    19815 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6220 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/_dataplane.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18777 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/_routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bfd.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bfd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    25554 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2043 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/bgp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    11312 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/dhcp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/dhcp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      605 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/eigrp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/eigrp.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    17618 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/evpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/evpn.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6744 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/gateway.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/gateway.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/initial.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2629 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/isis.py
+-rw-r--r--   0 runner    (1001) docker     (127)      990 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/isis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     7126 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/mpls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/mpls.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/ospf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1288 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/ospf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/sr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      331 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/sr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      888 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/srv6.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/srv6.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    61378 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2342 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vlan.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    20957 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vrf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vrf.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     9895 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vxlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/modules/vxlan.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/outputs/
+-rw-r--r--   0 runner    (1001) docker     (127)     2239 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10083 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/ansible.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10130 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/d2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/d2.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2856 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)      295 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7629 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/graph.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      619 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      342 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/none.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1987 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/outputs/yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)    11516 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6192 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/clab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1147 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/external.py
+-rw-r--r--   0 runner    (1001) docker     (127)      195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/external.yml
+-rw-r--r--   0 runner    (1001) docker     (127)    14817 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/libvirt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      392 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/virtualbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/providers/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/ansible.cfg.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.494491 networklab-1.8.1.post1/netsim/templates/provider/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.586491 networklab-1.8.1.post1/netsim/templates/provider/clab/
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/clab.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/hosts.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/interfaces.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/clab/frr/
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/frr/daemons.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/frr/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/clab/linux/
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/clab/linux/hosts.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.590491 networklab-1.8.1.post1/netsim/templates/provider/external/
+-rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/external/external.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/templates/provider/libvirt/
+-rw-r--r--   0 runner    (1001) docker     (127)      683 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/arubacx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      427 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/asav-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/csr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1177 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1334 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/define-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      438 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/dellos10-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      258 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/fortios-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      409 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/forwarded-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/iosv-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1835 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/iosxr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/none-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/routeros-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/routeros7-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vptx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vsrx-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/libvirt/vyos-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/arcos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/cumulus-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/eos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/frr-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/linux-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/nxos-domain.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      217 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/virtualbox-network.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/virtualbox-ports.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      267 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/provider/virtualbox/vsrx-domain.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/templates/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      166 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/clab.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/grpc.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      181 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/libvirt.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/templates/tests/virtualbox.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5084 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/graphite.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/graphite.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.594491 networklab-1.8.1.post1/netsim/tools/suzieq/
+-rw-r--r--   0 runner    (1001) docker     (127)      304 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/suzieq/suzieq-cfg.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      643 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/tools/suzieq.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/topology-defaults.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/netsim/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2438 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/bgp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/callback.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6226 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12293 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12143 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/read.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1236 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/sort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4090 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5108 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/strings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5585 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/templates.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4148 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/utils/versioning.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/netsim/validate/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/validate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      238 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/validate/frr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2415 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/netsim/validate/linux.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/networklab.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4307 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24814 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 08:33:48.000000 networklab-1.8.1.post1/networklab.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      196 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1550 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 08:33:48.598492 networklab-1.8.1.post1/tests/
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3377 2024-04-24 08:33:44.000000 networklab-1.8.1.post1/tests/test_transformation.py
```

### Comparing `networklab-1.8.1/LICENSE.md` & `networklab-1.8.1.post1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/PKG-INFO` & `networklab-1.8.1.post1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.1
+Version: 1.8.1.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.1/README.md` & `networklab-1.8.1.post1/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.1/netsim/ansible/collect-configs.ansible` & `networklab-1.8.1.post1/netsim/ansible/collect-configs.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/config.ansible` & `networklab-1.8.1.post1/netsim/ansible/config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/create-config.ansible` & `networklab-1.8.1.post1/netsim/ansible/create-config.ansible`

 * *Files 6% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 - name: Create initial device configurations
   hosts: all
   gather_facts: false
   vars:
     config_dir: "{{ lookup('env','PWD') }}/config"
   tasks:
   - block:
-    - name: Set variables that cannot be set with VARS
+    - name: Set variables that cannot be set with vars
       set_fact:
         netlab_device_type: "{{ netlab_device_type|default(ansible_network_os) }}"
         netlab_interfaces: "{{ ([ loopback ] if loopback is defined else []) + interfaces|default([]) }}"
 
     - name: Create config directory in {{ config_dir }}
       file:
         path: "{{ config_dir }}"
@@ -27,33 +27,39 @@
         vars:
           config_item: initial
           paths: "{{ paths_templates.dirs }}"
 
 - name: Create module-specific configurations
   hosts: modules
   tasks:
-  - name: Set variables that cannot be set with VARS
-    set_fact:
-      modlist: "{{ modlist.split(',') if modlist is defined else netlab_module }}"
+  - block:
+    - name: Set variables that cannot be set with vars
+      set_fact:
+        mod_select: "{{ modlist.split(',') if modlist is defined else netlab_module }}"
 
-  - name: Create device configurations for {{ netlab_module|intersect(modlist) }}
-    include_tasks: "tasks/create-config.yml"
-    loop: "{{ netlab_module|intersect(modlist) }}"
-    loop_control:
-      loop_var: config_item
-    when: config_item in module|default([])
-    args:
-      apply:
-        vars:
-          paths: "{{ paths_templates.dirs }}"
+    - name: Create device configurations for {{ mod_select }}
+      include_tasks: "tasks/create-config.yml"
+      loop: "{{ netlab_module }}"
+      when: >-
+        config_item in mod_select and
+        config_item in module|default([]) and
+        config_item not in _daemon_config|default([])
+      loop_control:
+        loop_var: config_item
+      args:
+        apply:
+          vars:
+            paths: "{{ paths_templates.dirs }}"
+
+    delegate_to: localhost
 
 - name: Create custom deployment templates
   hosts: custom_configs
   tasks:
-  - name: Create {{ custom_config }} custom device configuration
+  - name: Create {{ config }} custom device configuration
     include_tasks: "tasks/create-custom-config.yml"
     when: custom_config in config
     loop: "{{ netlab_custom_config }}"
     loop_control:
       loop_var: custom_config
     args:
       apply:
```

### Comparing `networklab-1.8.1/netsim/ansible/initial-config.ansible` & `networklab-1.8.1.post1/netsim/ansible/initial-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/reload-config.ansible` & `networklab-1.8.1.post1/netsim/ansible/reload-config.ansible`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/create-config.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/create-config.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 ---
 - delegate_to: localhost
   block:
-  - name: "Compute final module name for {{ config_item }}"
+  - name: Compute final module name for {{ config_item }}
     set_fact:
       config_module: "{{ config_item.replace('@','.') }}"
       item: "{{ config_item.replace('@','.') }}"
 
-  - name: "Find {{ config_module }} configuration template"
+  - name: Find {{ config_module }} configuration template
     set_fact:
       config_template: "{{ lookup('first_found',params,errors='ignore') }}"
     vars:
       params:
         paths: "{{ paths }}"
         files: "{{ paths_t_files.files }}"
 
   - name: Throw an error message if we can't find the configuration template
     fail:
       msg: >
         Missing configuration template for {{ config_module }} on device
         {{ netlab_device_type|default(ansible_network_os) }}/{{ ansible_network_os }}
     when: not config_template
 
-  - name: Create {{ config_module }} configuration from {{ config_template }}
+  - name: Create {{ config_module }} configuration
     template:
       src: "{{ config_template }}"
       dest: "{{config_dir}}/{{inventory_hostname}}.{{item}}.cfg"
     when: config_template
```

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/arubacx.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/frr.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/linux-clab.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/linux-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/routeros.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/srlinux.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/sros.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-config/vyos.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-config/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-custom-config.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-custom-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/deploy-module.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/deploy-module.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/fetch-config/cumulus.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/fetch-config/srlinux.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/fetch-config/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/fortinet.fortios.fortios/ospf.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/frr/deploy-config.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/frr/deploy-config.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/linux/dhcp.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/linux/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/linux/initial-clab.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/linux/initial-clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/iosxr-libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/readiness-check/vptx.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/readiness-check/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/tasks/vmx/initial.yml` & `networklab-1.8.1.post1/netsim/ansible/tasks/vmx/initial.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bfd/arubacx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bfd/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bfd/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bfd/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bfd/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bfd/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bfd/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bfd/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bfd/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bfd/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bfd/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bfd/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/arubacx.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/arubacx.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/asa.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/asa.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/asa.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/cumulus_nvue.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/dellos10.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/dellos10.macro.j2`

 * *Files 10% similar despite different names*

```diff
@@ -60,17 +60,20 @@
    activate
  exit
 {% endfor %}
 
 {#
   And now, **WTF**, since Dell OS10 cannot disable ipv4 AF by default, we need to:
 #}
-{% if n.activate['ipv4'] is not defined or (n.activate['ipv4'] is defined and not n.activate['ipv4']) %}
+{% if n.activate is defined %}
+{# keep default behavior in case n.activate is not defined #}
+{%   if n.activate['ipv4'] is not defined or (n.activate['ipv4'] is defined and not n.activate['ipv4']) %}
 !
  address-family ipv4 unicast
    no activate
  exit
+{%   endif %}
 {% endif %}
   
   no shutdown
   exit
 {%- endmacro %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/eos.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/eos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/frr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/ios.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/ios.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/iosxr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/junos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/routeros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/routeros.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/routeros7.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/routeros7.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.cli.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/srlinux.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/srlinux.macro.j2`

 * *Files 1% similar despite different names*

```diff
@@ -124,15 +124,15 @@
   val:
    admin-state: enable
 {{ bgp_families(neighbor) }}
    timers:
     connect-retry: 10
     _annotate_connect-retry: "Reduce default 120s to 10s"
     minimum-advertisement-interval: 1
-{% set list = vrf_bgp.community[type]|default([]) %}
+{% set list = bgp.community[type]|default([]) %}
    send-community:
     standard: {{ 'standard' in list }}
     large: {{ 'standard' in list }}
     _annotate_large: "Assuming 'standard' implies 'large' here"
 {% if 'ibgp' in type %}
    import-policy: accept_all
    export-policy: accept_all
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.gnmi.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/sros.md-cli.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/sros.openconfig.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.j2`

 * *Files 12% similar despite different names*

```diff
@@ -11,14 +11,17 @@
 configure
 
 set protocols bgp system-as {{ bgp.as }}
 
 {% if bgp.router_id|ipv4 %}
 set protocols bgp parameters router-id {{ bgp.router_id }}
 {% endif %}
+{% if bgp.rr|default(False) and bgp.rr_cluster_id|default(False) %}
+set protocols bgp parameters cluster-id {{ bgp.rr_cluster_id }}
+{% endif %}
 
 {% for n in bgp.neighbors %}
 {%   for af in ['ipv4','ipv6'] if n[af] is defined %}
 {{     bgpcfg.neighbor(n,n[af],bgp,af) }}
 {%   endfor %}
 {% endfor %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/bgp/vyos.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/bgp/vyos.macro.j2`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 
 {%   if bgp.next_hop_self is defined and bgp.next_hop_self %}
 set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast nexthop-self
 {%   endif %}
 {%   if bgp.rr|default('') and not n.rr|default('') and n.type == 'ibgp' %}
   set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast route-reflector-client
 {%   endif %}
+
+{# community handling -> need to configure what NOT TO SEND (set protocols bgp neighbor XXX address-family XXX disable-send-community <extended|standard>) #}
+{%   for ctype in ['standard', 'extended'] %}
+{%     if not ctype in bgp.community[n.type] %}
+set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast disable-send-community {{ ctype }}
+{%     endif %}
+{%   endfor %}
+
 {%- endmacro -%}
 {#
    BGP network statement
 #}
 {% macro bgp_network(af,pfx) %}
 set protocols bgp address-family {{ af }}-unicast network {{ pfx|ipaddr('0') }}
 {%- endmacro %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/dhcp/cumulus.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/dhcp/dnsmasq.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/dnsmasq.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/dhcp/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/dhcp/eos.server.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/eos.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/dhcp/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/dhcp/ios.server.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/ios.server.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/dhcp/linux-isc-dhcp-relay.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/eigrp/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/eigrp/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/eigrp/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/eigrp/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/arubacx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/cumulus.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/dellos10.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/dellos10.j2`

 * *Files 21% similar despite different names*

```diff
@@ -33,29 +33,46 @@
 
 {% if vrfs is defined %}
 {%   for n,v in vrfs.items() if v.af is defined %}
 {%     set import_target = v.import|join(' ') -%}
 {%     set export_target = v.export|join(' ') -%}
 
 evpn
+  no arp-nd-suppression disable
   vrf {{ n }}
     rd {{ bgp.router_id }}:{{ v.vrfidx }}
     route-target {{ v.import|join(' ') }} import
     route-target {{ v.export|join(' ') }} export
 {%     if import_target == export_target %}
     route-target {{ v.export|join(' ') }} both
 {%     endif %}
 {%     if v.evpn.transit_vni is defined %} 
     vni {{ v.evpn.transit_vni }}
 {%     endif %}
+
+{%     if v.af.ipv4|default(false) %}
     advertise ipv4 connected
     advertise ipv4 static
     advertise ipv4 ospf
     advertise ipv4 bgp
+{%     endif %}
+{%     if v.af.ipv6|default(false) %}
+    advertise ipv6 connected
+    advertise ipv6 static
+    advertise ipv6 ospf
+    advertise ipv6 bgp
+{%     endif %}
+
 !
 router bgp {{ bgp.as }}
   vrf {{ n }}
+{%     if v.af.ipv4|default(false) %}
     address-family ipv4 unicast
       redistribute l2vpn evpn
+{%     endif %}
+{%     if v.af.ipv6|default(false) %}
+    address-family ipv6 unicast
+      redistribute l2vpn evpn
+{%     endif %}
 !
 {%   endfor %}
 {% endif %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/frr.evpn-config.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/frr.evpn-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/srlinux.j2`

 * *Files 7% similar despite different names*

```diff
@@ -25,17 +25,17 @@
    - afi-safi-name: evpn
      evpn:
       rapid-update: True
 {% endfor %}
 
 {# Enable IP advertisement for all irb interfaces in EVPN vlans #}
 {% if vrfs is defined and vrfs %}
-{% for i in interfaces if i.vrf is defined and vrfs[i.vrf].evpn is defined and i.type=='svi' and i.vlan.mode|default('irb')=='irb' %}
+{% for i in interfaces if i.vrf is defined and i.type=='svi' and i.vlan.mode|default('irb')=='irb' %}
 {%  set vrf = vrfs[i.vrf] %}
-{%  set symmetric_irb = 'transit_vni' in vrf.evpn %}
+{%  set symmetric_irb = 'transit_vni' in vrf.evpn|default('') %}
 - path: /interface[name=irb0]/subinterface[index={{ i.ifname.split('.')[1] }}]
   val:
 {%  for ip,arpnd in [('ipv4','arp'),('ipv6','neighbor-discovery')] %}
 {%   if ip in i %}
    {{ ip }}:
      {{ arpnd }}:
        learn-unsolicited: {{ True if ip=='ipv4' else 'both' }}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/evpn/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/evpn/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/arubacx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/cumulus.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/dellos10.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/dellos10.j2`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,17 @@
 
 !
 interface {{ intf.ifname }}
 
 {%   if intf.gateway.protocol == 'anycast' and 'ipv4' in intf.gateway %}
   ip virtual-router address {{ intf.gateway.ipv4|ipaddr('address') }}
 {%   endif %}
+{%   if intf.gateway.protocol == 'anycast' and 'ipv6' in intf.gateway %}
+  ipv6 virtual-router address {{ intf.gateway.ipv6|ipaddr('address') }}
+{%   endif %}
 
 
 {%   if intf.gateway.protocol == 'vrrp' %}
 
 {%     for af in 'ipv4','ipv6' if af in intf.gateway %}
 {%       if af == 'ipv4' %}
   vrrp-group {{ intf.gateway.vrrp.group }}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/gateway/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/gateway/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/arcos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/arcos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/arubacx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/asa.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/cumulus.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/cumulus_nvue.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/dellos10.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/dellos10.vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/dellos10.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/frr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/iosxr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/junos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/junos.vlan.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/junos.vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/junos.vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/linux/hosts.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/linux/ubuntu.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/ubuntu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/linux/vanilla.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/linux/vanilla.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/routeros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/routeros.vlan.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/routeros7.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/routeros7.vlan.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/routeros7.vlan.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/srlinux.cli.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.j2`

 * *Files 1% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 {%  if l.name is defined %}
 {%   set desc = l.name|replace('->','~') + " (" + l.role|default('') + ")" %}
 {%  elif l.type|default("") == "stub" %}
 {%   set desc = "Stub interface" %}
 {%  endif %}
 
 {%  set portname = l.parent_ifname if l.type=='vlan_member' else l.ifname %}
-{%  if 'ixr' in clab.type %}
+{%  if 'ixr' in clab.type and clab.type != 'ixr-x' %}
 {#  Remove connector from port name for IXR platform #}
 {%  set portname = portname.replace("c","") %}
 {%  endif %}
 {%  if l.type in ['p2p','lan','vlan_member'] %}
 {%   if 'c' in portname %}
 - path: configure/port[port-id={{portname}}]
   val:
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/sros.md-cli.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/sros.openconfig.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/initial/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/initial/vyos.j2`

 * *Files 9% similar despite different names*

```diff
@@ -85,13 +85,18 @@
 {% endif %}
 
 {% endfor %}
 
 set service lldp interface all
 set service lldp interface {{ mgmt.ifname|default('eth0') }} disable
 
+{# IPv6 RA config #}
+{% for l in netlab_interfaces if 'ipv6' in l and l.type != 'loopback' %}
+set service router-advert interface {{ l.ifname }}
+{% endfor %}
+
 # Commit, save and exit from subshell
 
 commit
 save
 exit
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/asa.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/asa.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/frr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/iosxr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/iosxr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/junos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/sros.openconfig.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/isis/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/isis/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/eos.6pe.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.6pe.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/eos.bgp-lu.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/eos.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/frr.ldp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/frr.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/ios.bgp-lu.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/ios.bgp-lu.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/junos.ldp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/junos.mplsvpn.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/junos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/srlinux.ldp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/srlinux.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/sros.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/sros.ldp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.ldp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/sros.mplsvpn.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/sros.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/mpls/vyos.mplsvpn.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/arubacx.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/cumulus_nvue.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/cumulus_nvue.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/dellos10.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/eos.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/eos.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/frr.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/frr.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/ios.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/iosxr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/junos.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/junos.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/nxos.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/nxos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/routeros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.cli.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/srlinux.macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/srlinux.macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/sros.md-cli.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.md-cli.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/sros.openconfig.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/ospf/vyos.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/ospf/vyos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/sr/junos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/sr/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/sr/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/sr/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/sr/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/sr/sros.openconfig.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/sr/sros.openconfig.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/srv6/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/srv6/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/arubacx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/csr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/cumulus.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/dellos10.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/dellos10.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/frr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/routeros7.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/sros.j2`

 * *Files 4% similar despite different names*

```diff
@@ -18,17 +18,17 @@
   val:
    service-id: {{ vlan+10000 }}
    customer: "1"
 {%  if l.name is defined %}
    description: "{{ l.name }}"
 {%  endif %}
 {% if l.type in ['vlan_member','lan'] %}
-{% set sap_id = l.ifname.replace("c1/","") if 'ixr' in clab.type else (l.ifname + "/1") %}
+{% set sap_id = l.ifname.replace("c1/","") if 'ixr' in clab.type and 'ixr-x' not in clab.type else l.ifname %}
    sap:
-   - sap-id: {{ sap_id if ':' in sap_id else (sap_id+(":0" if native else "")) }}
+   - sap-id: {{ sap_id if ':' in sap_id else (sap_id+"/1"+(":0" if native else "")) }}
 {%  if native %}
      description: "Native untagged vlan"
 {%  endif %}
 {% endif %}
    admin-state: enable
 {% endif -%}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/vmx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/vmx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/vptx.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/vptx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vlan/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/arubacx.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.bgp-macro.j2`

 * *Files 10% similar despite different names*

```diff
@@ -60,17 +60,20 @@
    activate
  exit
 {% endfor %}
 
 {#
   And now, **WTF**, since Dell OS10 cannot disable ipv4 AF by default, we need to:
 #}
-{% if n.activate['ipv4'] is not defined or (n.activate['ipv4'] is defined and not n.activate['ipv4']) %}
+{% if n.activate is defined %}
+{# keep default behavior in case n.activate is not defined #}
+{%   if n.activate['ipv4'] is not defined or (n.activate['ipv4'] is defined and not n.activate['ipv4']) %}
 !
  address-family ipv4 unicast
    no activate
  exit
+{%   endif %}
 {% endif %}
   
   no shutdown
   exit
 {%- endmacro %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp.j2`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,22 @@
-{% import "dellos10.bgp-macro.j2" as bgpcfg %}
+{% import "ios.bgp-macro.j2" as bgpcfg %}
 !
 router bgp {{ bgp.as }}
 {% for vname,vdata in vrfs.items() %}
-!
- vrf {{ vname }}
-  router-id {{ bgp.router_id }}
-
-{%   for n in vdata.bgp.neighbors|default([]) %}
-{%     for af in ['ipv4','ipv6'] if n[af] is defined %}
-{{       bgpcfg.neighbor(n,n[af],bgp) }}
-{%     endfor %}
-{%   endfor %}
-
-{%   for af in ['ipv4','ipv6'] if af in vdata.af|default({}) %}
-!
- address-family {{ af }} unicast
-   redistribute connected
+{%   for af in ('ipv4','ipv6') if af in vdata.af|default({}) %}
+ address-family {{ af }} vrf {{ vname }}
+  bgp router-id {{ vdata.bgp.router_id|default(bgp.router_id) }}
+  redistribute connected
 {%     if 'ospf' in vdata %}
-   redistribute ospf {{ vdata.vrfidx }}
+  redistribute ospf {{ vdata.vrfidx }}
 {%     endif %}
+!
 {%     for n in vdata.networks|default([]) if af in n %}
-   network {{ n[af]|ipaddr('0') }}
+{{       bgpcfg.bgp_network(af,n[af]) }}
+{%     endfor %}
+!
+{%     for n in vdata.bgp.neighbors|default([]) if af in n %}
+{{       bgpcfg.neighbor_global(n,n[af]) }}
+{{       bgpcfg.neighbor_af(n,n[af],bgp) }}
 {%     endfor %}
 {%   endfor %}
-
 {% endfor %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/dellos10.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/eos.bgp-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/eos.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/eos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/eos.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/eos.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/eos.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/frr.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/frr.frr-config.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.frr-config.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/frr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/frr.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/frr.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/frr.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/ios.bgp-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/ios.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv2.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv2.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/ios.ospfv3.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/ios.ospfv3.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/junos.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/junos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/junos.ospf-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/junos.ospf-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/nxos.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/nxos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/routeros.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp-macro.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.bgp.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/routeros7.ospf-include.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp-macro.j2`

 * *Files 18% similar despite different names*

```diff
@@ -27,14 +27,22 @@
 
 {%   if bgp.next_hop_self is defined and bgp.next_hop_self %}
 set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast nexthop-self
 {%   endif %}
 {%   if bgp.rr|default('') and not n.rr|default('') and n.type == 'ibgp' %}
   set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast route-reflector-client
 {%   endif %}
+
+{# community handling -> need to configure what NOT TO SEND (set protocols bgp neighbor XXX address-family XXX disable-send-community <extended|standard>) #}
+{%   for ctype in ['standard', 'extended'] %}
+{%     if not ctype in bgp.community[n.type] %}
+set protocols bgp neighbor {{ peer }} address-family {{ af }}-unicast disable-send-community {{ ctype }}
+{%     endif %}
+{%   endfor %}
+
 {%- endmacro -%}
 {#
    BGP network statement
 #}
 {% macro bgp_network(af,pfx) %}
 set protocols bgp address-family {{ af }}-unicast network {{ pfx|ipaddr('0') }}
 {%- endmacro %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.bgp.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.bgp.j2`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 {% import "vyos.bgp-macro.j2" as bgpcfg %}
 
 set protocols bgp system-as {{ bgp.as }}
 
+{# force router-id on vrf as well #}
+{% if bgp.router_id|ipv4 %}
+set protocols bgp parameters router-id {{ bgp.router_id }}
+{% endif %}
 
 {% for af in ['ipv4','ipv6'] if af in vdata.af|default({}) %}
 set protocols bgp address-family {{ af }}-unicast rd vpn export {{ vdata.rd }}
 set protocols bgp address-family {{ af }}-unicast route-target vpn import "{{ vdata.import|join(' ') }}"
 set protocols bgp address-family {{ af }}-unicast route-target vpn export "{{ vdata.export|join(' ') }}"
 set protocols bgp address-family {{ af }}-unicast import vpn
 set protocols bgp address-family {{ af }}-unicast export vpn
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.j2`

 * *Files 27% similar despite different names*

```diff
@@ -4,16 +4,21 @@
 if [ "$(id -g -n)" != 'vyattacfg' ] ; then
     exec sg vyattacfg -c "/bin/vbash $(readlink -f $0) $@"
 fi
 
 # Configuration items start here
 configure
 
+{# Route leaking case: bgp.as can be set even without the BGP module, so - if present - need to enable BGP at global level #}
+{% if bgp.as is defined %}
+set protocols bgp system-as {{ bgp.as }}
+{% endif %}
+
 # Enter vrf sublevel
-{% for vname,vdata in vrfs.items() %}
+{% for vname,vdata in (vrfs|default({})).items() %}
 edit vrf name {{ vname }}
 
 {% if bgp.as is defined %}
 {% include 'vyos.bgp.j2' %}
 {% endif %}
 
 {% if 'ospf' in vdata %}
```

### Comparing `networklab-1.8.1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vrf/vyos.ospfv2-vrf.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vxlan/csr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/csr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vxlan/cumulus.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vxlan/frr.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vxlan/nxos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vxlan/srlinux.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vxlan/sros.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/ansible/templates/vxlan/vyos.j2` & `networklab-1.8.1.post1/netsim/ansible/templates/vxlan/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/api/__init__.py` & `networklab-1.8.1.post1/netsim/api/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/addressing.py` & `networklab-1.8.1.post1/netsim/augment/addressing.py`

 * *Files 0% similar despite different names*

```diff
@@ -249,16 +249,16 @@
   for af in list(pools[p]):
     if 'cache' in af:                                                 # Skipping over caches
       continue
     if not isinstance(pools[p][af],types.GeneratorType):              # Copy non-generator attributes
       prefixes[af] = pools[p][af]
       continue
 
+    subnet_cache = 'cache_%s' % af
     if n:                                                             # Allocating a specific prefix or IP address from a subnet
-      subnet_cache = 'cache_%s' % af
       if not subnet_cache in pools[p]:                                # Set up a cache to speed up things
         pools[p][subnet_cache] = []
       try:
         prefixes[af] = get_nth_subnet(n,pools[p][af],pools[p][subnet_cache])
       except StopIteration:
         log.error(
           f'Cannot allocate {n}-th {af} element from {p} pool',
```

### Comparing `networklab-1.8.1/netsim/augment/components.py` & `networklab-1.8.1.post1/netsim/augment/components.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/config.py` & `networklab-1.8.1.post1/netsim/augment/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/devices.py` & `networklab-1.8.1.post1/netsim/augment/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/groups.py` & `networklab-1.8.1.post1/netsim/augment/groups.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/links.py` & `networklab-1.8.1.post1/netsim/augment/links.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/main.py` & `networklab-1.8.1.post1/netsim/augment/main.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/nodes.py` & `networklab-1.8.1.post1/netsim/augment/nodes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/plugin.py` & `networklab-1.8.1.post1/netsim/augment/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/tools.py` & `networklab-1.8.1.post1/netsim/augment/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/topology.py` & `networklab-1.8.1.post1/netsim/augment/topology.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/augment/validate.py` & `networklab-1.8.1.post1/netsim/augment/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/__init__.py` & `networklab-1.8.1.post1/netsim/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/ansible.py` & `networklab-1.8.1.post1/netsim/cli/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/clab.py` & `networklab-1.8.1.post1/netsim/cli/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/clab_actions/build.py` & `networklab-1.8.1.post1/netsim/cli/clab_actions/build.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/clab_actions/tarball.py` & `networklab-1.8.1.post1/netsim/cli/clab_actions/tarball.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/collect.py` & `networklab-1.8.1.post1/netsim/cli/collect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/config.py` & `networklab-1.8.1.post1/netsim/cli/config.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/connect.py` & `networklab-1.8.1.post1/netsim/cli/connect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/create.py` & `networklab-1.8.1.post1/netsim/cli/create.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/down.py` & `networklab-1.8.1.post1/netsim/cli/down.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/external_commands.py` & `networklab-1.8.1.post1/netsim/cli/external_commands.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/graph.py` & `networklab-1.8.1.post1/netsim/cli/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/initial.py` & `networklab-1.8.1.post1/netsim/cli/initial.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,15 +72,15 @@
     rest = ['-t','module'] + rest
   
   if args.custom:
     deploy_parts.append("custom")
     rest = ['-t','custom'] + rest
 
   if args.output:
-    rest = ['-e','config_dir='+os.path.abspath(args.output) ] + rest
+    rest = ['-e',f'config_dir="{os.path.abspath(args.output)}"' ] + rest
 
   if args.fast or os.environ.get('NETLAB_FAST_CONFIG',None):
     rest = ['-e','netlab_strategy=free'] + rest
 
   if args.logging or args.verbose:
     print("Ansible playbook args: %s" % rest)
```

### Comparing `networklab-1.8.1/netsim/cli/inspect.py` & `networklab-1.8.1.post1/netsim/cli/inspect.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/install.py` & `networklab-1.8.1.post1/netsim/cli/install.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/libvirt.py` & `networklab-1.8.1.post1/netsim/cli/libvirt.py`

 * *Files 3% similar despite different names*

```diff
@@ -144,25 +144,50 @@
     abort_on_failure("virsh define template.xml")
     abort_on_failure("virsh start --console vm_box")
 
   vm_cleanup('vm_box',ignore_destroy=True)        # Have to ignore 'destroy' errors as the VM could be powered off
 
 def lp_create_box(args: argparse.Namespace,settings: Box) -> None:
   _files.create_file_from_text(
+    fname="Vagrantfile",
+    txt='''
+Vagrant.configure("2") do |config|
+  config.vm.provider :libvirt do |libvirt|
+    libvirt.driver = "kvm"
+    libvirt.host = ""
+    libvirt.connect_via_ssh = false
+    libvirt.storage_pool_name = "default"
+  end
+end
+''')
+  abort_on_failure('cp vm.qcow2 box.img')
+  img_json = external_commands.run_command('qemu-img info --output=json box.img',check_result=True,return_stdout=True)
+
+  try:
+    if isinstance(img_json,str) and img_json:
+      img_data = Box.from_json(json_string=img_json,box_dots=True)
+    else:
+      raise Exception('qemu-img failed')
+  except Exception as ex:
+    log.fatal(f'Cannot parse qemu-img virtual disk information: {ex}')
+
+  v_size = int((img_data['virtual-size'] - 1)/(2**30)) + 1
+
+  _files.create_file_from_text(
     fname="metadata.json",
-    txt='{"provider":"libvirt","format":"qcow2","virtual_size":4}\n')
-  print("Downloading vagrant-libvirt create_box.sh script")
-  abort_on_failure('curl -O https://raw.githubusercontent.com/vagrant-libvirt/vagrant-libvirt/master/tools/create_box.sh')
+    txt=f'{{"provider":"libvirt","format":"qcow2","virtual_size":{v_size}}}\n')
 
   boxfile = f"{args.device}.box"
   if os.path.isfile(boxfile):
     print(f"Removing old {boxfile}")
     os.remove(boxfile)
 
-  abort_on_failure(f'bash create_box.sh vm.qcow2 {boxfile}')
+  print(f'Creating tar archive {boxfile}')
+  abort_on_failure(f'tar cfz {boxfile} Vagrantfile metadata.json box.img')
+  abort_on_failure('rm box.img')
 
   devdata = settings.devices[args.device]
   boxname = devdata.libvirt.image
   if not boxname:
     log.fatal("Libvirt box name is not set for device {args.device}")
 
   print(f"""
```

### Comparing `networklab-1.8.1/netsim/cli/read.py` & `networklab-1.8.1.post1/netsim/cli/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/report.py` & `networklab-1.8.1.post1/netsim/cli/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/restart.py` & `networklab-1.8.1.post1/netsim/cli/restart.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show-usage.txt` & `networklab-1.8.1.post1/netsim/cli/show-usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show.py` & `networklab-1.8.1.post1/netsim/cli/show.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/__init__.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/attributes.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/attributes.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/defaults.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/defaults.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/devices.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/images.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/images.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/module_support.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/module_support.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/modules.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/modules.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/outputs.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/outputs.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/providers.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/providers.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/show_commands/reports.py` & `networklab-1.8.1.post1/netsim/cli/show_commands/reports.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/status.py` & `networklab-1.8.1.post1/netsim/cli/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/test.py` & `networklab-1.8.1.post1/netsim/cli/test.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/up.py` & `networklab-1.8.1.post1/netsim/cli/up.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/usage.txt` & `networklab-1.8.1.post1/netsim/cli/usage.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/cli/validate.py` & `networklab-1.8.1.post1/netsim/cli/validate.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/common.py` & `networklab-1.8.1.post1/netsim/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/daemons/bird.yml` & `networklab-1.8.1.post1/netsim/daemons/bird.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/data/__init__.py` & `networklab-1.8.1.post1/netsim/data/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/data/filemaps.py` & `networklab-1.8.1.post1/netsim/data/filemaps.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/data/global_vars.py` & `networklab-1.8.1.post1/netsim/data/global_vars.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/data/types.py` & `networklab-1.8.1.post1/netsim/data/types.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # Data validation routines
 #
 
 import typing,typing_extensions,types
 import functools
 import netaddr
 import re
+import textwrap
+
 from box import Box
 from ..utils import log
 from . import global_vars
 
 """
 Common error checking routines:
 
@@ -74,29 +76,29 @@
 
   if '_type' not in err_stat and '_value' not in err_stat:
     raise Exception("FATAL (wrong_type_message) err_stat does not contain _type or _value")
 
   if '_help' in err_stat:                               # Did the validation function specify extra help?
     if exp_type not in _wrong_type_help:                # Did we print this help before? Adjust context if not
       help = err_stat.get("_help")
-      ctxt.append(f'FYI: {exp_type} is {help}')
+      ctxt.extend(textwrap.wrap(f'FYI: {exp_type} is {help}'))
       _wrong_type_help[exp_type] = help
 
   if '_value' in err_stat:                             # _value contains explanation why the value is incorrect
     expected = err_stat.get('_value')                  # ... even though the type is correct
   else:
     if isinstance(context,dict) and '_alt_types' in context:
       expected += err_add_alt_types(context)
       ctxt = []
     expected += f', found {wrong_type}'                 # A more generic message, add wrong type
 
   if 'NOATTR:' in path:                                 # Deal with values that are not attributes
     path = path.replace('NOATTR:','')
   else:
-    path = f'attribute {path}'
+    path = f"attribute '{path}'"
 
   # Display hint only when we know the hint ID
   if '_hint_id' in err_stat:
     if _attr_help_cache is None:                        # Initialize help messages cache if needed
       from ..data import get_empty_box
       _attr_help_cache = get_empty_box()
 
@@ -445,15 +447,15 @@
 def must_be_id(value: typing.Any, max_length: int = 16) -> dict:
   match_str = f'[a-zA-Z_][a-zA-Z0-9_-]{{0,{max_length - 1}}}'
 #  print(f'must_be_id: v={value} m={match_str}')
   if not isinstance(value,str) or not re.fullmatch(match_str,value):
     return {
       '_valid': False,
       '_type' : f'a {max_length}-character identifier',
-      '_help' : f'a string containing up to {max_length} alphanumeric characters, numbers and underscores'
+      '_help' : f'a string starting with a letter or an underscore and containing up to {max_length} letters, numbers, or underscores'
     }
 
   return { '_valid': True } 
 
 @type_test()
 def must_be_int(
       value: typing.Any,
```

### Comparing `networklab-1.8.1/netsim/data/validate.py` & `networklab-1.8.1.post1/netsim/data/validate.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 def check_required_keys(data: Box, attributes: Box, path: str,module: str) -> bool:
   result = True
   for k,v in attributes.items():
     if isinstance(v,Box) and '_required' in v and v._required:
       if k in data:
         continue
       log.error(
-        f'Mandatory attribute {path}.{k} is missing',
+        f"Mandatory attribute '{path}.{k}' is missing",
         log.MissingValue,
         module)
       result = False
 
   return result
 
 """
@@ -215,15 +215,15 @@
   #
   if not '_keys' in data_type:                    # If the dictionary does not have the valid keys
     return return_value                           # ... there's nothing further to validate, return what we accumulated so far
 
   for k in data.keys():                           # Iterate over the elements
     if not k in data_type._keys:                  # ... and report elements with invalid name
       log.error(
-        f'Incorrect {data_name} attribute {k} in {parent_path}',
+        f"Incorrect {data_name} attribute '{k}' in {parent_path}",
         log.IncorrectAttr,
         module)
       return_value = False
     else:                                         # For valid elements, validate them
       validate_item(
         parent=data,
         key=k,
```

### Comparing `networklab-1.8.1/netsim/defaults/attributes.yml` & `networklab-1.8.1.post1/netsim/defaults/attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/defaults/hints.yml` & `networklab-1.8.1.post1/netsim/defaults/hints.yml`

 * *Files 13% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 # Error message hints
+---
 evpn:
   irb_group: >
     All VLANs that are part of a VRF using asymmetric IRB have to be present on all nodes
     using that VRF. The easiest way to achieve that is to create a group with all
     participating nodes and list VLANs in the 'vlans' attribute of that group
   node_bundle: |
     evpn.bundle attribute can be used only in global VRF definition
@@ -14,7 +15,15 @@
   igp: >
     Add a supported IGP (ospf, isis, eigrp) to the list of modules.
 report:
   source: >
     A report can be specified in a file with .j2 suffix within 'reports' subdirectory in
     package-, system-, user- or current directory. You can also specify a report in a
     defaults.outputs.report setting.
+quirks:
+  junos_lb: >
+    Junos devices cannot have more than one loopback interface per routing instance
+
+vrf:
+  inactive: >
+    A globally-defined VRF is not used on a node unless that node is attached to a VRF link,
+    or has the VRF listed in the node 'vrfs' dictionary and uses VRF loopbacks.
```

### Comparing `networklab-1.8.1/netsim/defaults/paths.yml` & `networklab-1.8.1.post1/netsim/defaults/paths.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/__init__.py` & `networklab-1.8.1.post1/netsim/devices/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
 
 mod_load: typing.Dict = {}
 
 def device_quirk(node: Box, topology: Box, method: str = 'device_quirks') -> None:
   global mod_load
 
   if log.debug_active('quirks'):
-    print(f'Processing {method} device quirks')
+    print(f'Processing device quirks: method {method}, node {node.name}/{node.device}')
   device = node.device
 
   if not device in mod_load:
     dev_quirk = os.path.dirname(__file__)+"/"+device+".py"
     if os.path.exists(dev_quirk):
       mod_load[device] = _Quirks.load(device,topology.defaults.devices.get(device))
     else:
```

### Comparing `networklab-1.8.1/netsim/devices/arubacx.py` & `networklab-1.8.1.post1/netsim/devices/arubacx.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/arubacx.yml` & `networklab-1.8.1.post1/netsim/devices/arubacx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/asav.py` & `networklab-1.8.1.post1/netsim/devices/asav.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/asav.yml` & `networklab-1.8.1.post1/netsim/devices/asav.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/csr.yml` & `networklab-1.8.1.post1/netsim/devices/csr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/cumulus.yml` & `networklab-1.8.1.post1/netsim/devices/cumulus.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/cumulus_nvue.yml` & `networklab-1.8.1.post1/netsim/devices/cumulus_nvue.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/dellos10.yml` & `networklab-1.8.1.post1/netsim/devices/dellos10.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/eos.py` & `networklab-1.8.1.post1/netsim/devices/eos.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/eos.yml` & `networklab-1.8.1.post1/netsim/devices/eos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/fortios.yml` & `networklab-1.8.1.post1/netsim/devices/fortios.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/frr.yml` & `networklab-1.8.1.post1/netsim/devices/frr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/iosv.py` & `networklab-1.8.1.post1/netsim/devices/iosv.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #
 # Cisco IOSv quirks
 #
 from box import Box
 
 from . import _Quirks
 from ..utils import log
+from ..modules import _routing
 from ..augment import devices
 
 # Cisco IOSv does not support VRRP on BVI interfaces. Go figure...
 #
 def check_vrrp_bvi(node: Box, topology: Box) -> None:
   for intf in node.interfaces:
     if intf.get('gateway.protocol',None) != 'vrrp':                     # No VRRP, move on
@@ -26,7 +27,10 @@
 class IOS(_Quirks):
 
   @classmethod
   def device_quirks(self, node: Box, topology: Box) -> None:
     mods = node.get('module',[])
     if 'gateway' in mods:
       check_vrrp_bvi(node,topology)
+
+    if 'ospf' in mods:
+      _routing.get_unique_router_ids(node,'ospf',topology)
```

### Comparing `networklab-1.8.1/netsim/devices/iosv.yml` & `networklab-1.8.1.post1/netsim/devices/iosv.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/iosxr.yml` & `networklab-1.8.1.post1/netsim/devices/iosxr.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/junos.yml` & `networklab-1.8.1.post1/netsim/devices/junos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/linux.py` & `networklab-1.8.1.post1/netsim/devices/linux.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/linux.yml` & `networklab-1.8.1.post1/netsim/devices/linux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/none.yml` & `networklab-1.8.1.post1/netsim/devices/none.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/nxos.yml` & `networklab-1.8.1.post1/netsim/devices/nxos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/routeros.yml` & `networklab-1.8.1.post1/netsim/devices/routeros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/routeros7.yml` & `networklab-1.8.1.post1/netsim/devices/routeros7.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/srlinux.yml` & `networklab-1.8.1.post1/netsim/devices/srlinux.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/sros.yml` & `networklab-1.8.1.post1/netsim/devices/sros.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/unknown.py` & `networklab-1.8.1.post1/netsim/devices/unknown.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/vptx.yml` & `networklab-1.8.1.post1/netsim/devices/vptx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/vsrx.yml` & `networklab-1.8.1.post1/netsim/devices/vsrx.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/devices/vyos.yml` & `networklab-1.8.1.post1/netsim/devices/vyos.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.domain/plugin.py` & `networklab-1.8.1.post1/netsim/extra/bgp.domain/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.originate/plugin.py` & `networklab-1.8.1.post1/netsim/extra/bgp.originate/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/_route_map_aoscx.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_aoscx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/_route_map_ios.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/_route_map_ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/arubacx.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/cumulus.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/defaults.yml` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/eos.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/frr.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/ios.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/plugin.py` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/simple-attributes.yml` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/simple-attributes.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.policy/srlinux.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.policy/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/_sample_bfd_template.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/_sample_bfd_template.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/arubacx.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/cumulus.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/cumulus.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/default-originate.yml` & `networklab-1.8.1.post1/netsim/extra/bgp.session/default-originate.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/defaults.yml` & `networklab-1.8.1.post1/netsim/extra/bgp.session/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/eos.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/frr.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/ios.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/junos.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/junos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/nxos.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/nxos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/plugin.py` & `networklab-1.8.1.post1/netsim/extra/bgp.session/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/routeros7.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/routeros7.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/srlinux.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/sros.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/bgp.session/vyos.j2` & `networklab-1.8.1.post1/netsim/extra/bgp.session/vyos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/arubacx.j2` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/arubacx.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/defaults.yml` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ebgp-multihop-load-balancing.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/eos.j2` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/eos.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/evpn-ebgp-over-ebgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/frr.j2` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/frr.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/ios.j2` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/ios.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/plugin.py` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/srlinux.j2` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/ebgp.multihop/sros.j2` & `networklab-1.8.1.post1/netsim/extra/ebgp.multihop/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/fabric/plugin.py` & `networklab-1.8.1.post1/netsim/extra/fabric/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/multilab/__init__.py` & `networklab-1.8.1.post1/netsim/extra/multilab/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/proxy-arp/plugin.py` & `networklab-1.8.1.post1/netsim/extra/proxy-arp/plugin.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/proxy-arp/srlinux.j2` & `networklab-1.8.1.post1/netsim/extra/proxy-arp/srlinux.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/extra/proxy-arp/sros.j2` & `networklab-1.8.1.post1/netsim/extra/proxy-arp/sros.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/ansible.sh` & `networklab-1.8.1.post1/netsim/install/ansible.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/containerlab.sh` & `networklab-1.8.1.post1/netsim/install/containerlab.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/grpc.sh` & `networklab-1.8.1.post1/netsim/install/grpc.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/arubacx.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/arubacx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/asav/day0-config` & `networklab-1.8.1.post1/netsim/install/libvirt/asav/day0-config`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/csr.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/csr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/dellos10.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/dellos10.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/eos.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/eos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/eos.xml.j2` & `networklab-1.8.1.post1/netsim/install/libvirt/eos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/iosv.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/iosv.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/iosv.xml.j2` & `networklab-1.8.1.post1/netsim/install/libvirt/iosv.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/iosxr.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/iosxr.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/nxos.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/nxos.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/nxos.xml.j2` & `networklab-1.8.1.post1/netsim/install/libvirt/nxos.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/routeros7.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/routeros7.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/vptx/juniper.conf` & `networklab-1.8.1.post1/netsim/install/libvirt/vptx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/vptx/make-config.sh` & `networklab-1.8.1.post1/netsim/install/libvirt/vptx/make-config.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/vptx.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/vptx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/vptx.xml.j2` & `networklab-1.8.1.post1/netsim/install/libvirt/vptx.xml.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/vsrx/juniper.conf` & `networklab-1.8.1.post1/netsim/install/libvirt/vsrx/juniper.conf`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt/vsrx.txt` & `networklab-1.8.1.post1/netsim/install/libvirt/vsrx.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/libvirt.sh` & `networklab-1.8.1.post1/netsim/install/libvirt.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/install/ubuntu.sh` & `networklab-1.8.1.post1/netsim/install/ubuntu.sh`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/__init__.py` & `networklab-1.8.1.post1/netsim/modules/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/_dataplane.py` & `networklab-1.8.1.post1/netsim/modules/_dataplane.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/_routing.py` & `networklab-1.8.1.post1/netsim/modules/_routing.py`

 * *Files 15% similar despite different names*

```diff
@@ -136,62 +136,72 @@
   # there's at most one router attached to the link. However, there might be host daemons
   # attached to it, so we have to do further checks
   #
   # Note that we cannot fix this by setting link role to something else, as the 'stub' role
   # triggers the generation of default gateway which is used for default routing on daemons
   intf[proto].passive = is_true_stub(intf,topology,proto)
 
+# Get a router ID prefix from the router_id pool
+#
+def get_router_id_prefix(node: Box, proto: str, pools: Box, use_id: bool = True) -> typing.Optional[Box]:
+  if not pools.router_id:
+    log.error(
+      f'Cannot create a router ID for protocol {proto} on node {node.name}: router_id addressing pool is not defined',
+      log.MissingValue,
+      proto)
+    return None
+
+  pool = 'router_id'
+  pfx = addressing.get(pools,[ pool ],node.id if use_id else None)
+  if not pfx:
+    log.error(
+      f'Cannot create a router ID prefix from {pool} pool for protocol {proto} on node {node.name}',
+      log.IncorrectValue,
+      proto)
+    return None
+
+  if not pfx.get('ipv4',None):
+    log.error(
+      f'{pool} pool did not return a usable IPv4 address to use as router ID for protocol {proto} on node {node.name}',
+      log.IncorrectValue,
+      proto)
+    return None
+
+  return pfx
+
 # Create router ID if needed
 #
 def router_id(node: Box, proto: str, pools: Box) -> None:
   if 'router_id' in node.get(proto,{}):       # User-configured per-protocol router ID, get out of here
     try:
       node[proto].router_id = str(netaddr.IPAddress(node[proto].router_id).ipv4())
     except Exception as ex:
       log.error(
         f'{proto} router_id "{node[proto].router_id}" specified on node {node.name} is not an IPv4 address',
         log.IncorrectValue,
         proto)
     return
 
-  if 'router_id' in node:                     # Node as configured router ID, copy it and get out
+  if 'router_id' in node:                     # Node has a configured router ID, copy it and get out
     try:
       node.router_id = str(netaddr.IPAddress(node.router_id).ipv4())
       node[proto].router_id = node.router_id
     except Exception as ex:
       log.error(
         f'router_id "{node.router_id}" specified on node {node.name} is not an IPv4 address',
         log.IncorrectValue,
         proto)
     return
 
   if 'ipv4' in node.get('loopback',{}):       # Do we have IPv4 address on the loopback? If so, use it as router ID
     node[proto].router_id = str(netaddr.IPNetwork(node.loopback.ipv4).ip)
     return
 
-  if not pools.router_id:
-    log.error(
-      f'Cannot create a router ID for protocol {proto} on node {node.name}: router_id addressing pool is not defined',
-      log.MissingValue,
-      proto)
-    return
-
-  pfx = addressing.get(pools,['router_id'],node.id)
+  pfx = get_router_id_prefix(node,proto,pools)
   if not pfx:
-    log.error(
-      f'Cannot create a router ID prefix from router_id pool for protocol {proto} on node {node.name}',
-      log.IncorrectValue,
-      proto)
-    return
-
-  if not pfx.get('ipv4',None):
-    log.error(
-      f'router_id pool did not return a usable IPv4 address to use as router ID for protocol {proto} on node {node.name}',
-      log.IncorrectValue,
-      proto)
     return
 
   node.router_id = str(netaddr.IPNetwork(pfx['ipv4']).ip)
   node[proto].router_id = node.router_id
 
 #
 # remove_vrf_interfaces -- remove interfaces in a VRF from a routing process that is not VRF-aware
@@ -244,27 +254,32 @@
   for intf in node.interfaces:
     if proto in intf:
       if not any(af in intf for af in ('ipv4','ipv6','unnumbered')):        # Do we have at least some addressing on the interface?
         intf.pop(proto,None)                                                # Nope, no need to run IGP on that interface
 #
 # remove_unused_igp -- remove IGP module if it's not configured on any interface
 #
-def remove_unused_igp(node: Box, proto: str) -> None:
+def remove_unused_igp(node: Box, proto: str, warning: bool = False) -> None:
   if not any(proto in ifdata for ifdata in node.interfaces):                # Is protocol configured on any non-loopback interface?
     node.pop(proto,None)                                                    # ... no, remove protocol data from node
 
   if proto in node and 'af' in node[proto] and node[proto].af:              # Is at least one global AF active for the protocol?
     return                                                                  # ... OK, we're good
 
   for vdata in node.get('vrfs',{}).values():                                # Is protocol active in at least one VRF?
     if proto in vdata:
       return                                                                # ... OK, we're good
 
   node.module = [ m for m in node.module if m != proto ]                    # Makes no sense to keep it, remove the config module
-
+  if warning:
+    log.error(
+      f'{node.name} does not use {proto} on any non-loopback interface or VRF',
+      more_hints=f'It has been removed from the list of modules active on {node.name}',
+      category=Warning,
+      module=proto)
 #
 # remove_vrf_routing_blocks -- remove 'proto: False' VRF settings
 #
 
 def remove_vrf_routing_blocks(node: Box, proto: str) -> None:
   if not 'vrfs' in node:                                                    # No VRFs, no work
     return
@@ -320,7 +335,71 @@
   if 'loopback' in n and n.get('role') != 'host':           # The node has loopback and is not a host
     return n.loopback                                       # ... can't use loopback if the node has no routing
 
   if n.interfaces:                                          # Hope the node has at least one usable interface
     return n.interfaces[0]                                  # ... if it does, return that
 
   return data.get_empty_box()                               # Otherwise return an empty box
+
+"""
+get_router_id_blacklist: As we generate router IDs in various ways, we have no way of
+figuring out which ones were already used. The only bruteforce method is thus to build
+a list of router ID per protocol
+"""
+def get_router_id_blacklist(topology: Box, proto: str) -> list:
+  blist = []
+  for ndata in topology.nodes.values():                     # Iterate over all nodes
+    blist.append(ndata.get(f'{proto}.router_id',None))      # Blindly add router ID from global proto instance
+    for vdata in ndata.get('vrfs',{}).values():
+      blist.append(vdata.get(f'{proto}.router_id',None))    # ... and from all VRFs
+
+  return [ x for x in blist if x is not None ]              # Obviously some of those values do not exist
+                                                            # ... so we have to filter them out
+
+"""
+get_unique_router_ids: change router IDs in VRF routing protocols for devices that want
+to have a unique router_id per routing protocol instance (Cisco IOSv)
+
+This could be part of IOSv quirks, but we might have other devices with similarly weird
+behavior
+"""
+def get_unique_router_ids(node: Box, proto: str, topology: Box) -> None:
+  if 'vrfs' not in node:
+    return
+
+  rid_list: list = []                                       # Keep track of on-device RIDs
+  rid_blacklist: list = []                                  # ... and a global list of already-used RIDs
+  if proto in node:
+    rid_list.append(node.get(f'{proto}.router_id'))         # The node is running a global copy of the protocol
+
+  for vname,vdata in node.vrfs.items():                     # Now iterate over all VRFs
+    if proto not in vdata:                                  # ... protocol not running in VRF, move on
+      continue
+    rid = vdata.get(f'{proto}.router_id')
+    if rid not in rid_list:                                 # VRF router ID is unique, move on
+      rid_list.append(rid)
+      continue
+
+    if not rid_blacklist:                                   # Get the global black lisf if needed
+      rid_blacklist = get_router_id_blacklist(topology,proto)
+      print(f'blacklist: {rid_blacklist}')
+
+    while True:                                             # Try to get the next router ID from the pool
+      rid_pfx = get_router_id_prefix(node,proto,topology.pools,use_id=False)
+      if not rid_pfx:
+        break
+      router_id = str(netaddr.IPNetwork(rid_pfx['ipv4']).ip)
+      if router_id not in rid_blacklist:                    # ... until it's not in the blacklist
+        break
+
+    if rid_pfx:                                             # If we have a prefix, we also have a RID
+      vdata[proto].router_id = router_id                    # ... so set it and report the change
+      log.error(
+        f'router ID for VRF {vname} on node {node.name} was changed from {rid} to {vdata[proto].router_id}',
+        category=Warning,
+        module=proto,
+        more_hints=f'Device {node.device} requires a unique router ID for each {proto} instance')
+    else:                                                   # Ran out of RID pool, report another error
+      log.error(
+        f'Cannot change router ID for VRF {vname} on node {node.name}',
+        category=Warning,
+        module=proto)
```

### Comparing `networklab-1.8.1/netsim/modules/bfd.py` & `networklab-1.8.1.post1/netsim/modules/bfd.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/bfd.yml` & `networklab-1.8.1.post1/netsim/modules/bfd.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/bgp.py` & `networklab-1.8.1.post1/netsim/modules/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/bgp.yml` & `networklab-1.8.1.post1/netsim/modules/bgp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/dhcp.py` & `networklab-1.8.1.post1/netsim/modules/dhcp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/dhcp.yml` & `networklab-1.8.1.post1/netsim/modules/dhcp.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/evpn.py` & `networklab-1.8.1.post1/netsim/modules/evpn.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/evpn.yml` & `networklab-1.8.1.post1/netsim/modules/evpn.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/gateway.py` & `networklab-1.8.1.post1/netsim/modules/gateway.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/gateway.yml` & `networklab-1.8.1.post1/netsim/modules/gateway.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/isis.py` & `networklab-1.8.1.post1/netsim/modules/isis.py`

 * *Files 6% similar despite different names*

```diff
@@ -69,8 +69,8 @@
     # * Calculate address families
     # * Enable BFD
     # * Remove ISIS module if there are no IS-IS enabled global interfaces
     #
     _routing.remove_unaddressed_intf(node,'isis')
     _routing.remove_vrf_interfaces(node,'isis')
     _routing.routing_af(node,'isis')
-    _routing.remove_unused_igp(node,'isis')
+    _routing.remove_unused_igp(node,'isis',topology.defaults.get('isis.warnings.inactive',False))
```

### Comparing `networklab-1.8.1/netsim/modules/isis.yml` & `networklab-1.8.1.post1/netsim/modules/isis.yml`

 * *Files 9% similar despite different names*

```diff
@@ -35,7 +35,9 @@
     network_type: { type: str, valid_values: [ point-to-point ] }
     passive: bool
 features:
   unnumbered:
     ipv4: IPv4 unnumbered interfaces
     ipv6: IPv6 unnumbered interfaces
     network: multi-access unnumbered links
+warnings:
+  inactive: True
```

### Comparing `networklab-1.8.1/netsim/modules/mpls.py` & `networklab-1.8.1.post1/netsim/modules/mpls.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/mpls.yml` & `networklab-1.8.1.post1/netsim/modules/mpls.yml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 # MPLS (LDP, BGP LU, L3VPN, 6PE) default settings and attributes
 #
+---
 config_after: [ vlan, ospf, isis, bgp ]
-transform_after: [ vlan, bgp ]
+transform_after: [ vlan, bgp, vrf ]
 ldp: True
 attributes:
   global:
     ldp:
       _alt_types: [ bool ]
       router_id: { type: ipv4, use: id }
       igp_sync: bool
```

### Comparing `networklab-1.8.1/netsim/modules/ospf.py` & `networklab-1.8.1.post1/netsim/modules/ospf.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,10 +124,10 @@
     # * Propagate OSPF attributes into loopback interface and VRFs
     #
     _routing.remove_unaddressed_intf(node,'ospf')
     _routing.build_vrf_interface_list(node,'ospf',topology)
     _routing.routing_af(node,'ospf')
     _routing.remove_vrf_routing_blocks(node,'ospf')
     propagate_node_attributes(node,topology)
-    _routing.remove_unused_igp(node,'ospf')
+    _routing.remove_unused_igp(node,'ospf',topology.defaults.get('ospf.warnings.inactive',False))
     _routing.check_vrf_protocol_support(node,'ospf','ipv4','ospfv2',topology)
     _routing.check_vrf_protocol_support(node,'ospf','ipv6','ospfv3',topology)
```

### Comparing `networklab-1.8.1/netsim/modules/ospf.yml` & `networklab-1.8.1.post1/netsim/modules/ospf.yml`

 * *Files 14% similar despite different names*

```diff
@@ -38,7 +38,9 @@
     area: { type: ipv4, use: id }
     bfd: bool
     passive: bool
     network_type: { type: str, valid_values: [ point-to-point, point-to-multipoint, broadcast, non-broadcast ] }
 features:
   unnumbered: Can run OSPFv2 over unnumbered IPv4 interfaces
   strict_bfd: Supports strict BFD mode (RFC 9355)
+warnings:
+  inactive: True
```

### Comparing `networklab-1.8.1/netsim/modules/srv6.py` & `networklab-1.8.1.post1/netsim/modules/srv6.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/vlan.py` & `networklab-1.8.1.post1/netsim/modules/vlan.py`

 * *Files 1% similar despite different names*

```diff
@@ -1024,14 +1024,40 @@
         f'Device type {node.device} does not support mixed bridged/routed VLAN trunks\n'+ \
         f'... node {node.name} interface {parent_intf.ifname}: {parent_intf.name}',
         log.IncorrectValue,
         'vlan')
     err_ifmap[parent_intf.ifindex] = True
 
 """
+Another scenario that can trip us is a native routed VLAN combined with bridged VLAN trunk.
+This works well on devices acting as routers, and fails consistently on devices that use
+the l3-switch model.
+"""
+def check_mixed_native_trunk(node: Box, topology: Box) -> None:
+  features = devices.get_device_features(node,topology.defaults)
+  if not 'switch' in features.vlan.model:                             # Device is not using 'switch' model, we're OK
+    return
+
+  for intf in node.interfaces:                                        # Check all interfaces
+    if intf.get('virtual_interface',False):                           # Skip the virtual ones
+      continue
+
+    if 'ipv4' not in intf and 'ipv6' not in intf:                     # Skip interfaces that don't do routing on
+      continue                                                        # ... native VLAN
+
+    if not intf.get('vlan.trunk_id',[]):                              # Skip interfaces that don't have a trunk of
+      continue                                                        # ... bridged VLANs
+
+    log.error(
+      f'Device type {node.device} (node {node.name}) cannot have a routed native VLAN with a bridged trunk',
+      category=log.IncorrectValue,
+      module='vlan',
+      more_data=f'Found on interface {intf.ifname} ({intf.name})')
+
+"""
 fix_vlan_gateways -- set VLAN-wide gateway IP
 
 The link augmentation code sets gateway IP for hosts connected to physical links. That approach does not work
 for VLAN subnets stretched across multiple physical links. We have to fix that here based on host neighbor list.
 
 We have to do a two-step process because the first-hop gateway is not applied consistently on every segment of the 
 VLAN (because a VLAN is modeled as a number of link).
@@ -1254,14 +1280,15 @@
       if 'vlan' in n.get('module',[]):
         populate_node_vlan_data(n,topology)
         vlan_ifmap = create_svi_interfaces(n,topology)
         map_trunk_vlans(n,topology)
         rename_vlan_subinterfaces(n,topology)
         cleanup_routed_native_vlan(n,topology)
         check_mixed_trunks(n,topology)
+        check_mixed_native_trunk(n,topology)
 
     for n in topology.nodes.values():
       set_svi_neighbor_list(n,topology)
 
     topology.links = [ link for link in topology.links if link.type != 'vlan_member' ]
 
     cleanup_vlan_flags(topology)
```

### Comparing `networklab-1.8.1/netsim/modules/vlan.yml` & `networklab-1.8.1.post1/netsim/modules/vlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/vrf.py` & `networklab-1.8.1.post1/netsim/modules/vrf.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,24 +27,30 @@
   else:
     node_data = node.vrfs[vname]                      # We have some node VRF data, and we assume it's a Box
     topo_data = topo_data or {}                       # Global data must be a dict/Box or the merge will fail
     return topo_data + node_data                      # Now merge global+node data
                                                       # ... note that the result will always be a Box
 
 #
-# Build the global data structures needed for ID/RD allocation and populate
-# them with preconfigured global- and node VRF data
+# Initialize global data structures needed for ID/RD allocation
 #
-def populate_vrf_static_ids(topology: Box) -> None:
+
+def init_vrf_static_ids(topology: Box) -> None:
   for k in ('id','rd'):
     _dataplane.create_id_set(f'vrf_{k}')
-    _dataplane.extend_id_set(f'vrf_{k}',_dataplane.build_id_set(topology,'vrfs',k,'topology'))
 
   _dataplane.set_id_counter('vrf_id',1,4095)
 
+#
+# Populate the global ID/RD/RT data structures with preconfigured global- and node VRF data
+#
+def populate_vrf_static_ids(topology: Box) -> None:
+  for k in ('id','rd'):
+    _dataplane.extend_id_set(f'vrf_{k}',_dataplane.build_id_set(topology,'vrfs',k,'topology'))
+
   for n in topology.nodes.values():
     for k in ('id','rd'):
       _dataplane.extend_id_set(f'vrf_{k}',_dataplane.build_id_set(n,'vrfs',k,f'nodes.{n.name}'))
 
 #
 # Get a usable AS number. Try bgp.as then vrf.as from node and global settings
 #
@@ -390,14 +396,16 @@
 
   # Note: validation of 'vrfs' dictionary has already been done during top-level element validation
   def module_pre_transform(self, topology: Box) -> None:
 
     if 'groups' in topology:
       groups.export_group_node_data(topology,'vrfs','vrf',copy_keys=['rd','export','import'])
 
+    init_vrf_static_ids(topology)
+
     if not 'vrfs' in topology:                          # No global VRFs, nothing to do
       return
 
     create_vrf_links(topology)                          # Create VRF links (and remove 'links' attribute)
     log.exit_on_error()
     normalize_vrf_ids(topology)
     populate_vrf_static_ids(topology)
@@ -454,53 +462,70 @@
         node.vrfs[vname] = topology.vrfs[vname] + node.vrfs[vname]      # ... and do the data merge
 
   def node_post_transform(self, node: Box, topology: Box) -> None:
     vrf_count = 0
 
     for ifdata in node.interfaces:
       if 'vrf' in ifdata:
-        vrf_count = vrf_count + 1
+        vrf_count += 1
         if not node.vrfs[ifdata.vrf].rd:
           log.error(
             f'VRF {ifdata.vrf} used on an interface in {node.name} does not have a usable RD',
             log.MissingValue,
             'vrf')
           continue
 
         for af in ['v4','v6']:
           if f'ip{af}' in ifdata:
             node.af[f'vpn{af}'] = True
             node.vrfs[ifdata.vrf].af[f'ip{af}'] = True
 
+    vrf_lb = node.get('vrf.loopback',False)
+    for vdata in node.get('vrfs',{}).values():
+      if 'loopback' in vdata or vrf_lb:
+        vrf_count += 1
+
     if log.debug_active('vrf'):
-      print( f"vrf node_post_transform on {node.name}: counted {vrf_count} VRFs on interfaces" )
+      print( f"vrf node_post_transform on {node.name}: counted {vrf_count} VRFs on interfaces/loopbacks" )
     features = devices.get_device_features(node,topology.defaults)
-    if not vrf_count and ('vrf' not in features or not features.vrf.keep_module): # Remove VRF module from the node if the node has no VRFs, unless flag set
-      node.module = [ m for m in node.module if m != 'vrf' ]
-      node.pop('vrfs',None)
-    else:
-      node.vrfs = node.vrfs or {}     # ... otherwise make sure the 'vrfs' dictionary is not empty
-      vrfidx = 100
 
-      # Check that all VRFs have a well-defined data structure (should be at this point, unless someone used groups.node_data)
-      for k,v in node.vrfs.items():
-        if v is None or not 'id' in v:
-          log.error(
-            f"Found invalid VRF {k} on node {node.name}. Did you mention it only in groups.node_data? You can't do that.",
-            log.IncorrectValue,
-            'vrf')
-          log.exit_on_error()
+    # Do we have any need for the VRF module?
+    if not vrf_count:
+      if topology.defaults.get('vrf.warnings.inactive',False):
+        log.error(
+          f"Node {node.name} uses no VRFs, removing 'vrf' from node modules",
+          category=Warning,
+          module='vrf',
+          hint='inactive')
+      # Remove VRF module from the node if the node has no VRFs, unless the vrf.keep_module flag is set
+      if not features.get('vrf.keep_module',False):
+        node.module = [ m for m in node.module if m != 'vrf' ]
+        node.pop('vrfs',None)
+      
+      return
+
+    node.vrfs = node.vrfs or {}     # ... otherwise make sure the 'vrfs' dictionary is not empty
+    vrfidx = 100
+
+    # Check that all VRFs have a well-defined data structure (should be at this point, unless someone used groups.node_data)
+    for k,v in node.vrfs.items():
+      if v is None or not 'id' in v:
+        log.error(
+          f"Found invalid VRF {k} on node {node.name}. Did you mention it only in groups.node_data? You can't do that.",
+          log.IncorrectValue,
+          'vrf')
+        log.exit_on_error()
 
-      # We need unique VRF index to create OSPF processes, assign in order sorted by VRF ID "for consistency"
-      for v in sorted(node.vrfs.values(),key=lambda v: v.id):
-        v.vrfidx = vrfidx
-        vrfidx = vrfidx + 1
+    # We need unique VRF index to create OSPF processes, assign in order sorted by VRF ID "for consistency"
+    for v in sorted(node.vrfs.values(),key=lambda v: v.id):
+      v.vrfidx = vrfidx
+      vrfidx = vrfidx + 1
 
-      validate_vrf_route_leaking(node)
+    validate_vrf_route_leaking(node)
 
-      # Set additional loopbacks (one for each defined VRF)
-      vrf_loopbacks(node, topology)
+    # Set additional loopbacks (one for each defined VRF)
+    vrf_loopbacks(node, topology)
 
     # Finally, set BGP router ID if we set BGP AS number
     #
     if node.get('bgp.as',None) and not node.get('bgp.router_id',None):
       _routing.router_id(node,'bgp',topology.pools)
```

### Comparing `networklab-1.8.1/netsim/modules/vrf.yml` & `networklab-1.8.1.post1/netsim/modules/vrf.yml`

 * *Files 12% similar despite different names*

```diff
@@ -1,21 +1,24 @@
 # VRF default settings and attributes
 #
+---
 config_after: [ vlan, ospf, isis, bgp, mpls ]
 transform_after: [ vlan, bgp ]
 as: 65000
 attributes:
   global:
     as: asn
     loopback: bool
   node:
     as:
     loopback:
   link: id
   interface: id
+warnings:
+  inactive: True
 _top:                               # Modification of global defaults
   attributes:
     vrf:                            # Define the VRF object type
       _description: Global or node-level VRF definition
       rd: rd
       import: list
       export: list
@@ -30,8 +33,8 @@
         _keytype: id                # ... where the VRF names must be valid identifiers
         _requires: [ vrf ]          # ... that requires VRF module
     node:
       vrfs:                         # Repeat the definition for node vrfs
         type: dict
         _subtype: vrf
         _keytype: id
-        _requires: [ vrf ]
+        _requires: [ vrf ]
```

### Comparing `networklab-1.8.1/netsim/modules/vxlan.py` & `networklab-1.8.1.post1/netsim/modules/vxlan.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/modules/vxlan.yml` & `networklab-1.8.1.post1/netsim/modules/vxlan.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/__init__.py` & `networklab-1.8.1.post1/netsim/outputs/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/ansible.py` & `networklab-1.8.1.post1/netsim/outputs/ansible.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/common.py` & `networklab-1.8.1.post1/netsim/outputs/common.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/d2.py` & `networklab-1.8.1.post1/netsim/outputs/d2.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/d2.yml` & `networklab-1.8.1.post1/netsim/outputs/d2.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/devices.py` & `networklab-1.8.1.post1/netsim/outputs/devices.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/graph.py` & `networklab-1.8.1.post1/netsim/outputs/graph.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/graphite.py` & `networklab-1.8.1.post1/netsim/outputs/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/provider.py` & `networklab-1.8.1.post1/netsim/outputs/provider.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/report.py` & `networklab-1.8.1.post1/netsim/outputs/report.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/tools.py` & `networklab-1.8.1.post1/netsim/outputs/tools.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/outputs/yaml.py` & `networklab-1.8.1.post1/netsim/outputs/yaml.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/providers/__init__.py` & `networklab-1.8.1.post1/netsim/providers/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/providers/clab.py` & `networklab-1.8.1.post1/netsim/providers/clab.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/providers/clab.yml` & `networklab-1.8.1.post1/netsim/providers/clab.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/providers/external.py` & `networklab-1.8.1.post1/netsim/providers/external.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/providers/libvirt.py` & `networklab-1.8.1.post1/netsim/providers/libvirt.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/providers/libvirt.yml` & `networklab-1.8.1.post1/netsim/providers/libvirt.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/clab/clab.j2` & `networklab-1.8.1.post1/netsim/templates/provider/clab/clab.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/clab/cumulus/hosts.j2` & `networklab-1.8.1.post1/netsim/templates/provider/clab/cumulus/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/clab/frr/daemons.j2` & `networklab-1.8.1.post1/netsim/templates/provider/clab/frr/daemons.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/clab/frr/hosts.j2` & `networklab-1.8.1.post1/netsim/templates/provider/clab/frr/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/clab/linux/hosts.j2` & `networklab-1.8.1.post1/netsim/templates/provider/clab/linux/hosts.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/external/external.j2` & `networklab-1.8.1.post1/netsim/templates/provider/external/external.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/Vagrantfile.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/cumulus_nvue-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/define-domain.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/define-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/iosxr-domain.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/iosxr-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-bridge.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-bridge.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/libvirt-tunnel.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/libvirt-tunnel.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/nxos-domain.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/nxos-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/vagrant-libvirt.xml` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/vagrant-libvirt.xml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/vptx-domain.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/vptx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/libvirt/vsrx-domain.j2` & `networklab-1.8.1.post1/netsim/templates/provider/libvirt/vsrx-domain.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/templates/provider/virtualbox/Vagrantfile.j2` & `networklab-1.8.1.post1/netsim/templates/provider/virtualbox/Vagrantfile.j2`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/tools/__init__.py` & `networklab-1.8.1.post1/netsim/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/tools/graphite.py` & `networklab-1.8.1.post1/netsim/tools/graphite.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/tools/graphite.yml` & `networklab-1.8.1.post1/netsim/tools/graphite.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/tools/suzieq.yml` & `networklab-1.8.1.post1/netsim/tools/suzieq.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/topology-defaults.yml` & `networklab-1.8.1.post1/netsim/topology-defaults.yml`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/bgp.py` & `networklab-1.8.1.post1/netsim/utils/bgp.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/callback.py` & `networklab-1.8.1.post1/netsim/utils/callback.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/files.py` & `networklab-1.8.1.post1/netsim/utils/files.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/log.py` & `networklab-1.8.1.post1/netsim/utils/log.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/read.py` & `networklab-1.8.1.post1/netsim/utils/read.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/sort.py` & `networklab-1.8.1.post1/netsim/utils/sort.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/status.py` & `networklab-1.8.1.post1/netsim/utils/status.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/strings.py` & `networklab-1.8.1.post1/netsim/utils/strings.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/templates.py` & `networklab-1.8.1.post1/netsim/utils/templates.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/utils/versioning.py` & `networklab-1.8.1.post1/netsim/utils/versioning.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/netsim/validate/linux.py` & `networklab-1.8.1.post1/netsim/validate/linux.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/networklab.egg-info/PKG-INFO` & `networklab-1.8.1.post1/networklab.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: networklab
-Version: 1.8.1
+Version: 1.8.1.post1
 Summary: CLI-based Virtual Networking Lab Abstraction Layer
 Home-page: https://github.com/ipspace/netlab
 Author: Ivan Pepelnjak
 Author-email: ip@ipspace.net
 Classifier: Topic :: Utilities
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -40,15 +40,15 @@
 
 Instead of wasting time creating lab topology in a GUI and configuring boring details, you'll start with a lab preconfigured according to your specifications.
 
 Interested? [Read the documentation](https://netlab.tools) and [installation guidelines](https://netlab.tools/install/).
 
 ## Releases
 
-The latest release is [release 1.8.1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
+The latest release is [release 1.8.1-post1](https://github.com/ipspace/netlab/releases/tag/release_1.8.1-post1), and as always, it might have a few bugs. Should you encounter one of those creatures, please report it with [a GitHub issue](https://github.com/ipspace/netlab/issues/new/choose) and use release [1.8.0](https://github.com/ipspace/netlab/releases/tag/release_1.8.0) or [1.7.2](https://github.com/ipspace/netlab/releases/tag/release_1.7.2).
 
 <!--
 If you encounter bugs using release 1.7.x, please downgrade to [1.6.4](https://github.com/ipspace/netlab/releases/tag/release_1.6.4) and [open a GitHub issue](https://github.com/ipspace/netlab/issues).
 -->
 
 ## An Overview of CLI Commands
```

### Comparing `networklab-1.8.1/networklab.egg-info/SOURCES.txt` & `networklab-1.8.1.post1/networklab.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/setup.py` & `networklab-1.8.1.post1/setup.py`

 * *Files identical despite different names*

### Comparing `networklab-1.8.1/tests/test_transformation.py` & `networklab-1.8.1.post1/tests/test_transformation.py`

 * *Files identical despite different names*

