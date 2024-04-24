# Comparing `tmp/catalyst_sdwan_lab-2.0.6.tar.gz` & `tmp/catalyst_sdwan_lab-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catalyst_sdwan_lab-2.0.6.tar", max compression
+gzip compressed data, was "catalyst_sdwan_lab-2.0.7.tar", max compression
```

## Comparing `catalyst_sdwan_lab-2.0.6.tar` & `catalyst_sdwan_lab-2.0.7.tar`

### file list

```diff
@@ -1,434 +1,434 @@
--rw-r--r--   0        0        0     1516 2024-04-16 08:33:04.603981 catalyst_sdwan_lab-2.0.6/LICENSE
--rw-r--r--   0        0        0    19229 2024-04-16 15:57:51.063863 catalyst_sdwan_lab-2.0.6/README.md
--rw-r--r--   0        0        0      357 2024-04-16 08:33:04.604676 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/__init__.py
--rw-r--r--   0        0        0    20068 2024-04-16 08:33:04.604869 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/__main__.py
--rwxr-xr-x   0        0        0      443 2024-04-16 08:33:04.605268 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/cacsr_details.txt
--rw-r--r--   0        0        0     3033 2024-04-16 08:33:04.605371 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/chainCA.pem
--rwxr-xr-x   0        0        0      790 2024-04-16 08:33:04.605466 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/openssl-commands.md
--rw-r--r--   0        0        0     1517 2024-04-16 08:33:04.605558 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/rootCA.pem
--rw-r--r--   0        0        0       17 2024-04-16 08:33:04.605641 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/rootCA.srl
--rwxr-xr-x   0        0        0      485 2024-04-16 08:33:04.605726 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/rootca_details.txt
--rw-r--r--   0        0        0     1074 2024-04-16 08:33:04.605816 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/signCA.csr
--rw-r--r--   0        0        0     1675 2024-04-16 08:33:04.605901 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/signCA.key
--rw-r--r--   0        0        0     1517 2024-04-16 08:33:04.605993 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/signCA.pem
--rwxr-xr-x   0        0        0      352 2024-04-16 08:33:04.606080 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/v3ext.cnf
--rw-r--r--   0        0        0      421 2024-04-16 08:33:04.606291 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/controller-cloud-init.j2
--rw-r--r--   0        0        0      851 2024-04-16 08:33:04.606406 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2
--rw-r--r--   0        0        0      523 2024-04-16 08:33:04.606490 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2
--rw-r--r--   0        0        0      895 2024-04-16 08:33:04.606567 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2
--rw-r--r--   0        0        0      415 2024-04-16 08:33:04.606646 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/validator-cloud-init.j2
--rw-r--r--   0        0        0    16330 2024-04-17 10:52:48.959748 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2
--rw-r--r--   0        0        0     2292 2024-04-16 08:33:04.606928 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2
--rw-r--r--   0        0        0     3182 2024-04-16 08:33:04.607005 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2
--rw-r--r--   0        0        0     1383 2024-04-16 08:33:04.607080 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2
--rw-r--r--   0        0        0     2327 2024-04-16 08:33:04.607158 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2
--rw-r--r--   0        0        0     2087 2024-04-16 08:33:04.607310 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml
--rw-r--r--   0        0        0     1981 2024-04-16 08:33:04.607407 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml
--rw-r--r--   0        0        0     2094 2024-04-16 14:01:04.557230 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml
--rw-r--r--   0        0        0     2097 2024-04-16 08:33:04.607580 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml
--rw-r--r--   0        0        0     1859 2024-04-16 08:33:04.607903 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1866 2024-04-16 08:33:04.608015 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
--rw-r--r--   0        0        0     1833 2024-04-16 08:33:04.608123 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1736 2024-04-16 08:33:04.608220 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
--rw-r--r--   0        0        0     1702 2024-04-16 08:33:04.608316 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
--rw-r--r--   0        0        0     1910 2024-04-16 08:33:04.608408 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
--rw-r--r--   0        0        0     1686 2024-04-16 08:33:04.608503 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1615 2024-04-16 08:33:04.608610 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2516 2024-04-16 08:33:04.608695 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2510 2024-04-16 08:33:04.608788 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
--rw-r--r--   0        0        0     2293 2024-04-16 08:33:04.608891 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
--rw-r--r--   0        0        0     2657 2024-04-16 08:33:04.608985 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
--rw-r--r--   0        0        0     2365 2024-04-16 08:33:04.609081 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
--rw-r--r--   0        0        0     3215 2024-04-16 08:33:04.609191 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json
--rw-r--r--   0        0        0     2924 2024-04-16 08:33:04.609293 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json
--rw-r--r--   0        0        0     2260 2024-04-16 08:33:04.609391 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json
--rw-r--r--   0        0        0     1347 2024-04-16 08:33:04.609479 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json
--rw-r--r--   0        0        0     2454 2024-04-16 08:33:04.609588 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json
--rw-r--r--   0        0        0    19645 2024-04-16 08:33:04.609801 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
--rw-r--r--   0        0        0     7062 2024-04-16 08:33:04.610024 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24745 2024-04-16 08:33:04.610164 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5515 2024-04-16 08:33:04.610516 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
--rw-r--r--   0        0        0    12013 2024-04-16 08:33:04.610663 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5591 2024-04-16 08:33:04.610789 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
--rw-r--r--   0        0        0     6135 2024-04-16 08:33:04.610909 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24962 2024-04-16 08:33:04.611041 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0    11984 2024-04-16 08:33:04.611170 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5492 2024-04-16 08:33:04.611281 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5564 2024-04-16 08:33:04.611390 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     3456 2024-04-16 08:33:04.611528 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json
--rw-r--r--   0        0        0    19638 2024-04-16 08:33:04.611720 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
--rw-r--r--   0        0        0     9573 2024-04-16 08:33:04.611873 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
--rw-r--r--   0        0        0    12289 2024-04-16 08:33:04.611990 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
--rw-r--r--   0        0        0     8173 2024-04-16 08:33:04.612121 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json
--rw-r--r--   0        0        0     2216 2024-04-16 08:33:04.612238 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json
--rw-r--r--   0        0        0     6228 2024-04-16 08:33:04.612343 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json
--rw-r--r--   0        0        0     1607 2024-04-16 08:33:04.612434 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json
--rw-r--r--   0        0        0    22837 2024-04-16 08:33:04.612542 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
--rw-r--r--   0        0        0    10441 2024-04-16 08:33:04.612664 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
--rw-r--r--   0        0        0    22817 2024-04-16 08:33:04.612772 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
--rw-r--r--   0        0        0    22819 2024-04-16 08:33:04.612892 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
--rw-r--r--   0        0        0    10419 2024-04-16 08:33:04.613025 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
--rw-r--r--   0        0        0    18079 2024-04-16 08:33:04.613143 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
--rw-r--r--   0        0        0    11073 2024-04-16 08:33:04.613272 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
--rw-r--r--   0        0        0    11073 2024-04-16 08:33:04.613370 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
--rw-r--r--   0        0        0    11073 2024-04-16 08:33:04.613472 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
--rw-r--r--   0        0        0    11095 2024-04-16 08:33:04.613574 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
--rw-r--r--   0        0        0    11071 2024-04-16 08:33:04.613676 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
--rw-r--r--   0        0        0    11071 2024-04-16 08:33:04.613777 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
--rw-r--r--   0        0        0    11075 2024-04-16 08:33:04.613866 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
--rw-r--r--   0        0        0    11071 2024-04-16 08:33:04.613957 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
--rw-r--r--   0        0        0     7066 2024-04-16 08:33:04.614060 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25121 2024-04-16 08:33:04.614191 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
--rw-r--r--   0        0        0     7603 2024-04-16 08:33:04.614364 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
--rw-r--r--   0        0        0     5572 2024-04-16 08:33:04.614482 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
--rw-r--r--   0        0        0    11992 2024-04-16 08:33:04.614613 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
--rw-r--r--   0        0        0     7025 2024-04-16 08:33:04.614730 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24720 2024-04-16 08:33:04.614853 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5478 2024-04-16 08:33:04.614982 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5550 2024-04-16 08:33:04.615086 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     2144 2024-04-16 08:33:04.615181 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json
--rw-r--r--   0        0        0     7061 2024-04-16 08:33:04.615286 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25114 2024-04-16 08:33:04.615408 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5514 2024-04-16 08:33:04.615536 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     4915 2024-04-16 08:33:04.615787 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json
--rw-r--r--   0        0        0     6290 2024-04-16 08:33:04.615921 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json
--rw-r--r--   0        0        0    24529 2024-04-16 08:33:04.616062 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json
--rw-r--r--   0        0        0    12375 2024-04-16 08:33:04.616211 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    12084 2024-04-16 08:33:04.616326 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json
--rw-r--r--   0        0        0     5570 2024-04-16 08:33:04.616436 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    12106 2024-04-16 08:33:04.616551 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json
--rw-r--r--   0        0        0     8510 2024-04-16 08:33:04.616658 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10463 2024-04-16 08:33:04.616862 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json
--rw-r--r--   0        0        0    25674 2024-04-16 08:33:04.617017 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
--rw-r--r--   0        0        0    13302 2024-04-16 08:33:04.617159 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    13021 2024-04-16 08:33:04.617279 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
--rw-r--r--   0        0        0     4729 2024-04-16 08:33:04.617394 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    13047 2024-04-16 08:33:04.617515 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
--rw-r--r--   0        0        0     8131 2024-04-16 08:33:04.617629 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10082 2024-04-16 08:33:04.617734 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
--rw-r--r--   0        0        0     2191 2024-04-16 08:33:04.617843 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json
--rw-r--r--   0        0        0     5921 2024-04-16 08:33:04.617954 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json
--rw-r--r--   0        0        0     6998 2024-04-16 08:33:04.618060 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json
--rw-r--r--   0        0        0     4315 2024-04-16 08:33:04.618164 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json
--rw-r--r--   0        0        0     4323 2024-04-16 08:33:04.618269 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json
--rw-r--r--   0        0        0     6985 2024-04-16 08:33:04.618403 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json
--rw-r--r--   0        0        0    20010 2024-04-16 08:33:04.618542 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json
--rw-r--r--   0        0        0     3218 2024-04-16 08:33:04.618668 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
--rw-r--r--   0        0        0     7296 2024-04-16 08:33:04.618797 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
--rw-r--r--   0        0        0     1739 2024-04-16 08:33:04.618898 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json
--rw-r--r--   0        0        0     4104 2024-04-16 08:33:04.619001 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json
--rw-r--r--   0        0        0    14537 2024-04-16 08:33:04.619138 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
--rw-r--r--   0        0        0     4186 2024-04-16 08:33:04.619257 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json
--rw-r--r--   0        0        0     7502 2024-04-16 08:33:04.619367 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     4511 2024-04-16 08:33:04.619455 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json
--rw-r--r--   0        0        0     8107 2024-04-16 08:33:04.619562 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json
--rw-r--r--   0        0        0     4416 2024-04-16 08:33:04.619663 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
--rw-r--r--   0        0        0    13607 2024-04-16 08:33:04.619794 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
--rw-r--r--   0        0        0     4333 2024-04-16 08:33:04.619903 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
--rw-r--r--   0        0        0     3938 2024-04-16 08:33:04.619988 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
--rw-r--r--   0        0        0    27208 2024-04-16 08:33:04.620096 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
--rw-r--r--   0        0        0    25438 2024-04-16 08:33:04.620230 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
--rw-r--r--   0        0        0     8351 2024-04-16 08:33:04.620376 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json
--rw-r--r--   0        0        0     9978 2024-04-16 08:33:04.620521 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json
--rw-r--r--   0        0        0    11257 2024-04-16 08:33:04.620613 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
--rw-r--r--   0        0        0     4976 2024-04-16 08:33:04.620723 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json
--rw-r--r--   0        0        0    10714 2024-04-16 08:33:04.620840 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json
--rw-r--r--   0        0        0     2008 2024-04-16 08:33:04.620936 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json
--rw-r--r--   0        0        0    11386 2024-04-16 08:33:04.621056 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
--rw-r--r--   0        0        0    12016 2024-04-16 08:33:04.621166 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
--rw-r--r--   0        0        0     7360 2024-04-16 08:33:04.621291 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
--rw-r--r--   0        0        0     1303 2024-04-16 08:33:04.621398 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json
--rw-r--r--   0        0        0    11243 2024-04-16 08:33:04.621504 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json
--rw-r--r--   0        0        0    11964 2024-04-16 08:33:04.621603 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json
--rw-r--r--   0        0        0    11788 2024-04-16 08:33:04.621757 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
--rw-r--r--   0        0        0    14115 2024-04-16 08:33:04.621894 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
--rw-r--r--   0        0        0    12000 2024-04-16 08:33:04.621998 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
--rw-r--r--   0        0        0     6868 2024-04-16 08:33:04.622107 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
--rw-r--r--   0        0        0    25394 2024-04-16 08:33:04.622226 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
--rw-r--r--   0        0        0     9260 2024-04-16 08:33:04.622368 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json
--rw-r--r--   0        0        0    25074 2024-04-16 08:33:04.622489 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json
--rw-r--r--   0        0        0    31516 2024-04-16 08:33:04.622624 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
--rw-r--r--   0        0        0    24593 2024-04-16 08:33:04.622758 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
--rw-r--r--   0        0        0     4859 2024-04-16 08:33:04.622921 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json
--rw-r--r--   0        0        0     9400 2024-04-16 08:33:04.623057 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
--rw-r--r--   0        0        0     9394 2024-04-16 08:33:04.623172 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
--rw-r--r--   0        0        0    14686 2024-04-16 08:33:04.623343 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
--rw-r--r--   0        0        0    19630 2024-04-16 08:33:04.623453 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
--rw-r--r--   0        0        0     6475 2024-04-16 08:33:04.623577 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json
--rw-r--r--   0        0        0     3858 2024-04-16 08:33:04.623694 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json
--rw-r--r--   0        0        0     5138 2024-04-16 08:33:04.623843 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     2080 2024-04-16 08:33:04.623944 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
--rw-r--r--   0        0        0     5653 2024-04-16 08:33:04.624102 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json
--rw-r--r--   0        0        0     4099 2024-04-16 08:33:04.624207 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
--rw-r--r--   0        0        0     4106 2024-04-16 08:33:04.624308 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
--rw-r--r--   0        0        0     2608 2024-04-16 08:33:04.624412 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json
--rw-r--r--   0        0        0      984 2024-04-16 08:33:04.624523 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
--rw-r--r--   0        0        0     4382 2024-04-16 08:33:04.624668 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
--rw-r--r--   0        0        0     3155 2024-04-16 08:33:04.624800 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
--rw-r--r--   0        0        0     1442 2024-04-16 08:33:04.624902 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
--rw-r--r--   0        0        0    34849 2024-04-16 08:33:04.625085 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json
--rw-r--r--   0        0        0     5401 2024-04-16 08:33:04.625270 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json
--rw-r--r--   0        0        0    10612 2024-04-16 08:33:04.625380 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json
--rw-r--r--   0        0        0      868 2024-04-16 08:33:04.625484 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json
--rw-r--r--   0        0        0    12306 2024-04-16 08:33:04.625586 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json
--rw-r--r--   0        0        0    29668 2024-04-16 08:33:04.625707 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json
--rw-r--r--   0        0        0    27664 2024-04-16 08:33:04.625833 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json
--rw-r--r--   0        0        0     7826 2024-04-16 08:33:04.626110 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json
--rw-r--r--   0        0        0     3871 2024-04-16 08:33:04.626213 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json
--rw-r--r--   0        0        0    13751 2024-04-16 08:33:04.626336 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json
--rw-r--r--   0        0        0     9628 2024-04-16 08:33:04.626529 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json
--rw-r--r--   0        0        0   597414 2024-04-16 08:33:04.627507 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json
--rw-r--r--   0        0        0    14055 2024-04-16 08:33:04.627680 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json
--rw-r--r--   0        0        0     1317 2024-04-16 08:33:04.627778 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json
--rw-r--r--   0        0        0     3720 2024-04-16 08:33:04.627883 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json
--rw-r--r--   0        0        0      532 2024-04-16 08:33:04.628093 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json
--rw-r--r--   0        0        0      596 2024-04-16 08:33:04.628178 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json
--rw-r--r--   0        0        0     2748 2024-04-16 08:33:04.628297 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json
--rw-r--r--   0        0        0     1605 2024-04-16 08:33:04.628387 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json
--rw-r--r--   0        0        0      450 2024-04-16 08:33:04.628496 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/REAL_TIME_APPS.json
--rw-r--r--   0        0        0      386 2024-04-16 08:33:04.628593 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/VIDEO_CONF.json
--rw-r--r--   0        0        0      452 2024-04-16 08:33:04.628677 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/WEB_TOOLS_APP.json
--rw-r--r--   0        0        0      608 2024-04-16 08:33:04.628779 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json
--rw-r--r--   0        0        0      379 2024-04-16 08:33:04.628874 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/box_net_apps.json
--rw-r--r--   0        0        0      380 2024-04-16 08:33:04.628964 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/concur_apps.json
--rw-r--r--   0        0        0      383 2024-04-16 08:33:04.629051 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/dropbox_apps.json
--rw-r--r--   0        0        0      430 2024-04-16 08:33:04.629212 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/gotomeeting_apps.json
--rw-r--r--   0        0        0      380 2024-04-16 08:33:04.629313 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/intuit_apps.json
--rw-r--r--   0        0        0     1052 2024-04-16 08:33:04.629427 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json
--rw-r--r--   0        0        0      596 2024-04-16 08:33:04.629523 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json
--rw-r--r--   0        0        0      392 2024-04-16 08:33:04.629639 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/salesforce_apps.json
--rw-r--r--   0        0        0      388 2024-04-16 08:33:04.629727 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/sugar_crm_apps.json
--rw-r--r--   0        0        0      383 2024-04-16 08:33:04.629814 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zendesk_apps.json
--rw-r--r--   0        0        0      391 2024-04-16 08:33:04.629899 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zoho_crm_apps.json
--rw-r--r--   0        0        0      386 2024-04-16 08:33:04.630052 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Browsing.json
--rw-r--r--   0        0        0      375 2024-04-16 08:33:04.630151 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/ICMP.json
--rw-r--r--   0        0        0      428 2024-04-16 08:33:04.630260 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Yahoo.json
--rw-r--r--   0        0        0      415 2024-04-16 08:33:04.630416 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Best-Effort.json
--rw-r--r--   0        0        0      419 2024-04-16 08:33:04.630527 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Bulk-Data.json
--rw-r--r--   0        0        0      427 2024-04-16 08:33:04.630620 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Critical.json
--rw-r--r--   0        0        0      419 2024-04-16 08:33:04.630697 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Data.json
--rw-r--r--   0        0        0      415 2024-04-16 08:33:04.630781 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Default.json
--rw-r--r--   0        0        0      408 2024-04-16 08:33:04.630858 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Realtime.json
--rw-r--r--   0        0        0      435 2024-04-16 08:33:04.630954 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Transactional-Data.json
--rw-r--r--   0        0        0      428 2024-04-16 08:33:04.631060 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Voice-And-Video.json
--rw-r--r--   0        0        0       32 2024-04-16 08:33:04.631141 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/server_info.json
--rw-r--r--   0        0        0    15002 2024-04-16 08:33:04.631349 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json
--rw-r--r--   0        0        0     1628 2024-04-16 08:33:04.631544 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json
--rw-r--r--   0        0        0      295 2024-04-16 08:33:04.631720 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/attached/controller_basic.json
--rw-r--r--   0        0        0     1859 2024-04-16 08:33:04.631869 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1866 2024-04-16 08:33:04.631948 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
--rw-r--r--   0        0        0     1833 2024-04-16 08:33:04.632042 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1736 2024-04-16 08:33:04.632124 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
--rw-r--r--   0        0        0     1702 2024-04-16 08:33:04.632221 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
--rw-r--r--   0        0        0     1910 2024-04-16 08:33:04.632316 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
--rw-r--r--   0        0        0     1720 2024-04-16 08:33:04.632408 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1686 2024-04-16 08:33:04.632497 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json
--rw-r--r--   0        0        0     1615 2024-04-16 08:33:04.632616 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2516 2024-04-16 08:33:04.632712 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
--rw-r--r--   0        0        0     2510 2024-04-16 08:33:04.632835 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
--rw-r--r--   0        0        0     2293 2024-04-16 08:33:04.632941 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
--rw-r--r--   0        0        0     2657 2024-04-16 08:33:04.633058 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
--rw-r--r--   0        0        0     2365 2024-04-16 08:33:04.633182 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
--rw-r--r--   0        0        0     3207 2024-04-16 08:33:04.633280 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json
--rw-r--r--   0        0        0     2924 2024-04-16 08:33:04.633401 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json
--rw-r--r--   0        0        0     2260 2024-04-16 08:33:04.633506 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json
--rw-r--r--   0        0        0     1347 2024-04-16 08:33:04.633628 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json
--rw-r--r--   0        0        0     2454 2024-04-16 08:33:04.633749 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json
--rw-r--r--   0        0        0     4130 2024-04-16 08:33:04.633932 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json
--rw-r--r--   0        0        0      776 2024-04-16 08:33:04.634275 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json
--rw-r--r--   0        0        0     6189 2024-04-16 08:33:04.634429 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json
--rw-r--r--   0        0        0    12229 2024-04-16 08:33:04.634583 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json
--rw-r--r--   0        0        0    13293 2024-04-16 08:33:04.634727 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json
--rw-r--r--   0        0        0    20244 2024-04-16 08:33:04.634896 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
--rw-r--r--   0        0        0     7063 2024-04-16 08:33:04.635010 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24746 2024-04-16 08:33:04.635099 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5516 2024-04-16 08:33:04.635202 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
--rw-r--r--   0        0        0    12014 2024-04-16 08:33:04.635286 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5592 2024-04-16 08:33:04.635383 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
--rw-r--r--   0        0        0     6136 2024-04-16 08:33:04.635615 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24963 2024-04-16 08:33:04.635775 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0    11984 2024-04-16 08:33:04.635916 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     5493 2024-04-16 08:33:04.636021 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5565 2024-04-16 08:33:04.636123 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     3457 2024-04-16 08:33:04.636232 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json
--rw-r--r--   0        0        0    20238 2024-04-16 08:33:04.636359 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
--rw-r--r--   0        0        0    10172 2024-04-16 08:33:04.636482 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
--rw-r--r--   0        0        0    12888 2024-04-16 08:33:04.636597 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
--rw-r--r--   0        0        0     8773 2024-04-16 08:33:04.636706 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json
--rw-r--r--   0        0        0     2216 2024-04-16 08:33:04.636806 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json
--rw-r--r--   0        0        0     6229 2024-04-16 08:33:04.636935 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json
--rw-r--r--   0        0        0     1608 2024-04-16 08:33:04.637033 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json
--rw-r--r--   0        0        0    22838 2024-04-16 08:33:04.637156 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
--rw-r--r--   0        0        0    10442 2024-04-16 08:33:04.637276 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
--rw-r--r--   0        0        0    22818 2024-04-16 08:33:04.637391 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
--rw-r--r--   0        0        0    22820 2024-04-16 08:33:04.637537 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
--rw-r--r--   0        0        0    10420 2024-04-16 08:33:04.637661 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
--rw-r--r--   0        0        0    18100 2024-04-16 08:33:04.637772 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
--rw-r--r--   0        0        0    11094 2024-04-16 08:33:04.637914 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
--rw-r--r--   0        0        0    11094 2024-04-16 08:33:04.638019 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
--rw-r--r--   0        0        0    11094 2024-04-16 08:33:04.638137 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
--rw-r--r--   0        0        0    11115 2024-04-16 08:33:04.638259 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
--rw-r--r--   0        0        0    11091 2024-04-16 08:33:04.638386 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
--rw-r--r--   0        0        0    11092 2024-04-16 08:33:04.638510 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
--rw-r--r--   0        0        0    11095 2024-04-16 08:33:04.638626 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
--rw-r--r--   0        0        0    11092 2024-04-16 08:33:04.638720 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
--rw-r--r--   0        0        0     9231 2024-04-16 08:33:04.638829 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json
--rw-r--r--   0        0        0     7813 2024-04-16 08:33:04.638928 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0     9262 2024-04-16 08:33:04.639040 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json
--rw-r--r--   0        0        0    28713 2024-04-16 08:33:04.639167 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json
--rw-r--r--   0        0        0     7245 2024-04-16 08:33:04.639275 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     7067 2024-04-16 08:33:04.639377 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25122 2024-04-16 08:33:04.639519 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
--rw-r--r--   0        0        0     7604 2024-04-16 08:33:04.639637 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
--rw-r--r--   0        0        0     5573 2024-04-16 08:33:04.639736 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
--rw-r--r--   0        0        0    11993 2024-04-16 08:33:04.639830 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
--rw-r--r--   0        0        0     7026 2024-04-16 08:33:04.639927 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    24721 2024-04-16 08:33:04.640022 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5479 2024-04-16 08:33:04.640122 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     5551 2024-04-16 08:33:04.640209 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json
--rw-r--r--   0        0        0     2145 2024-04-16 08:33:04.640309 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json
--rw-r--r--   0        0        0     7062 2024-04-16 08:33:04.640423 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
--rw-r--r--   0        0        0    25115 2024-04-16 08:33:04.640532 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
--rw-r--r--   0        0        0     5515 2024-04-16 08:33:04.640640 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
--rw-r--r--   0        0        0     4936 2024-04-16 08:33:04.640739 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json
--rw-r--r--   0        0        0     6311 2024-04-16 08:33:04.640844 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json
--rw-r--r--   0        0        0    24530 2024-04-16 08:33:04.640947 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json
--rw-r--r--   0        0        0    12376 2024-04-16 08:33:04.641065 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    12085 2024-04-16 08:33:04.641162 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json
--rw-r--r--   0        0        0     5570 2024-04-16 08:33:04.641255 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    12106 2024-04-16 08:33:04.641353 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json
--rw-r--r--   0        0        0     8511 2024-04-16 08:33:04.641454 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10464 2024-04-16 08:33:04.641548 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json
--rw-r--r--   0        0        0    25675 2024-04-16 08:33:04.641655 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
--rw-r--r--   0        0        0    13303 2024-04-16 08:33:04.641834 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
--rw-r--r--   0        0        0    13022 2024-04-16 08:33:04.641965 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
--rw-r--r--   0        0        0     4730 2024-04-16 08:33:04.642084 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
--rw-r--r--   0        0        0    13048 2024-04-16 08:33:04.642229 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
--rw-r--r--   0        0        0     8132 2024-04-16 08:33:04.642342 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
--rw-r--r--   0        0        0    10083 2024-04-16 08:33:04.642461 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
--rw-r--r--   0        0        0     2192 2024-04-16 08:33:04.642563 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json
--rw-r--r--   0        0        0     5922 2024-04-16 08:33:04.642657 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json
--rw-r--r--   0        0        0     7019 2024-04-16 08:33:04.642754 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json
--rw-r--r--   0        0        0     4336 2024-04-16 08:33:04.642847 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json
--rw-r--r--   0        0        0     4343 2024-04-16 08:33:04.642943 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json
--rw-r--r--   0        0        0     7211 2024-04-16 08:33:04.643090 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json
--rw-r--r--   0        0        0    20011 2024-04-16 08:33:04.643202 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json
--rw-r--r--   0        0        0     3219 2024-04-16 08:33:04.643319 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
--rw-r--r--   0        0        0     7321 2024-04-16 08:33:04.643420 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
--rw-r--r--   0        0        0     1740 2024-04-16 08:33:04.643507 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json
--rw-r--r--   0        0        0     4330 2024-04-16 08:33:04.643598 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json
--rw-r--r--   0        0        0    14763 2024-04-16 08:33:04.643714 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
--rw-r--r--   0        0        0     4412 2024-04-16 08:33:04.643810 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json
--rw-r--r--   0        0        0     7728 2024-04-16 08:33:04.643909 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     4737 2024-04-16 08:33:04.644013 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json
--rw-r--r--   0        0        0     8333 2024-04-16 08:33:04.644123 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json
--rw-r--r--   0        0        0     4642 2024-04-16 08:33:04.644227 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
--rw-r--r--   0        0        0    13632 2024-04-16 08:33:04.644373 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
--rw-r--r--   0        0        0     4561 2024-04-16 08:33:04.644480 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
--rw-r--r--   0        0        0     3938 2024-04-16 08:33:04.644586 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
--rw-r--r--   0        0        0    27208 2024-04-16 08:33:04.644692 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
--rw-r--r--   0        0        0    25439 2024-04-16 08:33:04.645103 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
--rw-r--r--   0        0        0     8352 2024-04-16 08:33:04.645216 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json
--rw-r--r--   0        0        0     9978 2024-04-16 08:33:04.645338 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json
--rw-r--r--   0        0        0    11258 2024-04-16 08:33:04.645456 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
--rw-r--r--   0        0        0     5397 2024-04-16 08:33:04.645563 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json
--rw-r--r--   0        0        0    10940 2024-04-16 08:33:04.645683 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json
--rw-r--r--   0        0        0     2008 2024-04-16 08:33:04.645780 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json
--rw-r--r--   0        0        0    11387 2024-04-16 08:33:04.645912 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
--rw-r--r--   0        0        0    12016 2024-04-16 08:33:04.646019 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
--rw-r--r--   0        0        0     7360 2024-04-16 08:33:04.646123 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
--rw-r--r--   0        0        0     1304 2024-04-16 08:33:04.646240 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json
--rw-r--r--   0        0        0    11244 2024-04-16 08:33:04.646359 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json
--rw-r--r--   0        0        0    11965 2024-04-16 08:33:04.646457 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json
--rw-r--r--   0        0        0    11789 2024-04-16 08:33:04.646556 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
--rw-r--r--   0        0        0    14116 2024-04-16 08:33:04.646667 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
--rw-r--r--   0        0        0    12001 2024-04-16 08:33:04.646792 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
--rw-r--r--   0        0        0     6868 2024-04-16 08:33:04.646896 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
--rw-r--r--   0        0        0    25394 2024-04-16 08:33:04.647004 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
--rw-r--r--   0        0        0     9261 2024-04-16 08:33:04.647112 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json
--rw-r--r--   0        0        0    25075 2024-04-16 08:33:04.647212 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json
--rw-r--r--   0        0        0    31517 2024-04-16 08:33:04.647351 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
--rw-r--r--   0        0        0    24594 2024-04-16 08:33:04.647467 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
--rw-r--r--   0        0        0     4905 2024-04-16 08:33:04.647571 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json
--rw-r--r--   0        0        0     9401 2024-04-16 08:33:04.647694 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
--rw-r--r--   0        0        0     9395 2024-04-16 08:33:04.647800 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
--rw-r--r--   0        0        0    14687 2024-04-16 08:33:04.647933 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
--rw-r--r--   0        0        0    19631 2024-04-16 08:33:04.648026 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
--rw-r--r--   0        0        0     6476 2024-04-16 08:33:04.648133 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json
--rw-r--r--   0        0        0     3859 2024-04-16 08:33:04.648224 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json
--rw-r--r--   0        0        0     5139 2024-04-16 08:33:04.648304 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
--rw-r--r--   0        0        0     2081 2024-04-16 08:33:04.648376 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
--rw-r--r--   0        0        0     5654 2024-04-16 08:33:04.648485 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json
--rw-r--r--   0        0        0     4100 2024-04-16 08:33:04.648610 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
--rw-r--r--   0        0        0     4109 2024-04-16 08:33:04.648720 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
--rw-r--r--   0        0        0     2609 2024-04-16 08:33:04.648818 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json
--rw-r--r--   0        0        0      985 2024-04-16 08:33:04.648934 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
--rw-r--r--   0        0        0     4383 2024-04-16 08:33:04.649028 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
--rw-r--r--   0        0        0     3156 2024-04-16 08:33:04.649147 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
--rw-r--r--   0        0        0     1443 2024-04-16 08:33:04.649242 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
--rw-r--r--   0        0        0    34850 2024-04-16 08:33:04.649382 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json
--rw-r--r--   0        0        0     5402 2024-04-16 08:33:04.649481 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json
--rw-r--r--   0        0        0    10613 2024-04-16 08:33:04.649567 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json
--rw-r--r--   0        0        0      869 2024-04-16 08:33:04.649651 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json
--rw-r--r--   0        0        0    12307 2024-04-16 08:33:04.649816 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json
--rw-r--r--   0        0        0    29670 2024-04-16 08:33:04.649971 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json
--rw-r--r--   0        0        0    27666 2024-04-16 08:33:04.650119 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json
--rw-r--r--   0        0        0     7827 2024-04-16 08:33:04.650237 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json
--rw-r--r--   0        0        0     3872 2024-04-16 08:33:04.650337 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json
--rw-r--r--   0        0        0    13753 2024-04-16 08:33:04.650431 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json
--rw-r--r--   0        0        0     1760 2024-04-16 08:33:04.650567 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json
--rw-r--r--   0        0        0    10179 2024-04-16 08:33:04.650656 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json
--rw-r--r--   0        0        0      316 2024-04-16 08:33:04.650799 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_cli.json
--rw-r--r--   0        0        0      320 2024-04-16 08:33:04.650926 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_service.json
--rw-r--r--   0        0        0      322 2024-04-16 08:33:04.651026 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_system.json
--rw-r--r--   0        0        0      322 2024-04-16 08:33:04.651136 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_transport.json
--rw-r--r--   0        0        0   628759 2024-04-16 08:33:04.655299 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json
--rw-r--r--   0        0        0    20494 2024-04-16 08:33:04.655912 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json
--rw-r--r--   0        0        0     1215 2024-04-16 08:33:04.656041 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json
--rw-r--r--   0        0        0     3440 2024-04-16 08:33:04.656144 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json
--rw-r--r--   0        0        0      532 2024-04-16 08:33:04.656328 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json
--rw-r--r--   0        0        0      596 2024-04-16 08:33:04.656429 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json
--rw-r--r--   0        0        0     3010 2024-04-16 08:33:04.656506 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json
--rw-r--r--   0        0        0      904 2024-04-16 08:33:04.656588 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json
--rw-r--r--   0        0        0     1605 2024-04-16 08:33:04.656664 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json
--rw-r--r--   0        0        0      450 2024-04-16 08:33:04.656746 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/REAL_TIME_APPS.json
--rw-r--r--   0        0        0      386 2024-04-16 08:33:04.656827 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/VIDEO_CONF.json
--rw-r--r--   0        0        0     4079 2024-04-16 08:33:04.656917 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json
--rw-r--r--   0        0        0      452 2024-04-16 08:33:04.656998 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/WEB_TOOLS_APP.json
--rw-r--r--   0        0        0      608 2024-04-16 08:33:04.657072 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json
--rw-r--r--   0        0        0      379 2024-04-16 08:33:04.657146 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/box_net_apps.json
--rw-r--r--   0        0        0      380 2024-04-16 08:33:04.657241 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/concur_apps.json
--rw-r--r--   0        0        0      383 2024-04-16 08:33:04.657348 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/dropbox_apps.json
--rw-r--r--   0        0        0      430 2024-04-16 08:33:04.657424 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/gotomeeting_apps.json
--rw-r--r--   0        0        0      380 2024-04-16 08:33:04.657504 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/intuit_apps.json
--rw-r--r--   0        0        0     1174 2024-04-16 08:33:04.657599 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json
--rw-r--r--   0        0        0      596 2024-04-16 08:33:04.657687 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json
--rw-r--r--   0        0        0      392 2024-04-16 08:33:04.657765 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/salesforce_apps.json
--rw-r--r--   0        0        0      388 2024-04-16 08:33:04.657837 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/sugar_crm_apps.json
--rw-r--r--   0        0        0      962 2024-04-16 08:33:04.657914 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json
--rw-r--r--   0        0        0      383 2024-04-16 08:33:04.657993 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zendesk_apps.json
--rw-r--r--   0        0        0      391 2024-04-16 08:33:04.658079 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zoho_crm_apps.json
--rw-r--r--   0        0        0      386 2024-04-16 08:33:04.658211 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Browsing.json
--rw-r--r--   0        0        0      375 2024-04-16 08:33:04.658298 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/ICMP.json
--rw-r--r--   0        0        0      428 2024-04-16 08:33:04.658407 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Yahoo.json
--rw-r--r--   0        0        0      414 2024-04-16 08:33:04.658533 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Best-Effort.json
--rw-r--r--   0        0        0      418 2024-04-16 08:33:04.658607 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Bulk-Data.json
--rw-r--r--   0        0        0      426 2024-04-16 08:33:04.658693 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Critical.json
--rw-r--r--   0        0        0      418 2024-04-16 08:33:04.658776 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Data.json
--rw-r--r--   0        0        0      414 2024-04-16 08:33:04.658855 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Default.json
--rw-r--r--   0        0        0      407 2024-04-16 08:33:04.658944 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Realtime.json
--rw-r--r--   0        0        0      434 2024-04-16 08:33:04.659046 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Transactional-Data.json
--rw-r--r--   0        0        0      427 2024-04-16 08:33:04.659135 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Voice-And-Video.json
--rw-r--r--   0        0        0       33 2024-04-16 08:33:04.659209 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/server_info.json
--rw-r--r--   0        0        0     2564 2024-04-16 08:33:04.659334 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela
--rw-r--r--   0        0        0     2905 2024-04-16 08:33:04.659404 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela
--rw-r--r--   0        0        0      196 2024-04-16 08:33:04.659541 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/__init__.py
--rw-r--r--   0        0        0    29801 2024-04-17 16:04:00.455565 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/add.py
--rw-r--r--   0        0        0    23332 2024-04-17 16:11:17.231239 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/backup.py
--rw-r--r--   0        0        0     1626 2024-04-16 08:33:04.659963 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/delete.py
--rw-r--r--   0        0        0     7005 2024-04-17 16:03:44.661059 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/deploy.py
--rw-r--r--   0        0        0    17977 2024-04-17 16:04:00.460729 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/restore.py
--rw-r--r--   0        0        0     9824 2024-04-16 16:03:27.580724 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/setup.py
--rw-r--r--   0        0        0    21040 2024-04-24 13:21:11.947230 catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/utils.py
--rw-r--r--   0        0        0      975 2024-04-16 15:05:59.202648 catalyst_sdwan_lab-2.0.6/pyproject.toml
--rw-r--r--   0        0        0    20475 1970-01-01 00:00:00.000000 catalyst_sdwan_lab-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0     1516 2024-04-24 14:08:20.797486 catalyst_sdwan_lab-2.0.7/LICENSE
+-rw-r--r--   0        0        0    19200 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/README.md
+-rw-r--r--   0        0        0      357 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/__init__.py
+-rw-r--r--   0        0        0    20068 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/__main__.py
+-rwxr-xr-x   0        0        0      443 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/cacsr_details.txt
+-rw-r--r--   0        0        0     3033 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/chainCA.pem
+-rwxr-xr-x   0        0        0      790 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/openssl-commands.md
+-rw-r--r--   0        0        0     1517 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/rootCA.pem
+-rw-r--r--   0        0        0       17 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/rootCA.srl
+-rwxr-xr-x   0        0        0      485 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/rootca_details.txt
+-rw-r--r--   0        0        0     1074 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/signCA.csr
+-rw-r--r--   0        0        0     1675 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/signCA.key
+-rw-r--r--   0        0        0     1517 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/signCA.pem
+-rwxr-xr-x   0        0        0      352 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/v3ext.cnf
+-rw-r--r--   0        0        0      421 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/controller-cloud-init.j2
+-rw-r--r--   0        0        0      851 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2
+-rw-r--r--   0        0        0      523 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2
+-rw-r--r--   0        0        0      895 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2
+-rw-r--r--   0        0        0      415 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/validator-cloud-init.j2
+-rw-r--r--   0        0        0    16330 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2
+-rw-r--r--   0        0        0     2292 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2
+-rw-r--r--   0        0        0     3182 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2
+-rw-r--r--   0        0        0     1383 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2
+-rw-r--r--   0        0        0     2327 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2
+-rw-r--r--   0        0        0     2087 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml
+-rw-r--r--   0        0        0     1981 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml
+-rw-r--r--   0        0        0     2094 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml
+-rw-r--r--   0        0        0     2097 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml
+-rw-r--r--   0        0        0     1859 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1866 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
+-rw-r--r--   0        0        0     1833 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1736 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1702 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1910 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
+-rw-r--r--   0        0        0     1686 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1615 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2516 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2510 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
+-rw-r--r--   0        0        0     2293 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
+-rw-r--r--   0        0        0     2657 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
+-rw-r--r--   0        0        0     2365 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
+-rw-r--r--   0        0        0     3215 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json
+-rw-r--r--   0        0        0     2924 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json
+-rw-r--r--   0        0        0     2260 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json
+-rw-r--r--   0        0        0     1347 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json
+-rw-r--r--   0        0        0     2454 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json
+-rw-r--r--   0        0        0    19645 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
+-rw-r--r--   0        0        0     7062 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24745 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5515 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
+-rw-r--r--   0        0        0    12013 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5591 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
+-rw-r--r--   0        0        0     6135 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24962 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0    11984 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5492 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5564 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     3456 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json
+-rw-r--r--   0        0        0    19638 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
+-rw-r--r--   0        0        0     9573 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
+-rw-r--r--   0        0        0    12289 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
+-rw-r--r--   0        0        0     8173 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json
+-rw-r--r--   0        0        0     2216 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json
+-rw-r--r--   0        0        0     6228 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json
+-rw-r--r--   0        0        0     1607 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json
+-rw-r--r--   0        0        0    22837 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
+-rw-r--r--   0        0        0    10441 2024-04-24 14:08:20.801486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
+-rw-r--r--   0        0        0    22817 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
+-rw-r--r--   0        0        0    22819 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
+-rw-r--r--   0        0        0    10419 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
+-rw-r--r--   0        0        0    18079 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
+-rw-r--r--   0        0        0    11073 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
+-rw-r--r--   0        0        0    11073 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
+-rw-r--r--   0        0        0    11073 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
+-rw-r--r--   0        0        0    11095 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
+-rw-r--r--   0        0        0    11071 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
+-rw-r--r--   0        0        0    11071 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
+-rw-r--r--   0        0        0    11075 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
+-rw-r--r--   0        0        0    11071 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
+-rw-r--r--   0        0        0     7066 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25121 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
+-rw-r--r--   0        0        0     7603 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
+-rw-r--r--   0        0        0     5572 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
+-rw-r--r--   0        0        0    11992 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
+-rw-r--r--   0        0        0     7025 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24720 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5478 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5550 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     2144 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json
+-rw-r--r--   0        0        0     7061 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25114 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5514 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     4915 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json
+-rw-r--r--   0        0        0     6290 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json
+-rw-r--r--   0        0        0    24529 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json
+-rw-r--r--   0        0        0    12375 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    12084 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     5570 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    12106 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8510 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10463 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json
+-rw-r--r--   0        0        0    25674 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
+-rw-r--r--   0        0        0    13302 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    13021 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     4729 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    13047 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8131 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10082 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
+-rw-r--r--   0        0        0     2191 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json
+-rw-r--r--   0        0        0     5921 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json
+-rw-r--r--   0        0        0     6998 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json
+-rw-r--r--   0        0        0     4315 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json
+-rw-r--r--   0        0        0     4323 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json
+-rw-r--r--   0        0        0     6985 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json
+-rw-r--r--   0        0        0    20010 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json
+-rw-r--r--   0        0        0     3218 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
+-rw-r--r--   0        0        0     7296 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
+-rw-r--r--   0        0        0     1739 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json
+-rw-r--r--   0        0        0     4104 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json
+-rw-r--r--   0        0        0    14537 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
+-rw-r--r--   0        0        0     4186 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json
+-rw-r--r--   0        0        0     7502 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     4511 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json
+-rw-r--r--   0        0        0     8107 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json
+-rw-r--r--   0        0        0     4416 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
+-rw-r--r--   0        0        0    13607 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
+-rw-r--r--   0        0        0     4333 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
+-rw-r--r--   0        0        0     3938 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
+-rw-r--r--   0        0        0    27208 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
+-rw-r--r--   0        0        0    25438 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
+-rw-r--r--   0        0        0     8351 2024-04-24 14:08:20.805486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json
+-rw-r--r--   0        0        0     9978 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json
+-rw-r--r--   0        0        0    11257 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
+-rw-r--r--   0        0        0     4976 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json
+-rw-r--r--   0        0        0    10714 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json
+-rw-r--r--   0        0        0     2008 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json
+-rw-r--r--   0        0        0    11386 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
+-rw-r--r--   0        0        0    12016 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
+-rw-r--r--   0        0        0     7360 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
+-rw-r--r--   0        0        0     1303 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json
+-rw-r--r--   0        0        0    11243 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json
+-rw-r--r--   0        0        0    11964 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json
+-rw-r--r--   0        0        0    11788 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
+-rw-r--r--   0        0        0    14115 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
+-rw-r--r--   0        0        0    12000 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
+-rw-r--r--   0        0        0     6868 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
+-rw-r--r--   0        0        0    25394 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
+-rw-r--r--   0        0        0     9260 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json
+-rw-r--r--   0        0        0    25074 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json
+-rw-r--r--   0        0        0    31516 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
+-rw-r--r--   0        0        0    24593 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
+-rw-r--r--   0        0        0     4859 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json
+-rw-r--r--   0        0        0     9400 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
+-rw-r--r--   0        0        0     9394 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
+-rw-r--r--   0        0        0    14686 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
+-rw-r--r--   0        0        0    19630 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
+-rw-r--r--   0        0        0     6475 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json
+-rw-r--r--   0        0        0     3858 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json
+-rw-r--r--   0        0        0     5138 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     2080 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
+-rw-r--r--   0        0        0     5653 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json
+-rw-r--r--   0        0        0     4099 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
+-rw-r--r--   0        0        0     4106 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
+-rw-r--r--   0        0        0     2608 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json
+-rw-r--r--   0        0        0      984 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
+-rw-r--r--   0        0        0     4382 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
+-rw-r--r--   0        0        0     3155 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
+-rw-r--r--   0        0        0     1442 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
+-rw-r--r--   0        0        0    34849 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json
+-rw-r--r--   0        0        0     5401 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json
+-rw-r--r--   0        0        0    10612 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json
+-rw-r--r--   0        0        0      868 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json
+-rw-r--r--   0        0        0    12306 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json
+-rw-r--r--   0        0        0    29668 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json
+-rw-r--r--   0        0        0    27664 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json
+-rw-r--r--   0        0        0     7826 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json
+-rw-r--r--   0        0        0     3871 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json
+-rw-r--r--   0        0        0    13751 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json
+-rw-r--r--   0        0        0     9628 2024-04-24 14:08:20.809486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json
+-rw-r--r--   0        0        0   597414 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json
+-rw-r--r--   0        0        0    14055 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json
+-rw-r--r--   0        0        0     1317 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json
+-rw-r--r--   0        0        0     3720 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json
+-rw-r--r--   0        0        0      532 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json
+-rw-r--r--   0        0        0      596 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json
+-rw-r--r--   0        0        0     2748 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json
+-rw-r--r--   0        0        0     1605 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json
+-rw-r--r--   0        0        0      450 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/REAL_TIME_APPS.json
+-rw-r--r--   0        0        0      386 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/VIDEO_CONF.json
+-rw-r--r--   0        0        0      452 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/WEB_TOOLS_APP.json
+-rw-r--r--   0        0        0      608 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json
+-rw-r--r--   0        0        0      379 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/box_net_apps.json
+-rw-r--r--   0        0        0      380 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/concur_apps.json
+-rw-r--r--   0        0        0      383 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/dropbox_apps.json
+-rw-r--r--   0        0        0      430 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/gotomeeting_apps.json
+-rw-r--r--   0        0        0      380 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/intuit_apps.json
+-rw-r--r--   0        0        0     1052 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json
+-rw-r--r--   0        0        0      596 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json
+-rw-r--r--   0        0        0      392 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/salesforce_apps.json
+-rw-r--r--   0        0        0      388 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/sugar_crm_apps.json
+-rw-r--r--   0        0        0      383 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zendesk_apps.json
+-rw-r--r--   0        0        0      391 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/zoho_crm_apps.json
+-rw-r--r--   0        0        0      386 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Browsing.json
+-rw-r--r--   0        0        0      375 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/ICMP.json
+-rw-r--r--   0        0        0      428 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/LocalApp/Yahoo.json
+-rw-r--r--   0        0        0      415 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Best-Effort.json
+-rw-r--r--   0        0        0      419 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Bulk-Data.json
+-rw-r--r--   0        0        0      427 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Critical.json
+-rw-r--r--   0        0        0      419 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Business-Data.json
+-rw-r--r--   0        0        0      415 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Default.json
+-rw-r--r--   0        0        0      408 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Realtime.json
+-rw-r--r--   0        0        0      435 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Transactional-Data.json
+-rw-r--r--   0        0        0      428 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/SLA/Voice-And-Video.json
+-rw-r--r--   0        0        0       32 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/server_info.json
+-rw-r--r--   0        0        0    15002 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json
+-rw-r--r--   0        0        0     1628 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json
+-rw-r--r--   0        0        0      295 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/attached/controller_basic.json
+-rw-r--r--   0        0        0     1859 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1866 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json
+-rw-r--r--   0        0        0     1833 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1736 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1702 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json
+-rw-r--r--   0        0        0     1910 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json
+-rw-r--r--   0        0        0     1720 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1686 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     1615 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2516 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json
+-rw-r--r--   0        0        0     2510 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json
+-rw-r--r--   0        0        0     2293 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json
+-rw-r--r--   0        0        0     2657 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json
+-rw-r--r--   0        0        0     2365 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json
+-rw-r--r--   0        0        0     3207 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json
+-rw-r--r--   0        0        0     2924 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json
+-rw-r--r--   0        0        0     2260 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json
+-rw-r--r--   0        0        0     1347 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json
+-rw-r--r--   0        0        0     2454 2024-04-24 14:08:20.813486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json
+-rw-r--r--   0        0        0     4130 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json
+-rw-r--r--   0        0        0      776 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json
+-rw-r--r--   0        0        0     6189 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json
+-rw-r--r--   0        0        0    12229 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json
+-rw-r--r--   0        0        0    13293 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json
+-rw-r--r--   0        0        0    20244 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json
+-rw-r--r--   0        0        0     7063 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24746 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5516 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json
+-rw-r--r--   0        0        0    12014 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5592 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json
+-rw-r--r--   0        0        0     6136 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24963 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0    11984 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     5493 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5565 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     3457 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json
+-rw-r--r--   0        0        0    20238 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json
+-rw-r--r--   0        0        0    10172 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json
+-rw-r--r--   0        0        0    12888 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json
+-rw-r--r--   0        0        0     8773 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json
+-rw-r--r--   0        0        0     2216 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json
+-rw-r--r--   0        0        0     6229 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json
+-rw-r--r--   0        0        0     1608 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json
+-rw-r--r--   0        0        0    22838 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json
+-rw-r--r--   0        0        0    10442 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json
+-rw-r--r--   0        0        0    22818 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json
+-rw-r--r--   0        0        0    22820 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json
+-rw-r--r--   0        0        0    10420 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json
+-rw-r--r--   0        0        0    18100 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json
+-rw-r--r--   0        0        0    11094 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json
+-rw-r--r--   0        0        0    11094 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json
+-rw-r--r--   0        0        0    11094 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json
+-rw-r--r--   0        0        0    11115 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json
+-rw-r--r--   0        0        0    11091 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json
+-rw-r--r--   0        0        0    11092 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json
+-rw-r--r--   0        0        0    11095 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json
+-rw-r--r--   0        0        0    11092 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json
+-rw-r--r--   0        0        0     9231 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json
+-rw-r--r--   0        0        0     7813 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0     9262 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json
+-rw-r--r--   0        0        0    28713 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json
+-rw-r--r--   0        0        0     7245 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     7067 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25122 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json
+-rw-r--r--   0        0        0     7604 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json
+-rw-r--r--   0        0        0     5573 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json
+-rw-r--r--   0        0        0    11993 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json
+-rw-r--r--   0        0        0     7026 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    24721 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5479 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     5551 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json
+-rw-r--r--   0        0        0     2145 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json
+-rw-r--r--   0        0        0     7062 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json
+-rw-r--r--   0        0        0    25115 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json
+-rw-r--r--   0        0        0     5515 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json
+-rw-r--r--   0        0        0     4936 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json
+-rw-r--r--   0        0        0     6311 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json
+-rw-r--r--   0        0        0    24530 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json
+-rw-r--r--   0        0        0    12376 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    12085 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     5570 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    12106 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8511 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10464 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json
+-rw-r--r--   0        0        0    25675 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json
+-rw-r--r--   0        0        0    13303 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json
+-rw-r--r--   0        0        0    13022 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json
+-rw-r--r--   0        0        0     4730 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json
+-rw-r--r--   0        0        0    13048 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json
+-rw-r--r--   0        0        0     8132 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json
+-rw-r--r--   0        0        0    10083 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json
+-rw-r--r--   0        0        0     2192 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json
+-rw-r--r--   0        0        0     5922 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json
+-rw-r--r--   0        0        0     7019 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json
+-rw-r--r--   0        0        0     4336 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json
+-rw-r--r--   0        0        0     4343 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json
+-rw-r--r--   0        0        0     7211 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json
+-rw-r--r--   0        0        0    20011 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json
+-rw-r--r--   0        0        0     3219 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json
+-rw-r--r--   0        0        0     7321 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json
+-rw-r--r--   0        0        0     1740 2024-04-24 14:08:20.817486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json
+-rw-r--r--   0        0        0     4330 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json
+-rw-r--r--   0        0        0    14763 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json
+-rw-r--r--   0        0        0     4412 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json
+-rw-r--r--   0        0        0     7728 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     4737 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json
+-rw-r--r--   0        0        0     8333 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json
+-rw-r--r--   0        0        0     4642 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json
+-rw-r--r--   0        0        0    13632 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json
+-rw-r--r--   0        0        0     4561 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json
+-rw-r--r--   0        0        0     3938 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json
+-rw-r--r--   0        0        0    27208 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json
+-rw-r--r--   0        0        0    25439 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json
+-rw-r--r--   0        0        0     8352 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json
+-rw-r--r--   0        0        0     9978 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json
+-rw-r--r--   0        0        0    11258 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json
+-rw-r--r--   0        0        0     5397 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json
+-rw-r--r--   0        0        0    10940 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json
+-rw-r--r--   0        0        0     2008 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json
+-rw-r--r--   0        0        0    11387 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json
+-rw-r--r--   0        0        0    12016 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json
+-rw-r--r--   0        0        0     7360 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json
+-rw-r--r--   0        0        0     1304 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json
+-rw-r--r--   0        0        0    11244 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json
+-rw-r--r--   0        0        0    11965 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json
+-rw-r--r--   0        0        0    11789 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json
+-rw-r--r--   0        0        0    14116 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json
+-rw-r--r--   0        0        0    12001 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json
+-rw-r--r--   0        0        0     6868 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json
+-rw-r--r--   0        0        0    25394 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json
+-rw-r--r--   0        0        0     9261 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json
+-rw-r--r--   0        0        0    25075 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json
+-rw-r--r--   0        0        0    31517 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json
+-rw-r--r--   0        0        0    24594 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json
+-rw-r--r--   0        0        0     4905 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json
+-rw-r--r--   0        0        0     9401 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json
+-rw-r--r--   0        0        0     9395 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json
+-rw-r--r--   0        0        0    14687 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json
+-rw-r--r--   0        0        0    19631 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json
+-rw-r--r--   0        0        0     6476 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json
+-rw-r--r--   0        0        0     3859 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json
+-rw-r--r--   0        0        0     5139 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json
+-rw-r--r--   0        0        0     2081 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json
+-rw-r--r--   0        0        0     5654 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json
+-rw-r--r--   0        0        0     4100 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json
+-rw-r--r--   0        0        0     4109 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json
+-rw-r--r--   0        0        0     2609 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json
+-rw-r--r--   0        0        0      985 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json
+-rw-r--r--   0        0        0     4383 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json
+-rw-r--r--   0        0        0     3156 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json
+-rw-r--r--   0        0        0     1443 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json
+-rw-r--r--   0        0        0    34850 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json
+-rw-r--r--   0        0        0     5402 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json
+-rw-r--r--   0        0        0    10613 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json
+-rw-r--r--   0        0        0      869 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json
+-rw-r--r--   0        0        0    12307 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json
+-rw-r--r--   0        0        0    29670 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json
+-rw-r--r--   0        0        0    27666 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json
+-rw-r--r--   0        0        0     7827 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json
+-rw-r--r--   0        0        0     3872 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json
+-rw-r--r--   0        0        0    13753 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json
+-rw-r--r--   0        0        0     1760 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json
+-rw-r--r--   0        0        0    10179 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json
+-rw-r--r--   0        0        0      316 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_cli.json
+-rw-r--r--   0        0        0      320 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_service.json
+-rw-r--r--   0        0        0      322 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_system.json
+-rw-r--r--   0        0        0      322 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_profiles_sdwan_transport.json
+-rw-r--r--   0        0        0   628759 2024-04-24 14:08:20.821486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json
+-rw-r--r--   0        0        0    20494 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json
+-rw-r--r--   0        0        0     1215 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json
+-rw-r--r--   0        0        0     3440 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json
+-rw-r--r--   0        0        0      532 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json
+-rw-r--r--   0        0        0      596 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json
+-rw-r--r--   0        0        0     3010 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json
+-rw-r--r--   0        0        0      904 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json
+-rw-r--r--   0        0        0     1605 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json
+-rw-r--r--   0        0        0      450 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/REAL_TIME_APPS.json
+-rw-r--r--   0        0        0      386 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/VIDEO_CONF.json
+-rw-r--r--   0        0        0     4079 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json
+-rw-r--r--   0        0        0      452 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/WEB_TOOLS_APP.json
+-rw-r--r--   0        0        0      608 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json
+-rw-r--r--   0        0        0      379 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/box_net_apps.json
+-rw-r--r--   0        0        0      380 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/concur_apps.json
+-rw-r--r--   0        0        0      383 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/dropbox_apps.json
+-rw-r--r--   0        0        0      430 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/gotomeeting_apps.json
+-rw-r--r--   0        0        0      380 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/intuit_apps.json
+-rw-r--r--   0        0        0     1174 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json
+-rw-r--r--   0        0        0      596 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json
+-rw-r--r--   0        0        0      392 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/salesforce_apps.json
+-rw-r--r--   0        0        0      388 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/sugar_crm_apps.json
+-rw-r--r--   0        0        0      962 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json
+-rw-r--r--   0        0        0      383 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zendesk_apps.json
+-rw-r--r--   0        0        0      391 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/zoho_crm_apps.json
+-rw-r--r--   0        0        0      386 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Browsing.json
+-rw-r--r--   0        0        0      375 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/ICMP.json
+-rw-r--r--   0        0        0      428 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/LocalApp/Yahoo.json
+-rw-r--r--   0        0        0      414 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Best-Effort.json
+-rw-r--r--   0        0        0      418 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Bulk-Data.json
+-rw-r--r--   0        0        0      426 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Critical.json
+-rw-r--r--   0        0        0      418 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Business-Data.json
+-rw-r--r--   0        0        0      414 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Default.json
+-rw-r--r--   0        0        0      407 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Realtime.json
+-rw-r--r--   0        0        0      434 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Transactional-Data.json
+-rw-r--r--   0        0        0      427 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/SLA/Voice-And-Video.json
+-rw-r--r--   0        0        0       33 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/server_info.json
+-rw-r--r--   0        0        0     2564 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela
+-rw-r--r--   0        0        0     2905 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela
+-rw-r--r--   0        0        0      196 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/__init__.py
+-rw-r--r--   0        0        0    29801 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/add.py
+-rw-r--r--   0        0        0    23332 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/backup.py
+-rw-r--r--   0        0        0     1626 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/delete.py
+-rw-r--r--   0        0        0     7005 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/deploy.py
+-rw-r--r--   0        0        0    17977 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/restore.py
+-rw-r--r--   0        0        0     9824 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/setup.py
+-rw-r--r--   0        0        0    21040 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/utils.py
+-rw-r--r--   0        0        0      975 2024-04-24 14:08:20.825486 catalyst_sdwan_lab-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0    20446 1970-01-01 00:00:00.000000 catalyst_sdwan_lab-2.0.7/PKG-INFO
```

### Comparing `catalyst_sdwan_lab-2.0.6/LICENSE` & `catalyst_sdwan_lab-2.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/README.md` & `catalyst_sdwan_lab-2.0.7/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -36,17 +36,17 @@
     
 - Note that the prompt is updated with the virtual environment name (venv), indicating that the virtual environment is active.
     
 Upgrade initial virtual environment packages:
 
     pip install --upgrade pip setuptools
 
-To install SD-WAN Lab:
+To install SD-WAN Lab Deployment Tool:
 
-    pip install --upgrade git+https://github.com/cisco-open/sdwan-lab-deployment-tool.git
+    pip install --upgrade catalyst-sdwan-lab
     
 Verify that SD-WAN Lab tool can run:
 
     sdwan-lab --version
 
 You can also use the following shortcut to run any lab task:
```

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/__main__.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/__main__.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/chainCA.pem` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/chainCA.pem`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/openssl-commands.md` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/openssl-commands.md`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/rootCA.pem` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/rootCA.pem`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/signCA.csr` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/signCA.csr`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/signCA.key` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/signCA.key`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/certs/signCA.pem` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/certs/signCA.pem`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/edge-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/manager-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/backup/sdrouting-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/cml-base-topology.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/controller-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/manager-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/sdrouting-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_lab_definition/deploy/validator-cloud-init.j2`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-controller.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-edge.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-manager.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/cml_nodes_definition/cat-sdwan-validator.yaml`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_GCP_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_ISRv_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_CSR_1000V_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_DC1_HUB.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/Factory_Default_ISR_4331_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/controller_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/device_templates/template/edge_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BFD_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BOOTSTRAP_DHCP_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_BootStrap_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Cellular_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_SVI_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_Switch_Port_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_GCP_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Logging_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_NTP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_OMP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_Security_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_System_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_0_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_1_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Default_VPN_512_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AAA_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_AppQoE_Standalone_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_BFD_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_BFD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Logging_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Cisco_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_DC1_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_EIO_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Global_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Logging_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_BGP_To_OMP.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Banner.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Branch_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_Regular_BFD.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN0_LTE.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_UTD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Cellular_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_Security_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_aaa.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/controller_basic_vpn0_eth1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_cli.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi1_inet.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn0_gi2_mpls.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_dhcp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/feature_templates/edge_basic_vpn1_gi3_lan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/device_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/feature_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_app.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_localapp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/inventory/policy_lists_sla.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_BULK_DATA.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/APP_Scavengers.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Google_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/Microsoft_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/amazon_aws_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/office365_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v1/policy_lists/App/oracle_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/certificates/edge_certificates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/config_groups/group/edge_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_AWS_TGW_CSR1000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_Azure_vWAN_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_DHCP_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_BOOTSTRAP_STATIC_8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_DHCP_DNS_ICGW_CSR1000V_Template_V02.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_EQUINIX_ICGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_GCP_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_MEGAPORT_ICGW_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_C8000V_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_ISRv_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Default_SDBranch_vEdge_cloud_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_1_TLOC_Branch_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C1111_8PLTELA_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_C8000V_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_DC1_HUB.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/Factory_Default_ISR_4331_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/controller_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/template/edge_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/device_templates/values/controller_basic.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/cli/edge_basic_cli.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/service/edge_basic_lan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/system/edge_basic_system.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_profiles/sdwan/transport/edge_basic_wan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/DEFAULT_BOOTSTRAP_STATIC.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_AWS_TGW_CSR_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Azure_vWAN_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BFD_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BOOTSTRAP_DHCP_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_DHCP_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_Static_VPN_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_BootStrap_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Cellular_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_SVI_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_Switch_Port_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_C1111_VPN_Interface_ge_0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_g0_0_1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_ISR4331_Interface_gig0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet3_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet4_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet5_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet6_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet7_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet8_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Cisco_VPN_interface_GigabitEthernet9_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_C8000V_GLOBAL_CISCO_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_DNS_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN0_INTF_GE2_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DHCP_INTF_GE2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN0_DNS.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_EQUINIX_ICGW_CSR1000V_VPN512_INTF_GE24.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_GCP_C8000V_VPN512_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Logging_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_OMP_IPv46_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_INTF_GE1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_MEGAPORT_ICGW_C8000V_VPN0_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_NTP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_OMP_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INET_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_INTERNAL_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_MGMT_VPN511_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_SVC_INT_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_Service_VPN1_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_SDBranch_vEdge_VPN0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_Security_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_System_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_0_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_1_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Default_VPN_512_Cisco_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AAA_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_ExternalServiceNode_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_AppQoE_Standalone_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_BFD_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_BFD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_DHCP_Tunnel_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Logging_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_DHCP_Ethernet_Interface_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Cisco_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_EMPLOYEE_DHCP_SERVER.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_INET_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_MPLS_VPN0_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_DC1_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Dynamic_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_EIO_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Global_CISCO_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Logging_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_AcquisitionServiceSideNAT_VPN.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Acquistion_INTF_VPN2.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_BGP_To_OMP.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Banner.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_System.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Branch_VPN0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_INTF_VPN3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Employee_VPN_VLAN_3.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_GUEST_INTF_VPN99.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Guest_Wifi_NAT_DIA_Route.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_MPLS_Enabled_VPN_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_Regular_BFD.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN0_LTE.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_Retail_VPN_O_INET_NAT_Enabled.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_TLOC_EXTENSION_MPLS_R1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_UTD_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_100B_M_WM_Mgmt_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Cellular_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_DHCP_Tunnel_Interface_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Management_Interface.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_OMP_ipv46_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_Security_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_0_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vEdge_VPN_512_Template_V01.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_OMP_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_Security_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_System_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_0_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/Factory_Default_vSmart_vManage_VPN_512_Template.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_aaa.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/controller_basic_vpn0_eth1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_cli.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi1_inet.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn0_gi2_mpls.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_dhcp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/feature_templates/edge_basic_vpn1_gi3_lan.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/config_groups.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/device_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/feature_templates.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_app.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_localapp.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/inventory/policy_lists_sla.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_BULK_DATA.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/APP_Scavengers.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Google_Workspace_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Microsoft_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/Voice_Apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/amazon_aws_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/office365_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/oracle_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/manager_configs/v2/policy_lists/App/webex_apps.json`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/serial_files/serialFile-v1.viptela`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/data/serial_files/serialFile-v2.viptela`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/add.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/add.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/backup.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/backup.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/delete.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/delete.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/deploy.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/deploy.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/restore.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/restore.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/setup.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/setup.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/catalyst_sdwan_lab/tasks/utils.py` & `catalyst_sdwan_lab-2.0.7/catalyst_sdwan_lab/tasks/utils.py`

 * *Files identical despite different names*

### Comparing `catalyst_sdwan_lab-2.0.6/pyproject.toml` & `catalyst_sdwan_lab-2.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "catalyst-sdwan-lab"
-version = "2.0.6"
+version = "2.0.7"
 description = "Catalyst SD-WAN Lab Deployment Tool - Automation Tool for managing Cisco Catalyst SD-WAN labs inside Cisco Modelling Labs"
 license = "BSD-3-Clause"
 authors = ["Tomasz Zarski <tzarski@cisco.com>"]
 readme = "README.md"
 repository = "https://github.com/cisco-open/sdwan-lab-deployment-tool"
 keywords = ["cisco", "catalyst", "sdwan", "lab"]
```

### Comparing `catalyst_sdwan_lab-2.0.6/PKG-INFO` & `catalyst_sdwan_lab-2.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: catalyst-sdwan-lab
-Version: 2.0.6
+Version: 2.0.7
 Summary: Catalyst SD-WAN Lab Deployment Tool - Automation Tool for managing Cisco Catalyst SD-WAN labs inside Cisco Modelling Labs
 Home-page: https://github.com/cisco-open/sdwan-lab-deployment-tool
 License: BSD-3-Clause
 Keywords: cisco,catalyst,sdwan,lab
 Author: Tomasz Zarski
 Author-email: tzarski@cisco.com
 Requires-Python: >=3.9,<4.0
@@ -65,17 +65,17 @@
     
 - Note that the prompt is updated with the virtual environment name (venv), indicating that the virtual environment is active.
     
 Upgrade initial virtual environment packages:
 
     pip install --upgrade pip setuptools
 
-To install SD-WAN Lab:
+To install SD-WAN Lab Deployment Tool:
 
-    pip install --upgrade git+https://github.com/cisco-open/sdwan-lab-deployment-tool.git
+    pip install --upgrade catalyst-sdwan-lab
     
 Verify that SD-WAN Lab tool can run:
 
     sdwan-lab --version
 
 You can also use the following shortcut to run any lab task:
```

