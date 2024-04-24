# Comparing `tmp/skale.py-6.2b0.tar.gz` & `tmp/skale.py-7.dev11.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skale.py-6.2b0.tar", last modified: Thu Jan 11 18:56:56 2024, max compression
+gzip compressed data, was "skale.py-7.dev11.tar", last modified: Wed Apr 24 15:12:16 2024, max compression
```

## Comparing `skale.py-6.2b0.tar` & `skale.py-7.dev11.tar`

### file list

```diff
@@ -1,106 +1,105 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.603981 skale.py-6.2b0/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-01-11 18:55:43.000000 skale.py-6.2b0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-01-11 18:55:43.000000 skale.py-6.2b0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-11 18:56:56.603981 skale.py-6.2b0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-01-11 18:55:43.000000 skale.py-6.2b0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-11 18:56:56.603981 skale.py-6.2b0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1583 2024-01-11 18:56:56.000000 skale.py-6.2b0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.591981 skale.py-6.2b0/skale/
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.591981 skale.py-6.2b0/skale/contracts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.591981 skale.py-6.2b0/skale/contracts/allocator/
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/allocator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/allocator/allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4493 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/allocator/escrow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/base_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/contract_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.591981 skale.py-6.2b0/skale/contracts/ima/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/ima/linker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.595981 skale.py-6.2b0/skale/contracts/manager/
--rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/bounty_v2.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/constants_holder.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.595981 skale.py-6.2b0/skale/contracts/manager/delegation/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/delegation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/delegation/delegation_controller.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/delegation/delegation_period_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/delegation/distributor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/delegation/slashing_table.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/delegation/token_state.py
--rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/delegation/validator_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/dkg.py
--rw-r--r--   0 runner    (1001) docker     (127)      893 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/key_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/node_rotation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/punisher.py
--rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/schains.py
--rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/schains_internal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/sync_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.595981 skale.py-6.2b0/skale/contracts/manager/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/test/time_helpers_with_debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/contracts/manager/wallets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.599981 skale.py-6.2b0/skale/dataclasses/
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/dataclasses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/dataclasses/delegation_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/dataclasses/node_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/dataclasses/schain_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/dataclasses/skaled_ports.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.599981 skale.py-6.2b0/skale/schain_config/
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/schain_config/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/schain_config/ports_allocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/schain_config/rotation_history.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/skale_allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4653 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/skale_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/skale_ima.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/skale_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.599981 skale.py-6.2b0/skale/transactions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/transactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/transactions/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/transactions/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/transactions/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.599981 skale.py-6.2b0/skale/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/abi_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/account_tools.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/contract_info.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/contract_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.599981 skale.py-6.2b0/skale/utils/contracts_provision/
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/contracts_provision/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/contracts_provision/allocator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/contracts_provision/fake_multisig_contract.py
--rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/contracts_provision/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/contracts_provision/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     5055 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/helper.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.599981 skale.py-6.2b0/skale/utils/random_names/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/random_names/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/random_names/generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/random_names/vocabulary.py
--rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/utils/web3_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.603981 skale.py-6.2b0/skale/wallets/
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/wallets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/wallets/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/wallets/ledger_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/wallets/redis_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/wallets/sgx_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-01-11 18:55:43.000000 skale.py-6.2b0/skale/wallets/web3_wallet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.591981 skale.py-6.2b0/skale.py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2024-01-11 18:56:56.000000 skale.py-6.2b0/skale.py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2917 2024-01-11 18:56:56.000000 skale.py-6.2b0/skale.py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-11 18:56:56.000000 skale.py-6.2b0/skale.py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-01-11 18:56:56.000000 skale.py-6.2b0/skale.py.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-01-11 18:56:56.000000 skale.py-6.2b0/skale.py.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.591981 skale.py-6.2b0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-11 18:56:56.603981 skale.py-6.2b0/tests/schain_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-11 18:55:43.000000 skale.py-6.2b0/tests/schain_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      804 2024-01-11 18:55:43.000000 skale.py-6.2b0/tests/schain_config/generator_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-01-11 18:55:43.000000 skale.py-6.2b0/tests/schain_config/ports_allocation_test.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.186797 skale.py-7.dev11/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-04-24 15:11:04.000000 skale.py-7.dev11/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-24 15:11:04.000000 skale.py-7.dev11/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 15:12:16.182796 skale.py-7.dev11/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3400 2024-04-24 15:11:04.000000 skale.py-7.dev11/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 15:12:16.186797 skale.py-7.dev11/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-04-24 15:12:15.000000 skale.py-7.dev11/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/contracts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/contracts/allocator/
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/allocator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6004 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/allocator/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/allocator/escrow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4858 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/base_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1333 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/contract_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale/contracts/ima/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/ima/linker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/contracts/manager/
+-rw-r--r--   0 runner    (1001) docker     (127)     1508 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/bounty_v2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/constants_holder.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/contracts/manager/delegation/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7916 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/delegation_controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/delegation_period_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2844 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/distributor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1208 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/slashing_table.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/token_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11013 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/delegation/validator_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6072 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/dkg.py
+-rw-r--r--   0 runner    (1001) docker     (127)      893 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/key_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4242 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5101 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/node_rotation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6369 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1283 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/punisher.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6103 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/schains.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3645 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/schains_internal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2607 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/sync_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/contracts/manager/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1522 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/test/time_helpers_with_debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1624 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/contracts/manager/wallets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/dataclasses/
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/delegation_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1621 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/node_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1888 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/schain_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/dataclasses/skaled_ports.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.178796 skale.py-7.dev11/skale/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1317 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1495 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/ports_allocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7160 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/schain_config/rotation_history.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2215 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5121 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_ima.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/skale_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/transactions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2194 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6350 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/transactions/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4263 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/account_tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1094 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contract_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contract_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/utils/contracts_provision/
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/allocator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3397 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/fake_multisig_contract.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12190 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/contracts_provision/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1340 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5372 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/helper.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/utils/random_names/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/random_names/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/random_names/generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6032 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/random_names/vocabulary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8904 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/utils/web3_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/skale/wallets/
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7846 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/ledger_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6171 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/redis_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3865 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/sgx_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3835 2024-04-24 15:11:04.000000 skale.py-7.dev11/skale/wallets/web3_wallet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.174796 skale.py-7.dev11/skale.py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      607 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      441 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 15:12:16.000000 skale.py-7.dev11/skale.py.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.170796 skale.py-7.dev11/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 15:12:16.182796 skale.py-7.dev11/tests/schain_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 15:11:04.000000 skale.py-7.dev11/tests/schain_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      804 2024-04-24 15:11:04.000000 skale.py-7.dev11/tests/schain_config/generator_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 15:11:04.000000 skale.py-7.dev11/tests/schain_config/ports_allocation_test.py
```

### Comparing `skale.py-6.2b0/LICENSE` & `skale.py-7.dev11/LICENSE`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/PKG-INFO` & `skale.py-7.dev11/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 6.2b0
+Version: 7.dev11
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 Keywords: skale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `skale.py-6.2b0/README.md` & `skale.py-7.dev11/README.md`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/setup.py` & `skale.py-7.dev11/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -29,26 +29,27 @@
 
 extras_require['dev'] = (
     extras_require['linter'] + extras_require['dev'] + extras_require['hw-wallet']
 )
 
 setup(
     name='skale.py',
-    version='6.2b0',
+    version='7dev11',
     description='SKALE client tools',
     long_description_markdown_filename='README.md',
     author='SKALE Labs',
     author_email='support@skalelabs.com',
     url='https://github.com/skalenetwork/skale.py',
     include_package_data=True,
     install_requires=[
         "asyncio==3.4.3",
         "pyyaml==6.0",
-        "sgx.py==0.9dev2",
         "redis==4.4.4",
+        "sgx.py==0.9dev2",
+        "skale-contracts==1.0.1a5",
         "typing-extensions==4.9.0",
         "web3==6.13.0"
     ],
 
     python_requires='>=3.7,<4',
     extras_require=extras_require,
```

### Comparing `skale.py-6.2b0/skale/config.py` & `skale.py-7.dev11/skale/config.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/allocator/allocator.py` & `skale.py-7.dev11/skale/contracts/allocator/allocator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/allocator/escrow.py` & `skale.py-7.dev11/skale/contracts/allocator/escrow.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,27 @@
 from skale.contracts.base_contract import BaseContract, transaction_method
 from skale.transactions.result import TxRes
 
 
 def beneficiary_escrow(transaction):
     @functools.wraps(transaction)
     def wrapper(self, *args, beneficiary_address, **kwargs):
-        self.contract = self.init_beneficiary_contract(beneficiary_address)
+        self.contract = self.skale.instance.get_contract('Escrow', beneficiary_address)
         return transaction(self, *args, **kwargs)
     return wrapper
 
 
 class Escrow(BaseContract):
     @property
     @functools.lru_cache()
     def allocator(self):
         return self.skale.allocator
 
-    def init_beneficiary_contract(self, beneficiary_address: str):
-        beneficiary_escrow_address = self.allocator.get_escrow_address(beneficiary_address)
-        return Escrow(self.skale, f'escrow_{beneficiary_address}', beneficiary_escrow_address,
-                      self.contract.abi).contract
+    def init_contract(self, skale, address, abi) -> None:
+        self.contract = None
 
     @beneficiary_escrow
     @transaction_method
     def retrieve(self) -> TxRes:
         """Allows Holder to retrieve vested tokens from the Escrow contract
 
         :returns: Transaction results
```

### Comparing `skale.py-6.2b0/skale/contracts/base_contract.py` & `skale.py-7.dev11/skale/contracts/base_contract.py`

 * *Files 3% similar despite different names*

```diff
@@ -117,15 +117,18 @@
 
 
 class BaseContract:
     def __init__(self, skale, name, address, abi):
         self.skale = skale
         self.name = name
         self.address = Web3.to_checksum_address(address)
-        self.contract = skale.web3.eth.contract(address=self.address, abi=abi)
+        self.init_contract(skale, address, abi)
+
+    def init_contract(self, skale, address, abi) -> None:
+        self.contract = skale.web3.eth.contract(address=address, abi=abi)
 
     def __getattr__(self, attr):
         """Fallback for contract calls"""
         logger.debug("Calling contract function: %s", attr)
 
         def wrapper(*args, **kw):
             logger.debug('called with %r and %r' % (args, kw))
```

### Comparing `skale.py-6.2b0/skale/contracts/contract_manager.py` & `skale.py-7.dev11/skale/contracts/contract_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/ima/linker.py` & `skale.py-7.dev11/skale/contracts/ima/linker.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/__init__.py` & `skale.py-7.dev11/skale/contracts/manager/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/bounty_v2.py` & `skale.py-7.dev11/skale/contracts/manager/bounty_v2.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/constants_holder.py` & `skale.py-7.dev11/skale/contracts/manager/constants_holder.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/delegation/delegation_controller.py` & `skale.py-7.dev11/skale/contracts/manager/delegation/delegation_controller.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/delegation/delegation_period_manager.py` & `skale.py-7.dev11/skale/contracts/manager/delegation/delegation_period_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/delegation/distributor.py` & `skale.py-7.dev11/skale/contracts/manager/delegation/distributor.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/delegation/slashing_table.py` & `skale.py-7.dev11/skale/contracts/manager/delegation/slashing_table.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/delegation/token_state.py` & `skale.py-7.dev11/skale/contracts/manager/delegation/token_state.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/delegation/validator_service.py` & `skale.py-7.dev11/skale/contracts/manager/delegation/validator_service.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/dkg.py` & `skale.py-7.dev11/skale/contracts/manager/dkg.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/groups.py` & `skale.py-7.dev11/skale/contracts/manager/groups.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/key_storage.py` & `skale.py-7.dev11/skale/contracts/manager/key_storage.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/manager.py` & `skale.py-7.dev11/skale/contracts/manager/manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/node_rotation.py` & `skale.py-7.dev11/skale/contracts/manager/node_rotation.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/nodes.py` & `skale.py-7.dev11/skale/contracts/manager/nodes.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/punisher.py` & `skale.py-7.dev11/skale/contracts/manager/punisher.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/schains.py` & `skale.py-7.dev11/skale/contracts/manager/schains.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/schains_internal.py` & `skale.py-7.dev11/skale/contracts/manager/schains_internal.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/sync_manager.py` & `skale.py-7.dev11/skale/contracts/manager/sync_manager.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/test/time_helpers_with_debug.py` & `skale.py-7.dev11/skale/contracts/manager/test/time_helpers_with_debug.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/token.py` & `skale.py-7.dev11/skale/contracts/manager/token.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/contracts/manager/wallets.py` & `skale.py-7.dev11/skale/contracts/manager/wallets.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/dataclasses/__init__.py` & `skale.py-7.dev11/skale/dataclasses/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/dataclasses/delegation_status.py` & `skale.py-7.dev11/skale/dataclasses/delegation_status.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/dataclasses/node_info.py` & `skale.py-7.dev11/skale/dataclasses/node_info.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/dataclasses/schain_options.py` & `skale.py-7.dev11/skale/dataclasses/schain_options.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/dataclasses/skaled_ports.py` & `skale.py-7.dev11/skale/dataclasses/skaled_ports.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/schain_config/__init__.py` & `skale.py-7.dev11/skale/schain_config/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/schain_config/generator.py` & `skale.py-7.dev11/skale/schain_config/generator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/schain_config/ports_allocation.py` & `skale.py-7.dev11/skale/schain_config/ports_allocation.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/schain_config/rotation_history.py` & `skale.py-7.dev11/skale/schain_config/rotation_history.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/skale_allocator.py` & `skale.py-7.dev11/skale/skale_allocator.py`

 * *Files 12% similar despite different names*

```diff
@@ -12,24 +12,30 @@
 #   SKALE.py is distributed in the hope that it will be useful,
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
+from __future__ import annotations
 
 import logging
+from typing import TYPE_CHECKING
+from web3.constants import ADDRESS_ZERO
 
 from skale.skale_base import SkaleBase
 import skale.contracts.allocator as contracts
 from skale.contracts.contract_manager import ContractManager
 from skale.utils.contract_info import ContractInfo
 from skale.utils.contract_types import ContractTypes
 from skale.utils.helper import get_contracts_info
 
+if TYPE_CHECKING:
+    from eth_typing import ChecksumAddress
+
 
 logger = logging.getLogger(__name__)
 
 
 CONTRACTS_INFO = [
     ContractInfo('contract_manager', 'ContractManager',
                  ContractManager, ContractTypes.API, False),
@@ -41,10 +47,19 @@
 
 
 def spawn_skale_allocator_lib(skale):
     return SkaleAllocator(skale._endpoint, skale._abi_filepath, skale.wallet)
 
 
 class SkaleAllocator(SkaleBase):
+    """Represents skale-allocator smart contracts"""
+    @property
+    def project_name(self) -> str:
+        return 'skale-allocator'
+
+    def get_contract_address(self, name) -> ChecksumAddress:
+        if name == 'Escrow':
+            return ADDRESS_ZERO
+        return super().get_contract_address(name)
+
     def set_contracts_info(self):
-        self.init_contract_manager()
         self._SkaleBase__contracts_info = get_contracts_info(CONTRACTS_INFO)
```

### Comparing `skale.py-6.2b0/skale/skale_base.py` & `skale.py-7.dev11/skale/skale_base.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,54 +13,67 @@
 #   but WITHOUT ANY WARRANTY; without even the implied warranty of
 #   MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
 #   GNU Affero General Public License for more details.
 #
 #   You should have received a copy of the GNU Affero General Public License
 #   along with SKALE.py.  If not, see <https://www.gnu.org/licenses/>.
 
+from __future__ import annotations
+
 import abc
 import logging
+from typing import TYPE_CHECKING
+
+from skale_contracts import skale_contracts
 
 from skale.wallets import BaseWallet
-from skale.utils.abi_utils import get_contract_address_by_name, get_contract_abi_by_name
 from skale.utils.exceptions import InvalidWalletError, EmptyWalletError
 from skale.utils.web3_utils import default_gas_price, init_web3
 
-from skale.utils.helper import get_abi
 from skale.contracts.contract_manager import ContractManager
 
+if TYPE_CHECKING:
+    from eth_typing import Address, ChecksumAddress
+
 
 logger = logging.getLogger(__name__)
 
 
 class EmptyPrivateKey(Exception):
     pass
 
 
 class SkaleBase:
     __metaclass__ = abc.ABCMeta
 
-    def __init__(self, endpoint, abi_filepath,
+    def __init__(self, endpoint, alias_or_address: str,
                  wallet=None, state_path=None,
                  ts_diff=None, provider_timeout=30):
-        logger.info(f'Initing skale.py, endpoint: {endpoint}, '
-                    f'wallet: {type(wallet).__name__}')
-        self._abi_filepath = abi_filepath
+        logger.info('Initializing skale.py, endpoint: %s, wallet: %s',
+                    endpoint, type(wallet).__name__)
         self._endpoint = endpoint
         self.web3 = init_web3(endpoint,
                               state_path=state_path,
                               ts_diff=ts_diff,
                               provider_timeout=provider_timeout)
+        self.network = skale_contracts.get_network_by_provider(self.web3.provider)
+        self.project = self.network.get_project(self.project_name)
+        self.instance = self.project.get_instance(alias_or_address)
         self.__contracts = {}
         self.__contracts_info = {}
         self.set_contracts_info()
         if wallet:
             self.wallet = wallet
 
     @property
+    @abc.abstractmethod
+    def project_name(self) -> str:
+        """Name of smart contracts project"""
+
+    @property
     def gas_price(self):
         return default_gas_price(self.web3)
 
     @property
     def wallet(self):
         if not self._wallet:
             raise EmptyWalletError('No wallet provided')
@@ -78,50 +91,56 @@
         return abi.get('time_helpers_with_debug_address', None)
 
     @abc.abstractmethod
     def set_contracts_info(self):
         return
 
     def init_contract_manager(self):
-        abi = get_abi(self._abi_filepath)
-        self.add_lib_contract('contract_manager', ContractManager, abi)
+        self.add_lib_contract('contract_manager', ContractManager, 'ContractManager')
 
-    def __init_contract_from_info(self, abi, contract_info):
+    def __init_contract_from_info(self, contract_info):
         if contract_info.upgradeable:
-            self.init_upgradeable_contract(contract_info, abi)
+            self.init_upgradeable_contract(contract_info)
         else:
-            self.add_lib_contract(contract_info.name, contract_info.contract_class,
-                                  abi)
+            self.add_lib_contract(
+                contract_info.name,
+                contract_info.contract_class,
+                contract_info.contract_name
+            )
 
-    def init_upgradeable_contract(self, contract_info, abi):
+    def init_upgradeable_contract(self, contract_info):
         address = self.get_contract_address(contract_info.contract_name)
-        self.add_lib_contract(contract_info.name, contract_info.contract_class,
-                              abi, address)
-
-    def add_lib_contract(self, name, contract_class,
-                         abi, contract_address=None):
-        address = contract_address or get_contract_address_by_name(
-            abi, name)
-        logger.debug(f'Fetching abi for {name}, address {address}')
-        contract_abi = get_contract_abi_by_name(abi, name)
+        self.add_lib_contract(
+            contract_info.name,
+            contract_info.contract_class,
+            contract_info.contract_name,
+            address
+        )
+
+    def add_lib_contract(self, name: str, contract_class,
+                         contract_name: str, contract_address: Address = None):
+        address = contract_address or self.instance.get_contract_address(contract_name)
+        logger.debug('Fetching abi for %s, address %s', name, address)
+        contract_abi = self.instance.abi[contract_name]
         self.add_contract(name, contract_class(
             self, name, address, contract_abi))
 
     def add_contract(self, name, contract):
         self.__contracts[name] = contract
 
-    def get_contract_address(self, name):
-        return self.contract_manager.get_contract_address(name)
+    def get_contract_address(self, name) -> ChecksumAddress:
+        return self.web3.to_checksum_address(
+            self.instance.get_contract_address(name)
+        )
 
     def __get_contract_by_name(self, name):
         return self.__contracts[name]
 
     def __getattr__(self, name):
         if name not in self.__contracts:
             if not self.__contracts_info.get(name):
-                logger.warning(f'{name} method/contract wasn\'t found')
+                logger.warning("%s method/contract wasn't found", name)
                 return None
-            logger.debug(f'Contract {name} wasn\'t inited, creating now')
+            logger.debug("Contract %s wasn't inited, creating now", name)
             contract_info = self.__contracts_info[name]
-            abi = get_abi(self._abi_filepath)
-            self.__init_contract_from_info(abi, contract_info)
+            self.__init_contract_from_info(contract_info)
         return self.__get_contract_by_name(name)
```

### Comparing `skale.py-6.2b0/skale/skale_ima.py` & `skale.py-7.dev11/skale/skale_ima.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/skale_manager.py` & `skale.py-7.dev11/skale/skale_manager.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import logging
 
 from skale.skale_base import SkaleBase
 import skale.contracts.manager as contracts
 from skale.contracts.contract_manager import ContractManager
 from skale.utils.contract_info import ContractInfo
 from skale.utils.contract_types import ContractTypes
-from skale.utils.helper import get_abi, get_contracts_info
+from skale.utils.helper import get_contracts_info
 
 
 logger = logging.getLogger(__name__)
 
 
 CONTRACTS_INFO = [
     ContractInfo('contract_manager', 'ContractManager',
@@ -56,41 +56,36 @@
                  contracts.DelegationPeriodManager, ContractTypes.API, False),
     ContractInfo('validator_service', 'ValidatorService', contracts.ValidatorService,
                  ContractTypes.API, False),
     ContractInfo('token_state', 'TokenState', contracts.TokenState,
                  ContractTypes.API, False),
     ContractInfo('distributor', 'Distributor', contracts.Distributor,
                  ContractTypes.API, False),
-    ContractInfo('slashing_table', 'Distributor', contracts.SlashingTable,
+    ContractInfo('slashing_table', 'SlashingTable', contracts.SlashingTable,
                  ContractTypes.API, False),
     ContractInfo('wallets', 'Wallets', contracts.Wallets,
                  ContractTypes.API, True),
-    ContractInfo('bounty_v2', 'Bounty', contracts.BountyV2,
+    ContractInfo('bounty_v2', 'BountyV2', contracts.BountyV2,
                  ContractTypes.API, True),
     ContractInfo('punisher', 'Punisher', contracts.Punisher,
                  ContractTypes.API, True),
     ContractInfo('sync_manager', 'SyncManager', contracts.SyncManager,
                  ContractTypes.API, False),
-]
-
-
-DEBUG_CONTRACTS_INFO = [
-
     ContractInfo('time_helpers_with_debug', 'TimeHelpersWithDebug', contracts.TimeHelpersWithDebug,
                  ContractTypes.API, False)
 ]
 
 
 def spawn_skale_manager_lib(skale):
     """ Clone skale manager object with the same wallet """
     return SkaleManager(skale._endpoint, skale._abi_filepath, skale.wallet)
 
 
 class SkaleManager(SkaleBase):
+    """Represents skale-manager smart contracts"""
+    @property
+    def project_name(self) -> str:
+        return 'skale-manager'
+
     def set_contracts_info(self):
         self.init_contract_manager()
-        abi = get_abi(self._abi_filepath)
         self._SkaleBase__contracts_info = get_contracts_info(CONTRACTS_INFO)
-        if self._SkaleBase__is_debug_contracts(abi):
-            logger.info('Debug contracts found in ABI file')
-            self._SkaleBase__contracts_info.update(
-                get_contracts_info(DEBUG_CONTRACTS_INFO))
```

### Comparing `skale.py-6.2b0/skale/transactions/exceptions.py` & `skale.py-7.dev11/skale/transactions/exceptions.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/transactions/result.py` & `skale.py-7.dev11/skale/transactions/result.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/transactions/tools.py` & `skale.py-7.dev11/skale/transactions/tools.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/account_tools.py` & `skale.py-7.dev11/skale/utils/account_tools.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/constants.py` & `skale.py-7.dev11/skale/utils/constants.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/contract_info.py` & `skale.py-7.dev11/skale/utils/contract_info.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/contract_types.py` & `skale.py-7.dev11/skale/utils/contract_types.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/contracts_provision/__init__.py` & `skale.py-7.dev11/skale/utils/contracts_provision/__init__.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/contracts_provision/allocator.py` & `skale.py-7.dev11/skale/utils/contracts_provision/allocator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/contracts_provision/fake_multisig_contract.py` & `skale.py-7.dev11/skale/utils/contracts_provision/fake_multisig_contract.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/contracts_provision/main.py` & `skale.py-7.dev11/skale/utils/contracts_provision/main.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/contracts_provision/utils.py` & `skale.py-7.dev11/skale/utils/contracts_provision/utils.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/exceptions.py` & `skale.py-7.dev11/skale/utils/exceptions.py`

 * *Files 11% similar despite different names*

```diff
@@ -30,19 +30,12 @@
     """Raised when wrong wallet class passed"""
 
 
 class SChainNotFoundException(Exception):
     """Raised when requested sChain is not found"""
 
 
-class IncompatibleAbiError(Exception):
-    """Raised when required contract is not found in the ABI file"""
-    def __init__(self, key):
-        message = f'Required field was not found in the ABI file: {key}'
-        super().__init__(message)
-
-
 class InvalidNodeIdError(Exception):
     """Raised when wrong node id passed"""
     def __init__(self, node_id):
         message = f'Node with ID = {node_id} doesn\'t exist!'
         super().__init__(message)
```

### Comparing `skale.py-6.2b0/skale/utils/helper.py` & `skale.py-7.dev11/skale/utils/helper.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,17 +90,27 @@
     try:
         ipaddress.IPv4Address(address)
     except ValueError:
         return False
     return True
 
 
-def get_abi(abi_filepath=None):
-    with open(abi_filepath) as data_file:
-        return json.load(data_file)
+def get_abi(abi_filepath: string = None):
+    if abi_filepath:
+        with open(abi_filepath, encoding='utf-8') as data_file:
+            return json.load(data_file)
+    return {}
+
+
+def get_skale_manager_address(abi_filepath: string = None) -> str:
+    return get_abi(abi_filepath)['skale_manager_address']
+
+
+def get_allocator_address(abi_filepath: string = None) -> str:
+    return get_abi(abi_filepath)['allocator_address']
 
 
 def generate_nonce():  # pragma: no cover
     return randint(0, 65534)
 
 
 def random_string(size=6, chars=string.ascii_lowercase):  # pragma: no cover
```

### Comparing `skale.py-6.2b0/skale/utils/random_names/generator.py` & `skale.py-7.dev11/skale/utils/random_names/generator.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/random_names/vocabulary.py` & `skale.py-7.dev11/skale/utils/random_names/vocabulary.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/utils/web3_utils.py` & `skale.py-7.dev11/skale/utils/web3_utils.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/wallets/common.py` & `skale.py-7.dev11/skale/wallets/common.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/wallets/ledger_wallet.py` & `skale.py-7.dev11/skale/wallets/ledger_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/wallets/redis_wallet.py` & `skale.py-7.dev11/skale/wallets/redis_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/wallets/sgx_wallet.py` & `skale.py-7.dev11/skale/wallets/sgx_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale/wallets/web3_wallet.py` & `skale.py-7.dev11/skale/wallets/web3_wallet.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/skale.py.egg-info/PKG-INFO` & `skale.py-7.dev11/skale.py.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: skale.py
-Version: 6.2b0
+Version: 7.dev11
 Summary: SKALE client tools
 Home-page: https://github.com/skalenetwork/skale.py
 Author: SKALE Labs
 Author-email: support@skalelabs.com
 Keywords: skale
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `skale.py-6.2b0/skale.py.egg-info/SOURCES.txt` & `skale.py-7.dev11/skale.py.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,14 @@
 skale/schain_config/ports_allocation.py
 skale/schain_config/rotation_history.py
 skale/transactions/__init__.py
 skale/transactions/exceptions.py
 skale/transactions/result.py
 skale/transactions/tools.py
 skale/utils/__init__.py
-skale/utils/abi_utils.py
 skale/utils/account_tools.py
 skale/utils/constants.py
 skale/utils/contract_info.py
 skale/utils/contract_types.py
 skale/utils/exceptions.py
 skale/utils/helper.py
 skale/utils/web3_utils.py
```

### Comparing `skale.py-6.2b0/tests/schain_config/generator_test.py` & `skale.py-7.dev11/tests/schain_config/generator_test.py`

 * *Files identical despite different names*

### Comparing `skale.py-6.2b0/tests/schain_config/ports_allocation_test.py` & `skale.py-7.dev11/tests/schain_config/ports_allocation_test.py`

 * *Files identical despite different names*

