# Comparing `tmp/pantos_service_node-1.5.3-py3-none-any.whl.zip` & `tmp/pantos_service_node-1.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,95 +1,103 @@
-Zip file size: 118411 bytes, number of entries: 93
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 15:47 pantos/__init__.py
--rw-r--r--  2.0 unx     3251 b- defN 24-Feb-12 15:48 pantos/alembic.ini
--rw-r--r--  2.0 unx     7809 b- defN 24-Feb-12 15:48 pantos/bids.yaml
--rw-r--r--  2.0 unx     7182 b- defN 24-Feb-12 15:48 pantos/pantos-service-node.conf
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 15:47 pantos/common/__init__.py
--rw-r--r--  2.0 unx     4863 b- defN 24-Feb-12 15:47 pantos/common/configuration.py
--rw-r--r--  2.0 unx     4739 b- defN 24-Feb-12 15:47 pantos/common/entities.py
--rw-r--r--  2.0 unx     3311 b- defN 24-Feb-12 15:47 pantos/common/exceptions.py
--rw-r--r--  2.0 unx     7012 b- defN 24-Feb-12 15:47 pantos/common/logging.py
--rw-r--r--  2.0 unx     2969 b- defN 24-Feb-12 15:47 pantos/common/restapi.py
--rw-r--r--  2.0 unx    12286 b- defN 24-Feb-12 15:47 pantos/common/servicenodes.py
--rw-r--r--  2.0 unx     5315 b- defN 24-Feb-12 15:47 pantos/common/signer.py
--rw-r--r--  2.0 unx      509 b- defN 24-Feb-12 15:47 pantos/common/types.py
--rw-r--r--  2.0 unx       55 b- defN 24-Feb-12 15:47 pantos/common/blockchains/__init__.py
--rw-r--r--  2.0 unx      974 b- defN 24-Feb-12 15:47 pantos/common/blockchains/avalanche.py
--rw-r--r--  2.0 unx    41394 b- defN 24-Feb-12 15:47 pantos/common/blockchains/base.py
--rw-r--r--  2.0 unx      969 b- defN 24-Feb-12 15:47 pantos/common/blockchains/bnbchain.py
--rw-r--r--  2.0 unx      922 b- defN 24-Feb-12 15:47 pantos/common/blockchains/celo.py
--rw-r--r--  2.0 unx      938 b- defN 24-Feb-12 15:47 pantos/common/blockchains/cronos.py
--rw-r--r--  2.0 unx     1670 b- defN 24-Feb-12 15:47 pantos/common/blockchains/enums.py
--rw-r--r--  2.0 unx    19505 b- defN 24-Feb-12 15:47 pantos/common/blockchains/ethereum.py
--rw-r--r--  2.0 unx     3678 b- defN 24-Feb-12 15:47 pantos/common/blockchains/factory.py
--rw-r--r--  2.0 unx      938 b- defN 24-Feb-12 15:47 pantos/common/blockchains/fantom.py
--rw-r--r--  2.0 unx      946 b- defN 24-Feb-12 15:47 pantos/common/blockchains/polygon.py
--rw-r--r--  2.0 unx     3681 b- defN 24-Feb-12 15:47 pantos/common/blockchains/solana.py
--rw-r--r--  2.0 unx     6505 b- defN 24-Feb-12 15:47 pantos/common/blockchains/tasks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/__init__.py
--rw-r--r--  2.0 unx    33098 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/avalanche_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/avalanche_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/avalanche_standard_token.abi
--rw-r--r--  2.0 unx    33098 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/bnb_chain_standard_token.abi
--rw-r--r--  2.0 unx    33098 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/celo_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/celo_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/celo_standard_token.abi
--rw-r--r--  2.0 unx    33098 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/cronos_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/cronos_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/cronos_standard_token.abi
--rw-r--r--  2.0 unx    33098 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/ethereum_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/ethereum_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/ethereum_standard_token.abi
--rw-r--r--  2.0 unx    33098 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/fantom_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/fantom_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/fantom_standard_token.abi
--rw-r--r--  2.0 unx    33098 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/polygon_pantos_hub.abi
--rw-r--r--  2.0 unx     4069 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/polygon_pantos_token.abi
--rw-r--r--  2.0 unx     4840 b- defN 24-Feb-12 15:47 pantos/common/blockchains/contracts/polygon_standard_token.abi
--rw-r--r--  2.0 unx       79 b- defN 24-Feb-12 15:47 pantos/servicenode/__init__.py
--rw-r--r--  2.0 unx      806 b- defN 24-Feb-12 15:47 pantos/servicenode/__main__.py
--rw-r--r--  2.0 unx     3215 b- defN 24-Feb-12 15:47 pantos/servicenode/application.py
--rw-r--r--  2.0 unx     2636 b- defN 24-Feb-12 15:47 pantos/servicenode/celery.py
--rw-r--r--  2.0 unx     9094 b- defN 24-Feb-12 15:47 pantos/servicenode/configuration.py
--rw-r--r--  2.0 unx      221 b- defN 24-Feb-12 15:47 pantos/servicenode/exceptions.py
--rw-r--r--  2.0 unx    13968 b- defN 24-Feb-12 15:47 pantos/servicenode/restapi.py
--rw-r--r--  2.0 unx      198 b- defN 24-Feb-12 15:47 pantos/servicenode/wsgi.py
--rw-r--r--  2.0 unx       53 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/__init__.py
--rw-r--r--  2.0 unx      957 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/avalanche.py
--rw-r--r--  2.0 unx    22418 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/base.py
--rw-r--r--  2.0 unx      952 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/bnbchain.py
--rw-r--r--  2.0 unx      905 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/celo.py
--rw-r--r--  2.0 unx      921 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/cronos.py
--rw-r--r--  2.0 unx    16850 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/ethereum.py
--rw-r--r--  2.0 unx     1101 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/factory.py
--rw-r--r--  2.0 unx      921 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/fantom.py
--rw-r--r--  2.0 unx      929 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/polygon.py
--rw-r--r--  2.0 unx     2846 b- defN 24-Feb-12 15:47 pantos/servicenode/blockchains/solana.py
--rw-r--r--  2.0 unx       40 b- defN 24-Feb-12 15:47 pantos/servicenode/business/__init__.py
--rw-r--r--  2.0 unx      341 b- defN 24-Feb-12 15:47 pantos/servicenode/business/base.py
--rw-r--r--  2.0 unx     3579 b- defN 24-Feb-12 15:47 pantos/servicenode/business/bids.py
--rw-r--r--  2.0 unx     3341 b- defN 24-Feb-12 15:47 pantos/servicenode/business/node.py
--rw-r--r--  2.0 unx     4446 b- defN 24-Feb-12 15:47 pantos/servicenode/business/plugins.py
--rw-r--r--  2.0 unx    37736 b- defN 24-Feb-12 15:47 pantos/servicenode/business/transfers.py
--rw-r--r--  2.0 unx     2778 b- defN 24-Feb-12 15:47 pantos/servicenode/database/__init__.py
--rw-r--r--  2.0 unx    20036 b- defN 24-Feb-12 15:47 pantos/servicenode/database/access.py
--rw-r--r--  2.0 unx     1166 b- defN 24-Feb-12 15:47 pantos/servicenode/database/enums.py
--rw-r--r--  2.0 unx     1234 b- defN 24-Feb-12 15:47 pantos/servicenode/database/exceptions.py
--rw-r--r--  2.0 unx    13701 b- defN 24-Feb-12 15:47 pantos/servicenode/database/models.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 15:47 pantos/servicenode/database/migrations/__init__.py
--rw-r--r--  2.0 unx     2080 b- defN 24-Feb-12 15:47 pantos/servicenode/database/migrations/env.py
--rw-r--r--  2.0 unx      817 b- defN 24-Feb-12 15:47 pantos/servicenode/database/migrations/versions/5e552e0ec844_remove_id_from_bids_table.py
--rw-r--r--  2.0 unx     1520 b- defN 24-Feb-12 15:47 pantos/servicenode/database/migrations/versions/85982c1f3b95_create_deferrable_constraint.py
--rw-r--r--  2.0 unx        0 b- defN 24-Feb-12 15:47 pantos/servicenode/database/migrations/versions/__init__.py
--rw-r--r--  2.0 unx     4152 b- defN 24-Feb-12 15:47 pantos/servicenode/database/migrations/versions/bd913c5bfdfb_off_chain_bids.py
--rw-r--r--  2.0 unx     7067 b- defN 24-Feb-12 15:47 pantos/servicenode/database/migrations/versions/c4c46d14ca6a_initial_database_schema.py
--rw-r--r--  2.0 unx     1675 b- defN 24-Feb-12 15:47 pantos/servicenode/plugins/__init__.py
--rw-r--r--  2.0 unx     2476 b- defN 24-Feb-12 15:47 pantos/servicenode/plugins/base.py
--rw-r--r--  2.0 unx     3368 b- defN 24-Feb-12 15:47 pantos/servicenode/plugins/bids.py
--rw-r--r--  2.0 unx    35148 b- defN 24-Feb-12 15:48 pantos_service_node-1.5.3.dist-info/LICENSE.md
--rw-r--r--  2.0 unx      775 b- defN 24-Feb-12 15:48 pantos_service_node-1.5.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-12 15:48 pantos_service_node-1.5.3.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Feb-12 15:48 pantos_service_node-1.5.3.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     9226 b- defN 24-Feb-12 15:48 pantos_service_node-1.5.3.dist-info/RECORD
-93 files, 671341 bytes uncompressed, 103303 bytes compressed:  84.6%
+Zip file size: 128420 bytes, number of entries: 101
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/__init__.py
+-rw-r--r--  2.0 unx     3251 b- defN 24-Apr-23 10:21 pantos/alembic.ini
+-rw-r--r--  2.0 unx     7809 b- defN 24-Apr-23 10:21 pantos/bids.yml
+-rw-r--r--  2.0 unx     5415 b- defN 24-Apr-23 10:21 pantos/service-node-config.env
+-rw-r--r--  2.0 unx    14841 b- defN 24-Apr-23 10:21 pantos/service-node-config.yml
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/common/__init__.py
+-rw-r--r--  2.0 unx     6041 b- defN 24-Apr-23 10:20 pantos/common/configuration.py
+-rw-r--r--  2.0 unx     4739 b- defN 24-Apr-23 10:20 pantos/common/entities.py
+-rw-r--r--  2.0 unx     3311 b- defN 24-Apr-23 10:20 pantos/common/exceptions.py
+-rw-r--r--  2.0 unx     7012 b- defN 24-Apr-23 10:20 pantos/common/logging.py
+-rw-r--r--  2.0 unx     2969 b- defN 24-Apr-23 10:20 pantos/common/restapi.py
+-rw-r--r--  2.0 unx    12286 b- defN 24-Apr-23 10:20 pantos/common/servicenodes.py
+-rw-r--r--  2.0 unx     5043 b- defN 24-Apr-23 10:20 pantos/common/signer.py
+-rw-r--r--  2.0 unx      509 b- defN 24-Apr-23 10:20 pantos/common/types.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-23 10:20 pantos/common/blockchains/__init__.py
+-rw-r--r--  2.0 unx      974 b- defN 24-Apr-23 10:20 pantos/common/blockchains/avalanche.py
+-rw-r--r--  2.0 unx    41291 b- defN 24-Apr-23 10:20 pantos/common/blockchains/base.py
+-rw-r--r--  2.0 unx      969 b- defN 24-Apr-23 10:20 pantos/common/blockchains/bnbchain.py
+-rw-r--r--  2.0 unx      922 b- defN 24-Apr-23 10:20 pantos/common/blockchains/celo.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-23 10:20 pantos/common/blockchains/cronos.py
+-rw-r--r--  2.0 unx     1695 b- defN 24-Apr-23 10:20 pantos/common/blockchains/enums.py
+-rw-r--r--  2.0 unx    19287 b- defN 24-Apr-23 10:20 pantos/common/blockchains/ethereum.py
+-rw-r--r--  2.0 unx     3642 b- defN 24-Apr-23 10:20 pantos/common/blockchains/factory.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-23 10:20 pantos/common/blockchains/fantom.py
+-rw-r--r--  2.0 unx      946 b- defN 24-Apr-23 10:20 pantos/common/blockchains/polygon.py
+-rw-r--r--  2.0 unx     3596 b- defN 24-Apr-23 10:20 pantos/common/blockchains/solana.py
+-rw-r--r--  2.0 unx     6505 b- defN 24-Apr-23 10:20 pantos/common/blockchains/tasks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/__init__.py
+-rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi
+-rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_pantos_hub.abi
+-rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_pantos_token.abi
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/avalanche_standard_token.abi
+-rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi
+-rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi
+-rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/bnb_chain_standard_token.abi
+-rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_pantos_forwarder.abi
+-rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_pantos_hub.abi
+-rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_pantos_token.abi
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/celo_standard_token.abi
+-rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi
+-rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_pantos_hub.abi
+-rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_pantos_token.abi
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/cronos_standard_token.abi
+-rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi
+-rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_pantos_hub.abi
+-rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_pantos_token.abi
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/ethereum_standard_token.abi
+-rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi
+-rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_pantos_hub.abi
+-rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_pantos_token.abi
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/fantom_standard_token.abi
+-rw-r--r--  2.0 unx     7229 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi
+-rw-r--r--  2.0 unx    42156 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_pantos_hub.abi
+-rw-r--r--  2.0 unx     4069 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_pantos_token.abi
+-rw-r--r--  2.0 unx     4840 b- defN 24-Apr-23 10:20 pantos/common/blockchains/contracts/polygon_standard_token.abi
+-rw-r--r--  2.0 unx       79 b- defN 24-Apr-23 10:20 pantos/servicenode/__init__.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-23 10:20 pantos/servicenode/__main__.py
+-rw-r--r--  2.0 unx     3257 b- defN 24-Apr-23 10:20 pantos/servicenode/application.py
+-rw-r--r--  2.0 unx     2641 b- defN 24-Apr-23 10:20 pantos/servicenode/celery.py
+-rw-r--r--  2.0 unx     9432 b- defN 24-Apr-23 10:20 pantos/servicenode/configuration.py
+-rw-r--r--  2.0 unx      221 b- defN 24-Apr-23 10:20 pantos/servicenode/exceptions.py
+-rw-r--r--  2.0 unx    13968 b- defN 24-Apr-23 10:20 pantos/servicenode/restapi.py
+-rw-r--r--  2.0 unx      198 b- defN 24-Apr-23 10:20 pantos/servicenode/wsgi.py
+-rw-r--r--  2.0 unx       53 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/__init__.py
+-rw-r--r--  2.0 unx      957 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/avalanche.py
+-rw-r--r--  2.0 unx    22379 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/base.py
+-rw-r--r--  2.0 unx      952 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/bnbchain.py
+-rw-r--r--  2.0 unx      905 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/celo.py
+-rw-r--r--  2.0 unx      921 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/cronos.py
+-rw-r--r--  2.0 unx    16807 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/ethereum.py
+-rw-r--r--  2.0 unx     1101 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/factory.py
+-rw-r--r--  2.0 unx      921 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/fantom.py
+-rw-r--r--  2.0 unx      929 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/polygon.py
+-rw-r--r--  2.0 unx     2846 b- defN 24-Apr-23 10:20 pantos/servicenode/blockchains/solana.py
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-23 10:20 pantos/servicenode/business/__init__.py
+-rw-r--r--  2.0 unx      341 b- defN 24-Apr-23 10:20 pantos/servicenode/business/base.py
+-rw-r--r--  2.0 unx     3574 b- defN 24-Apr-23 10:20 pantos/servicenode/business/bids.py
+-rw-r--r--  2.0 unx     3341 b- defN 24-Apr-23 10:20 pantos/servicenode/business/node.py
+-rw-r--r--  2.0 unx     4446 b- defN 24-Apr-23 10:20 pantos/servicenode/business/plugins.py
+-rw-r--r--  2.0 unx    37731 b- defN 24-Apr-23 10:20 pantos/servicenode/business/transfers.py
+-rw-r--r--  2.0 unx     3477 b- defN 24-Apr-23 10:20 pantos/servicenode/database/__init__.py
+-rw-r--r--  2.0 unx    20036 b- defN 24-Apr-23 10:20 pantos/servicenode/database/access.py
+-rw-r--r--  2.0 unx     1166 b- defN 24-Apr-23 10:20 pantos/servicenode/database/enums.py
+-rw-r--r--  2.0 unx     1234 b- defN 24-Apr-23 10:20 pantos/servicenode/database/exceptions.py
+-rw-r--r--  2.0 unx    13701 b- defN 24-Apr-23 10:20 pantos/servicenode/database/models.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/__init__.py
+-rw-r--r--  2.0 unx     2080 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/env.py
+-rw-r--r--  2.0 unx      817 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/5e552e0ec844_remove_id_from_bids_table.py
+-rw-r--r--  2.0 unx     1520 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/85982c1f3b95_create_deferrable_constraint.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/__init__.py
+-rw-r--r--  2.0 unx     4152 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/bd913c5bfdfb_off_chain_bids.py
+-rw-r--r--  2.0 unx     7067 b- defN 24-Apr-23 10:20 pantos/servicenode/database/migrations/versions/c4c46d14ca6a_initial_database_schema.py
+-rw-r--r--  2.0 unx     1675 b- defN 24-Apr-23 10:20 pantos/servicenode/plugins/__init__.py
+-rw-r--r--  2.0 unx     2476 b- defN 24-Apr-23 10:20 pantos/servicenode/plugins/base.py
+-rw-r--r--  2.0 unx     3368 b- defN 24-Apr-23 10:20 pantos/servicenode/plugins/bids.py
+-rw-r--r--  2.0 unx    35148 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx      856 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    10159 b- defN 24-Apr-23 10:21 pantos_service_node-1.6.0.dist-info/RECORD
+101 files, 800919 bytes uncompressed, 111752 bytes compressed:  86.0%
```

## zipnote {}

```diff
@@ -1,17 +1,20 @@
 Filename: pantos/__init__.py
 Comment: 
 
 Filename: pantos/alembic.ini
 Comment: 
 
-Filename: pantos/bids.yaml
+Filename: pantos/bids.yml
 Comment: 
 
-Filename: pantos/pantos-service-node.conf
+Filename: pantos/service-node-config.env
+Comment: 
+
+Filename: pantos/service-node-config.yml
 Comment: 
 
 Filename: pantos/common/__init__.py
 Comment: 
 
 Filename: pantos/common/configuration.py
 Comment: 
@@ -75,68 +78,89 @@
 
 Filename: pantos/common/blockchains/tasks.py
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/__init__.py
 Comment: 
 
+Filename: pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi
+Comment: 
+
 Filename: pantos/common/blockchains/contracts/avalanche_pantos_hub.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/avalanche_pantos_token.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/avalanche_standard_token.abi
 Comment: 
 
+Filename: pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi
+Comment: 
+
 Filename: pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/bnb_chain_standard_token.abi
 Comment: 
 
+Filename: pantos/common/blockchains/contracts/celo_pantos_forwarder.abi
+Comment: 
+
 Filename: pantos/common/blockchains/contracts/celo_pantos_hub.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/celo_pantos_token.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/celo_standard_token.abi
 Comment: 
 
+Filename: pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi
+Comment: 
+
 Filename: pantos/common/blockchains/contracts/cronos_pantos_hub.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/cronos_pantos_token.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/cronos_standard_token.abi
 Comment: 
 
+Filename: pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi
+Comment: 
+
 Filename: pantos/common/blockchains/contracts/ethereum_pantos_hub.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/ethereum_pantos_token.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/ethereum_standard_token.abi
 Comment: 
 
+Filename: pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi
+Comment: 
+
 Filename: pantos/common/blockchains/contracts/fantom_pantos_hub.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/fantom_pantos_token.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/fantom_standard_token.abi
 Comment: 
 
+Filename: pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi
+Comment: 
+
 Filename: pantos/common/blockchains/contracts/polygon_pantos_hub.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/polygon_pantos_token.abi
 Comment: 
 
 Filename: pantos/common/blockchains/contracts/polygon_standard_token.abi
@@ -258,23 +282,23 @@
 
 Filename: pantos/servicenode/plugins/base.py
 Comment: 
 
 Filename: pantos/servicenode/plugins/bids.py
 Comment: 
 
-Filename: pantos_service_node-1.5.3.dist-info/LICENSE.md
+Filename: pantos_service_node-1.6.0.dist-info/LICENSE.md
 Comment: 
 
-Filename: pantos_service_node-1.5.3.dist-info/METADATA
+Filename: pantos_service_node-1.6.0.dist-info/METADATA
 Comment: 
 
-Filename: pantos_service_node-1.5.3.dist-info/WHEEL
+Filename: pantos_service_node-1.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: pantos_service_node-1.5.3.dist-info/top_level.txt
+Filename: pantos_service_node-1.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: pantos_service_node-1.5.3.dist-info/RECORD
+Filename: pantos_service_node-1.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pantos/common/configuration.py

```diff
@@ -1,21 +1,57 @@
 """Module for loading and parsing a configuration file.
 
 """
+import errno
 import importlib.resources
 import logging
+import os
 import pathlib
 
 import cerberus  # type: ignore
+import dotenv
+import pyaml_env  # type: ignore
 import yaml
 
 from pantos.common.exceptions import BaseError
 
 _logger = logging.getLogger(__name__)
 
+# Ordered by priority
+_CONFIGURATION_PATHS = [
+    pathlib.Path.cwd(),
+    pathlib.Path.home(),
+    pathlib.Path.home() / '.config',
+    pathlib.Path('/etc/pantos'),
+    pathlib.Path('/etc')
+]
+
+if os.environ.get('PANTOS_CONFIG'):
+    _logger.info('loading configuration from environment variable '
+                 'PANTOS_CONFIG')
+    _CONFIGURATION_PATHS.insert(0, pathlib.Path(os.environ['PANTOS_CONFIG']))
+
+
+class _CustomValidator(cerberus.Validator):
+    def _validate_one_not_present(self, other: str, field: str, value: str):
+        if (bool(value)) == (bool(self.document.get(other))):
+            self._error(field, "only one field can be present: " + other)
+
+    def _normalize_coerce_load_if_file(self, value: str):
+        path = pathlib.Path(value)
+        try:
+            # This method may trigger an exception if the path is not valid
+            if path.is_file():
+                with open(path, 'r') as file:
+                    return file.read()
+        except OSError as error:
+            if error.errno != errno.ENAMETOOLONG:
+                raise error
+        return value
+
 
 class ConfigError(BaseError):
     """Exception class for all configuration errors.
 
     """
     pass
 
@@ -76,71 +112,71 @@
             # Use the specified configuration file
             path = pathlib.Path(file_path)
             if not path.is_file():
                 raise ConfigError('no configuration file found at '
                                   '{}'.format(file_path))
             return path
         # Find the configuration file at common locations
-        # Current working directory
-        path = pathlib.Path.cwd() / self.default_file_name
-        if path.is_file():
-            return path
-        # Home directory
-        path = pathlib.Path.home() / self.default_file_name
-        if path.is_file():
-            return path
-        # Hidden file in home directory
-        path = pathlib.Path.home() / '.{}'.format(self.default_file_name)
-        if path.is_file():
-            return path
-        # Subdirectory .config in home directory
-        path = pathlib.Path.home() / '.config' / self.default_file_name
-        if path.is_file():
-            return path
-        # Configuration directory /etc
-        path = pathlib.Path('/etc') / self.default_file_name
-        if path.is_file():
-            return path
+        for path in _CONFIGURATION_PATHS:
+            config_path = path
+            if config_path.is_dir():
+                config_path = config_path / self.default_file_name
+            if config_path.is_file():
+                return config_path
         # Package resource
         if importlib.resources.is_resource('pantos', self.default_file_name):
             with importlib.resources.path('pantos',
                                           self.default_file_name) as path:
                 return path
         # No configuration file found at common locations
         raise ConfigError('no configuration file found')
 
     def __parse_file(self, path):
         """TODO
 
         """
         assert isinstance(path, pathlib.Path)
-        with path.open() as config_file:
-            # Parse the YAML code in the configuration file
-            try:
-                return yaml.safe_load(config_file)
-            except yaml.YAMLError as error:
-                if hasattr(error, 'problem_mark'):
-                    line = error.problem_mark.line + 1
-                    column = error.problem_mark.column + 1
-                    raise ConfigError('YAML code in configuration file '
-                                      'invalid at line {} and '
-                                      'column {}'.format(line, column))
-                else:
-                    raise ConfigError('YAML code in configuration file '
-                                      'invalid')
+        # List of potential .env file paths
+        env_files = [
+            pathlib.Path(path.as_posix() + '.env'),
+            pathlib.Path(path.with_suffix('.env').as_posix())
+        ]
+
+        # Iterate over the potential .env file paths
+        for env_file in env_files:
+            if env_file.is_file():
+                try:
+                    dotenv.load_dotenv(env_file)
+                    _logger.info(f'loaded .env from file {env_file}')
+                    break
+                except Exception:
+                    raise ConfigError(f'unable to load .env file {env_file}')
+        # Parse the YAML code in the configuration file
+        try:
+            return pyaml_env.parse_config(path.as_posix(), default_value='')
+        except yaml.YAMLError as error:
+            if hasattr(error, 'problem_mark'):
+                line = error.problem_mark.line + 1
+                column = error.problem_mark.column + 1
+                raise ConfigError('YAML code in configuration file '
+                                  'invalid at line {} and '
+                                  'column {}'.format(line, column))
+            else:
+                raise ConfigError('YAML code in configuration file '
+                                  'invalid')
 
     def __validate(self, config_dict, validation_schema):
         """TODO
 
         """
         assert isinstance(config_dict, dict)
         assert isinstance(validation_schema, dict)
         # Create the validator and validate the validation schema
         try:
-            validator = cerberus.Validator(validation_schema)
+            validator = _CustomValidator(validation_schema)
         except cerberus.schema.SchemaError as error:
             raise ConfigError('validation schema invalid: {}'.format(error))
         # Validate the configuration
         if not validator.validate(config_dict):
             raise ConfigError('configuration file invalid: '
                               '{}'.format(validator.errors))
         # Add default configuration values
```

## pantos/common/signer.py

```diff
@@ -1,9 +1,8 @@
 import getpass
-import pathlib
 import typing
 
 import Crypto.PublicKey.ECC
 import Crypto.Signature.eddsa
 
 
 class SignerError(Exception):
@@ -24,27 +23,27 @@
             Additional information about the error as keyword arguments.
 
         """
         super().__init__(message, name, **kwargs)
 
 
 class _Signer:
-    def __init__(self, pem_path: str, pem_password: str):
+    def __init__(self, pem_value: str, pem_password: str):
         """
         Constructor of Signer class.
 
         Parameters
         ----------
-        pem_path : str
-            Path to the PEM file containing the private key.
+        pem_value : str
+            Value of the encrypted private key.
         pem_password : str
             Password to unlock the PEM file.
 
         """
-        self.__signer = self._load_signer(pem_path, pem_password)
+        self.__signer = self._load_signer(pem_value, pem_password)
 
     def sign_message(self, message: str) -> str:
         """Sign a message.
 
         Parameters
         ----------
         message : str
@@ -123,23 +122,23 @@
         message = ''
         for message_part in message_parts:
             message += f'{str(message_part)}{separator}'
         # cutting of last separator
         return message[:-1]
 
     def _load_signer(
-            self, pem_path: str,
+            self, pem_value: str,
             pem_password: str) -> Crypto.Signature.eddsa.EdDSASigScheme:
         """Load the EdDSA signer object from a password-encrypted pem file.
         The key must be on the curve Ed25519 or Ed448.
 
         Parameters
         ----------
-        pem_path : str
-            Path to the PEM file containing the private key.
+        pem_value : str
+            Value of the encrypted private key.
         pem_password : str
             Password to unlock the PEM file.
 
         Returns
         -------
         Crypto.Signature.eddsa.EdDSASigScheme
             An EdDSA signature object.
@@ -147,41 +146,38 @@
         Raises
         ------
         SignerError
             If the EdDSA signer cannot be loaded.
 
         """
         try:
-            private_key_path = pathlib.Path(pem_path)
-            if not private_key_path.is_file():
-                raise SignerError(
-                    f'private key "{private_key_path}" is not a file')
             if pem_password is None:
                 pem_password = getpass.getpass(
                     'Password for decrypting the pem file')
+
             private_key = Crypto.PublicKey.ECC.import_key(
-                open(private_key_path).read(), passphrase=pem_password)
+                pem_value, passphrase=pem_password)
             return Crypto.Signature.eddsa.new(private_key,
                                               'rfc8032')  # type: ignore
         except SignerError:
             raise
         except Exception:
             raise SignerError('cannot load the private key')
 
 
 _signer: typing.Optional[_Signer] = None
 
 
-def get_signer(pem_path: str, pem_password: str) -> _Signer:
+def get_signer(pem_value: str, pem_password: str) -> _Signer:
     """Get a _Signer object.
 
     Parameters
     ----------
-    pem_path : str
-        Path to the PEM file containing the private key.
+    pem_value : str
+        Value of the encrypted private key.
     pem_password : str
         Password to unlock the PEM file.
 
     Returns
     -------
     _Signer
         Signer object used for signing and verifying messages.
@@ -190,9 +186,9 @@
     ------
     SignerError
         If the signer cannot be gotten.
 
     """
     global _signer
     if not _signer:
-        _signer = _Signer(pem_path, pem_password)
+        _signer = _Signer(pem_value, pem_password)
     return _signer
```

## pantos/common/blockchains/base.py

```diff
@@ -255,15 +255,15 @@
 
             """
             self.__objects = [object_[index] for object_ in self.__objects]
             return self
 
         def __call__(
                 self, *args: typing.Any, **kwargs: typing.Any) -> \
-                'NodeConnections.Wrapper' | typing.Any:
+                typing.Union['NodeConnections.Wrapper', typing.Any]:
             """Forward the called method to the wrapped objects. If it
             sends a transaction to the blockchain node, it will be
             forwarded to only one of them, randomly chosen.
 
             Returns
             -------
             Wrapper or Any
@@ -424,16 +424,15 @@
 
     """
     def __init__(self, blockchain_node_urls: list[str],
                  fallback_blockchain_node_urls: list[str],
                  average_block_time: int,
                  required_transaction_confirmations: int,
                  transaction_network_id: typing.Optional[int],
-                 default_private_key: typing.Optional[tuple[pathlib.Path,
-                                                            str]] = None,
+                 default_private_key: typing.Optional[tuple[str, str]] = None,
                  celery_tasks_enabled: bool = False):
         """Construct a blockchain utilities instance.
 
         Parameters
         ----------
         blockchain_node_urls : list of str
             The URLs of the nodes to use for communication with the
@@ -450,17 +449,17 @@
         transaction_network_id : int or None
             The unique public (i.e. non-Pantos-specific) blockchain
             network identifier (partly called chain ID) to be used for
             signing transactions (to prevent replay attacks between
             different compatible blockchain networks). It is assumed to
             be the identifier of the main or a test network of the
             blockchain supported by the blockchain utilities subclass.
-        default_private_key : tuple of pathlib.Path and str, optional
-            The keystore file path and password of the default private
-            key to be used by the blockchain utilities (default: None).
+        default_private_key : tuple of str and str, optional
+            The keystore value and password of the default private
+            key to be used by the blockchain utilities. (default: None).
         celery_tasks_enabled : bool, optional
             If True, Celery tasks are enabled for enhanced
             functionalities (default: False). This requires a proper
             Celery environment to be set up by the project using the
             blockchain utilities.
 
         Raises
@@ -487,15 +486,15 @@
         self.average_block_time = average_block_time
         self.required_transaction_confirmations = \
             required_transaction_confirmations
         self.transaction_network_id = transaction_network_id
         self._blockchain_node_urls = blockchain_node_urls
         self._fallback_blockchain_node_urls = fallback_blockchain_node_urls
         self._default_private_key = (
-            None if default_private_key is None else self.load_private_key(
+            None if default_private_key is None else self.decrypt_private_key(
                 default_private_key[0], default_private_key[1]))
         self._default_address = (None if self._default_private_key is None else
                                  self.get_address(self._default_private_key))
         self._celery_tasks_enabled = celery_tasks_enabled
         self.__loaded_contract_abis: dict[ContractAbi, list[typing.Any]] = {}
 
     def create_node_connections(
@@ -686,33 +685,33 @@
             self.__loaded_contract_abis[contract_abi] = loaded_contract_abi
             return loaded_contract_abi
         except Exception:
             raise self._create_error('unable to load a contract ABI',
                                      contract_abi=contract_abi)
 
     @abc.abstractmethod
-    def load_private_key(self, key_path: pathlib.Path, password: str) -> str:
-        """Load the private key from a password-encrypted key file.
+    def decrypt_private_key(self, encrypted_key: str, password: str) -> str:
+        """Load the private key from a password-encrypted key.
 
         Parameters
         ----------
-        key_path : pathlib.Path
-            The path to the key file.
+        encrypted_key: str
+            The encrypted key.
         password : str
-            The password to decrypt the key file.
+            The password to decrypt the key.
 
         Returns
         -------
         str
             The decrypted private key.
 
         Raises
         ------
         BlockchainUtilitiesError
-            If the private key cannot be loaded from the key file.
+            If the private key cannot be decrypted.
 
         """
         pass  # pragma: no cover
 
     @abc.abstractmethod
     def read_transaction_status(
             self, transaction_id: str,
```

## pantos/common/blockchains/enums.py

```diff
@@ -51,14 +51,15 @@
 class ContractAbi(enum.Enum):
     """Enumeration of supported contract ABIs.
 
     """
     STANDARD_TOKEN = 0
     PANTOS_TOKEN = 1
     PANTOS_HUB = 2
+    PANTOS_FORWARDER = 3
 
     def get_file_name(self, blockchain: Blockchain) -> str:
         """Get the name of the contract ABI file.
 
         Parameters
         ----------
         blockchain : Blockchain
```

## pantos/common/blockchains/ethereum.py

```diff
@@ -1,12 +1,11 @@
 """Module for Ethereum-specific utilities and errors.
 
 """
 import logging
-import pathlib
 import typing
 import urllib.parse
 
 import web3
 import web3.contract.contract
 import web3.exceptions
 import web3.middleware
@@ -46,16 +45,15 @@
 
     """
     def __init__(self, blockchain_node_urls: list[str],
                  fallback_blockchain_node_urls: list[str],
                  average_block_time: int,
                  required_transaction_confirmations: int,
                  transaction_network_id: typing.Optional[int],
-                 default_private_key: typing.Optional[tuple[pathlib.Path,
-                                                            str]] = None,
+                 default_private_key: typing.Optional[tuple[str, str]] = None,
                  celery_tasks_enabled: bool = False):
         # Docstring inherited
         if transaction_network_id is None:
             raise self._create_error(
                 'transaction network ID (chain ID) must be given')
         super().__init__(blockchain_node_urls, fallback_blockchain_node_urls,
                          average_block_time,
@@ -218,23 +216,20 @@
         # Docstring inherited
         return address_one.lower() == address_two.lower()
 
     def _get_transaction_method_names(self) -> list[str]:
         # Docstring inherited
         return _TRANSACTION_METHOD_NAMES
 
-    def load_private_key(self, key_path: pathlib.Path, password: str) -> str:
+    def decrypt_private_key(self, encrypted_key: str, password: str) -> str:
         # Docstring inherited
         try:
-            with key_path.open() as key_file:
-                encrypted_key = key_file.read()
             private_key = web3.Account.decrypt(encrypted_key, password).hex()
         except Exception:
-            raise self._create_error(
-                'cannot load the private key "{}"'.format(key_path))
+            raise self._create_error('cannot load the private key')
         # Return the private key hex string without the leading 0x
         assert private_key.startswith('0x')
         return private_key[2:]
 
     def read_transaction_status(
             self, transaction_id: str,
             node_connections: typing.Optional[NodeConnections] = None) \
```

## pantos/common/blockchains/factory.py

```diff
@@ -1,11 +1,10 @@
 """Factory for Pantos blockchain utilities.
 
 """
-import pathlib
 import typing
 
 from pantos.common.blockchains.base import BlockchainUtilities
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.exceptions import NotInitializedError
 
 _blockchain_utilities: dict[Blockchain, BlockchainUtilities] = {}
@@ -16,15 +15,15 @@
 
 
 def initialize_blockchain_utilities(
         blockchain: Blockchain, blockchain_node_urls: list[str],
         fallback_blockchain_node_urls: list[str], average_block_time: int,
         required_transaction_confirmations: int,
         transaction_network_id: typing.Optional[int],
-        default_private_key: typing.Optional[tuple[pathlib.Path, str]] = None,
+        default_private_key: typing.Optional[tuple[str, str]] = None,
         celery_tasks_enabled: bool = False) -> None:
     """Initialize the utilities for the specified blockchain.
 
     Parameters
     ----------
     blockchain : Blockchain
         The blockchain to initialize a utilities instance for.
@@ -43,17 +42,17 @@
     transaction_network_id : int or None
         The unique public (i.e. non-Pantos-specific) blockchain network
         identifier (partly called chain ID) to be used for signing
         transactions (to prevent replay attacks between different
         compatible blockchain networks). It is assumed to be the
         identifier of the main or a test network of the specified
         blockchain.
-    default_private_key : tuple of pathlib.Path and str, optional
-        The keystore file path and password of the default private key
-        to be used by the blockchain utilities (default: None).
+    default_private_key : tuple of str and str, optional
+        The keystore value and password of the default private
+        key to be used by the blockchain utilities. (default: None).
     celery_tasks_enabled : bool, optional
         If True, Celery tasks are enabled for enhanced functionalities
         (default: False). This requires a proper Celery environment to
         be set up by the project using the blockchain utilities.
 
     Raises
     ------
```

## pantos/common/blockchains/solana.py

```diff
@@ -1,11 +1,10 @@
 """Module for Solana-specific utilities and errors.
 
 """
-import pathlib
 import typing
 
 from pantos.common.blockchains.base import BlockchainUtilities
 from pantos.common.blockchains.base import BlockchainUtilitiesError
 from pantos.common.blockchains.base import NodeConnections
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.entities import TransactionStatus
@@ -23,16 +22,15 @@
 
     """
     def __init__(self, blockchain_node_urls: list[str],
                  fallback_blockchain_node_urls: list[str],
                  average_block_time: int,
                  required_transaction_confirmations: int,
                  transaction_network_id: typing.Optional[int],
-                 default_private_key: typing.Optional[tuple[pathlib.Path,
-                                                            str]] = None,
+                 default_private_key: typing.Optional[tuple[str, str]] = None,
                  celery_tasks_enabled: bool = False):
         # Docstring inherited
         super().__init__(blockchain_node_urls, fallback_blockchain_node_urls,
                          average_block_time,
                          required_transaction_confirmations,
                          transaction_network_id,
                          default_private_key=default_private_key,
@@ -67,15 +65,15 @@
         # Docstring inherited
         raise NotImplementedError
 
     def _get_transaction_method_names(self) -> list[str]:
         # Docstring inherited
         raise NotImplementedError  # pragma: no cover
 
-    def load_private_key(self, key_path: pathlib.Path, password: str) -> str:
+    def decrypt_private_key(self, encrypted_key: str, password: str) -> str:
         # Docstring inherited
         raise NotImplementedError  # pragma: no cover
 
     def read_transaction_status(
             self, transaction_id: str,
             node_connections: typing.Optional[NodeConnections] = None) \
             -> TransactionStatus:
```

## pantos/common/blockchains/contracts/avalanche_pantos_hub.abi

### Pretty-printed

 * *Similarity: 0.48589743589743595%*

 * *Differences: {'13': "{'name': 'getPrimaryValidatorNode'}",*

 * * '18': "{'inputs': [], 'name': 'getUnbondingPeriodServiceNodeStake', 'outputs': {0: "*

 * *       "{'internalType': 'uint256', 'type': 'uint256', delete: ['components']}}}",*

 * * '19': "{'inputs': [OrderedDict([('name', 'blockchainId'), ('type', 'uint256'), ('internalType', "*

 * *       "'uint256')])], 'name': 'getValidatorFeeRecord', 'outputs': {0: {'internalType': 'struct "*

 * *       "PantosTypes.ValidatorFeeRecord', 'type': 'tuple', 'components': [OrderedDict([('name', "*

 * *    […]*

```diff
@@ -1,405 +1,9 @@
 [
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainNameUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "minimumTrustedValidatorFeeUpdatePeriod",
-                "type": "uint256"
-            }
-        ],
-        "name": "MinimumTrustedValidatorFeeUpdatePeriodUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosForwarder",
-                "type": "address"
-            }
-        ],
-        "name": "PantosForwarderSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosToken",
-                "type": "address"
-            }
-        ],
-        "name": "PantosTokenSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosValidator",
-                "type": "address"
-            }
-        ],
-        "name": "PantosValidatorSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUrlUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "transferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "recipient",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sourceToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "destinationToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "TransferFrom",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceTransactionId",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sender",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "destinationToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "TransferTo",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "oldFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "newFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "validFrom",
-                "type": "uint256"
-            }
-        ],
-        "name": "TrustedValidatorFeeUpdated",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             }
         ],
@@ -548,15 +152,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getMinimumTrustedValidatorFeeUpdatePeriod",
+        "name": "getMinimumValidatorFeeUpdatePeriod",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
@@ -613,15 +217,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPantosValidator",
+        "name": "getPrimaryValidatorNode",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
@@ -733,22 +337,35 @@
                 "type": "address[]"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "getUnbondingPeriodServiceNodeStake",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint256",
                 "name": "blockchainId",
                 "type": "uint256"
             }
         ],
-        "name": "getTrustedValidatorFeeRecord",
+        "name": "getValidatorFeeRecord",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "oldFactor",
                         "type": "uint256"
@@ -760,36 +377,23 @@
                     },
                     {
                         "internalType": "uint256",
                         "name": "validFrom",
                         "type": "uint256"
                     }
                 ],
-                "internalType": "struct PantosTypes.TrustedValidatorFeeRecord",
+                "internalType": "struct PantosTypes.ValidatorFeeRecord",
                 "name": "",
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getUnbondingPeriodServiceNodeStake",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             },
             {
@@ -839,44 +443,44 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidPantosValidatorNonce",
+        "name": "isValidSenderNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidSenderNonce",
+        "name": "isValidValidatorNodeNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
@@ -1145,17 +749,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "transferTo",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
@@ -1403,17 +1012,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "verifyTransferTo",
         "outputs": [],
         "stateMutability": "view",
         "type": "function"
     },
@@ -1425,9 +1039,462 @@
                 "type": "address"
             }
         ],
         "name": "withdrawServiceNodeStake",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainNameUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumTokenStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumTokenStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumValidatorFeeUpdatePeriod",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumValidatorFeeUpdatePeriodUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosForwarder",
+                "type": "address"
+            }
+        ],
+        "name": "PantosForwarderSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosToken",
+                "type": "address"
+            }
+        ],
+        "name": "PantosTokenSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "primaryValidatorNodeAddress",
+                "type": "address"
+            }
+        ],
+        "name": "PrimaryValidatorNodeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUrlUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "transferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "Transfer",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "recipient",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sourceToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "destinationToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "TransferFrom",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceTransactionId",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sender",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "destinationToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "nonce",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
+            }
+        ],
+        "name": "TransferTo",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "unbondingPeriodServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "UnbondingPeriodServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "oldFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "newFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "validFrom",
+                "type": "uint256"
+            }
+        ],
+        "name": "ValidatorFeeUpdated",
+        "type": "event"
     }
 ]
```

## pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi

### Pretty-printed

 * *Similarity: 0.48589743589743595%*

 * *Differences: {'13': "{'name': 'getPrimaryValidatorNode'}",*

 * * '18': "{'inputs': [], 'name': 'getUnbondingPeriodServiceNodeStake', 'outputs': {0: "*

 * *       "{'internalType': 'uint256', 'type': 'uint256', delete: ['components']}}}",*

 * * '19': "{'inputs': [OrderedDict([('name', 'blockchainId'), ('type', 'uint256'), ('internalType', "*

 * *       "'uint256')])], 'name': 'getValidatorFeeRecord', 'outputs': {0: {'internalType': 'struct "*

 * *       "PantosTypes.ValidatorFeeRecord', 'type': 'tuple', 'components': [OrderedDict([('name', "*

 * *    […]*

```diff
@@ -1,405 +1,9 @@
 [
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainNameUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "minimumTrustedValidatorFeeUpdatePeriod",
-                "type": "uint256"
-            }
-        ],
-        "name": "MinimumTrustedValidatorFeeUpdatePeriodUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosForwarder",
-                "type": "address"
-            }
-        ],
-        "name": "PantosForwarderSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosToken",
-                "type": "address"
-            }
-        ],
-        "name": "PantosTokenSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosValidator",
-                "type": "address"
-            }
-        ],
-        "name": "PantosValidatorSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUrlUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "transferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "recipient",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sourceToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "destinationToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "TransferFrom",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceTransactionId",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sender",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "destinationToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "TransferTo",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "oldFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "newFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "validFrom",
-                "type": "uint256"
-            }
-        ],
-        "name": "TrustedValidatorFeeUpdated",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             }
         ],
@@ -548,15 +152,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getMinimumTrustedValidatorFeeUpdatePeriod",
+        "name": "getMinimumValidatorFeeUpdatePeriod",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
@@ -613,15 +217,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPantosValidator",
+        "name": "getPrimaryValidatorNode",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
@@ -733,22 +337,35 @@
                 "type": "address[]"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "getUnbondingPeriodServiceNodeStake",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint256",
                 "name": "blockchainId",
                 "type": "uint256"
             }
         ],
-        "name": "getTrustedValidatorFeeRecord",
+        "name": "getValidatorFeeRecord",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "oldFactor",
                         "type": "uint256"
@@ -760,36 +377,23 @@
                     },
                     {
                         "internalType": "uint256",
                         "name": "validFrom",
                         "type": "uint256"
                     }
                 ],
-                "internalType": "struct PantosTypes.TrustedValidatorFeeRecord",
+                "internalType": "struct PantosTypes.ValidatorFeeRecord",
                 "name": "",
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getUnbondingPeriodServiceNodeStake",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             },
             {
@@ -839,44 +443,44 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidPantosValidatorNonce",
+        "name": "isValidSenderNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidSenderNonce",
+        "name": "isValidValidatorNodeNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
@@ -1145,17 +749,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "transferTo",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
@@ -1403,17 +1012,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "verifyTransferTo",
         "outputs": [],
         "stateMutability": "view",
         "type": "function"
     },
@@ -1425,9 +1039,462 @@
                 "type": "address"
             }
         ],
         "name": "withdrawServiceNodeStake",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainNameUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumTokenStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumTokenStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumValidatorFeeUpdatePeriod",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumValidatorFeeUpdatePeriodUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosForwarder",
+                "type": "address"
+            }
+        ],
+        "name": "PantosForwarderSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosToken",
+                "type": "address"
+            }
+        ],
+        "name": "PantosTokenSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "primaryValidatorNodeAddress",
+                "type": "address"
+            }
+        ],
+        "name": "PrimaryValidatorNodeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUrlUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "transferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "Transfer",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "recipient",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sourceToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "destinationToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "TransferFrom",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceTransactionId",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sender",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "destinationToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "nonce",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
+            }
+        ],
+        "name": "TransferTo",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "unbondingPeriodServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "UnbondingPeriodServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "oldFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "newFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "validFrom",
+                "type": "uint256"
+            }
+        ],
+        "name": "ValidatorFeeUpdated",
+        "type": "event"
     }
 ]
```

## pantos/common/blockchains/contracts/celo_pantos_hub.abi

### Pretty-printed

 * *Similarity: 0.48589743589743595%*

 * *Differences: {'13': "{'name': 'getPrimaryValidatorNode'}",*

 * * '18': "{'inputs': [], 'name': 'getUnbondingPeriodServiceNodeStake', 'outputs': {0: "*

 * *       "{'internalType': 'uint256', 'type': 'uint256', delete: ['components']}}}",*

 * * '19': "{'inputs': [OrderedDict([('name', 'blockchainId'), ('type', 'uint256'), ('internalType', "*

 * *       "'uint256')])], 'name': 'getValidatorFeeRecord', 'outputs': {0: {'internalType': 'struct "*

 * *       "PantosTypes.ValidatorFeeRecord', 'type': 'tuple', 'components': [OrderedDict([('name', "*

 * *    […]*

```diff
@@ -1,405 +1,9 @@
 [
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainNameUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "minimumTrustedValidatorFeeUpdatePeriod",
-                "type": "uint256"
-            }
-        ],
-        "name": "MinimumTrustedValidatorFeeUpdatePeriodUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosForwarder",
-                "type": "address"
-            }
-        ],
-        "name": "PantosForwarderSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosToken",
-                "type": "address"
-            }
-        ],
-        "name": "PantosTokenSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosValidator",
-                "type": "address"
-            }
-        ],
-        "name": "PantosValidatorSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUrlUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "transferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "recipient",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sourceToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "destinationToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "TransferFrom",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceTransactionId",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sender",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "destinationToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "TransferTo",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "oldFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "newFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "validFrom",
-                "type": "uint256"
-            }
-        ],
-        "name": "TrustedValidatorFeeUpdated",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             }
         ],
@@ -548,15 +152,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getMinimumTrustedValidatorFeeUpdatePeriod",
+        "name": "getMinimumValidatorFeeUpdatePeriod",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
@@ -613,15 +217,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPantosValidator",
+        "name": "getPrimaryValidatorNode",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
@@ -733,22 +337,35 @@
                 "type": "address[]"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "getUnbondingPeriodServiceNodeStake",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint256",
                 "name": "blockchainId",
                 "type": "uint256"
             }
         ],
-        "name": "getTrustedValidatorFeeRecord",
+        "name": "getValidatorFeeRecord",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "oldFactor",
                         "type": "uint256"
@@ -760,36 +377,23 @@
                     },
                     {
                         "internalType": "uint256",
                         "name": "validFrom",
                         "type": "uint256"
                     }
                 ],
-                "internalType": "struct PantosTypes.TrustedValidatorFeeRecord",
+                "internalType": "struct PantosTypes.ValidatorFeeRecord",
                 "name": "",
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getUnbondingPeriodServiceNodeStake",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             },
             {
@@ -839,44 +443,44 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidPantosValidatorNonce",
+        "name": "isValidSenderNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidSenderNonce",
+        "name": "isValidValidatorNodeNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
@@ -1145,17 +749,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "transferTo",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
@@ -1403,17 +1012,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "verifyTransferTo",
         "outputs": [],
         "stateMutability": "view",
         "type": "function"
     },
@@ -1425,9 +1039,462 @@
                 "type": "address"
             }
         ],
         "name": "withdrawServiceNodeStake",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainNameUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumTokenStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumTokenStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumValidatorFeeUpdatePeriod",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumValidatorFeeUpdatePeriodUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosForwarder",
+                "type": "address"
+            }
+        ],
+        "name": "PantosForwarderSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosToken",
+                "type": "address"
+            }
+        ],
+        "name": "PantosTokenSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "primaryValidatorNodeAddress",
+                "type": "address"
+            }
+        ],
+        "name": "PrimaryValidatorNodeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUrlUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "transferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "Transfer",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "recipient",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sourceToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "destinationToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "TransferFrom",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceTransactionId",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sender",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "destinationToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "nonce",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
+            }
+        ],
+        "name": "TransferTo",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "unbondingPeriodServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "UnbondingPeriodServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "oldFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "newFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "validFrom",
+                "type": "uint256"
+            }
+        ],
+        "name": "ValidatorFeeUpdated",
+        "type": "event"
     }
 ]
```

## pantos/common/blockchains/contracts/cronos_pantos_hub.abi

### Pretty-printed

 * *Similarity: 0.48589743589743595%*

 * *Differences: {'13': "{'name': 'getPrimaryValidatorNode'}",*

 * * '18': "{'inputs': [], 'name': 'getUnbondingPeriodServiceNodeStake', 'outputs': {0: "*

 * *       "{'internalType': 'uint256', 'type': 'uint256', delete: ['components']}}}",*

 * * '19': "{'inputs': [OrderedDict([('name', 'blockchainId'), ('type', 'uint256'), ('internalType', "*

 * *       "'uint256')])], 'name': 'getValidatorFeeRecord', 'outputs': {0: {'internalType': 'struct "*

 * *       "PantosTypes.ValidatorFeeRecord', 'type': 'tuple', 'components': [OrderedDict([('name', "*

 * *    […]*

```diff
@@ -1,405 +1,9 @@
 [
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainNameUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "minimumTrustedValidatorFeeUpdatePeriod",
-                "type": "uint256"
-            }
-        ],
-        "name": "MinimumTrustedValidatorFeeUpdatePeriodUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosForwarder",
-                "type": "address"
-            }
-        ],
-        "name": "PantosForwarderSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosToken",
-                "type": "address"
-            }
-        ],
-        "name": "PantosTokenSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosValidator",
-                "type": "address"
-            }
-        ],
-        "name": "PantosValidatorSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUrlUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "transferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "recipient",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sourceToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "destinationToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "TransferFrom",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceTransactionId",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sender",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "destinationToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "TransferTo",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "oldFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "newFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "validFrom",
-                "type": "uint256"
-            }
-        ],
-        "name": "TrustedValidatorFeeUpdated",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             }
         ],
@@ -548,15 +152,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getMinimumTrustedValidatorFeeUpdatePeriod",
+        "name": "getMinimumValidatorFeeUpdatePeriod",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
@@ -613,15 +217,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPantosValidator",
+        "name": "getPrimaryValidatorNode",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
@@ -733,22 +337,35 @@
                 "type": "address[]"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "getUnbondingPeriodServiceNodeStake",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint256",
                 "name": "blockchainId",
                 "type": "uint256"
             }
         ],
-        "name": "getTrustedValidatorFeeRecord",
+        "name": "getValidatorFeeRecord",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "oldFactor",
                         "type": "uint256"
@@ -760,36 +377,23 @@
                     },
                     {
                         "internalType": "uint256",
                         "name": "validFrom",
                         "type": "uint256"
                     }
                 ],
-                "internalType": "struct PantosTypes.TrustedValidatorFeeRecord",
+                "internalType": "struct PantosTypes.ValidatorFeeRecord",
                 "name": "",
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getUnbondingPeriodServiceNodeStake",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             },
             {
@@ -839,44 +443,44 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidPantosValidatorNonce",
+        "name": "isValidSenderNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidSenderNonce",
+        "name": "isValidValidatorNodeNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
@@ -1145,17 +749,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "transferTo",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
@@ -1403,17 +1012,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "verifyTransferTo",
         "outputs": [],
         "stateMutability": "view",
         "type": "function"
     },
@@ -1425,9 +1039,462 @@
                 "type": "address"
             }
         ],
         "name": "withdrawServiceNodeStake",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainNameUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumTokenStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumTokenStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumValidatorFeeUpdatePeriod",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumValidatorFeeUpdatePeriodUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosForwarder",
+                "type": "address"
+            }
+        ],
+        "name": "PantosForwarderSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosToken",
+                "type": "address"
+            }
+        ],
+        "name": "PantosTokenSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "primaryValidatorNodeAddress",
+                "type": "address"
+            }
+        ],
+        "name": "PrimaryValidatorNodeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUrlUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "transferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "Transfer",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "recipient",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sourceToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "destinationToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "TransferFrom",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceTransactionId",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sender",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "destinationToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "nonce",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
+            }
+        ],
+        "name": "TransferTo",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "unbondingPeriodServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "UnbondingPeriodServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "oldFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "newFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "validFrom",
+                "type": "uint256"
+            }
+        ],
+        "name": "ValidatorFeeUpdated",
+        "type": "event"
     }
 ]
```

## pantos/common/blockchains/contracts/ethereum_pantos_hub.abi

### Pretty-printed

 * *Similarity: 0.48589743589743595%*

 * *Differences: {'13': "{'name': 'getPrimaryValidatorNode'}",*

 * * '18': "{'inputs': [], 'name': 'getUnbondingPeriodServiceNodeStake', 'outputs': {0: "*

 * *       "{'internalType': 'uint256', 'type': 'uint256', delete: ['components']}}}",*

 * * '19': "{'inputs': [OrderedDict([('name', 'blockchainId'), ('type', 'uint256'), ('internalType', "*

 * *       "'uint256')])], 'name': 'getValidatorFeeRecord', 'outputs': {0: {'internalType': 'struct "*

 * *       "PantosTypes.ValidatorFeeRecord', 'type': 'tuple', 'components': [OrderedDict([('name', "*

 * *    […]*

```diff
@@ -1,405 +1,9 @@
 [
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainNameUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "minimumTrustedValidatorFeeUpdatePeriod",
-                "type": "uint256"
-            }
-        ],
-        "name": "MinimumTrustedValidatorFeeUpdatePeriodUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosForwarder",
-                "type": "address"
-            }
-        ],
-        "name": "PantosForwarderSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosToken",
-                "type": "address"
-            }
-        ],
-        "name": "PantosTokenSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosValidator",
-                "type": "address"
-            }
-        ],
-        "name": "PantosValidatorSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUrlUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "transferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "recipient",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sourceToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "destinationToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "TransferFrom",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceTransactionId",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sender",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "destinationToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "TransferTo",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "oldFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "newFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "validFrom",
-                "type": "uint256"
-            }
-        ],
-        "name": "TrustedValidatorFeeUpdated",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             }
         ],
@@ -548,15 +152,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getMinimumTrustedValidatorFeeUpdatePeriod",
+        "name": "getMinimumValidatorFeeUpdatePeriod",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
@@ -613,15 +217,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPantosValidator",
+        "name": "getPrimaryValidatorNode",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
@@ -733,22 +337,35 @@
                 "type": "address[]"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "getUnbondingPeriodServiceNodeStake",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint256",
                 "name": "blockchainId",
                 "type": "uint256"
             }
         ],
-        "name": "getTrustedValidatorFeeRecord",
+        "name": "getValidatorFeeRecord",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "oldFactor",
                         "type": "uint256"
@@ -760,36 +377,23 @@
                     },
                     {
                         "internalType": "uint256",
                         "name": "validFrom",
                         "type": "uint256"
                     }
                 ],
-                "internalType": "struct PantosTypes.TrustedValidatorFeeRecord",
+                "internalType": "struct PantosTypes.ValidatorFeeRecord",
                 "name": "",
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getUnbondingPeriodServiceNodeStake",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             },
             {
@@ -839,44 +443,44 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidPantosValidatorNonce",
+        "name": "isValidSenderNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidSenderNonce",
+        "name": "isValidValidatorNodeNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
@@ -1145,17 +749,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "transferTo",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
@@ -1403,17 +1012,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "verifyTransferTo",
         "outputs": [],
         "stateMutability": "view",
         "type": "function"
     },
@@ -1425,9 +1039,462 @@
                 "type": "address"
             }
         ],
         "name": "withdrawServiceNodeStake",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainNameUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumTokenStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumTokenStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumValidatorFeeUpdatePeriod",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumValidatorFeeUpdatePeriodUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosForwarder",
+                "type": "address"
+            }
+        ],
+        "name": "PantosForwarderSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosToken",
+                "type": "address"
+            }
+        ],
+        "name": "PantosTokenSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "primaryValidatorNodeAddress",
+                "type": "address"
+            }
+        ],
+        "name": "PrimaryValidatorNodeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUrlUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "transferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "Transfer",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "recipient",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sourceToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "destinationToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "TransferFrom",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceTransactionId",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sender",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "destinationToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "nonce",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
+            }
+        ],
+        "name": "TransferTo",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "unbondingPeriodServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "UnbondingPeriodServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "oldFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "newFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "validFrom",
+                "type": "uint256"
+            }
+        ],
+        "name": "ValidatorFeeUpdated",
+        "type": "event"
     }
 ]
```

## pantos/common/blockchains/contracts/fantom_pantos_hub.abi

### Pretty-printed

 * *Similarity: 0.48589743589743595%*

 * *Differences: {'13': "{'name': 'getPrimaryValidatorNode'}",*

 * * '18': "{'inputs': [], 'name': 'getUnbondingPeriodServiceNodeStake', 'outputs': {0: "*

 * *       "{'internalType': 'uint256', 'type': 'uint256', delete: ['components']}}}",*

 * * '19': "{'inputs': [OrderedDict([('name', 'blockchainId'), ('type', 'uint256'), ('internalType', "*

 * *       "'uint256')])], 'name': 'getValidatorFeeRecord', 'outputs': {0: {'internalType': 'struct "*

 * *       "PantosTypes.ValidatorFeeRecord', 'type': 'tuple', 'components': [OrderedDict([('name', "*

 * *    […]*

```diff
@@ -1,405 +1,9 @@
 [
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainNameUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "minimumTrustedValidatorFeeUpdatePeriod",
-                "type": "uint256"
-            }
-        ],
-        "name": "MinimumTrustedValidatorFeeUpdatePeriodUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosForwarder",
-                "type": "address"
-            }
-        ],
-        "name": "PantosForwarderSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosToken",
-                "type": "address"
-            }
-        ],
-        "name": "PantosTokenSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosValidator",
-                "type": "address"
-            }
-        ],
-        "name": "PantosValidatorSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUrlUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "transferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "recipient",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sourceToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "destinationToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "TransferFrom",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceTransactionId",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sender",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "destinationToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "TransferTo",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "oldFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "newFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "validFrom",
-                "type": "uint256"
-            }
-        ],
-        "name": "TrustedValidatorFeeUpdated",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             }
         ],
@@ -548,15 +152,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getMinimumTrustedValidatorFeeUpdatePeriod",
+        "name": "getMinimumValidatorFeeUpdatePeriod",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
@@ -613,15 +217,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPantosValidator",
+        "name": "getPrimaryValidatorNode",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
@@ -733,22 +337,35 @@
                 "type": "address[]"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "getUnbondingPeriodServiceNodeStake",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint256",
                 "name": "blockchainId",
                 "type": "uint256"
             }
         ],
-        "name": "getTrustedValidatorFeeRecord",
+        "name": "getValidatorFeeRecord",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "oldFactor",
                         "type": "uint256"
@@ -760,36 +377,23 @@
                     },
                     {
                         "internalType": "uint256",
                         "name": "validFrom",
                         "type": "uint256"
                     }
                 ],
-                "internalType": "struct PantosTypes.TrustedValidatorFeeRecord",
+                "internalType": "struct PantosTypes.ValidatorFeeRecord",
                 "name": "",
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getUnbondingPeriodServiceNodeStake",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             },
             {
@@ -839,44 +443,44 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidPantosValidatorNonce",
+        "name": "isValidSenderNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidSenderNonce",
+        "name": "isValidValidatorNodeNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
@@ -1145,17 +749,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "transferTo",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
@@ -1403,17 +1012,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "verifyTransferTo",
         "outputs": [],
         "stateMutability": "view",
         "type": "function"
     },
@@ -1425,9 +1039,462 @@
                 "type": "address"
             }
         ],
         "name": "withdrawServiceNodeStake",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainNameUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumTokenStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumTokenStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumValidatorFeeUpdatePeriod",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumValidatorFeeUpdatePeriodUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosForwarder",
+                "type": "address"
+            }
+        ],
+        "name": "PantosForwarderSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosToken",
+                "type": "address"
+            }
+        ],
+        "name": "PantosTokenSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "primaryValidatorNodeAddress",
+                "type": "address"
+            }
+        ],
+        "name": "PrimaryValidatorNodeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUrlUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "transferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "Transfer",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "recipient",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sourceToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "destinationToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "TransferFrom",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceTransactionId",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sender",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "destinationToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "nonce",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
+            }
+        ],
+        "name": "TransferTo",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "unbondingPeriodServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "UnbondingPeriodServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "oldFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "newFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "validFrom",
+                "type": "uint256"
+            }
+        ],
+        "name": "ValidatorFeeUpdated",
+        "type": "event"
     }
 ]
```

## pantos/common/blockchains/contracts/polygon_pantos_hub.abi

### Pretty-printed

 * *Similarity: 0.48589743589743595%*

 * *Differences: {'13': "{'name': 'getPrimaryValidatorNode'}",*

 * * '18': "{'inputs': [], 'name': 'getUnbondingPeriodServiceNodeStake', 'outputs': {0: "*

 * *       "{'internalType': 'uint256', 'type': 'uint256', delete: ['components']}}}",*

 * * '19': "{'inputs': [OrderedDict([('name', 'blockchainId'), ('type', 'uint256'), ('internalType', "*

 * *       "'uint256')])], 'name': 'getValidatorFeeRecord', 'outputs': {0: {'internalType': 'struct "*

 * *       "PantosTypes.ValidatorFeeRecord', 'type': 'tuple', 'components': [OrderedDict([('name', "*

 * *    […]*

```diff
@@ -1,405 +1,9 @@
 [
     {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainNameUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "BlockchainUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            }
-        ],
-        "name": "ExternalTokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "minimumTrustedValidatorFeeUpdatePeriod",
-                "type": "uint256"
-            }
-        ],
-        "name": "MinimumTrustedValidatorFeeUpdatePeriodUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosForwarder",
-                "type": "address"
-            }
-        ],
-        "name": "PantosForwarderSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosToken",
-                "type": "address"
-            }
-        ],
-        "name": "PantosTokenSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "pantosValidator",
-                "type": "address"
-            }
-        ],
-        "name": "PantosValidatorSet",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "ServiceNodeUrlUpdated",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenRegistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            }
-        ],
-        "name": "TokenUnregistered",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "transferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "token",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "Transfer",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "recipient",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "sourceToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "destinationToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "fee",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "serviceNode",
-                "type": "address"
-            }
-        ],
-        "name": "TransferFrom",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceBlockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "sourceTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceTransactionId",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "destinationTransferId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sender",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "recipient",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "string",
-                "name": "sourceToken",
-                "type": "string"
-            },
-            {
-                "indexed": false,
-                "internalType": "address",
-                "name": "destinationToken",
-                "type": "address"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "amount",
-                "type": "uint256"
-            }
-        ],
-        "name": "TransferTo",
-        "type": "event"
-    },
-    {
-        "anonymous": false,
-        "inputs": [
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "blockchainId",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "oldFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "newFactor",
-                "type": "uint256"
-            },
-            {
-                "indexed": false,
-                "internalType": "uint256",
-                "name": "validFrom",
-                "type": "uint256"
-            }
-        ],
-        "name": "TrustedValidatorFeeUpdated",
-        "type": "event"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             }
         ],
@@ -548,15 +152,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getMinimumTrustedValidatorFeeUpdatePeriod",
+        "name": "getMinimumValidatorFeeUpdatePeriod",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
                 "type": "uint256"
             }
         ],
@@ -613,15 +217,15 @@
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [],
-        "name": "getPantosValidator",
+        "name": "getPrimaryValidatorNode",
         "outputs": [
             {
                 "internalType": "address",
                 "name": "",
                 "type": "address"
             }
         ],
@@ -733,22 +337,35 @@
                 "type": "address[]"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
+        "inputs": [],
+        "name": "getUnbondingPeriodServiceNodeStake",
+        "outputs": [
+            {
+                "internalType": "uint256",
+                "name": "",
+                "type": "uint256"
+            }
+        ],
+        "stateMutability": "view",
+        "type": "function"
+    },
+    {
         "inputs": [
             {
                 "internalType": "uint256",
                 "name": "blockchainId",
                 "type": "uint256"
             }
         ],
-        "name": "getTrustedValidatorFeeRecord",
+        "name": "getValidatorFeeRecord",
         "outputs": [
             {
                 "components": [
                     {
                         "internalType": "uint256",
                         "name": "oldFactor",
                         "type": "uint256"
@@ -760,36 +377,23 @@
                     },
                     {
                         "internalType": "uint256",
                         "name": "validFrom",
                         "type": "uint256"
                     }
                 ],
-                "internalType": "struct PantosTypes.TrustedValidatorFeeRecord",
+                "internalType": "struct PantosTypes.ValidatorFeeRecord",
                 "name": "",
                 "type": "tuple"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
-        "inputs": [],
-        "name": "getUnbondingPeriodServiceNodeStake",
-        "outputs": [
-            {
-                "internalType": "uint256",
-                "name": "",
-                "type": "uint256"
-            }
-        ],
-        "stateMutability": "view",
-        "type": "function"
-    },
-    {
         "inputs": [
             {
                 "internalType": "address",
                 "name": "serviceNodeAddress",
                 "type": "address"
             },
             {
@@ -839,44 +443,44 @@
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidPantosValidatorNonce",
+        "name": "isValidSenderNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
         "stateMutability": "view",
         "type": "function"
     },
     {
         "inputs": [
             {
-                "internalType": "address",
-                "name": "sender",
-                "type": "address"
-            },
-            {
                 "internalType": "uint256",
                 "name": "nonce",
                 "type": "uint256"
             }
         ],
-        "name": "isValidSenderNonce",
+        "name": "isValidValidatorNodeNonce",
         "outputs": [
             {
                 "internalType": "bool",
                 "name": "",
                 "type": "bool"
             }
         ],
@@ -1145,17 +749,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "transferTo",
         "outputs": [
             {
                 "internalType": "uint256",
                 "name": "",
@@ -1403,17 +1012,22 @@
                     }
                 ],
                 "internalType": "struct PantosTypes.TransferToRequest",
                 "name": "request",
                 "type": "tuple"
             },
             {
-                "internalType": "bytes",
-                "name": "signature",
-                "type": "bytes"
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
             }
         ],
         "name": "verifyTransferTo",
         "outputs": [],
         "stateMutability": "view",
         "type": "function"
     },
@@ -1425,9 +1039,462 @@
                 "type": "address"
             }
         ],
         "name": "withdrawServiceNodeStake",
         "outputs": [],
         "stateMutability": "nonpayable",
         "type": "function"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainNameUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "BlockchainUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            }
+        ],
+        "name": "ExternalTokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumTokenStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumTokenStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "minimumValidatorFeeUpdatePeriod",
+                "type": "uint256"
+            }
+        ],
+        "name": "MinimumValidatorFeeUpdatePeriodUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosForwarder",
+                "type": "address"
+            }
+        ],
+        "name": "PantosForwarderSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "pantosToken",
+                "type": "address"
+            }
+        ],
+        "name": "PantosTokenSet",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "primaryValidatorNodeAddress",
+                "type": "address"
+            }
+        ],
+        "name": "PrimaryValidatorNodeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "ServiceNodeUrlUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenRegistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            }
+        ],
+        "name": "TokenUnregistered",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "transferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "token",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "Transfer",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sender",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "recipient",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "sourceToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "destinationToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "fee",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "serviceNode",
+                "type": "address"
+            }
+        ],
+        "name": "TransferFrom",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceBlockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "sourceTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceTransactionId",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "destinationTransferId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sender",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "recipient",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "string",
+                "name": "sourceToken",
+                "type": "string"
+            },
+            {
+                "indexed": false,
+                "internalType": "address",
+                "name": "destinationToken",
+                "type": "address"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "amount",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "nonce",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "address[]",
+                "name": "signerAddresses",
+                "type": "address[]"
+            },
+            {
+                "indexed": false,
+                "internalType": "bytes[]",
+                "name": "signatures",
+                "type": "bytes[]"
+            }
+        ],
+        "name": "TransferTo",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "unbondingPeriodServiceNodeStake",
+                "type": "uint256"
+            }
+        ],
+        "name": "UnbondingPeriodServiceNodeStakeUpdated",
+        "type": "event"
+    },
+    {
+        "anonymous": false,
+        "inputs": [
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "blockchainId",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "oldFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "newFactor",
+                "type": "uint256"
+            },
+            {
+                "indexed": false,
+                "internalType": "uint256",
+                "name": "validFrom",
+                "type": "uint256"
+            }
+        ],
+        "name": "ValidatorFeeUpdated",
+        "type": "event"
     }
 ]
```

## pantos/servicenode/application.py

```diff
@@ -23,26 +23,26 @@
 """Logger for this module."""
 
 
 def create_application() -> flask.Flask:
     """Create the service node application.
 
     """
-    initialize_application()
+    initialize_application(True)
     # Imported here to ensure Celery is initialized after loading the
     # configuration and before updating the registrations
     import pantos.servicenode.celery  # noqa: F401
     _update_registrations()
     initialize_plugins(start_worker=False)
     # Imported here to prevent a circular import
     from pantos.servicenode.restapi import flask_app
     return flask_app
 
 
-def initialize_application() -> None:
+def initialize_application(is_flask_app: bool = False) -> None:
     """Initialize the service node application.
 
     """
     # Logging for loading the configuration
     logging.basicConfig(level=logging.INFO)
     # Load the configuration
     try:
@@ -66,15 +66,15 @@
         initialize_logger(root_logger, log_format, standard_output, log_file,
                           debug)
     except Exception:
         _logger.critical('unable to initialize logging', exc_info=True)
         sys.exit(1)
     # Package-specific initialization
     try:
-        initialize_database_package()
+        initialize_database_package(is_flask_app)
     except Exception:
         _logger.critical('unable to initialize the database', exc_info=True)
         sys.exit(1)
     try:
         initialize_blockchain_clients()
     except Exception:
         _logger.critical('unable to initialize the blockchain clients',
```

## pantos/servicenode/celery.py

```diff
@@ -17,15 +17,15 @@
 
 def is_celery_worker_process() -> bool:
     return (len(sys.argv) > 0 and sys.argv[0].endswith('celery')
             and 'worker' in sys.argv)
 
 
 if is_celery_worker_process():
-    initialize_application()  # pragma: no cover
+    initialize_application(False)  # pragma: no cover
 
 celery_app = celery.Celery(
     'pantos.servicenode', broker=config['celery']['broker'],
     backend=config['celery']['backend'], include=[
         'pantos.common.blockchains.tasks',
         'pantos.servicenode.business.transfers',
         'pantos.servicenode.business.plugins'
```

## pantos/servicenode/configuration.py

```diff
@@ -6,15 +6,15 @@
 import typing
 
 from pantos.common.blockchains.base import MIN_ADAPTABLE_FEE_INCREASE_FACTOR
 from pantos.common.blockchains.enums import Blockchain
 from pantos.common.configuration import Config
 from pantos.common.logging import LogFormat
 
-_DEFAULT_FILE_NAME: typing.Final[str] = 'pantos-service-node.conf'
+_DEFAULT_FILE_NAME: typing.Final[str] = 'service-node-config.yml'
 """Default configuration file name."""
 
 config = Config(_DEFAULT_FILE_NAME)
 """Singleton object holding the configuration values."""
 
 _VALIDATION_SCHEMA_BLOCKCHAIN = {
     'type': 'dict',
@@ -27,15 +27,16 @@
             'type': 'string',
             'required': True,
             'empty': False
         },
         'private_key': {
             'type': 'string',
             'required': True,
-            'empty': False
+            'empty': False,
+            'coerce': 'load_if_file'
         },
         'private_key_password': {
             'type': 'string',
             'required': True,
             'empty': False
         },
         'provider': {
@@ -193,14 +194,23 @@
             'max_overflow': {
                 'type': 'integer',
                 'required': True
             },
             'echo': {
                 'type': 'boolean',
                 'default': False
+            },
+            'alembic_config': {
+                'type': 'string',
+                'required': True,
+                'empty': False
+            },
+            'apply_migrations': {
+                'type': 'boolean',
+                'default': False,
             }
         }
     },
     'celery': {
         'type': 'dict',
         'schema': {
             'broker': {
@@ -215,17 +225,18 @@
             },
             'log': _VALIDATION_SCHEMA_LOG
         }
     },
     'signer': {
         'type': 'dict',
         'schema': {
-            'pem_path': {
+            'pem': {
                 'type': 'string',
-                'required': True
+                'required': True,
+                'coerce': 'load_if_file'
             },
             'pem_password': {
                 'type': 'string',
                 'required': True
             }
         }
     },
```

## pantos/servicenode/blockchains/base.py

```diff
@@ -1,14 +1,13 @@
 """Base classes for all blockchain clients and errors.
 
 """
 import abc
 import dataclasses
 import logging
-import pathlib
 import typing
 import uuid
 
 from pantos.common.blockchains.base import BlockchainHandler
 from pantos.common.blockchains.base import BlockchainUtilities
 from pantos.common.blockchains.base import BlockchainUtilitiesError
 from pantos.common.blockchains.base import NodeConnections
@@ -82,22 +81,22 @@
         blockchain_node_url = self._get_config()['provider']
         fallback_blockchain_nodes_urls = self._get_config().get(
             'fallback_providers', [])
         average_block_time = self._get_config()['average_block_time']
         required_transaction_confirmations = \
             self._get_config()['confirmations']
         transaction_network_id = self._get_config().get('chain_id')
-        private_key_path = pathlib.Path(self._get_config()['private_key'])
+        private_key = self._get_config()['private_key']
         private_key_password = self._get_config()['private_key_password']
         try:
             initialize_blockchain_utilities(
                 self.get_blockchain(), [blockchain_node_url],
                 fallback_blockchain_nodes_urls, average_block_time,
                 required_transaction_confirmations, transaction_network_id,
-                default_private_key=(private_key_path, private_key_password),
+                default_private_key=(private_key, private_key_password),
                 celery_tasks_enabled=True)
         except BlockchainUtilitiesError:
             raise self._create_error(
                 f'unable to initialize the {self.get_blockchain_name()} '
                 'utilities')
 
     @abc.abstractmethod
```

## pantos/servicenode/blockchains/ethereum.py

```diff
@@ -1,13 +1,12 @@
 """Module for Ethereum-specific clients and errors.
 
 """
 import json
 import logging
-import pathlib
 import time
 import typing
 import uuid
 
 import web3
 import web3.contract.contract
 import web3.exceptions
@@ -62,18 +61,18 @@
 class EthereumClient(BlockchainClient):
     """Ethereum-specific blockchain client.
 
     """
     def __init__(self):
         # Docstring inherited
         super().__init__()
-        private_key_path = pathlib.Path(self._get_config()['private_key'])
+        private_key = self._get_config()['private_key']
         private_key_password = self._get_config()['private_key_password']
-        private_key = self._get_utilities().load_private_key(
-            private_key_path, private_key_password)
+        private_key = self._get_utilities().decrypt_private_key(
+            private_key, private_key_password)
         self.__address = self._get_utilities().get_address(private_key)
 
     @classmethod
     def get_blockchain(cls) -> Blockchain:
         # Docstring inherited
         return Blockchain.ETHEREUM
 
@@ -281,15 +280,15 @@
             raise self._create_error('unable to unregister the service node')
 
     def get_validator_fee_factor(self, blockchain: Blockchain) -> int:
         # Docstring inherited
         try:
             node_connections = self.__create_node_connections()
             hub_contract = self._create_hub_contract(node_connections)
-            fee_record = hub_contract.functions.getTrustedValidatorFeeRecord(
+            fee_record = hub_contract.functions.getValidatorFeeRecord(
                 blockchain.value).call().get()
             # Check if the valid from of the factor has passed
             if time.time() >= fee_record[2]:
                 # Return new factor
                 return fee_record[1]
             # Return old factor
             return fee_record[0]
```

## pantos/servicenode/business/bids.py

```diff
@@ -76,15 +76,15 @@
         """
         try:
             _logger.info('Reading cross-blockchain bids from database')
             raw_bids = database_access.read_cross_blockchain_bids(
                 source_blockchain_id, destination_blockchain_id)
             bids = []
             signer_config = get_signer_config()
-            signer = get_signer(signer_config['pem_path'],
+            signer = get_signer(signer_config['pem'],
                                 signer_config['pem_password'])
             for bid in raw_bids:
                 bid_message = signer.build_message('', int(bid.fee),
                                                    int(bid.valid_until),
                                                    source_blockchain_id,
                                                    destination_blockchain_id,
                                                    int(bid.execution_time))
```

## pantos/servicenode/business/transfers.py

```diff
@@ -513,15 +513,15 @@
 
         Returns
         -------
         bool
             True if the bid is valid, False otherwise.
         """
         signer_config = get_signer_config()
-        signer = get_signer(signer_config['pem_path'],
+        signer = get_signer(signer_config['pem'],
                             signer_config['pem_password'])
         bid_message = signer.build_message('', fee, bid_valid_until,
                                            source_blockchain_id,
                                            destination_blockchain_id,
                                            execution_time)
         return signer.verify_message(bid_message, bid_signature)
```

## pantos/servicenode/database/__init__.py

```diff
@@ -1,25 +1,29 @@
 """Package for managing and accessing the database.
 
 """
+import logging
 import typing
 
 import sqlalchemy  # type: ignore
 import sqlalchemy.exc  # type: ignore
 import sqlalchemy.orm  # type: ignore
+from alembic import command
+from alembic.config import Config
 
 from pantos.common.blockchains.enums import Blockchain
 from pantos.servicenode.configuration import config
 from pantos.servicenode.database.enums import TransferStatus
 from pantos.servicenode.database.exceptions import DatabaseError
 from pantos.servicenode.database.models import Blockchain as Blockchain_
 from pantos.servicenode.database.models import \
     TransferStatus as TransferStatus_
 
 _session_maker: typing.Optional[sqlalchemy.orm.sessionmaker] = None
+_logger = logging.getLogger(__name__)
 
 
 def get_session_maker() -> sqlalchemy.orm.sessionmaker:
     """Get the session maker for making sessions for managing
     persistence operations for ORM-mapped objects.
 
     Returns
@@ -52,15 +56,29 @@
     DatabaseError
         If the database package has not been initialized.
 
     """
     return get_session_maker()()
 
 
-def initialize_package() -> None:
+def run_migrations(config_path: str, dsn: str) -> None:
+    _logger.info('running DB migrations using %r', config_path)
+    alembic_cfg = Config(config_path)
+    alembic_cfg.set_main_option('sqlalchemy.url', dsn)
+    command.upgrade(alembic_cfg, 'head')
+    _logger.info('db migrations done')
+
+
+def initialize_package(is_flask_app: bool = False) -> None:
+    # Before connecting, run alembic to ensure
+    # the database schema is up to date
+    if is_flask_app and config['database']['apply_migrations']:
+        run_migrations(config['database']['alembic_config'],
+                       config['database']['url'])
+
     sql_engine = sqlalchemy.create_engine(
         config['database']['url'], pool_size=config['database']['pool_size'],
         max_overflow=config['database']['max_overflow'], pool_pre_ping=True,
         echo=config['database']['echo'])
     global _session_maker
     _session_maker = sqlalchemy.orm.sessionmaker(bind=sql_engine)
     # Initialize the tables
```

## Comparing `pantos/bids.yaml` & `pantos/bids.yml`

 * *Files identical despite different names*

## Comparing `pantos_service_node-1.5.3.dist-info/LICENSE.md` & `pantos_service_node-1.6.0.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pantos_service_node-1.5.3.dist-info/METADATA` & `pantos_service_node-1.6.0.dist-info/METADATA`

 * *Files 21% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 Metadata-Version: 2.1
 Name: pantos-service-node
-Version: 1.5.3
+Version: 1.6.0
 Summary: Service node reference implementation for the Pantos multi-blockchain system
 Home-page: https://github.com/pantos-io/servicenode
 Author: Pantos
-Author-email: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
+License-File: LICENSE.md
 Requires-Dist: alembic (==1.11.1)
 Requires-Dist: celery (==5.3.1)
 Requires-Dist: Cerberus (==1.3.4)
 Requires-Dist: Flask (==2.3.2)
 Requires-Dist: Flask-Cors (==4.0.0)
 Requires-Dist: Flask-RESTful (==0.3.10)
 Requires-Dist: marshmallow (==3.19.0)
-Requires-Dist: psycopg2 (==2.9.6)
+Requires-Dist: psycopg2-binary (==2.9.6)
 Requires-Dist: PyYAML (==6.0.1)
 Requires-Dist: SQLAlchemy (==2.0.18)
 Requires-Dist: web3 (==6.5.0)
 Requires-Dist: JSON-log-formatter (==0.5.2)
+Requires-Dist: pyaml-env (==1.2.1)
+Requires-Dist: python-dotenv (==1.0.1)
+Requires-Dist: hexbytes (==0.3.1)
 
 Service node reference implementation for the Pantos multi-blockchain system
-
-
```

## Comparing `pantos_service_node-1.5.3.dist-info/RECORD` & `pantos_service_node-1.6.0.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,93 +1,101 @@
 pantos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pantos/alembic.ini,sha256=SraEdqNrumzTEkBaw9C0WeOZUqR6AyLBh00TpRs1COk,3251
-pantos/bids.yaml,sha256=uK9oXnNt7Ex_i_kLbU-vCYRrv8Qi2QUf4t2iROgC7A8,7809
-pantos/pantos-service-node.conf,sha256=fhv3kmRPeSHl3YYBrXfm1C1tAhtjyI8MUZL_jayAOpM,7182
+pantos/bids.yml,sha256=uK9oXnNt7Ex_i_kLbU-vCYRrv8Qi2QUf4t2iROgC7A8,7809
+pantos/service-node-config.env,sha256=Ba7LN_ZS32Xlp_2GIy86m29-RIEEHWxZDziLhlD1D2A,5415
+pantos/service-node-config.yml,sha256=7GABJCwqfEBKCR8EvhVWuMZEY7CfrOIBlzUqGOnL2vk,14841
 pantos/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pantos/common/configuration.py,sha256=DKKKUU-KFT8G00Ql98N8DpdDXOQ0PrW4geh4X6CdqzY,4863
+pantos/common/configuration.py,sha256=D888HPFvypPmdO-IkhC7rSC-EN5E9WDAQixG4EGosmI,6041
 pantos/common/entities.py,sha256=9WA2lxrpdL5qWAyZE5rlQi_6CvwKmzyxymtMaIeWrgI,4739
 pantos/common/exceptions.py,sha256=2EWzJkb3UUTOpGTCwvfN0ySFxhoh1xFF5GR_xFWHY90,3311
 pantos/common/logging.py,sha256=5WB9cXhuvhK7x0_R3L02PZ39faoqdY-heXpd8CunGkc,7012
 pantos/common/restapi.py,sha256=0BfvbXGBHbDIZazkc3lj6DaU9FJqL9SzdaZwS6dU_pQ,2969
 pantos/common/servicenodes.py,sha256=DvaTdnkUkc8ZxhJ7bTZTYkq1ey7nJ-dP5BIDan3Yg64,12286
-pantos/common/signer.py,sha256=8IL-8QUfDMUkoBwz2qKXXRSww008nSmYaB_gLJzBVhw,5315
+pantos/common/signer.py,sha256=3T70jryXn2xVh9Q8zmXX_eXwMJp8h2KBL2re4lrxJWo,5043
 pantos/common/types.py,sha256=FZvTMzMuSoX3txGJwHnEaSpdJlXj_giI21KCRxf1jKA,509
 pantos/common/blockchains/__init__.py,sha256=7uHu0tVlVK0YSZF66hzc0kMUFKzBZsQeRwMaHeekFMs,55
 pantos/common/blockchains/avalanche.py,sha256=7YuB_LLQ1WUG1yntiou_GmwSDKwgB9mw0sQAXcj6qpU,974
-pantos/common/blockchains/base.py,sha256=Y0fmJK8ACdsUbtr8R6Xj97Hw0u8cg1lEMWjqFuYTsEE,41394
+pantos/common/blockchains/base.py,sha256=7lK0rw4JtT-BYHhZhRrQFkPFJRQmc7b5XefXJz4Yqi4,41291
 pantos/common/blockchains/bnbchain.py,sha256=xBU3u7TasL1v8tcLXVc4xS04soKK_WTS5ZTX5O_XclE,969
 pantos/common/blockchains/celo.py,sha256=YlSL6XYu4TWSo9m1X_9w6u8uJj67LenXTZDKea5xE6A,922
 pantos/common/blockchains/cronos.py,sha256=JzlugruvSt4GniRftxrzSuEc5FnGu5AkrL8fHGk_QQQ,938
-pantos/common/blockchains/enums.py,sha256=9aul88uCnBq_myi_vXvRTzv9mZ_amOBytbJ2SDZU92U,1670
-pantos/common/blockchains/ethereum.py,sha256=ikI26VgiMbr_1ubjanRWelDO9Y7obpeatsdvYTfeOcM,19505
-pantos/common/blockchains/factory.py,sha256=wcyKDRfHOgRT4iAvrlohSB6FBibalA2bzMqLR0GdO1c,3678
+pantos/common/blockchains/enums.py,sha256=WhAX9SY5SkFjO6ZnUTZI69lSzQaWX70Ql_DkGpq4XD0,1695
+pantos/common/blockchains/ethereum.py,sha256=HUf-rMOCkm-SXNBBIdofAvpHKshCsw-LBEzIVK_NSHk,19287
+pantos/common/blockchains/factory.py,sha256=ARjd6IibmNMqArpsQMXdZSu1v4cl89NiYieGqnT4XuE,3642
 pantos/common/blockchains/fantom.py,sha256=y0R5Egzwb25DJXdTyitzCyXMLw1BUXxMG_-dYjhNNHQ,938
 pantos/common/blockchains/polygon.py,sha256=4BqCKuwuGf0-BS1ER1yUqLKGodY3HHAa6jQaOUa2Vuc,946
-pantos/common/blockchains/solana.py,sha256=VatQHYVHfX9aX3Nz6gY3ckiZ-ohuxTMloSXWZsTw1Pk,3681
+pantos/common/blockchains/solana.py,sha256=RuVdZ98HLdf0oRAB7FSoHKRCIrxCzWTXl6DTOFBdxgU,3596
 pantos/common/blockchains/tasks.py,sha256=E646ci_VMGd-h0BtIlD5GVJNLjeYswO9-sBZvnTw67c,6505
 pantos/common/blockchains/contracts/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-pantos/common/blockchains/contracts/avalanche_pantos_hub.abi,sha256=XH4RU3pbgPUjlhlNDkP9l63bEgUL1m1aNW5FMn3H8Vk,33098
+pantos/common/blockchains/contracts/avalanche_pantos_forwarder.abi,sha256=udZYZcnMm9xQApQNAxda87p-jrHKNsReUjL5EKXYOwc,7229
+pantos/common/blockchains/contracts/avalanche_pantos_hub.abi,sha256=QEFEzDk6LYzjsF8Q1n-P2puHzILBnG5RV0IvsJI_g80,42156
 pantos/common/blockchains/contracts/avalanche_pantos_token.abi,sha256=hqSqiE6SaYnRu067CJTJL9na11yb7QJdQWlE_OyEsDc,4069
 pantos/common/blockchains/contracts/avalanche_standard_token.abi,sha256=prb4qk4CbSVeYxX5kyFI4upPHNv0f94wBlR1ynW0Sow,4840
-pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi,sha256=XH4RU3pbgPUjlhlNDkP9l63bEgUL1m1aNW5FMn3H8Vk,33098
+pantos/common/blockchains/contracts/bnb_chain_pantos_forwarder.abi,sha256=udZYZcnMm9xQApQNAxda87p-jrHKNsReUjL5EKXYOwc,7229
+pantos/common/blockchains/contracts/bnb_chain_pantos_hub.abi,sha256=QEFEzDk6LYzjsF8Q1n-P2puHzILBnG5RV0IvsJI_g80,42156
 pantos/common/blockchains/contracts/bnb_chain_pantos_token.abi,sha256=hqSqiE6SaYnRu067CJTJL9na11yb7QJdQWlE_OyEsDc,4069
 pantos/common/blockchains/contracts/bnb_chain_standard_token.abi,sha256=prb4qk4CbSVeYxX5kyFI4upPHNv0f94wBlR1ynW0Sow,4840
-pantos/common/blockchains/contracts/celo_pantos_hub.abi,sha256=XH4RU3pbgPUjlhlNDkP9l63bEgUL1m1aNW5FMn3H8Vk,33098
+pantos/common/blockchains/contracts/celo_pantos_forwarder.abi,sha256=udZYZcnMm9xQApQNAxda87p-jrHKNsReUjL5EKXYOwc,7229
+pantos/common/blockchains/contracts/celo_pantos_hub.abi,sha256=QEFEzDk6LYzjsF8Q1n-P2puHzILBnG5RV0IvsJI_g80,42156
 pantos/common/blockchains/contracts/celo_pantos_token.abi,sha256=hqSqiE6SaYnRu067CJTJL9na11yb7QJdQWlE_OyEsDc,4069
 pantos/common/blockchains/contracts/celo_standard_token.abi,sha256=prb4qk4CbSVeYxX5kyFI4upPHNv0f94wBlR1ynW0Sow,4840
-pantos/common/blockchains/contracts/cronos_pantos_hub.abi,sha256=XH4RU3pbgPUjlhlNDkP9l63bEgUL1m1aNW5FMn3H8Vk,33098
+pantos/common/blockchains/contracts/cronos_pantos_forwarder.abi,sha256=udZYZcnMm9xQApQNAxda87p-jrHKNsReUjL5EKXYOwc,7229
+pantos/common/blockchains/contracts/cronos_pantos_hub.abi,sha256=QEFEzDk6LYzjsF8Q1n-P2puHzILBnG5RV0IvsJI_g80,42156
 pantos/common/blockchains/contracts/cronos_pantos_token.abi,sha256=hqSqiE6SaYnRu067CJTJL9na11yb7QJdQWlE_OyEsDc,4069
 pantos/common/blockchains/contracts/cronos_standard_token.abi,sha256=prb4qk4CbSVeYxX5kyFI4upPHNv0f94wBlR1ynW0Sow,4840
-pantos/common/blockchains/contracts/ethereum_pantos_hub.abi,sha256=XH4RU3pbgPUjlhlNDkP9l63bEgUL1m1aNW5FMn3H8Vk,33098
+pantos/common/blockchains/contracts/ethereum_pantos_forwarder.abi,sha256=udZYZcnMm9xQApQNAxda87p-jrHKNsReUjL5EKXYOwc,7229
+pantos/common/blockchains/contracts/ethereum_pantos_hub.abi,sha256=QEFEzDk6LYzjsF8Q1n-P2puHzILBnG5RV0IvsJI_g80,42156
 pantos/common/blockchains/contracts/ethereum_pantos_token.abi,sha256=hqSqiE6SaYnRu067CJTJL9na11yb7QJdQWlE_OyEsDc,4069
 pantos/common/blockchains/contracts/ethereum_standard_token.abi,sha256=prb4qk4CbSVeYxX5kyFI4upPHNv0f94wBlR1ynW0Sow,4840
-pantos/common/blockchains/contracts/fantom_pantos_hub.abi,sha256=XH4RU3pbgPUjlhlNDkP9l63bEgUL1m1aNW5FMn3H8Vk,33098
+pantos/common/blockchains/contracts/fantom_pantos_forwarder.abi,sha256=udZYZcnMm9xQApQNAxda87p-jrHKNsReUjL5EKXYOwc,7229
+pantos/common/blockchains/contracts/fantom_pantos_hub.abi,sha256=QEFEzDk6LYzjsF8Q1n-P2puHzILBnG5RV0IvsJI_g80,42156
 pantos/common/blockchains/contracts/fantom_pantos_token.abi,sha256=hqSqiE6SaYnRu067CJTJL9na11yb7QJdQWlE_OyEsDc,4069
 pantos/common/blockchains/contracts/fantom_standard_token.abi,sha256=prb4qk4CbSVeYxX5kyFI4upPHNv0f94wBlR1ynW0Sow,4840
-pantos/common/blockchains/contracts/polygon_pantos_hub.abi,sha256=XH4RU3pbgPUjlhlNDkP9l63bEgUL1m1aNW5FMn3H8Vk,33098
+pantos/common/blockchains/contracts/polygon_pantos_forwarder.abi,sha256=udZYZcnMm9xQApQNAxda87p-jrHKNsReUjL5EKXYOwc,7229
+pantos/common/blockchains/contracts/polygon_pantos_hub.abi,sha256=QEFEzDk6LYzjsF8Q1n-P2puHzILBnG5RV0IvsJI_g80,42156
 pantos/common/blockchains/contracts/polygon_pantos_token.abi,sha256=hqSqiE6SaYnRu067CJTJL9na11yb7QJdQWlE_OyEsDc,4069
 pantos/common/blockchains/contracts/polygon_standard_token.abi,sha256=prb4qk4CbSVeYxX5kyFI4upPHNv0f94wBlR1ynW0Sow,4840
 pantos/servicenode/__init__.py,sha256=ETX19tUZfC7cOqtkDBTnCA7NcUPKcFluo_4Glx-GthQ,79
 pantos/servicenode/__main__.py,sha256=DY-M2JvmNJxdi3fDCiTB6M_S0Ky6nv8XnlfwZf3faHc,806
-pantos/servicenode/application.py,sha256=L738Iof68sum_kFACdcY-0lf0p53G9fGCzlrJqWoNWM,3215
-pantos/servicenode/celery.py,sha256=LG-VQkFwp4G1MaWgV5wY3n5nxAaUyslfiZuIm-94_5o,2636
-pantos/servicenode/configuration.py,sha256=1xkHxPaW1j2tYNU-ZwW60tFSZGdFHeCQGE7KrQROcLk,9094
+pantos/servicenode/application.py,sha256=LyxIXC-b0HI9WQFSDVVhigwwosPLMIBQh9eilmmlnDw,3257
+pantos/servicenode/celery.py,sha256=r3VQXExFpdmHYyjjqEbXuNYjv9vFABWMEaxGnu5imNk,2641
+pantos/servicenode/configuration.py,sha256=Hs7kcbskve_Qk4ID7Q8sXspm5THbJvcArBQKzGid2nk,9432
 pantos/servicenode/exceptions.py,sha256=u7F8sakEIgZJxmduuNGXF1DI2AlhtUVbU2WBiVYzOQs,221
 pantos/servicenode/restapi.py,sha256=rvJVVSJ432VNtmhrToH3QngAT_-Ff-d9wyikI_SmbiE,13968
 pantos/servicenode/wsgi.py,sha256=huL0s_DAz9PBqalrjIhBVhlC4lji5MAnoWM2uyPkhoU,198
 pantos/servicenode/blockchains/__init__.py,sha256=k1FtBt79-1fj0Cma-eKiP20FOxgtPaJhXdaI3usof4g,53
 pantos/servicenode/blockchains/avalanche.py,sha256=6a11YEnLJqoC7yuis7DYPbxgaLffxBGS5ve_2IHIO2I,957
-pantos/servicenode/blockchains/base.py,sha256=WLpubBtDekWhwjMBA8kgpIUkYZmTf9Crv2AfZ_AwzwQ,22418
+pantos/servicenode/blockchains/base.py,sha256=Y9pEoHHkeuTcZBxEXTIjlx087uFoag0zbDJ1awrjbB4,22379
 pantos/servicenode/blockchains/bnbchain.py,sha256=wKSQBQh3Gfk5itJB3REcLyGftS-SJizyX6y_rn6m3gU,952
 pantos/servicenode/blockchains/celo.py,sha256=AAPw8_d9fej-2cGHFBGk5-pCfW9r5hXPzLJn2snfyzE,905
 pantos/servicenode/blockchains/cronos.py,sha256=k0_mm1MSvTv0RjWy7zZJ_vFubSnIhhMq6xwL1BCbTTg,921
-pantos/servicenode/blockchains/ethereum.py,sha256=R7wMDSg3xwXZUtpoT_8ijeVNBPSDGYFUpDz2q-8uY30,16850
+pantos/servicenode/blockchains/ethereum.py,sha256=JaLjyYgsuyji7yZa6y_L3s1DmMOe0egqgHoBjMTiEsg,16807
 pantos/servicenode/blockchains/factory.py,sha256=1FvHqiqWDybzpQc1o6RND10Tcmm7J3JZLrXAHf0CRiY,1101
 pantos/servicenode/blockchains/fantom.py,sha256=9_ex2187pTA_ptyZAYIqZmjkJZu39FzunLvslx7bYjI,921
 pantos/servicenode/blockchains/polygon.py,sha256=0sHBG2LNtFkp31gzsCotlb-jpIo3aTjoHUONktlID8k,929
 pantos/servicenode/blockchains/solana.py,sha256=EJzYnw4jPv7Zvs-N4Du11taS0OJiHXVWcc6JnJ8NmFs,2846
 pantos/servicenode/business/__init__.py,sha256=U9mFvZWALPhpJPUJEtzUOv1iJB40UMuzMk_iV2T2DNw,40
 pantos/servicenode/business/base.py,sha256=h4k1oCDiulhrc8bErncZnEASfL6gj5hi4Wu3l-Hcpc0,341
-pantos/servicenode/business/bids.py,sha256=GQB3rZ9xSDZVwLEFcIi6bN_qVddNs6TnfL74H7USgyM,3579
+pantos/servicenode/business/bids.py,sha256=UwFawuJccUXOHo2eZM4nu9EaH2Th8poocgljnhlEoW4,3574
 pantos/servicenode/business/node.py,sha256=HneUUhCy9jW271LyiewcTYRydWgZSgYufuahn-wla0Q,3341
 pantos/servicenode/business/plugins.py,sha256=iZqePXr0uRfegD91rL2Ik1Qr_fMwQR4EkVVls9-IPsw,4446
-pantos/servicenode/business/transfers.py,sha256=MXkcIc_xSvBjzsDBRHj0bleuYp7EECIDKtMUGzlf0ro,37736
-pantos/servicenode/database/__init__.py,sha256=0Fn_XbnoL9jBqjIMqBuIvZEHszSG_7sZGlfzbJoXAKo,2778
+pantos/servicenode/business/transfers.py,sha256=kOtkqGv_uWaqVT-5ZWYqRFnvZ_8tbql7U7yf1eDpheg,37731
+pantos/servicenode/database/__init__.py,sha256=dhZci-8pn_T7qqKWao3_ExgZS9IR9BqvV8eNJVRoDuU,3477
 pantos/servicenode/database/access.py,sha256=Vp8DguYlB3MRTuzcz4Yz9PjFb6bxHqqKgi-uAwoANDE,20036
 pantos/servicenode/database/enums.py,sha256=-eRnbbVJy6PzgbybnJNcOtkGx26vsTPhdo6mKNJLuBw,1166
 pantos/servicenode/database/exceptions.py,sha256=sJPxPTowlipTQFIFzOVP_pSwv_rZzNAx9FTxqqLNndg,1234
 pantos/servicenode/database/models.py,sha256=hD9P4pSaVARRUzE6cNYN6UtVnjhKzyNJ5-DO-cpTL1o,13701
 pantos/servicenode/database/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pantos/servicenode/database/migrations/env.py,sha256=hfw0h5uFB75vPI-OGCRBXjwPCpUbtWLNqg7ggN2oOwI,2080
 pantos/servicenode/database/migrations/versions/5e552e0ec844_remove_id_from_bids_table.py,sha256=0YvRN8tekD6Ia4AsmqDI_-V2UtbtVRqWvxNGtj1t4QM,817
 pantos/servicenode/database/migrations/versions/85982c1f3b95_create_deferrable_constraint.py,sha256=LJ-8QixhxMmdXFQt2NCc628-96SiPOMKcoEbj01Sf8k,1520
 pantos/servicenode/database/migrations/versions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pantos/servicenode/database/migrations/versions/bd913c5bfdfb_off_chain_bids.py,sha256=v1qxnipk6AP5fiGwKVkHMoUjUnLhIMIY_k1GomIa3ag,4152
 pantos/servicenode/database/migrations/versions/c4c46d14ca6a_initial_database_schema.py,sha256=mtWf6rGimqIUC9PN1KRCvGjji02Iota3RYDgyKtnskw,7067
 pantos/servicenode/plugins/__init__.py,sha256=RCE3-Bbwru-bDBYQPCnKQD8g0a8afUCQrWuKczzB46w,1675
 pantos/servicenode/plugins/base.py,sha256=5enINvzrzPskYzG5ZNYUzOgy0Grm2kOP1AipqxhO4Y8,2476
 pantos/servicenode/plugins/bids.py,sha256=pzpOVURWWFAmjmA4OC3Dv2dFHnVhlzttxMt-XziBOXo,3368
-pantos_service_node-1.5.3.dist-info/LICENSE.md,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
-pantos_service_node-1.5.3.dist-info/METADATA,sha256=IPp36nNVjD7aJhDP_FuCRV4yxp_f90ZEy7OGFJGCkjo,775
-pantos_service_node-1.5.3.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-pantos_service_node-1.5.3.dist-info/top_level.txt,sha256=rIHpe7p19Knq5pBCNAwzI7IaXD1Wb0Mguwi7_oltlLY,7
-pantos_service_node-1.5.3.dist-info/RECORD,,
+pantos_service_node-1.6.0.dist-info/LICENSE.md,sha256=ixuiBLtpoK3iv89l7ylKkg9rs2GzF9ukPH7ynZYzK5s,35148
+pantos_service_node-1.6.0.dist-info/METADATA,sha256=Q05FaHBghBdX9nN1GxX7gtdwwaRwrw42YSKF7zZ3dUA,856
+pantos_service_node-1.6.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+pantos_service_node-1.6.0.dist-info/top_level.txt,sha256=rIHpe7p19Knq5pBCNAwzI7IaXD1Wb0Mguwi7_oltlLY,7
+pantos_service_node-1.6.0.dist-info/RECORD,,
```

