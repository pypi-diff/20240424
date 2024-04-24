# Comparing `tmp/aries_cloudcontroller-0.9.0.post1.tar.gz` & `tmp/aries_cloudcontroller-0.9.0.post2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aries_cloudcontroller-0.9.0.post1.tar", last modified: Thu Oct 26 16:18:50 2023, max compression
+gzip compressed data, was "aries_cloudcontroller-0.9.0.post2.tar", last modified: Mon Nov 20 11:59:48 2023, max compression
```

## Comparing `aries_cloudcontroller-0.9.0.post1.tar` & `aries_cloudcontroller-0.9.0.post2.tar`

### file list

```diff
@@ -1,354 +1,354 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.066348 aries_cloudcontroller-0.9.0.post1/
--rw-r--r--   0 runner    (1001) docker     (127)    11319 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2023-10-26 16:18:50.066348 aries_cloudcontroller-0.9.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5182 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.018347 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/
--rw-r--r--   0 runner    (1001) docker     (127)     8372 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4560 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/acapy_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.026347 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    29084 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/action_menu_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6968 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/basicmessage_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    80761 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/connection_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    29144 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/credential_definition_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    49530 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/credentials_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/default_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    34066 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/did_exchange_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    13704 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/discover_features_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    14150 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/discover_features_v20_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    58559 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/endorse_transaction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7538 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/introduction_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    78910 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/issue_credential_v10_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    84973 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/issue_credential_v20_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11997 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/jsonld_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    52012 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/ledger_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    79558 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/mediation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    41876 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/multitenancy_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    16822 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/out_of_band_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    69659 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/present_proof_v10_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    69299 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/present_proof_v20_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     6244 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/resolver_api.py
--rw-r--r--   0 runner    (1001) docker     (127)   122484 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/revocation_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    26689 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/schema_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35069 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/server_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11527 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/settings_api.py
--rw-r--r--   0 runner    (1001) docker     (127)     7076 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/trustping_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    56295 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/wallet_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    28842 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    15204 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)     5386 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.062348 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/
--rw-r--r--   0 runner    (1001) docker     (127)    24059 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2652 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/action_menu_fetch_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2349 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_modules.py
--rw-r--r--   0 runner    (1001) docker     (127)     3060 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_status_liveliness.py
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_status_readiness.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/aml_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4500 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data1_jws.py
--rw-r--r--   0 runner    (1001) docker     (127)     4776 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data_jws.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data_jws_header.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attachment_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     2551 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attribute_mime_types_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2859 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/claim_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2610 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/clear_pending_revocations_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10982 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/conn_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     5159 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_invitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2903 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2409 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)     2414 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_metadata_set_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5593 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_static_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6069 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_static_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5812 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     4258 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     6260 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5051 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2955 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_def_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4410 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_def_value_primary.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_def_value_revocation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2864 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_info_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_rev_indy_records_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_rev_record_details_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2707 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_rev_record_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_revoked_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5664 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4832 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2922 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition_get_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3835 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition_send_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3389 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2530 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definitions_created_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4409 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (127)     3085 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     7411 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2473 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_status_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5400 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did.py
--rw-r--r--   0 runner    (1001) docker     (127)     3140 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3829 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3637 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (127)     4370 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_endpoint_with_type.py
--rw-r--r--   0 runner    (1001) docker     (127)     2814 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2600 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4732 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/didx_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3452 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_field.py
--rw-r--r--   0 runner    (1001) docker     (127)     2843 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_holder.py
--rw-r--r--   0 runner    (1001) docker     (127)     3186 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3693 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3432 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_proof_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3382 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/disclose.py
--rw-r--r--   0 runner    (1001) docker     (127)     2839 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/disclosures.py
--rw-r--r--   0 runner    (1001) docker     (127)     2767 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2560 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/endorser_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3876 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/endpoints_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     4276 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/generated.py
--rw-r--r--   0 runner    (1001) docker     (127)     3265 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/get_did_endpoint_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3191 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/get_did_verkey_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/get_nym_role_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_attr_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     4989 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_abstract.py
--rw-r--r--   0 runner    (1001) docker     (127)     6556 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     3398 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_precis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4736 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7206 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     4356 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_eq_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3967 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_ge_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3081 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_ge_proof_pred.py
--rw-r--r--   0 runner    (1001) docker     (127)     3359 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_key_correctness_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2419 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_non_revoc_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_non_revocation_interval.py
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3999 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3761 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     4834 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3894 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_primary_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_primary_proof_eq_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     4043 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     5882 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_identifier.py
--rw-r--r--   0 runner    (1001) docker     (127)     3649 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof_aggregated_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3688 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof_proofs_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof_proofs_proof_non_revoc_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_attr_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_pred_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2806 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_pred_spec_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (127)     6295 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2790 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_request_non_revoked.py
--rw-r--r--   0 runner    (1001) docker     (127)     6326 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2460 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof_predicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3246 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3360 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2669 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_requested_creds_requested_attr.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_requested_creds_requested_pred.py
--rw-r--r--   0 runner    (1001) docker     (127)     6114 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def.py
--rw-r--r--   0 runner    (1001) docker     (127)     4830 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     2939 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys_accum_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     3280 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_entry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_entry_value.py
--rw-r--r--   0 runner    (1001) docker     (127)     3991 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/input_descriptors.py
--rw-r--r--   0 runner    (1001) docker     (127)     5934 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5113 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     5521 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     7399 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/issuer_cred_rev_record.py
--rw-r--r--   0 runner    (1001) docker     (127)    10699 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/issuer_rev_reg_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/jws_create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/jws_verify.py
--rw-r--r--   0 runner    (1001) docker     (127)     2862 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/jws_verify_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2914 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2407 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_query_filter_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_query_paginate.py
--rw-r--r--   0 runner    (1001) docker     (127)     3377 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_update.py
--rw-r--r--   0 runner    (1001) docker     (127)     2916 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_update_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3462 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_update_rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     3131 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ld_proof_vc_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4932 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ld_proof_vc_detail_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     3165 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ledger_config_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ledger_config_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5492 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/linked_data_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2714 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2959 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_deny.py
--rw-r--r--   0 runner    (1001) docker     (127)     3003 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_grant.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_id_match_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4872 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_form.py
--rw-r--r--   0 runner    (1001) docker     (127)     3257 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_form_param.py
--rw-r--r--   0 runner    (1001) docker     (127)     3362 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_option.py
--rw-r--r--   0 runner    (1001) docker     (127)     2322 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/model_date.py
--rw-r--r--   0 runner    (1001) docker     (127)     4619 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/model_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     7100 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/oob_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2509 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/perform_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2568 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ping_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2398 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ping_request_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     5594 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/presentation_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/presentation_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3990 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/presentation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/profile_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     2606 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/protocol_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/publish_revocations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3217 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/queries.py
--rw-r--r--   0 runner    (1001) docker     (127)     3002 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/query.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/query_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2898 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/raw_encoded.py
--rw-r--r--   0 runner    (1001) docker     (127)     5175 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/receive_invitation_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/remove_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2475 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/resolution_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3604 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_create_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2478 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_issued_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_update_tails_file_uri.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_wallet_updated_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_regs_created.py
--rw-r--r--   0 runner    (1001) docker     (127)     7180 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/revoke_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4554 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/route_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2711 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_get_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_input_descriptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_send_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2392 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schemas_created_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3519 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schemas_input_descriptor_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2572 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/send_menu.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/send_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     3069 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/service_decorator.py
--rw-r--r--   0 runner    (1001) docker     (127)     2699 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/sign_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/sign_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2886 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/signature_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/signed_doc.py
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/submission_requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)     2514 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_accept.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_acceptance.py
--rw-r--r--   0 runner    (1001) docker     (127)     3756 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_info.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2617 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/tails_delete_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/transaction_jobs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2974 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/transaction_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/transaction_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3225 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_credential_definition_send_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_publish_revocations_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2915 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_register_ledger_nym_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3071 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_rev_reg_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3103 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_schema_send_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2427 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/update_profile_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4158 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/update_wallet_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5062 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_conn_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     7865 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_create.py
--rw-r--r--   0 runner    (1001) docker     (127)    13124 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5204 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_free_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2618 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2354 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     8075 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_proposal_request_mand.py
--rw-r--r--   0 runner    (1001) docker     (127)     8088 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_proposal_request_opt.py
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_store_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5710 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9670 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_exchange.py
--rw-r--r--   0 runner    (1001) docker     (127)     3096 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_exchange_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3939 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3716 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2967 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_attr_spec.py
--rw-r--r--   0 runner    (1001) docker     (127)     3218 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_bound_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5350 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_free.py
--rw-r--r--   0 runner    (1001) docker     (127)    10730 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2799 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3706 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6686 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_indy.py
--rw-r--r--   0 runner    (1001) docker     (127)     4694 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     6362 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_filter_indy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_filter_ld_proof.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     4837 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_issue.py
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_issue_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2594 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_issue_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5370 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_offer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4979 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_offer_conn_free_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     5105 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_offer_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     4563 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4210 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_request_free.py
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_request_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2333 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_store_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_discovery_exchange_list_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2739 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_discovery_exchange_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     5775 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_discovery_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     4687 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_issue_cred_schema_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres.py
--rw-r--r--   0 runner    (1001) docker     (127)     3670 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_create_request_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9718 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_ex_record_by_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2986 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_ex_record_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2330 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_problem_report_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4363 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_proposal_by_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3950 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_proposal_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_request_by_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     3820 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_send_request_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_spec_by_format_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2676 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_presentation_send_request_to_proposal.py
--rw-r--r--   0 runner    (1001) docker     (127)     3800 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/vc_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     2809 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/vc_record_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2645 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/verify_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/verify_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3962 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/w3_c_credentials_list_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     2929 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_list_with_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4825 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_record_with_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2313 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/write_ledger_request.py
--rw-r--r--   0 runner    (1001) docker     (127)     9712 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/rest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.062348 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/util/
--rw-r--r--   0 runner    (1001) docker     (127)      216 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/util/pydantic_model_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/util/regex_patterns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.022347 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5629 2023-10-26 16:18:49.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    17447 2023-10-26 16:18:49.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-26 16:18:49.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       94 2023-10-26 16:18:49.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-26 16:18:49.000000 aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-26 16:18:50.066348 aries_cloudcontroller-0.9.0.post1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.066348 aries_cloudcontroller-0.9.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.066348 aries_cloudcontroller-0.9.0.post1/tests/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      743 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/client/test_acapy_client.py
--rw-r--r--   0 runner    (1001) docker     (127)       74 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.066348 aries_cloudcontroller-0.9.0.post1/tests/model/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_attach_decorator_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_credential_definition.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_credential_offer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2103 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_did.py
--rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_invitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_presentation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4781 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_v20_cred_ex_record.py
--rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/model/test_v20_pres_ex_record.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:50.066348 aries_cloudcontroller-0.9.0.post1/tests/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-10-26 16:18:36.000000 aries_cloudcontroller-0.9.0.post1/tests/util/compare_dicts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.584812 aries_cloudcontroller-0.9.0.post2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11319 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2023-11-20 11:59:48.584812 aries_cloudcontroller-0.9.0.post2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.524812 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/
+-rw-r--r--   0 runner    (1001) docker     (127)     8372 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4629 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/acapy_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.532812 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1947 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50922 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/action_menu_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11640 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/basicmessage_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137878 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/connection_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49053 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/credential_definition_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    85933 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/credentials_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9624 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/default_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56141 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/did_exchange_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23195 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/discover_features_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23942 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/discover_features_v20_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   102704 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/endorse_transaction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12492 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/introduction_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136995 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/issue_credential_v10_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   147466 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/issue_credential_v20_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20668 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/jsonld_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    90918 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/ledger_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   138170 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/mediation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    72693 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/multitenancy_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27414 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/out_of_band_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   120593 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/present_proof_v10_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   119603 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/present_proof_v20_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10577 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/resolver_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)   213053 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/revocation_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45435 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/schema_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    63255 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/server_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20029 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/settings_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11734 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/trustping_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    97043 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/wallet_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25558 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15204 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5402 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.580813 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/
+-rw-r--r--   0 runner    (1001) docker     (127)    24059 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/action_menu_fetch_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2363 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2712 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2370 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_modules.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3074 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2380 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_status_liveliness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2375 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_status_readiness.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/aml_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4514 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4379 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data1_jws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4790 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data_jws.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3143 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data_jws_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attachment_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2565 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attribute_mime_types_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/claim_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/clear_pending_revocations_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10996 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/conn_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5173 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2917 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2423 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2428 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_metadata_set_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5607 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_static_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6083 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_static_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5826 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4272 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6274 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5065 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2500 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2442 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4424 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_def_value_primary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_def_value_revocation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2878 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_info_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_rev_indy_records_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2963 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_rev_record_details_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2721 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_rev_record_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_revoked_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5678 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4846 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2936 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3849 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2544 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definitions_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4423 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3099 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7425 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_status_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5414 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3154 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3651 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4384 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_endpoint_with_type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2828 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2614 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4746 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/didx_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2857 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_holder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3200 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3707 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_proof_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3396 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/disclose.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2853 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/disclosures.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2781 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/endorser_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3890 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/endpoints_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4290 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/generated.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3279 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/get_did_endpoint_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3205 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/get_did_verkey_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/get_nym_role_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2834 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_attr_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5003 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_abstract.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6570 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_precis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4750 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7220 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4370 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_eq_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3981 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_ge_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3095 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_ge_proof_pred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3373 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_key_correctness_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2433 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_non_revoc_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2800 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_non_revocation_interval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3884 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4013 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3775 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4848 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_primary_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4414 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_primary_proof_eq_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4057 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5896 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_identifier.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3663 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2589 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof_aggregated_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3702 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof_proofs_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2504 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof_proofs_proof_non_revoc_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_attr_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4253 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_pred_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2820 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_pred_spec_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6309 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_request_non_revoked.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6340 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof_predicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3374 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2683 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_requested_creds_requested_attr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2785 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_requested_creds_requested_pred.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6128 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4844 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2953 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2416 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys_accum_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3294 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_entry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_entry_value.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4005 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/input_descriptors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5948 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5127 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5535 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3170 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7413 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/issuer_cred_rev_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10713 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/issuer_rev_reg_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4213 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/jws_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/jws_verify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2876 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/jws_verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2928 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3313 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2421 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_query_filter_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2561 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_query_paginate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3391 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2930 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_update_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3476 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_update_rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3145 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ld_proof_vc_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ld_proof_vc_detail_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3179 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ledger_config_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3018 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ledger_config_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5506 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/linked_data_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2973 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_deny.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3017 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_grant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2426 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_id_match_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2970 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4886 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3823 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3561 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3271 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_form_param.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3376 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3326 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_option.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2336 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/model_date.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4633 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/model_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7114 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/oob_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2523 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/perform_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2582 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ping_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ping_request_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5608 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/presentation_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3703 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/presentation_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4004 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/presentation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/profile_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2620 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/protocol_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2501 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/publish_revocations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/queries.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/query.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2742 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/query_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/raw_encoded.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5189 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/receive_invitation_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2480 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/remove_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2489 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/resolution_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3618 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_create_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2492 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_issued_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2689 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2411 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_update_tails_file_uri.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_wallet_updated_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2386 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_regs_created.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7194 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/revoke_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4568 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/route_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2725 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_get_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_input_descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_send_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3467 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schemas_created_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3533 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schemas_input_descriptor_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/send_menu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/send_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/service_decorator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2713 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/sign_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/sign_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2900 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/signature_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/signed_doc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4346 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/submission_requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2528 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_accept.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_acceptance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3770 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2516 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2631 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/tails_delete_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3593 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/transaction_jobs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2988 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/transaction_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6140 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/transaction_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3239 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_credential_definition_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3156 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_publish_revocations_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2929 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_register_ledger_nym_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3085 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_rev_reg_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3117 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_schema_send_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2441 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/update_profile_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4172 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/update_wallet_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2887 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5076 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_conn_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7879 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13138 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3105 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_free_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2632 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2368 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8089 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_proposal_request_mand.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8102 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_proposal_request_opt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2371 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5724 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3580 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9684 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_exchange.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_exchange_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2376 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3953 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3730 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2981 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_attr_spec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_bound_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5364 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10744 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2813 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6700 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_indy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4708 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3109 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6376 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_filter_indy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2700 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_filter_ld_proof.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4851 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_issue.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2364 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_issue_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2608 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_issue_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5384 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_offer_conn_free_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5119 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_offer_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5205 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4577 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4224 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_request_free.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2347 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_store_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2974 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_discovery_exchange_list_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2753 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_discovery_exchange_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5789 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_discovery_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4701 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_issue_cred_schema_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4550 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3684 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_create_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9732 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2634 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_ex_record_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3000 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_ex_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2466 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_problem_report_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4377 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_proposal_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3964 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_proposal_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4720 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3114 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_request_by_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3834 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_send_request_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3316 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_spec_by_format_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2690 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_presentation_send_request_to_proposal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/vc_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/vc_record_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2659 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/verify_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2435 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/verify_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3976 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/w3_c_credentials_list_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2943 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_list_with_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1083 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_record_with_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/write_ledger_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5776 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/rest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.580813 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/util/
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/util/pydantic_model_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/util/regex_patterns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.528812 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5798 2023-11-20 11:59:48.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    17447 2023-11-20 11:59:48.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-20 11:59:48.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2023-11-20 11:59:48.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-11-20 11:59:48.000000 aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-20 11:59:48.584812 aries_cloudcontroller-0.9.0.post2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.580813 aries_cloudcontroller-0.9.0.post2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.580813 aries_cloudcontroller-0.9.0.post2/tests/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      743 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/client/test_acapy_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.584812 aries_cloudcontroller-0.9.0.post2/tests/model/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_attach_decorator_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_credential_definition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_credential_offer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2103 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_did.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3004 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_invitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_presentation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4781 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_v20_cred_ex_record.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3689 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/model/test_v20_pres_ex_record.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:48.584812 aries_cloudcontroller-0.9.0.post2/tests/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2023-11-20 11:59:38.000000 aries_cloudcontroller-0.9.0.post2/tests/util/compare_dicts.py
```

### Comparing `aries_cloudcontroller-0.9.0.post1/LICENSE` & `aries_cloudcontroller-0.9.0.post2/LICENSE`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/PKG-INFO` & `aries_cloudcontroller-0.9.0.post2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,7 @@
-Metadata-Version: 2.1
-Name: aries_cloudcontroller
-Version: 0.9.0.post1
-Summary: A simple python client for controlling an ACA-Py agent
-Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 <p align="center">
   <br />
   <img
     alt="Hyperledger Aries logo"
     src="https://raw.githubusercontent.com/didx-xyz/aries-cloudcontroller-python/main/assets/aries-logo.png"
     height="250px"
   />
```

#### html2text {}

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.9.0.post1 Summary:
-A simple python client for controlling an ACA-Py agent Home-page: https://
-github.com/didx-xyz/aries-cloudcontroller-python Classifier: Programming
-Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
-License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
-Description-Content-Type: text/markdown License-File: LICENSE
 
                            [Hyperledger Aries logo]
                   ************ AArriieess CClloouudd CCoonnttrroolllleerr PPyytthhoonn ************
        [Pipeline Status]_[_a_r_i_e_s_-_c_l_o_u_d_c_o_n_t_r_o_l_l_e_r_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_]
 
       _F_e_a_t_u_r_e_s  |  _U_s_a_g_e  |  _A_v_a_i_l_a_b_l_e_ _A_P_I_s  |  _C_o_n_t_r_i_b_u_t_i_n_g  |  _L_i_c_e_n_s_e
 The Aries CloudController is a client library, written in Python, for
```

### Comparing `aries_cloudcontroller-0.9.0.post1/README.md` & `aries_cloudcontroller-0.9.0.post2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: aries_cloudcontroller
+Version: 0.9.0.post2
+Summary: A simple python client for controlling an ACA-Py agent
+Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: aiohttp~=3.9.0
+Requires-Dist: pydantic~=2.5.1
+Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: typing-extensions~=4.8.0
+Requires-Dist: urllib3~=2.1.0
+
 <p align="center">
   <br />
   <img
     alt="Hyperledger Aries logo"
     src="https://raw.githubusercontent.com/didx-xyz/aries-cloudcontroller-python/main/assets/aries-logo.png"
     height="250px"
   />
```

#### html2text {}

```diff
@@ -1,7 +1,16 @@
+Metadata-Version: 2.1 Name: aries_cloudcontroller Version: 0.9.0.post2 Summary:
+A simple python client for controlling an ACA-Py agent Home-page: https://
+github.com/didx-xyz/aries-cloudcontroller-python Classifier: Programming
+Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
+License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+aiohttp~=3.9.0 Requires-Dist: pydantic~=2.5.1 Requires-Dist: python-
+dateutil~=2.8.2 Requires-Dist: typing-extensions~=4.8.0 Requires-Dist:
+urllib3~=2.1.0
 
                            [Hyperledger Aries logo]
                   ************ AArriieess CClloouudd CCoonnttrroolllleerr PPyytthhoonn ************
        [Pipeline Status]_[_a_r_i_e_s_-_c_l_o_u_d_c_o_n_t_r_o_l_l_e_r_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_]
 
       _F_e_a_t_u_r_e_s  |  _U_s_a_g_e  |  _A_v_a_i_l_a_b_l_e_ _A_P_I_s  |  _C_o_n_t_r_i_b_u_t_i_n_g  |  _L_i_c_e_n_s_e
 The Aries CloudController is a client library, written in Python, for
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/__init__.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/acapy_client.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/acapy_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,14 +73,17 @@
     ):
         if not api_key and not admin_insecure:
             raise Exception(
                 "api_key property is missing. Use admin_insecure=True if you want"
                 " to use the controller without authentication."
             )
 
+        self.api_key = api_key
+        self.tenant_jwt = tenant_jwt
+
         # We will configure an ApiClient instance and pass it to our API modules
         self.configuration = Configuration(host=base_url)
         self.api_client = ApiClient(self.configuration)
 
         # ApiClient init can only take one header, so configure api_key and tenant_jwt separately
         if api_key:
             self.api_client.default_headers["x-api-key"] = api_key
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api/__init__.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api_client.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api_client.py`

 * *Files 16% similar despite different names*

```diff
@@ -14,23 +14,32 @@
 
 import datetime
 import json
 import mimetypes
 import os
 import re
 import tempfile
+from typing import List, Optional, Tuple
 from urllib.parse import quote
 
 from dateutil.parser import parse
 
 import aries_cloudcontroller.models
 from aries_cloudcontroller import rest
 from aries_cloudcontroller.api_response import ApiResponse
 from aries_cloudcontroller.configuration import Configuration
-from aries_cloudcontroller.exceptions import ApiException, ApiValueError
+from aries_cloudcontroller.exceptions import (
+    ApiException,
+    ApiValueError,
+    BadRequestException,
+    ForbiddenException,
+    NotFoundException,
+    ServiceException,
+    UnauthorizedException,
+)
 
 
 class ApiClient:
     """Generic API client for OpenAPI client library builds.
 
     OpenAPI generic API client. This client handles the client-
     server communication, and is invariant across implementations. Specifics of
@@ -118,33 +127,51 @@
 
         It stores default ApiClient.
 
         :param default: object of ApiClient.
         """
         cls._default = default
 
-    async def __call_api(
+    def param_serialize(
         self,
-        resource_path,
         method,
+        resource_path,
         path_params=None,
         query_params=None,
         header_params=None,
         body=None,
         post_params=None,
         files=None,
-        response_types_map=None,
         auth_settings=None,
-        _return_http_data_only=None,
         collection_formats=None,
-        _preload_content=True,
-        _request_timeout=None,
         _host=None,
         _request_auth=None,
-    ):
+    ) -> Tuple:
+        """Builds the HTTP request params needed by the request.
+        :param method: Method to call.
+        :param resource_path: Path to method endpoint.
+        :param path_params: Path parameters in the url.
+        :param query_params: Query parameters in the url.
+        :param header_params: Header parameters to be
+            placed in the request header.
+        :param body: Request body.
+        :param post_params dict: Request post form parameters,
+            for `application/x-www-form-urlencoded`, `multipart/form-data`.
+        :param auth_settings list: Auth Settings names for the request.
+        :param files dict: key -> filename, value -> filepath,
+            for `multipart/form-data`.
+        :param collection_formats: dict of collection formats for path, query,
+            header, and post parameters.
+        :param _request_auth: set to override the auth_settings for an a single
+                              request; this effectively ignores the authentication
+                              in the spec for a single request.
+        :return: tuple of form (path, http_method, query_params, header_params,
+            body, post_params, files)
+        """
+
         config = self.configuration
 
         # header parameters
         header_params = header_params or {}
         header_params.update(self.default_headers)
         if self.cookie:
             header_params["Cookie"] = self.cookie
@@ -197,74 +224,115 @@
         if query_params:
             query_params = self.sanitize_for_serialization(
                 query_params, query_params=True
             )
             url_query = self.parameters_to_url_query(query_params, collection_formats)
             url += "?" + url_query
 
+        return method, url, header_params, body, post_params
+
+    async def call_api(
+        self,
+        method,
+        url,
+        header_params=None,
+        body=None,
+        post_params=None,
+        _request_timeout=None,
+    ) -> rest.RESTResponse:
+        """Makes the HTTP request (synchronous)
+        :param method: Method to call.
+        :param url: Path to method endpoint.
+        :param header_params: Header parameters to be
+            placed in the request header.
+        :param body: Request body.
+        :param post_params dict: Request post form parameters,
+            for `application/x-www-form-urlencoded`, `multipart/form-data`.
+        :param _request_timeout: timeout setting for this request.
+        :return: RESTResponse
+        """
+
         try:
             # perform request and return response
-            response_data = await self.request(
+            response_data = await self.rest_client.request(
                 method,
                 url,
-                query_params=query_params,
                 headers=header_params,
-                post_params=post_params,
                 body=body,
-                _preload_content=_preload_content,
+                post_params=post_params,
                 _request_timeout=_request_timeout,
             )
+
         except ApiException as e:
             if e.body:
                 e.body = e.body.decode("utf-8")
             raise e
 
-        self.last_response = response_data
-
-        return_data = None  # assuming deserialization is not needed
-        # data needs deserialization or returns HTTP data (deserialized) only
-        if _preload_content or _return_http_data_only:
-            response_type = response_types_map.get(str(response_data.status), None)
-            if (
-                not response_type
-                and isinstance(response_data.status, int)
-                and 100 <= response_data.status <= 599
-            ):
-                # if not found, look for '1XX', '2XX', etc.
-                response_type = response_types_map.get(
-                    str(response_data.status)[0] + "XX", None
-                )
-
-            if response_type == "bytearray":
-                response_data.data = response_data.data
-            else:
-                match = None
-                content_type = response_data.getheader("content-type")
-                if content_type is not None:
-                    match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
-                encoding = match.group(1) if match else "utf-8"
-                response_data.data = response_data.data.decode(encoding)
-
-            # deserialize response data
-            if response_type == "bytearray":
-                return_data = response_data.data
-            elif response_type:
-                return_data = self.deserialize(response_data, response_type)
-            else:
-                return_data = None
+        return response_data
 
-        if _return_http_data_only:
-            return return_data
+    def response_deserialize(
+        self, response_data=None, response_types_map=None
+    ) -> ApiResponse:
+        """Deserializes response into an object.
+        :param response_data: RESTResponse object to be deserialized.
+        :param response_types_map: dict of response types.
+        :return: ApiResponse
+        """
+
+        response_type = response_types_map.get(str(response_data.status), None)
+        if (
+            not response_type
+            and isinstance(response_data.status, int)
+            and 100 <= response_data.status <= 599
+        ):
+            # if not found, look for '1XX', '2XX', etc.
+            response_type = response_types_map.get(
+                str(response_data.status)[0] + "XX", None
+            )
+
+        if not 200 <= response_data.status <= 299:
+            if response_data.status == 400:
+                raise BadRequestException(http_resp=response_data)
+
+            if response_data.status == 401:
+                raise UnauthorizedException(http_resp=response_data)
+
+            if response_data.status == 403:
+                raise ForbiddenException(http_resp=response_data)
+
+            if response_data.status == 404:
+                raise NotFoundException(http_resp=response_data)
+
+            if 500 <= response_data.status <= 599:
+                raise ServiceException(http_resp=response_data)
+            raise ApiException(http_resp=response_data)
+
+        # deserialize response data
+
+        if response_type == "bytearray":
+            return_data = response_data.data
+        elif response_type is None:
+            return_data = None
+        elif response_type == "file":
+            return_data = self.__deserialize_file(response_data)
         else:
-            return ApiResponse(
-                status_code=response_data.status,
-                data=return_data,
-                headers=response_data.getheaders(),
-                raw_data=response_data.data,
-            )
+            match = None
+            content_type = response_data.getheader("content-type")
+            if content_type is not None:
+                match = re.search(r"charset=([a-zA-Z\-\d]+)[\s;]?", content_type)
+            encoding = match.group(1) if match else "utf-8"
+            response_text = response_data.data.decode(encoding)
+            return_data = self.deserialize(response_text, response_type)
+
+        return ApiResponse(
+            status_code=response_data.status,
+            data=return_data,
+            headers=response_data.getheaders(),
+            raw_data=response_data.data,
+        )
 
     def sanitize_for_serialization(self, obj, query_params=False):
         """Builds a JSON POST object.
 
         If obj is None, return None.
         If obj is str, int, long, float, bool, return directly.
         If obj is datetime.datetime, datetime.date
@@ -309,33 +377,29 @@
             obj_dict = obj.to_dict()
 
         return {
             key: self.sanitize_for_serialization(val, query_params=query_params)
             for key, val in obj_dict.items()
         }
 
-    def deserialize(self, response, response_type):
+    def deserialize(self, response_text, response_type):
         """Deserializes response into an object.
 
         :param response: RESTResponse object to be deserialized.
         :param response_type: class literal for
             deserialized object, or string of class name.
 
         :return: deserialized object.
         """
-        # handle file downloading
-        # save response body into a tmp file and return the instance
-        if response_type == "file":
-            return self.__deserialize_file(response)
 
         # fetch data from response object
         try:
-            data = json.loads(response.data)
+            data = json.loads(response_text)
         except ValueError:
-            data = response.data
+            data = response_text
 
         return self.__deserialize(data, response_type)
 
     def __deserialize(self, data, klass):
         """Deserializes dict, list, str into an object.
 
         :param data: dict, list or str.
@@ -380,181 +444,25 @@
         elif klass == datetime.date:
             return self.__deserialize_date(data)
         elif klass == datetime.datetime:
             return self.__deserialize_datetime(data)
         else:
             return self.__deserialize_model(data, klass)
 
-    async def call_api(
-        self,
-        resource_path,
-        method,
-        path_params=None,
-        query_params=None,
-        header_params=None,
-        body=None,
-        post_params=None,
-        files=None,
-        response_types_map=None,
-        auth_settings=None,
-        _return_http_data_only=None,
-        collection_formats=None,
-        _preload_content=True,
-        _request_timeout=None,
-        _host=None,
-        _request_auth=None,
-    ):
-        """Makes the HTTP request (synchronous) and returns deserialized data.
-
-        :param resource_path: Path to method endpoint.
-        :param method: Method to call.
-        :param path_params: Path parameters in the url.
-        :param query_params: Query parameters in the url.
-        :param header_params: Header parameters to be
-            placed in the request header.
-        :param body: Request body.
-        :param post_params dict: Request post form parameters,
-            for `application/x-www-form-urlencoded`, `multipart/form-data`.
-        :param auth_settings list: Auth Settings names for the request.
-        :param response: Response data type.
-        :param files dict: key -> filename, value -> filepath,
-            for `multipart/form-data`.
-        :param _return_http_data_only: response data instead of ApiResponse
-                                       object with status code, headers, etc
-        :param _preload_content: if False, the ApiResponse.data will
-                                 be set to none and raw_data will store the
-                                 HTTP response body without reading/decoding.
-                                 Default is True.
-        :param collection_formats: dict of collection formats for path, query,
-            header, and post parameters.
-        :param _request_timeout: timeout setting for this request. If one
-                                 number provided, it will be total request
-                                 timeout. It can also be a pair (tuple) of
-                                 (connection, read) timeouts.
-        :param _request_auth: set to override the auth_settings for an a single
-                              request; this effectively ignores the authentication
-                              in the spec for a single request.
-        :type _request_token: dict, optional
-        :return:
-            The response.
-        """
-        args = (
-            resource_path,
-            method,
-            path_params,
-            query_params,
-            header_params,
-            body,
-            post_params,
-            files,
-            response_types_map,
-            auth_settings,
-            _return_http_data_only,
-            collection_formats,
-            _preload_content,
-            _request_timeout,
-            _host,
-            _request_auth,
-        )
-        return await self.__call_api(*args)
-
-    async def request(
-        self,
-        method,
-        url,
-        query_params=None,
-        headers=None,
-        post_params=None,
-        body=None,
-        _preload_content=True,
-        _request_timeout=None,
-    ):
-        """Makes the HTTP request using RESTClient."""
-        if method == "GET":
-            return await self.rest_client.get_request(
-                url,
-                query_params=query_params,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout,
-                headers=headers,
-            )
-        elif method == "HEAD":
-            return await self.rest_client.head_request(
-                url,
-                query_params=query_params,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout,
-                headers=headers,
-            )
-        elif method == "OPTIONS":
-            return await self.rest_client.options_request(
-                url,
-                query_params=query_params,
-                headers=headers,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout,
-            )
-        elif method == "POST":
-            return await self.rest_client.post_request(
-                url,
-                query_params=query_params,
-                headers=headers,
-                post_params=post_params,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout,
-                body=body,
-            )
-        elif method == "PUT":
-            return await self.rest_client.put_request(
-                url,
-                query_params=query_params,
-                headers=headers,
-                post_params=post_params,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout,
-                body=body,
-            )
-        elif method == "PATCH":
-            return await self.rest_client.patch_request(
-                url,
-                query_params=query_params,
-                headers=headers,
-                post_params=post_params,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout,
-                body=body,
-            )
-        elif method == "DELETE":
-            return await self.rest_client.delete_request(
-                url,
-                query_params=query_params,
-                headers=headers,
-                _preload_content=_preload_content,
-                _request_timeout=_request_timeout,
-                body=body,
-            )
-        else:
-            raise ApiValueError(
-                "http method must be `GET`, `HEAD`, `OPTIONS`,"
-                " `POST`, `PATCH`, `PUT` or `DELETE`."
-            )
-
     def parameters_to_tuples(self, params, collection_formats):
         """Get parameters as list of tuples, formatting collections.
 
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: Parameters as list of tuples, collections formatted
         """
         new_params = []
         if collection_formats is None:
             collection_formats = {}
-        for k, v in (
-            params.items() if isinstance(params, dict) else params
-        ):  # noqa: E501
+        for k, v in params.items() if isinstance(params, dict) else params:
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == "multi":
                     new_params.extend((k, value) for value in v)
                 else:
                     if collection_format == "ssv":
                         delimiter = " "
@@ -575,21 +483,19 @@
         :param params: Parameters as dict or list of two-tuples
         :param dict collection_formats: Parameter collection formats
         :return: URL query string (e.g. a=Hello%20World&b=123)
         """
         new_params = []
         if collection_formats is None:
             collection_formats = {}
-        for k, v in (
-            params.items() if isinstance(params, dict) else params
-        ):  # noqa: E501
-            if isinstance(v, (int, float)):
-                v = str(v)
+        for k, v in params.items() if isinstance(params, dict) else params:
             if isinstance(v, bool):
                 v = str(v).lower()
+            if isinstance(v, (int, float)):
+                v = str(v)
             if isinstance(v, dict):
                 v = json.dumps(v)
 
             if k in collection_formats:
                 collection_format = collection_formats[k]
                 if collection_format == "multi":
                     new_params.extend((k, value) for value in v)
@@ -631,22 +537,22 @@
                             mimetypes.guess_type(filename)[0]
                             or "application/octet-stream"
                         )
                         params.append(tuple([k, tuple([filename, filedata, mimetype])]))
 
         return params
 
-    def select_header_accept(self, accepts):
+    def select_header_accept(self, accepts: List[str]) -> Optional[str]:
         """Returns `Accept` based on an array of accepts provided.
 
         :param accepts: List of headers.
         :return: Accept (e.g. application/json).
         """
         if not accepts:
-            return
+            return None
 
         for accept in accepts:
             if re.search("json", accept, re.IGNORECASE):
                 return accept
 
         return accepts[0]
 
@@ -670,15 +576,15 @@
         headers,
         queries,
         auth_settings,
         resource_path,
         method,
         body,
         request_auth=None,
-    ):
+    ) -> None:
         """Updates header and query params based on authentication setting.
 
         :param headers: Header parameters dict to be updated.
         :param queries: Query parameters tuple list to be updated.
         :param auth_settings: Authentication setting identifiers list.
         :resource_path: A string representation of the HTTP request resource path.
         :method: A string representation of the HTTP request method.
@@ -690,26 +596,25 @@
         if not auth_settings:
             return
 
         if request_auth:
             self._apply_auth_params(
                 headers, queries, resource_path, method, body, request_auth
             )
-            return
-
-        for auth in auth_settings:
-            auth_setting = self.configuration.auth_settings().get(auth)
-            if auth_setting:
-                self._apply_auth_params(
-                    headers, queries, resource_path, method, body, auth_setting
-                )
+        else:
+            for auth in auth_settings:
+                auth_setting = self.configuration.auth_settings().get(auth)
+                if auth_setting:
+                    self._apply_auth_params(
+                        headers, queries, resource_path, method, body, auth_setting
+                    )
 
     def _apply_auth_params(
         self, headers, queries, resource_path, method, body, auth_setting
-    ):
+    ) -> None:
         """Updates the request parameters based on a single auth_setting
 
         :param headers: Header parameters dict to be updated.
         :param queries: Query parameters tuple list to be updated.
         :resource_path: A string representation of the HTTP request resource path.
         :method: A string representation of the HTTP request method.
         :body: A object representing the body of the HTTP request.
@@ -728,14 +633,17 @@
 
     def __deserialize_file(self, response):
         """Deserializes body to file
 
         Saves response body into a file in a temporary folder,
         using the filename from the `Content-Disposition` header if provided.
 
+        handle file downloading
+        save response body into a tmp file and return the instance
+
         :param response:  RESTResponse.
         :return: file path.
         """
         fd, path = tempfile.mkstemp(dir=self.configuration.temp_folder_path)
         os.close(fd)
         os.remove(path)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/api_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/api_response.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,30 +1,24 @@
 """API response object."""
 
 from __future__ import annotations
 
-from typing import Any, Dict, Optional
+from typing import Dict, Generic, Optional, TypeVar
 
-from pydantic import Field, StrictInt, StrictStr
+from pydantic import BaseModel, Field, StrictBytes, StrictInt, StrictStr
 
+T = TypeVar("T")
 
-class ApiResponse:
+
+class ApiResponse(BaseModel, Generic[T]):
     """
     API response object
     """
 
-    status_code: Optional[StrictInt] = Field(None, description="HTTP status code")
+    status_code: StrictInt = Field(description="HTTP status code")
     headers: Optional[Dict[StrictStr, StrictStr]] = Field(
         None, description="HTTP headers"
     )
-    data: Optional[Any] = Field(
-        None, description="Deserialized data given the data type"
-    )
-    raw_data: Optional[Any] = Field(None, description="Raw data (HTTP response body)")
+    data: T = Field(description="Deserialized data given the data type")
+    raw_data: StrictBytes = Field(description="Raw data (HTTP response body)")
 
-    def __init__(
-        self, status_code=None, headers=None, data=None, raw_data=None
-    ) -> None:
-        self.status_code = status_code
-        self.headers = headers
-        self.data = data
-        self.raw_data = raw_data
+    model_config = {"arbitrary_types_allowed": True}
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/configuration.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/configuration.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/exceptions.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
 
 
 class ApiException(OpenApiException):
     def __init__(self, status=None, reason=None, http_resp=None) -> None:
         if http_resp:
             self.status = http_resp.status
             self.reason = http_resp.reason
-            self.body = http_resp.data
+            self.body = http_resp.data.decode("utf-8")
             self.headers = http_resp.getheaders()
         else:
             self.status = status
             self.reason = reason
             self.body = None
             self.headers = None
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/__init__.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/__init__.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/action_menu_fetch_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/action_menu_fetch_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ActionMenuFetchResult(BaseModel):
     """
     ActionMenuFetchResult
-    """
+    """  # noqa: E501
 
     result: Optional[Menu] = None
     __properties: ClassVar[List[str]] = ["result"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict["result"] = self.result.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ActionMenuFetchResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_config.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AdminConfig(BaseModel):
     """
     AdminConfig
-    """
+    """  # noqa: E501
 
     config: Optional[Union[str, Any]] = Field(
         default=None, description="Configuration settings"
     )
     __properties: ClassVar[List[str]] = ["config"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AdminConfig from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_mediation_deny.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_mediation_deny.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AdminMediationDeny(BaseModel):
     """
     AdminMediationDeny
-    """
+    """  # noqa: E501
 
     mediator_terms: Optional[List[StrictStr]] = Field(
         default=None, description="List of mediator rules for recipient"
     )
     recipient_terms: Optional[List[StrictStr]] = Field(
         default=None, description="List of recipient rules for mediation"
     )
@@ -70,15 +70,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AdminMediationDeny from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_modules.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_modules.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AdminModules(BaseModel):
     """
     AdminModules
-    """
+    """  # noqa: E501
 
     result: Optional[List[StrictStr]] = Field(
         default=None, description="List of admin modules"
     )
     __properties: ClassVar[List[str]] = ["result"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AdminModules from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_status.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_status.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AdminStatus(BaseModel):
     """
     AdminStatus
-    """
+    """  # noqa: E501
 
     conductor: Optional[Union[str, Any]] = Field(
         default=None, description="Conductor statistics"
     )
     label: Optional[StrictStr] = Field(default=None, description="Default label")
     timing: Optional[Union[str, Any]] = Field(
         default=None, description="Timing results"
@@ -77,15 +77,15 @@
         # and model_fields_set contains the field
         if self.label is None and "label" in self.model_fields_set:
             _dict["label"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AdminStatus from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_status_liveliness.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_status_liveliness.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AdminStatusLiveliness(BaseModel):
     """
     AdminStatusLiveliness
-    """
+    """  # noqa: E501
 
     alive: Optional[StrictBool] = Field(default=None, description="Liveliness status")
     __properties: ClassVar[List[str]] = ["alive"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AdminStatusLiveliness from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/admin_status_readiness.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/admin_status_readiness.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AdminStatusReadiness(BaseModel):
     """
     AdminStatusReadiness
-    """
+    """  # noqa: E501
 
     ready: Optional[StrictBool] = Field(default=None, description="Readiness status")
     __properties: ClassVar[List[str]] = ["ready"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AdminStatusReadiness from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/aml_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/aml_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AMLRecord(BaseModel):
     """
     AMLRecord
-    """
+    """  # noqa: E501
 
     aml: Optional[Dict[str, StrictStr]] = None
     aml_context: Optional[StrictStr] = Field(default=None, alias="amlContext")
     version: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["aml", "amlContext", "version"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AMLRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AttachDecorator(BaseModel):
     """
     AttachDecorator
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Attachment identifier", alias="@id"
     )
     byte_count: Optional[StrictInt] = Field(
         default=None, description="Byte count of data included by reference"
     )
@@ -111,15 +111,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of data
         if self.data:
             _dict["data"] = self.data.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AttachDecorator from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AttachDecoratorData(BaseModel):
     """
     AttachDecoratorData
-    """
+    """  # noqa: E501
 
     var_base64: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Base64-encoded data", alias="base64"
     )
     var_json: Optional[Union[Dict[str, Any], List[Dict[str, Any]]]] = Field(
         default=None, description="JSON-serialized data", alias="json"
     )
@@ -109,15 +109,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of jws
         if self.jws:
             _dict["jws"] = self.jws.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AttachDecoratorData from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data1_jws.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data1_jws.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AttachDecoratorData1JWS(BaseModel):
     """
     AttachDecoratorData1JWS
-    """
+    """  # noqa: E501
 
     header: AttachDecoratorDataJWSHeader
     protected: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="protected JWS header"
     )
     signature: Annotated[str, Field(strict=True)] = Field(description="signature")
     __properties: ClassVar[List[str]] = ["header", "protected", "signature"]
@@ -94,15 +94,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of header
         if self.header:
             _dict["header"] = self.header.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AttachDecoratorData1JWS from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data_jws.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data_jws.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AttachDecoratorDataJWS(BaseModel):
     """
     AttachDecoratorDataJWS
-    """
+    """  # noqa: E501
 
     header: Optional[AttachDecoratorDataJWSHeader] = None
     protected: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="protected JWS header"
     )
     signature: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="signature"
@@ -117,15 +117,15 @@
             for _item in self.signatures:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["signatures"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AttachDecoratorDataJWS from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attach_decorator_data_jws_header.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attach_decorator_data_jws_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AttachDecoratorDataJWSHeader(BaseModel):
     """
     AttachDecoratorDataJWSHeader
-    """
+    """  # noqa: E501
 
     kid: Annotated[str, Field(strict=True)] = Field(
         description="Key identifier, in W3C did:key or DID URL format"
     )
     __properties: ClassVar[List[str]] = ["kid"]
 
     @field_validator("kid")
@@ -81,15 +81,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AttachDecoratorDataJWSHeader from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attachment_def.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attachment_def.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AttachmentDef(BaseModel):
     """
     AttachmentDef
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(default=None, description="Attachment identifier")
     type: Optional[StrictStr] = Field(default=None, description="Attachment type")
     __properties: ClassVar[List[str]] = ["id", "type"]
 
     @field_validator("type")
     def type_validate_enum(cls, value):
@@ -78,15 +78,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AttachmentDef from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/attribute_mime_types_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/attribute_mime_types_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class AttributeMimeTypesResult(BaseModel):
     """
     AttributeMimeTypesResult
-    """
+    """  # noqa: E501
 
     results: Optional[Dict[str, StrictStr]] = None
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -70,15 +70,15 @@
         # and model_fields_set contains the field
         if self.results is None and "results" in self.model_fields_set:
             _dict["results"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of AttributeMimeTypesResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/claim_format.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/claim_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ClaimFormat(BaseModel):
     """
     ClaimFormat
-    """
+    """  # noqa: E501
 
     jwt: Optional[Union[str, Any]] = None
     jwt_vc: Optional[Union[str, Any]] = None
     jwt_vp: Optional[Union[str, Any]] = None
     ldp: Optional[Union[str, Any]] = None
     ldp_vc: Optional[Union[str, Any]] = None
     ldp_vp: Optional[Union[str, Any]] = None
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ClaimFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/clear_pending_revocations_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/clear_pending_revocations_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ClearPendingRevocationsRequest(BaseModel):
     """
     ClearPendingRevocationsRequest
-    """
+    """  # noqa: E501
 
     purge: Optional[Dict[str, List[Annotated[str, Field(strict=True)]]]] = Field(
         default=None,
         description="Credential revocation ids by revocation registry id: omit for all, specify null or empty list for all pending per revocation registry",
     )
     __properties: ClassVar[List[str]] = ["purge"]
 
@@ -69,15 +69,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ClearPendingRevocationsRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/conn_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/conn_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ConnRecord(BaseModel):
     """
     ConnRecord
-    """
+    """  # noqa: E501
 
     accept: Optional[StrictStr] = Field(
         default=None, description="Connection acceptance: manual or auto"
     )
     alias: Optional[StrictStr] = Field(
         default=None, description="Optional alias to apply to connection for later use"
     )
@@ -277,15 +277,15 @@
                 "rfc23_state",
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ConnRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_invitation.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_invitation.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ConnectionInvitation(BaseModel):
     """
     ConnectionInvitation
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -126,15 +126,15 @@
         # and model_fields_set contains the field
         if self.image_url is None and "image_url" in self.model_fields_set:
             _dict["imageUrl"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ConnectionInvitation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ConnectionList(BaseModel):
     """
     ConnectionList
-    """
+    """  # noqa: E501
 
     results: Optional[List[ConnRecord]] = Field(
         default=None, description="List of connection records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -75,15 +75,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ConnectionList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_metadata.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ConnectionMetadata(BaseModel):
     """
     ConnectionMetadata
-    """
+    """  # noqa: E501
 
     results: Optional[Union[str, Any]] = Field(
         default=None, description="Dictionary of metadata associated with connection."
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ConnectionMetadata from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_metadata_set_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_metadata_set_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ConnectionMetadataSetRequest(BaseModel):
     """
     ConnectionMetadataSetRequest
-    """
+    """  # noqa: E501
 
     metadata: Union[str, Any] = Field(
         description="Dictionary of metadata to set for connection."
     )
     __properties: ClassVar[List[str]] = ["metadata"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ConnectionMetadataSetRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_static_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_static_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ConnectionStaticRequest(BaseModel):
     """
     ConnectionStaticRequest
-    """
+    """  # noqa: E501
 
     alias: Optional[StrictStr] = Field(
         default=None, description="Alias to assign to this connection"
     )
     my_did: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Local DID"
     )
@@ -144,15 +144,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ConnectionStaticRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/connection_static_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/connection_static_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ConnectionStaticResult(BaseModel):
     """
     ConnectionStaticResult
-    """
+    """  # noqa: E501
 
     my_did: Annotated[str, Field(strict=True)] = Field(description="Local DID")
     my_endpoint: Annotated[str, Field(strict=True)] = Field(
         description="My URL endpoint"
     )
     my_verkey: Annotated[str, Field(strict=True)] = Field(
         description="My verification key"
@@ -149,15 +149,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of record
         if self.record:
             _dict["record"] = self.record.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ConnectionStaticResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/constraints.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/constraints.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Constraints(BaseModel):
     """
     Constraints
-    """
+    """  # noqa: E501
 
     fields: Optional[List[DIFField]] = None
     is_holder: Optional[List[DIFHolder]] = None
     limit_disclosure: Optional[StrictStr] = Field(
         default=None, description="LimitDisclosure"
     )
     status_active: Optional[StrictStr] = None
@@ -145,15 +145,15 @@
             for _item in self.is_holder:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["is_holder"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Constraints from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_invitation_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_invitation_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CreateInvitationRequest(BaseModel):
     """
     CreateInvitationRequest
-    """
+    """  # noqa: E501
 
     mediation_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Identifier for active mediation record to be used"
     )
     metadata: Optional[Union[str, Any]] = Field(
         default=None,
         description="Optional metadata to attach to the connection created with the invitation",
@@ -107,15 +107,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CreateInvitationRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CreateWalletRequest(BaseModel):
     """
     CreateWalletRequest
-    """
+    """  # noqa: E501
 
     extra_settings: Optional[Union[str, Any]] = Field(
         default=None, description="Agent config key-value pairs"
     )
     image_url: Optional[StrictStr] = Field(
         default=None,
         description="Image url for this wallet. This image url is publicized            (self-attested) to other agents as part of forming a connection.",
@@ -150,15 +150,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CreateWalletRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CreateWalletResponse(BaseModel):
     """
     CreateWalletResponse
-    """
+    """  # noqa: E501
 
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     key_management_mode: StrictStr = Field(
         description="Mode regarding management of wallet key"
     )
@@ -128,15 +128,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CreateWalletResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_token_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_token_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CreateWalletTokenRequest(BaseModel):
     """
     CreateWalletTokenRequest
-    """
+    """  # noqa: E501
 
     wallet_key: Optional[StrictStr] = Field(
         default=None,
         description="Master key used for key derivation. Only required for             unamanged wallets.",
     )
     __properties: ClassVar[List[str]] = ["wallet_key"]
 
@@ -68,15 +68,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CreateWalletTokenRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/create_wallet_token_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/create_wallet_token_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CreateWalletTokenResponse(BaseModel):
     """
     CreateWalletTokenResponse
-    """
+    """  # noqa: E501
 
     token: Optional[StrictStr] = Field(
         default=None, description="Authorization token to authenticate wallet requests"
     )
     __properties: ClassVar[List[str]] = ["token"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CreateWalletTokenResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_attr_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_attr_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredAttrSpec(BaseModel):
     """
     CredAttrSpec
-    """
+    """  # noqa: E501
 
     mime_type: Optional[StrictStr] = Field(
         default=None,
         description="MIME type: omit for (null) default",
         alias="mime-type",
     )
     name: StrictStr = Field(description="Attribute name")
@@ -78,15 +78,15 @@
         # and model_fields_set contains the field
         if self.mime_type is None and "mime_type" in self.model_fields_set:
             _dict["mime-type"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredAttrSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_def_value.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_def_value.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredDefValue(BaseModel):
     """
     CredDefValue
-    """
+    """  # noqa: E501
 
     primary: Optional[CredDefValuePrimary] = None
     revocation: Optional[CredDefValueRevocation] = None
     __properties: ClassVar[List[str]] = ["primary", "revocation"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -76,15 +76,15 @@
             _dict["primary"] = self.primary.to_dict()
         # override the default output from pydantic by calling `to_dict()` of revocation
         if self.revocation:
             _dict["revocation"] = self.revocation.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredDefValue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_def_value_primary.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_def_value_primary.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredDefValuePrimary(BaseModel):
     """
     CredDefValuePrimary
-    """
+    """  # noqa: E501
 
     n: Optional[Annotated[str, Field(strict=True)]] = None
     r: Optional[Generated] = None
     rctxt: Optional[Annotated[str, Field(strict=True)]] = None
     s: Optional[Annotated[str, Field(strict=True)]] = None
     z: Optional[Annotated[str, Field(strict=True)]] = None
     __properties: ClassVar[List[str]] = ["n", "r", "rctxt", "s", "z"]
@@ -115,15 +115,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of r
         if self.r:
             _dict["r"] = self.r.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredDefValuePrimary from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_def_value_revocation.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_def_value_revocation.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredDefValueRevocation(BaseModel):
     """
     CredDefValueRevocation
-    """
+    """  # noqa: E501
 
     g: Optional[StrictStr] = None
     g_dash: Optional[StrictStr] = None
     h: Optional[StrictStr] = None
     h0: Optional[StrictStr] = None
     h1: Optional[StrictStr] = None
     h2: Optional[StrictStr] = None
@@ -87,15 +87,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredDefValueRevocation from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_info_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_info_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredInfoList(BaseModel):
     """
     CredInfoList
-    """
+    """  # noqa: E501
 
     results: Optional[List[IndyCredInfo]] = None
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -73,15 +73,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredInfoList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_rev_indy_records_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_rev_indy_records_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredRevIndyRecordsResult(BaseModel):
     """
     CredRevIndyRecordsResult
-    """
+    """  # noqa: E501
 
     rev_reg_delta: Optional[Union[str, Any]] = Field(
         default=None, description="Indy revocation registry delta"
     )
     __properties: ClassVar[List[str]] = ["rev_reg_delta"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredRevIndyRecordsResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_rev_record_details_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_rev_record_details_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredRevRecordDetailsResult(BaseModel):
     """
     CredRevRecordDetailsResult
-    """
+    """  # noqa: E501
 
     results: Optional[List[IssuerCredRevRecord]] = None
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -73,15 +73,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredRevRecordDetailsResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_rev_record_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_rev_record_result.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredRevRecordResult(BaseModel):
     """
     CredRevRecordResult
-    """
+    """  # noqa: E501
 
     result: Optional[IssuerCredRevRecord] = None
     __properties: ClassVar[List[str]] = ["result"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict["result"] = self.result.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredRevRecordResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/cred_revoked_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_issued_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,47 +14,49 @@
 
 from __future__ import annotations
 
 import json
 import pprint
 from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, Field, StrictBool
+from pydantic import BaseModel, Field
+from typing_extensions import Annotated
 
 from aries_cloudcontroller.util import DEFAULT_PYDANTIC_MODEL_CONFIG
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class CredRevokedResult(BaseModel):
-    """
-    CredRevokedResult
+class RevRegIssuedResult(BaseModel):
     """
+    RevRegIssuedResult
+    """  # noqa: E501
 
-    revoked: Optional[StrictBool] = Field(
-        default=None, description="Whether credential is revoked on the ledger"
+    result: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(
+        default=None,
+        description="Number of credentials issued against revocation registry",
     )
-    __properties: ClassVar[List[str]] = ["revoked"]
+    __properties: ClassVar[List[str]] = ["result"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of CredRevokedResult from a JSON string"""
+        """Create an instance of RevRegIssuedResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,17 +69,17 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of CredRevokedResult from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of RevRegIssuedResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
-        _obj = cls.model_validate({"revoked": obj.get("revoked")})
+        _obj = cls.model_validate({"result": obj.get("result")})
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Credential(BaseModel):
     """
     Credential
-    """
+    """  # noqa: E501
 
     context: List[Union[str, Dict]] = Field(
         description="The JSON-LD context of the credential", alias="@context"
     )
     credential_subject: Union[str, Any] = Field(alias="credentialSubject")
     expiration_date: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="The expiration date", alias="expirationDate"
@@ -134,15 +134,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of proof
         if self.proof:
             _dict["proof"] = self.proof.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Credential from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialDefinition(BaseModel):
     """
     CredentialDefinition
-    """
+    """  # noqa: E501
 
     id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
     schema_id: Optional[StrictStr] = Field(
         default=None,
         description="Schema identifier within credential definition identifier",
@@ -120,15 +120,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of value
         if self.value:
             _dict["value"] = self.value.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialDefinition from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition_get_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition_get_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialDefinitionGetResult(BaseModel):
     """
     CredentialDefinitionGetResult
-    """
+    """  # noqa: E501
 
     credential_definition: Optional[CredentialDefinition] = None
     __properties: ClassVar[List[str]] = ["credential_definition"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of credential_definition
         if self.credential_definition:
             _dict["credential_definition"] = self.credential_definition.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialDefinitionGetResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition_send_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition_send_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialDefinitionSendRequest(BaseModel):
     """
     CredentialDefinitionSendRequest
-    """
+    """  # noqa: E501
 
     revocation_registry_size: Optional[
         Annotated[int, Field(le=32768, strict=True, ge=4)]
     ] = Field(default=None, description="Revocation registry size")
     schema_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Schema identifier"
     )
@@ -98,15 +98,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialDefinitionSendRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definition_send_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definition_send_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialDefinitionSendResult(BaseModel):
     """
     CredentialDefinitionSendResult
-    """
+    """  # noqa: E501
 
     credential_definition_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
     __properties: ClassVar[List[str]] = ["credential_definition_id"]
 
     @field_validator("credential_definition_id")
@@ -84,15 +84,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialDefinitionSendResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_definitions_created_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_definitions_created_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialDefinitionsCreatedResult(BaseModel):
     """
     CredentialDefinitionsCreatedResult
-    """
+    """  # noqa: E501
 
     credential_definition_ids: Optional[List[Annotated[str, Field(strict=True)]]] = None
     __properties: ClassVar[List[str]] = ["credential_definition_ids"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialDefinitionsCreatedResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_offer.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialOffer(BaseModel):
     """
     CredentialOffer
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -101,15 +101,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialOffer from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_preview.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_preview.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialPreview(BaseModel):
     """
     CredentialPreview
-    """
+    """  # noqa: E501
 
     type: Optional[StrictStr] = Field(
         default=None, description="Message type identifier", alias="@type"
     )
     attributes: List[CredAttrSpec]
     __properties: ClassVar[List[str]] = ["@type", "attributes"]
 
@@ -76,15 +76,15 @@
             for _item in self.attributes:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["attributes"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialPreview from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_proposal.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_proposal.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialProposal(BaseModel):
     """
     CredentialProposal
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -175,15 +175,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialProposal from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/credential_status_options.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/credential_status_options.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class CredentialStatusOptions(BaseModel):
     """
     CredentialStatusOptions
-    """
+    """  # noqa: E501
 
     type: StrictStr = Field(
         description="Credential status method type to use for the credential. Should match status method registered in the Verifiable Credential Extension Registry"
     )
     __properties: ClassVar[List[str]] = ["type"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of CredentialStatusOptions from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DID(BaseModel):
     """
     DID
-    """
+    """  # noqa: E501
 
     did: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="DID of interest"
     )
     key_type: Optional[Literal["ed25519", "bls12381g2"]] = Field(
         default=None, description="Key type associated with the DID"
     )
@@ -138,15 +138,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DID from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_create.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_create.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIDCreate(BaseModel):
     """
     DIDCreate
-    """
+    """  # noqa: E501
 
     method: Optional[StrictStr] = Field(
         default=None,
         description="Method for the requested DID.Supported methods are 'key', 'sov', and any other registered method.",
     )
     options: Optional[DIDCreateOptions] = None
     seed: Optional[StrictStr] = Field(
@@ -77,15 +77,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict["options"] = self.options.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIDCreate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_create_options.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_create_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIDCreateOptions(BaseModel):
     """
     DIDCreateOptions
-    """
+    """  # noqa: E501
 
     did: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None,
         description="Specify final value of the did (including did:<method>: prefix)if the method supports or requires so.",
     )
     key_type: StrictStr = Field(
         description="Key type to use for the DID keypair. Validated with the chosen DID method's supported key types."
@@ -95,15 +95,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIDCreateOptions from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_endpoint.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_endpoint.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIDEndpoint(BaseModel):
     """
     DIDEndpoint
-    """
+    """  # noqa: E501
 
     did: Annotated[str, Field(strict=True)] = Field(description="DID of interest")
     endpoint: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Endpoint to set (omit to delete)"
     )
     __properties: ClassVar[List[str]] = ["did", "endpoint"]
 
@@ -97,15 +97,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIDEndpoint from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_endpoint_with_type.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_endpoint_with_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIDEndpointWithType(BaseModel):
     """
     DIDEndpointWithType
-    """
+    """  # noqa: E501
 
     did: Annotated[str, Field(strict=True)] = Field(description="DID of interest")
     endpoint: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Endpoint to set (omit to delete)"
     )
     endpoint_type: Optional[StrictStr] = Field(
         default=None,
@@ -113,15 +113,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIDEndpointWithType from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIDList(BaseModel):
     """
     DIDList
-    """
+    """  # noqa: E501
 
     results: Optional[List[DID]] = Field(default=None, description="DID list")
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -73,15 +73,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIDList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/did_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_discovery_exchange_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,44 +16,44 @@
 
 import json
 import pprint
 from typing import Any, ClassVar, Dict, List, Optional
 
 from pydantic import BaseModel
 
-from aries_cloudcontroller.models.did import DID
+from aries_cloudcontroller.models.v20_discovery_record import V20DiscoveryRecord
 from aries_cloudcontroller.util import DEFAULT_PYDANTIC_MODEL_CONFIG
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class DIDResult(BaseModel):
-    """
-    DIDResult
+class V20DiscoveryExchangeResult(BaseModel):
     """
+    V20DiscoveryExchangeResult
+    """  # noqa: E501
 
-    result: Optional[DID] = None
-    __properties: ClassVar[List[str]] = ["result"]
+    results: Optional[V20DiscoveryRecord] = None
+    __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of DIDResult from a JSON string"""
+        """Create an instance of V20DiscoveryExchangeResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -63,29 +63,29 @@
           are ignored.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of result
-        if self.result:
-            _dict["result"] = self.result.to_dict()
+        # override the default output from pydantic by calling `to_dict()` of results
+        if self.results:
+            _dict["results"] = self.results.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of DIDResult from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of V20DiscoveryExchangeResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "result": DID.from_dict(obj.get("result"))
-                if obj.get("result") is not None
+                "results": V20DiscoveryRecord.from_dict(obj.get("results"))
+                if obj.get("results") is not None
                 else None
             }
         )
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/didx_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/didx_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIDXRequest(BaseModel):
     """
     DIDXRequest
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -117,15 +117,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of did_docattach
         if self.did_docattach:
             _dict["did_doc~attach"] = self.did_docattach.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIDXRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_field.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_field.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIFField(BaseModel):
     """
     DIFField
-    """
+    """  # noqa: E501
 
     filter: Optional[Filter] = None
     id: Optional[StrictStr] = Field(default=None, description="ID")
     path: Optional[List[StrictStr]] = None
     predicate: Optional[StrictStr] = Field(default=None, description="Preference")
     purpose: Optional[StrictStr] = Field(default=None, description="Purpose")
     __properties: ClassVar[List[str]] = ["filter", "id", "path", "predicate", "purpose"]
@@ -83,15 +83,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of filter
         if self.filter:
             _dict["filter"] = self.filter.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIFField from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_holder.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_holder.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIFHolder(BaseModel):
     """
     DIFHolder
-    """
+    """  # noqa: E501
 
     directive: Optional[StrictStr] = Field(default=None, description="Preference")
     field_id: Optional[List[Annotated[str, Field(strict=True)]]] = None
     __properties: ClassVar[List[str]] = ["directive", "field_id"]
 
     @field_validator("directive")
     def directive_validate_enum(cls, value):
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIFHolder from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_options.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_options.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIFOptions(BaseModel):
     """
     DIFOptions
-    """
+    """  # noqa: E501
 
     challenge: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Challenge protect against replay attack"
     )
     domain: Optional[StrictStr] = Field(
         default=None, description="Domain protect against replay attack"
     )
@@ -87,15 +87,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIFOptions from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_pres_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_pres_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIFPresSpec(BaseModel):
     """
     DIFPresSpec
-    """
+    """  # noqa: E501
 
     issuer_id: Optional[StrictStr] = Field(
         default=None,
         description="Issuer identifier to sign the presentation, if different from current public DID",
     )
     presentation_definition: Optional[PresentationDefinition] = None
     record_ids: Optional[Union[str, Any]] = Field(
@@ -86,15 +86,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of presentation_definition
         if self.presentation_definition:
             _dict["presentation_definition"] = self.presentation_definition.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIFPresSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_proof_proposal.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_proof_proposal.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIFProofProposal(BaseModel):
     """
     DIFProofProposal
-    """
+    """  # noqa: E501
 
     input_descriptors: Optional[List[InputDescriptors]] = None
     options: Optional[DIFOptions] = None
     __properties: ClassVar[List[str]] = ["input_descriptors", "options"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -78,15 +78,15 @@
             _dict["input_descriptors"] = _items
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict["options"] = self.options.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIFProofProposal from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/dif_proof_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/dif_proof_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class DIFProofRequest(BaseModel):
     """
     DIFProofRequest
-    """
+    """  # noqa: E501
 
     options: Optional[DIFOptions] = None
     presentation_definition: PresentationDefinition
     __properties: ClassVar[List[str]] = ["options", "presentation_definition"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["options"] = self.options.to_dict()
         # override the default output from pydantic by calling `to_dict()` of presentation_definition
         if self.presentation_definition:
             _dict["presentation_definition"] = self.presentation_definition.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of DIFProofRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/disclose.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/disclose.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Disclose(BaseModel):
     """
     Disclose
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -84,15 +84,15 @@
             for _item in self.protocols:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["protocols"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Disclose from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/disclosures.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/disclosures.py`

 * *Files 7% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Disclosures(BaseModel):
     """
     Disclosures
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -76,15 +76,15 @@
                 "type",
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Disclosures from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/doc.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/doc.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Doc(BaseModel):
     """
     Doc
-    """
+    """  # noqa: E501
 
     credential: Union[str, Any] = Field(description="Credential to sign")
     options: SignatureOptions
     __properties: ClassVar[List[str]] = ["credential", "options"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -70,15 +70,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict["options"] = self.options.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Doc from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/endorser_info.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/endorser_info.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class EndorserInfo(BaseModel):
     """
     EndorserInfo
-    """
+    """  # noqa: E501
 
     endorser_did: StrictStr = Field(description="Endorser DID")
     endorser_name: Optional[StrictStr] = Field(
         default=None, description="Endorser Name"
     )
     __properties: ClassVar[List[str]] = ["endorser_did", "endorser_name"]
 
@@ -68,15 +68,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of EndorserInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/endpoints_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/endpoints_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class EndpointsResult(BaseModel):
     """
     EndpointsResult
-    """
+    """  # noqa: E501
 
     my_endpoint: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="My endpoint"
     )
     their_endpoint: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Their endpoint"
     )
@@ -102,15 +102,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of EndpointsResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/filter.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Filter(BaseModel):
     """
     Filter
-    """
+    """  # noqa: E501
 
     const: Optional[Union[str, int, float]] = Field(default=None, description="Const")
     enum: Optional[List[Union[str, int, float]]] = None
     exclusive_maximum: Optional[Union[str, int, float]] = Field(
         default=None, description="ExclusiveMaximum", alias="exclusiveMaximum"
     )
     exclusive_minimum: Optional[Union[str, int, float]] = Field(
@@ -101,15 +101,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Filter from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/generated.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/generated.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Generated(BaseModel):
     """
     Generated
-    """
+    """  # noqa: E501
 
     master_secret: Optional[Annotated[str, Field(strict=True)]] = None
     number: Optional[Annotated[str, Field(strict=True)]] = None
     remainder: Optional[Annotated[str, Field(strict=True)]] = None
     __properties: ClassVar[List[str]] = ["master_secret", "number", "remainder"]
 
     @field_validator("master_secret")
@@ -99,15 +99,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Generated from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/get_did_endpoint_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/get_did_endpoint_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class GetDIDEndpointResponse(BaseModel):
     """
     GetDIDEndpointResponse
-    """
+    """  # noqa: E501
 
     endpoint: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Full verification key"
     )
     __properties: ClassVar[List[str]] = ["endpoint"]
 
     @field_validator("endpoint")
@@ -89,15 +89,15 @@
         # and model_fields_set contains the field
         if self.endpoint is None and "endpoint" in self.model_fields_set:
             _dict["endpoint"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of GetDIDEndpointResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/get_did_verkey_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/get_did_verkey_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class GetDIDVerkeyResponse(BaseModel):
     """
     GetDIDVerkeyResponse
-    """
+    """  # noqa: E501
 
     verkey: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Full verification key"
     )
     __properties: ClassVar[List[str]] = ["verkey"]
 
     @field_validator("verkey")
@@ -89,15 +89,15 @@
         # and model_fields_set contains the field
         if self.verkey is None and "verkey" in self.model_fields_set:
             _dict["verkey"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of GetDIDVerkeyResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/get_nym_role_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/get_nym_role_response.py`

 * *Files 8% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class GetNymRoleResponse(BaseModel):
     """
     GetNymRoleResponse
-    """
+    """  # noqa: E501
 
     role: Optional[StrictStr] = Field(default=None, description="Ledger role")
     __properties: ClassVar[List[str]] = ["role"]
 
     @field_validator("role")
     def role_validate_enum(cls, value):
         """Validates the enum"""
@@ -84,15 +84,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of GetNymRoleResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_attr_value.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_attr_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyAttrValue(BaseModel):
     """
     IndyAttrValue
-    """
+    """  # noqa: E501
 
     encoded: Annotated[str, Field(strict=True)] = Field(
         description="Attribute encoded value"
     )
     raw: StrictStr = Field(description="Attribute raw value")
     __properties: ClassVar[List[str]] = ["encoded", "raw"]
 
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyAttrValue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_abstract.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_abstract.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyCredAbstract(BaseModel):
     """
     IndyCredAbstract
-    """
+    """  # noqa: E501
 
     cred_def_id: Annotated[str, Field(strict=True)] = Field(
         description="Credential definition identifier"
     )
     key_correctness_proof: IndyKeyCorrectnessProof
     nonce: Annotated[str, Field(strict=True)] = Field(
         description="Nonce in credential abstract"
@@ -118,15 +118,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of key_correctness_proof
         if self.key_correctness_proof:
             _dict["key_correctness_proof"] = self.key_correctness_proof.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyCredAbstract from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_info.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyCredInfo(BaseModel):
     """
     IndyCredInfo
-    """
+    """  # noqa: E501
 
     attrs: Optional[Dict[str, StrictStr]] = Field(
         default=None, description="Attribute names and value"
     )
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
@@ -154,15 +154,15 @@
         # and model_fields_set contains the field
         if self.rev_reg_id is None and "rev_reg_id" in self.model_fields_set:
             _dict["rev_reg_id"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyCredInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_precis.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_precis.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyCredPrecis(BaseModel):
     """
     IndyCredPrecis
-    """
+    """  # noqa: E501
 
     cred_info: Optional[IndyCredInfo] = None
     interval: Optional[IndyNonRevocationInterval] = None
     presentation_referents: Optional[List[StrictStr]] = None
     __properties: ClassVar[List[str]] = [
         "cred_info",
         "interval",
@@ -81,15 +81,15 @@
             _dict["cred_info"] = self.cred_info.to_dict()
         # override the default output from pydantic by calling `to_dict()` of interval
         if self.interval:
             _dict["interval"] = self.interval.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyCredPrecis from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_cred_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_cred_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyCredRequest(BaseModel):
     """
     IndyCredRequest
-    """
+    """  # noqa: E501
 
     blinded_ms: Union[str, Any] = Field(description="Blinded master secret")
     blinded_ms_correctness_proof: Union[str, Any] = Field(
         description="Blinded master secret correctness proof"
     )
     cred_def_id: Annotated[str, Field(strict=True)] = Field(
         description="Credential definition identifier"
@@ -114,15 +114,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyCredRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_credential.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_credential.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyCredential(BaseModel):
     """
     IndyCredential
-    """
+    """  # noqa: E501
 
     cred_def_id: Annotated[str, Field(strict=True)] = Field(
         description="Credential definition identifier"
     )
     rev_reg: Optional[Union[str, Any]] = Field(
         default=None, description="Revocation registry state"
     )
@@ -157,15 +157,15 @@
         # and model_fields_set contains the field
         if self.witness is None and "witness" in self.model_fields_set:
             _dict["witness"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyCredential from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_eq_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_eq_proof.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyEQProof(BaseModel):
     """
     IndyEQProof
-    """
+    """  # noqa: E501
 
     a_prime: Optional[Annotated[str, Field(strict=True)]] = None
     e: Optional[Annotated[str, Field(strict=True)]] = None
     m: Optional[Dict[str, Annotated[str, Field(strict=True)]]] = None
     m2: Optional[Annotated[str, Field(strict=True)]] = None
     revealed_attrs: Optional[Dict[str, Annotated[str, Field(strict=True)]]] = None
     v: Optional[Annotated[str, Field(strict=True)]] = None
@@ -119,15 +119,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyEQProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_ge_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_ge_proof.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyGEProof(BaseModel):
     """
     IndyGEProof
-    """
+    """  # noqa: E501
 
     alpha: Optional[Annotated[str, Field(strict=True)]] = None
     mj: Optional[Annotated[str, Field(strict=True)]] = None
     predicate: Optional[IndyGEProofPred] = None
     r: Optional[Dict[str, Annotated[str, Field(strict=True)]]] = None
     t: Optional[Dict[str, Annotated[str, Field(strict=True)]]] = None
     u: Optional[Dict[str, Annotated[str, Field(strict=True)]]] = None
@@ -96,15 +96,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of predicate
         if self.predicate:
             _dict["predicate"] = self.predicate.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyGEProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_ge_proof_pred.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_ge_proof_pred.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyGEProofPred(BaseModel):
     """
     IndyGEProofPred
-    """
+    """  # noqa: E501
 
     attr_name: Optional[StrictStr] = Field(
         default=None, description="Attribute name, indy-canonicalized"
     )
     p_type: Optional[StrictStr] = Field(default=None, description="Predicate type")
     value: Optional[StrictInt] = Field(
         default=None, description="Predicate threshold value"
@@ -81,15 +81,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyGEProofPred from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_key_correctness_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_key_correctness_proof.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyKeyCorrectnessProof(BaseModel):
     """
     IndyKeyCorrectnessProof
-    """
+    """  # noqa: E501
 
     c: Annotated[str, Field(strict=True)] = Field(
         description="c in key correctness proof"
     )
     xr_cap: List[List[StrictStr]] = Field(description="xr_cap in key correctness proof")
     xz_cap: Annotated[str, Field(strict=True)] = Field(
         description="xz_cap in key correctness proof"
@@ -87,15 +87,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyKeyCorrectnessProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_non_revoc_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_non_revoc_proof.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyNonRevocProof(BaseModel):
     """
     IndyNonRevocProof
-    """
+    """  # noqa: E501
 
     c_list: Optional[Dict[str, StrictStr]] = None
     x_list: Optional[Dict[str, StrictStr]] = None
     __properties: ClassVar[List[str]] = ["c_list", "x_list"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyNonRevocProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_non_revocation_interval.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_non_revocation_interval.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyNonRevocationInterval(BaseModel):
     """
     IndyNonRevocationInterval
-    """
+    """  # noqa: E501
 
     var_from: Optional[
         Annotated[int, Field(le=18446744073709551615, strict=True, ge=0)]
     ] = Field(
         default=None,
         description="Earliest time of interest in non-revocation interval",
         alias="from",
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyNonRevocationInterval from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_attr_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_attr_spec.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyPresAttrSpec(BaseModel):
     """
     IndyPresAttrSpec
-    """
+    """  # noqa: E501
 
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = None
     mime_type: Optional[StrictStr] = Field(
         default=None, description="MIME type (default null)", alias="mime-type"
     )
     name: StrictStr = Field(description="Attribute name")
     referent: Optional[StrictStr] = Field(
@@ -96,15 +96,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyPresAttrSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_pred_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_pred_spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyPresPredSpec(BaseModel):
     """
     IndyPresPredSpec
-    """
+    """  # noqa: E501
 
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
     name: StrictStr = Field(description="Attribute name")
     predicate: StrictStr = Field(description="Predicate type ('<', '<=', '>=', or '>')")
     threshold: StrictInt = Field(description="Threshold value")
@@ -99,15 +99,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyPresPredSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_preview.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_preview.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyPresPreview(BaseModel):
     """
     IndyPresPreview
-    """
+    """  # noqa: E501
 
     type: Optional[StrictStr] = Field(
         default=None, description="Message type identifier", alias="@type"
     )
     attributes: List[IndyPresAttrSpec]
     predicates: List[IndyPresPredSpec]
     __properties: ClassVar[List[str]] = ["@type", "attributes", "predicates"]
@@ -85,15 +85,15 @@
             for _item in self.predicates:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["predicates"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyPresPreview from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_pres_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_pres_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyPresSpec(BaseModel):
     """
     IndyPresSpec
-    """
+    """  # noqa: E501
 
     requested_attributes: Dict[str, IndyRequestedCredsRequestedAttr] = Field(
         description="Nested object mapping proof request attribute referents to requested-attribute specifiers"
     )
     requested_predicates: Dict[str, IndyRequestedCredsRequestedPred] = Field(
         description="Nested object mapping proof request predicate referents to requested-predicate specifiers"
     )
@@ -101,15 +101,15 @@
             for _key in self.requested_predicates:
                 if self.requested_predicates[_key]:
                     _field_dict[_key] = self.requested_predicates[_key].to_dict()
             _dict["requested_predicates"] = _field_dict
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyPresSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_primary_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_primary_proof.py`

 * *Files 4% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyPrimaryProof(BaseModel):
     """
     IndyPrimaryProof
-    """
+    """  # noqa: E501
 
     eq_proof: Optional[IndyPrimaryProofEqProof] = None
     ge_proofs: Optional[List[IndyGEProof]] = Field(
         default=None, description="Indy GE proofs"
     )
     __properties: ClassVar[List[str]] = ["eq_proof", "ge_proofs"]
 
@@ -92,15 +92,15 @@
         # and model_fields_set contains the field
         if self.ge_proofs is None and "ge_proofs" in self.model_fields_set:
             _dict["ge_proofs"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyPrimaryProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_primary_proof_eq_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_primary_proof_eq_proof.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,16 +28,16 @@
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyPrimaryProofEqProof(BaseModel):
     """
-    Indy equality proof  # noqa: E501
-    """
+    Indy equality proof
+    """  # noqa: E501
 
     a_prime: Optional[Annotated[str, Field(strict=True)]] = None
     e: Optional[Annotated[str, Field(strict=True)]] = None
     m: Optional[Dict[str, Annotated[str, Field(strict=True)]]] = None
     m2: Optional[Annotated[str, Field(strict=True)]] = None
     revealed_attrs: Optional[Dict[str, Annotated[str, Field(strict=True)]]] = None
     v: Optional[Annotated[str, Field(strict=True)]] = None
@@ -119,15 +119,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyPrimaryProofEqProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProof(BaseModel):
     """
     IndyProof
-    """
+    """  # noqa: E501
 
     identifiers: Optional[List[IndyProofIdentifier]] = Field(
         default=None, description="Indy proof.identifiers content"
     )
     proof: Optional[IndyProofProof] = None
     requested_proof: Optional[IndyProofRequestedProof] = None
     __properties: ClassVar[List[str]] = ["identifiers", "proof", "requested_proof"]
@@ -87,15 +87,15 @@
             _dict["proof"] = self.proof.to_dict()
         # override the default output from pydantic by calling `to_dict()` of requested_proof
         if self.requested_proof:
             _dict["requested_proof"] = self.requested_proof.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_identifier.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_identifier.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofIdentifier(BaseModel):
     """
     IndyProofIdentifier
-    """
+    """  # noqa: E501
 
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
     rev_reg_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Revocation registry identifier"
     )
@@ -138,15 +138,15 @@
         # and model_fields_set contains the field
         if self.timestamp is None and "timestamp" in self.model_fields_set:
             _dict["timestamp"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofIdentifier from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofProof(BaseModel):
     """
     IndyProofProof
-    """
+    """  # noqa: E501
 
     aggregated_proof: Optional[IndyProofProofAggregatedProof] = None
     proofs: Optional[List[IndyProofProofProofsProof]] = Field(
         default=None, description="Indy proof proofs"
     )
     __properties: ClassVar[List[str]] = ["aggregated_proof", "proofs"]
 
@@ -84,15 +84,15 @@
             for _item in self.proofs:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["proofs"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof_aggregated_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof_aggregated_proof.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofProofAggregatedProof(BaseModel):
     """
     IndyProofProofAggregatedProof
-    """
+    """  # noqa: E501
 
     c_hash: Optional[StrictStr] = Field(default=None, description="c_hash value")
     c_list: Optional[List[List[StrictInt]]] = Field(
         default=None, description="c_list value"
     )
     __properties: ClassVar[List[str]] = ["c_hash", "c_list"]
 
@@ -68,15 +68,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofProofAggregatedProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof_proofs_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof_proofs_proof.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofProofProofsProof(BaseModel):
     """
     IndyProofProofProofsProof
-    """
+    """  # noqa: E501
 
     non_revoc_proof: Optional[IndyProofProofProofsProofNonRevocProof] = None
     primary_proof: Optional[IndyPrimaryProof] = None
     __properties: ClassVar[List[str]] = ["non_revoc_proof", "primary_proof"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -81,15 +81,15 @@
         # and model_fields_set contains the field
         if self.non_revoc_proof is None and "non_revoc_proof" in self.model_fields_set:
             _dict["non_revoc_proof"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofProofProofsProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_proof_proofs_proof_non_revoc_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_proof_proofs_proof_non_revoc_proof.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,16 +26,16 @@
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofProofProofsProofNonRevocProof(BaseModel):
     """
-    Indy non-revocation proof  # noqa: E501
-    """
+    Indy non-revocation proof
+    """  # noqa: E501
 
     c_list: Optional[Dict[str, StrictStr]] = None
     x_list: Optional[Dict[str, StrictStr]] = None
     __properties: ClassVar[List[str]] = ["c_list", "x_list"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofProofProofsProofNonRevocProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_attr_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_attr_spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofReqAttrSpec(BaseModel):
     """
     IndyProofReqAttrSpec
-    """
+    """  # noqa: E501
 
     name: Optional[StrictStr] = Field(default=None, description="Attribute name")
     names: Optional[List[StrictStr]] = Field(
         default=None, description="Attribute name group"
     )
     non_revoked: Optional[IndyProofReqAttrSpecNonRevoked] = None
     restrictions: Optional[List[Dict[str, StrictStr]]] = Field(
@@ -84,15 +84,15 @@
         # and model_fields_set contains the field
         if self.non_revoked is None and "non_revoked" in self.model_fields_set:
             _dict["non_revoked"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofReqAttrSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_attr_spec_non_revoked.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_attr_spec_non_revoked.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofReqAttrSpecNonRevoked(BaseModel):
     """
     IndyProofReqAttrSpecNonRevoked
-    """
+    """  # noqa: E501
 
     var_from: Optional[
         Annotated[int, Field(le=18446744073709551615, strict=True, ge=0)]
     ] = Field(
         default=None,
         description="Earliest time of interest in non-revocation interval",
         alias="from",
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofReqAttrSpecNonRevoked from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_pred_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_pred_spec.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofReqPredSpec(BaseModel):
     """
     IndyProofReqPredSpec
-    """
+    """  # noqa: E501
 
     name: StrictStr = Field(description="Attribute name")
     non_revoked: Optional[IndyProofReqPredSpecNonRevoked] = None
     p_type: StrictStr = Field(description="Predicate type ('<', '<=', '>=', or '>')")
     p_value: StrictInt = Field(description="Threshold value")
     restrictions: Optional[List[Dict[str, StrictStr]]] = Field(
         default=None,
@@ -96,15 +96,15 @@
         # and model_fields_set contains the field
         if self.non_revoked is None and "non_revoked" in self.model_fields_set:
             _dict["non_revoked"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofReqPredSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_req_pred_spec_non_revoked.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_req_pred_spec_non_revoked.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofReqPredSpecNonRevoked(BaseModel):
     """
     IndyProofReqPredSpecNonRevoked
-    """
+    """  # noqa: E501
 
     var_from: Optional[
         Annotated[int, Field(le=18446744073709551615, strict=True, ge=0)]
     ] = Field(
         default=None,
         description="Earliest time of interest in non-revocation interval",
         alias="from",
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofReqPredSpecNonRevoked from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofRequest(BaseModel):
     """
     IndyProofRequest
-    """
+    """  # noqa: E501
 
     name: Optional[StrictStr] = Field(default=None, description="Proof request name")
     non_revoked: Optional[IndyProofRequestNonRevoked] = None
     nonce: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Nonce"
     )
     requested_attributes: Dict[str, IndyProofReqAttrSpec] = Field(
@@ -134,15 +134,15 @@
         # and model_fields_set contains the field
         if self.non_revoked is None and "non_revoked" in self.model_fields_set:
             _dict["non_revoked"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_request_non_revoked.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_request_non_revoked.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofRequestNonRevoked(BaseModel):
     """
     IndyProofRequestNonRevoked
-    """
+    """  # noqa: E501
 
     var_from: Optional[
         Annotated[int, Field(le=18446744073709551615, strict=True, ge=0)]
     ] = Field(
         default=None,
         description="Earliest time of interest in non-revocation interval",
         alias="from",
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofRequestNonRevoked from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofRequestedProof(BaseModel):
     """
     IndyProofRequestedProof
-    """
+    """  # noqa: E501
 
     predicates: Optional[Dict[str, IndyProofRequestedProofPredicate]] = Field(
         default=None, description="Proof requested proof predicates."
     )
     revealed_attr_groups: Optional[
         Dict[str, IndyProofRequestedProofRevealedAttrGroup]
     ] = Field(
@@ -130,15 +130,15 @@
         # and model_fields_set contains the field
         if self.revealed_attrs is None and "revealed_attrs" in self.model_fields_set:
             _dict["revealed_attrs"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofRequestedProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof_predicate.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof_predicate.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofRequestedProofPredicate(BaseModel):
     """
     IndyProofRequestedProofPredicate
-    """
+    """  # noqa: E501
 
     sub_proof_index: Optional[StrictInt] = Field(
         default=None, description="Sub-proof index"
     )
     __properties: ClassVar[List[str]] = ["sub_proof_index"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofRequestedProofPredicate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofRequestedProofRevealedAttr(BaseModel):
     """
     IndyProofRequestedProofRevealedAttr
-    """
+    """  # noqa: E501
 
     encoded: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Encoded value"
     )
     raw: Optional[StrictStr] = Field(default=None, description="Raw value")
     sub_proof_index: Optional[StrictInt] = Field(
         default=None, description="Sub-proof index"
@@ -83,15 +83,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofRequestedProofRevealedAttr from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr_group.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_proof_requested_proof_revealed_attr_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyProofRequestedProofRevealedAttrGroup(BaseModel):
     """
     IndyProofRequestedProofRevealedAttrGroup
-    """
+    """  # noqa: E501
 
     sub_proof_index: Optional[StrictInt] = Field(
         default=None, description="Sub-proof index"
     )
     values: Optional[Dict[str, RawEncoded]] = Field(
         default=None,
         description="Indy proof requested proof revealed attr groups group value",
@@ -79,15 +79,15 @@
             for _key in self.values:
                 if self.values[_key]:
                     _field_dict[_key] = self.values[_key].to_dict()
             _dict["values"] = _field_dict
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyProofRequestedProofRevealedAttrGroup from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_requested_creds_requested_attr.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_requested_creds_requested_attr.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRequestedCredsRequestedAttr(BaseModel):
     """
     IndyRequestedCredsRequestedAttr
-    """
+    """  # noqa: E501
 
     cred_id: StrictStr = Field(
         description="Wallet credential identifier (typically but not necessarily a UUID)"
     )
     revealed: Optional[StrictBool] = Field(
         default=None, description="Whether to reveal attribute in proof (default true)"
     )
@@ -70,15 +70,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRequestedCredsRequestedAttr from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_requested_creds_requested_pred.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_requested_creds_requested_pred.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRequestedCredsRequestedPred(BaseModel):
     """
     IndyRequestedCredsRequestedPred
-    """
+    """  # noqa: E501
 
     cred_id: StrictStr = Field(
         description="Wallet credential identifier (typically but not necessarily a UUID)"
     )
     timestamp: Optional[
         Annotated[int, Field(le=18446744073709551615, strict=True, ge=0)]
     ] = Field(
@@ -73,15 +73,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRequestedCredsRequestedPred from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRevRegDef(BaseModel):
     """
     IndyRevRegDef
-    """
+    """  # noqa: E501
 
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier", alias="credDefId"
     )
     id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Indy revocation registry identifier"
     )
@@ -145,15 +145,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of value
         if self.value:
             _dict["value"] = self.value.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRevRegDef from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def_value.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def_value.py`

 * *Files 4% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRevRegDefValue(BaseModel):
     """
     IndyRevRegDefValue
-    """
+    """  # noqa: E501
 
     issuance_type: Optional[StrictStr] = Field(
         default=None, description="Issuance type", alias="issuanceType"
     )
     max_cred_num: Optional[Annotated[int, Field(strict=True, ge=1)]] = Field(
         default=None,
         description="Maximum number of credentials; registry size",
@@ -122,15 +122,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of public_keys
         if self.public_keys:
             _dict["publicKeys"] = self.public_keys.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRevRegDefValue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRevRegDefValuePublicKeys(BaseModel):
     """
     IndyRevRegDefValuePublicKeys
-    """
+    """  # noqa: E501
 
     accum_key: Optional[IndyRevRegDefValuePublicKeysAccumKey] = Field(
         default=None, alias="accumKey"
     )
     __properties: ClassVar[List[str]] = ["accumKey"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -73,15 +73,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of accum_key
         if self.accum_key:
             _dict["accumKey"] = self.accum_key.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRevRegDefValuePublicKeys from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys_accum_key.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_def_value_public_keys_accum_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRevRegDefValuePublicKeysAccumKey(BaseModel):
     """
     IndyRevRegDefValuePublicKeysAccumKey
-    """
+    """  # noqa: E501
 
     z: Optional[StrictStr] = Field(default=None, description="Value for z")
     __properties: ClassVar[List[str]] = ["z"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRevRegDefValuePublicKeysAccumKey from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_entry.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_entry.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRevRegEntry(BaseModel):
     """
     IndyRevRegEntry
-    """
+    """  # noqa: E501
 
     value: Optional[IndyRevRegEntryValue] = None
     ver: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Version of revocation registry entry"
     )
     __properties: ClassVar[List[str]] = ["value", "ver"]
 
@@ -84,15 +84,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of value
         if self.value:
             _dict["value"] = self.value.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRevRegEntry from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/indy_rev_reg_entry_value.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/indy_rev_reg_entry_value.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IndyRevRegEntryValue(BaseModel):
     """
     IndyRevRegEntryValue
-    """
+    """  # noqa: E501
 
     accum: Optional[StrictStr] = Field(default=None, description="Accumulator value")
     prev_accum: Optional[StrictStr] = Field(
         default=None, description="Previous accumulator value", alias="prevAccum"
     )
     revoked: Optional[List[StrictInt]] = Field(
         default=None, description="Revoked credential revocation identifiers"
@@ -71,15 +71,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IndyRevRegEntryValue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/input_descriptors.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/input_descriptors.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class InputDescriptors(BaseModel):
     """
     InputDescriptors
-    """
+    """  # noqa: E501
 
     constraints: Optional[Constraints] = None
     group: Optional[List[StrictStr]] = None
     id: Optional[StrictStr] = Field(default=None, description="ID")
     metadata: Optional[Union[str, Any]] = Field(
         default=None, description="Metadata dictionary"
     )
@@ -93,15 +93,15 @@
             _dict["constraints"] = self.constraints.to_dict()
         # override the default output from pydantic by calling `to_dict()` of var_schema
         if self.var_schema:
             _dict["schema"] = self.var_schema.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of InputDescriptors from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_create_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class InvitationCreateRequest(BaseModel):
     """
     InvitationCreateRequest
-    """
+    """  # noqa: E501
 
     accept: Optional[List[StrictStr]] = Field(
         default=None,
         description="List of mime type in order of preference that should be use in responding to the message",
     )
     alias: Optional[StrictStr] = Field(default=None, description="Alias for connection")
     attachments: Optional[List[AttachmentDef]] = Field(
@@ -134,15 +134,15 @@
             for _item in self.attachments:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["attachments"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of InvitationCreateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_message.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_message.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class InvitationMessage(BaseModel):
     """
     InvitationMessage
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -116,15 +116,15 @@
         # and model_fields_set contains the field
         if self.image_url is None and "image_url" in self.model_fields_set:
             _dict["imageUrl"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of InvitationMessage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class InvitationRecord(BaseModel):
     """
     InvitationRecord
-    """
+    """  # noqa: E501
 
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     invi_msg_id: Optional[StrictStr] = Field(
         default=None, description="Invitation message identifier"
     )
@@ -136,15 +136,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of invitation
         if self.invitation:
             _dict["invitation"] = self.invitation.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of InvitationRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/invitation_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/invitation_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class InvitationResult(BaseModel):
     """
     InvitationResult
-    """
+    """  # noqa: E501
 
     connection_id: Optional[StrictStr] = Field(
         default=None, description="Connection identifier"
     )
     invitation: Optional[ConnectionInvitation] = None
     invitation_url: Optional[StrictStr] = Field(
         default=None, description="Invitation URL"
@@ -79,15 +79,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of invitation
         if self.invitation:
             _dict["invitation"] = self.invitation.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of InvitationResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/issuer_cred_rev_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/issuer_cred_rev_record.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IssuerCredRevRecord(BaseModel):
     """
     IssuerCredRevRecord
-    """
+    """  # noqa: E501
 
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
@@ -174,15 +174,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IssuerCredRevRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/issuer_rev_reg_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/issuer_rev_reg_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class IssuerRevRegRecord(BaseModel):
     """
     IssuerRevRegRecord
-    """
+    """  # noqa: E501
 
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
@@ -239,15 +239,15 @@
             _dict["revoc_reg_def"] = self.revoc_reg_def.to_dict()
         # override the default output from pydantic by calling `to_dict()` of revoc_reg_entry
         if self.revoc_reg_entry:
             _dict["revoc_reg_entry"] = self.revoc_reg_entry.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of IssuerRevRegRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/jws_create.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/jws_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class JWSCreate(BaseModel):
     """
     JWSCreate
-    """
+    """  # noqa: E501
 
     did: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="DID of interest"
     )
     headers: Optional[Union[str, Any]] = None
     payload: Union[str, Any]
     verification_method: Optional[Annotated[str, Field(strict=True)]] = Field(
@@ -108,15 +108,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of JWSCreate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/jws_verify.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/jws_verify.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class JWSVerify(BaseModel):
     """
     JWSVerify
-    """
+    """  # noqa: E501
 
     jwt: Optional[Annotated[str, Field(strict=True)]] = None
     __properties: ClassVar[List[str]] = ["jwt"]
 
     @field_validator("jwt")
     def jwt_validate_regular_expression(cls, value):
         """Validates the regular expression"""
@@ -79,15 +79,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of JWSVerify from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/jws_verify_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/jws_verify_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class JWSVerifyResponse(BaseModel):
     """
     JWSVerifyResponse
-    """
+    """  # noqa: E501
 
     error: Optional[StrictStr] = Field(default=None, description="Error text")
     headers: Union[str, Any] = Field(description="Headers from verified JWT.")
     kid: StrictStr = Field(description="kid of signer")
     payload: Union[str, Any] = Field(description="Payload from verified JWT")
     valid: StrictBool
     __properties: ClassVar[List[str]] = ["error", "headers", "kid", "payload", "valid"]
@@ -69,15 +69,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of JWSVerifyResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Keylist(BaseModel):
     """
     Keylist
-    """
+    """  # noqa: E501
 
     results: Optional[List[RouteRecord]] = Field(
         default=None, description="List of keylist records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -75,15 +75,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Keylist from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_query.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_query.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class KeylistQuery(BaseModel):
     """
     KeylistQuery
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -81,15 +81,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of paginate
         if self.paginate:
             _dict["paginate"] = self.paginate.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of KeylistQuery from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_query_filter_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_query_filter_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class KeylistQueryFilterRequest(BaseModel):
     """
     KeylistQueryFilterRequest
-    """
+    """  # noqa: E501
 
     filter: Optional[Union[str, Any]] = Field(
         default=None, description="Filter for keylist query"
     )
     __properties: ClassVar[List[str]] = ["filter"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of KeylistQueryFilterRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_query_paginate.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_query_paginate.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class KeylistQueryPaginate(BaseModel):
     """
     KeylistQueryPaginate
-    """
+    """  # noqa: E501
 
     limit: Optional[StrictInt] = Field(
         default=None, description="Limit for keylist query"
     )
     offset: Optional[StrictInt] = Field(
         default=None, description="Offset value for query"
     )
@@ -70,15 +70,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of KeylistQueryPaginate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_update.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_update.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class KeylistUpdate(BaseModel):
     """
     KeylistUpdate
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -84,15 +84,15 @@
             for _item in self.updates:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["updates"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of KeylistUpdate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_update_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_update_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class KeylistUpdateRequest(BaseModel):
     """
     KeylistUpdateRequest
-    """
+    """  # noqa: E501
 
     updates: Optional[List[KeylistUpdateRule]] = None
     __properties: ClassVar[List[str]] = ["updates"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -73,15 +73,15 @@
             for _item in self.updates:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["updates"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of KeylistUpdateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/keylist_update_rule.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/keylist_update_rule.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class KeylistUpdateRule(BaseModel):
     """
     KeylistUpdateRule
-    """
+    """  # noqa: E501
 
     action: StrictStr = Field(description="Action for specific key")
     recipient_key: Annotated[str, Field(strict=True)] = Field(
         description="Key to remove or add"
     )
     __properties: ClassVar[List[str]] = ["action", "recipient_key"]
 
@@ -89,15 +89,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of KeylistUpdateRule from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ld_proof_vc_detail.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ld_proof_vc_detail.py`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class LDProofVCDetail(BaseModel):
     """
     LDProofVCDetail
-    """
+    """  # noqa: E501
 
     credential: Credential
     options: LDProofVCDetailOptions
     __properties: ClassVar[List[str]] = ["credential", "options"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -76,15 +76,15 @@
             _dict["credential"] = self.credential.to_dict()
         # override the default output from pydantic by calling `to_dict()` of options
         if self.options:
             _dict["options"] = self.options.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of LDProofVCDetail from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ld_proof_vc_detail_options.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ld_proof_vc_detail_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class LDProofVCDetailOptions(BaseModel):
     """
     LDProofVCDetailOptions
-    """
+    """  # noqa: E501
 
     challenge: Optional[StrictStr] = Field(
         default=None,
         description="A challenge to include in the proof. SHOULD be provided by the requesting party of the credential (=holder)",
     )
     created: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None,
@@ -117,15 +117,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of credential_status
         if self.credential_status:
             _dict["credentialStatus"] = self.credential_status.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of LDProofVCDetailOptions from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ledger_config_instance.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ledger_config_instance.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class LedgerConfigInstance(BaseModel):
     """
     LedgerConfigInstance
-    """
+    """  # noqa: E501
 
     genesis_file: Optional[StrictStr] = Field(default=None, description="genesis_file")
     genesis_transactions: Optional[StrictStr] = Field(
         default=None, description="genesis_transactions"
     )
     genesis_url: Optional[StrictStr] = Field(default=None, description="genesis_url")
     id: Optional[StrictStr] = Field(default=None, description="ledger_id")
@@ -79,15 +79,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of LedgerConfigInstance from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ledger_config_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ledger_config_list.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class LedgerConfigList(BaseModel):
     """
     LedgerConfigList
-    """
+    """  # noqa: E501
 
     ledger_config_list: List[LedgerConfigInstance]
     __properties: ClassVar[List[str]] = ["ledger_config_list"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -73,15 +73,15 @@
             for _item in self.ledger_config_list:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["ledger_config_list"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of LedgerConfigList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/linked_data_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/linked_data_proof.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class LinkedDataProof(BaseModel):
     """
     LinkedDataProof
-    """
+    """  # noqa: E501
 
     challenge: Optional[StrictStr] = Field(
         default=None,
         description="Associates a challenge with a proof, for use with a proofPurpose such as authentication",
     )
     created: Annotated[str, Field(strict=True)] = Field(
         description="The string value of an ISO8601 combined date and time string generated by the Signature Algorithm"
@@ -136,15 +136,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of LinkedDataProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_create_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_create_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MediationCreateRequest(BaseModel):
     """
     MediationCreateRequest
-    """
+    """  # noqa: E501
 
     mediator_terms: Optional[List[StrictStr]] = Field(
         default=None, description="List of mediator rules for recipient"
     )
     recipient_terms: Optional[List[StrictStr]] = Field(
         default=None, description="List of recipient rules for mediation"
     )
@@ -70,15 +70,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MediationCreateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_deny.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_deny.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MediationDeny(BaseModel):
     """
     MediationDeny
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -80,15 +80,15 @@
                 "type",
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MediationDeny from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_grant.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_grant.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MediationGrant(BaseModel):
     """
     MediationGrant
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -78,15 +78,15 @@
                 "type",
             },
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MediationGrant from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_id_match_info.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_id_match_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MediationIdMatchInfo(BaseModel):
     """
     MediationIdMatchInfo
-    """
+    """  # noqa: E501
 
     mediation_id: Optional[StrictStr] = Field(
         default=None, description="Mediation record identifier"
     )
     __properties: ClassVar[List[str]] = ["mediation_id"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MediationIdMatchInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MediationList(BaseModel):
     """
     MediationList
-    """
+    """  # noqa: E501
 
     results: Optional[List[MediationRecord]] = Field(
         default=None, description="List of mediation records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -75,15 +75,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MediationList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/mediation_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/mediation_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MediationRecord(BaseModel):
     """
     MediationRecord
-    """
+    """  # noqa: E501
 
     connection_id: StrictStr
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     endpoint: Optional[StrictStr] = None
     mediation_id: Optional[StrictStr] = None
@@ -121,15 +121,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MediationRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Menu(BaseModel):
     """
     Menu
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -96,15 +96,15 @@
             for _item in self.options:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["options"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Menu from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_form.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MenuForm(BaseModel):
     """
     MenuForm
-    """
+    """  # noqa: E501
 
     description: Optional[StrictStr] = Field(
         default=None, description="Additional descriptive text for menu form"
     )
     params: Optional[List[MenuFormParam]] = Field(
         default=None, description="List of form parameters"
     )
@@ -89,15 +89,15 @@
             for _item in self.params:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["params"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MenuForm from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_form_param.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_form_param.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MenuFormParam(BaseModel):
     """
     MenuFormParam
-    """
+    """  # noqa: E501
 
     default: Optional[StrictStr] = Field(
         default=None, description="Default parameter value"
     )
     description: Optional[StrictStr] = Field(
         default=None, description="Additional descriptive text for menu form parameter"
     )
@@ -85,15 +85,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MenuFormParam from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_json.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_json.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MenuJson(BaseModel):
     """
     MenuJson
-    """
+    """  # noqa: E501
 
     description: Optional[StrictStr] = Field(
         default=None, description="Introductory text for the menu"
     )
     errormsg: Optional[StrictStr] = Field(
         default=None, description="Optional error message to display in menu header"
     )
@@ -80,15 +80,15 @@
             for _item in self.options:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["options"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MenuJson from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/menu_option.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/menu_option.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class MenuOption(BaseModel):
     """
     MenuOption
-    """
+    """  # noqa: E501
 
     description: Optional[StrictStr] = Field(
         default=None, description="Additional descriptive text for menu option"
     )
     disabled: Optional[StrictBool] = Field(
         default=None, description="Whether to show option as disabled"
     )
@@ -83,15 +83,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of form
         if self.form:
             _dict["form"] = self.form.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of MenuOption from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/model_date.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/model_date.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ModelDate(BaseModel):
     """
     ModelDate
-    """
+    """  # noqa: E501
 
     expires_time: datetime = Field(description="Expiry Date")
     __properties: ClassVar[List[str]] = ["expires_time"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ModelDate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/model_schema.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/model_schema.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ModelSchema(BaseModel):
     """
     ModelSchema
-    """
+    """  # noqa: E501
 
     attr_names: Optional[List[StrictStr]] = Field(
         default=None, description="Schema attribute names", alias="attrNames"
     )
     id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Schema identifier"
     )
@@ -124,15 +124,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ModelSchema from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/oob_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/oob_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class OobRecord(BaseModel):
     """
     OobRecord
-    """
+    """  # noqa: E501
 
     attach_thread_id: Optional[StrictStr] = Field(
         default=None, description="Connection record identifier"
     )
     connection_id: Optional[StrictStr] = Field(
         default=None, description="Connection record identifier"
     )
@@ -169,15 +169,15 @@
             _dict["invitation"] = self.invitation.to_dict()
         # override the default output from pydantic by calling `to_dict()` of their_service
         if self.their_service:
             _dict["their_service"] = self.their_service.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of OobRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/perform_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/perform_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class PerformRequest(BaseModel):
     """
     PerformRequest
-    """
+    """  # noqa: E501
 
     name: Optional[StrictStr] = Field(default=None, description="Menu option name")
     params: Optional[Dict[str, StrictStr]] = Field(
         default=None, description="Input parameter values"
     )
     __properties: ClassVar[List[str]] = ["name", "params"]
 
@@ -68,15 +68,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of PerformRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ping_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ping_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class PingRequest(BaseModel):
     """
     PingRequest
-    """
+    """  # noqa: E501
 
     comment: Optional[StrictStr] = Field(
         default=None, description="Comment for the ping message"
     )
     __properties: ClassVar[List[str]] = ["comment"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -72,15 +72,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of PingRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/ping_request_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/ping_request_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class PingRequestResponse(BaseModel):
     """
     PingRequestResponse
-    """
+    """  # noqa: E501
 
     thread_id: Optional[StrictStr] = Field(
         default=None, description="Thread ID of the ping message"
     )
     __properties: ClassVar[List[str]] = ["thread_id"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of PingRequestResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/presentation_definition.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/presentation_definition.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class PresentationDefinition(BaseModel):
     """
     PresentationDefinition
-    """
+    """  # noqa: E501
 
     format: Optional[ClaimFormat] = None
     id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Unique Resource Identifier"
     )
     input_descriptors: Optional[List[InputDescriptors]] = None
     name: Optional[StrictStr] = Field(
@@ -122,15 +122,15 @@
             for _item in self.submission_requirements:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["submission_requirements"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of PresentationDefinition from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/presentation_proposal.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/presentation_proposal.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class PresentationProposal(BaseModel):
     """
     PresentationProposal
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -91,15 +91,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of PresentationProposal from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/presentation_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/presentation_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class PresentationRequest(BaseModel):
     """
     PresentationRequest
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -97,15 +97,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of PresentationRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/profile_settings.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/profile_settings.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ProfileSettings(BaseModel):
     """
     ProfileSettings
-    """
+    """  # noqa: E501
 
     settings: Optional[Union[str, Any]] = Field(
         default=None, description="Profile settings dict"
     )
     __properties: ClassVar[List[str]] = ["settings"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ProfileSettings from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/protocol_descriptor.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/protocol_descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ProtocolDescriptor(BaseModel):
     """
     ProtocolDescriptor
-    """
+    """  # noqa: E501
 
     pid: StrictStr
     roles: Optional[List[StrictStr]] = Field(default=None, description="List of roles")
     __properties: ClassVar[List[str]] = ["pid", "roles"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -71,15 +71,15 @@
         # and model_fields_set contains the field
         if self.roles is None and "roles" in self.model_fields_set:
             _dict["roles"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ProtocolDescriptor from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/publish_revocations.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/publish_revocations.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class PublishRevocations(BaseModel):
     """
     PublishRevocations
-    """
+    """  # noqa: E501
 
     rrid2crid: Optional[Dict[str, List[Annotated[str, Field(strict=True)]]]] = Field(
         default=None, description="Credential revocation ids by revocation registry id"
     )
     __properties: ClassVar[List[str]] = ["rrid2crid"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -68,15 +68,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of PublishRevocations from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/queries.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/queries.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Queries(BaseModel):
     """
     Queries
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -82,15 +82,15 @@
             for _item in self.queries:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["queries"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Queries from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/query.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/query.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class Query(BaseModel):
     """
     Query
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -80,15 +80,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of Query from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/query_item.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/query_item.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class QueryItem(BaseModel):
     """
     QueryItem
-    """
+    """  # noqa: E501
 
     feature_type: StrictStr = Field(description="feature type", alias="feature-type")
     match: StrictStr = Field(description="match")
     __properties: ClassVar[List[str]] = ["feature-type", "match"]
 
     @field_validator("feature_type")
     def feature_type_validate_enum(cls, value):
@@ -73,15 +73,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of QueryItem from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/raw_encoded.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/raw_encoded.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RawEncoded(BaseModel):
     """
     RawEncoded
-    """
+    """  # noqa: E501
 
     encoded: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Encoded value"
     )
     raw: Optional[StrictStr] = Field(default=None, description="Raw value")
     __properties: ClassVar[List[str]] = ["encoded", "raw"]
 
@@ -80,15 +80,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RawEncoded from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/receive_invitation_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/receive_invitation_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ReceiveInvitationRequest(BaseModel):
     """
     ReceiveInvitationRequest
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -126,15 +126,15 @@
         # and model_fields_set contains the field
         if self.image_url is None and "image_url" in self.model_fields_set:
             _dict["imageUrl"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ReceiveInvitationRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/remove_wallet_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/remove_wallet_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RemoveWalletRequest(BaseModel):
     """
     RemoveWalletRequest
-    """
+    """  # noqa: E501
 
     wallet_key: Optional[StrictStr] = Field(
         default=None,
         description="Master key used for key derivation. Only required for             unmanaged wallets.",
     )
     __properties: ClassVar[List[str]] = ["wallet_key"]
 
@@ -68,15 +68,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RemoveWalletRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/resolution_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/resolution_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ResolutionResult(BaseModel):
     """
     ResolutionResult
-    """
+    """  # noqa: E501
 
     did_document: Union[str, Any] = Field(description="DID Document")
     metadata: Union[str, Any] = Field(description="Resolution metadata")
     __properties: ClassVar[List[str]] = ["did_document", "metadata"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ResolutionResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_create_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_create_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RevRegCreateRequest(BaseModel):
     """
     RevRegCreateRequest
-    """
+    """  # noqa: E501
 
     credential_definition_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
     max_cred_num: Optional[Annotated[int, Field(le=32768, strict=True, ge=4)]] = Field(
         default=None, description="Revocation registry size"
     )
@@ -87,15 +87,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RevRegCreateRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_issued_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schemas_created_result.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,38 +25,35 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class RevRegIssuedResult(BaseModel):
-    """
-    RevRegIssuedResult
+class SchemasCreatedResult(BaseModel):
     """
+    SchemasCreatedResult
+    """  # noqa: E501
 
-    result: Optional[Annotated[int, Field(strict=True, ge=0)]] = Field(
-        default=None,
-        description="Number of credentials issued against revocation registry",
-    )
-    __properties: ClassVar[List[str]] = ["result"]
+    schema_ids: Optional[List[Annotated[str, Field(strict=True)]]] = None
+    __properties: ClassVar[List[str]] = ["schema_ids"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of RevRegIssuedResult from a JSON string"""
+        """Create an instance of SchemasCreatedResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,17 +66,17 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of RevRegIssuedResult from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of SchemasCreatedResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
-        _obj = cls.model_validate({"result": obj.get("result")})
+        _obj = cls.model_validate({"schema_ids": obj.get("schema_ids")})
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RevRegResult(BaseModel):
     """
     RevRegResult
-    """
+    """  # noqa: E501
 
     result: Optional[IssuerRevRegRecord] = None
     __properties: ClassVar[List[str]] = ["result"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict["result"] = self.result.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RevRegResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_update_tails_file_uri.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_update_tails_file_uri.py`

 * *Files 9% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RevRegUpdateTailsFileUri(BaseModel):
     """
     RevRegUpdateTailsFileUri
-    """
+    """  # noqa: E501
 
     tails_public_uri: StrictStr = Field(description="Public URI to the tails file")
     __properties: ClassVar[List[str]] = ["tails_public_uri"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RevRegUpdateTailsFileUri from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_reg_wallet_updated_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_reg_wallet_updated_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RevRegWalletUpdatedResult(BaseModel):
     """
     RevRegWalletUpdatedResult
-    """
+    """  # noqa: E501
 
     accum_calculated: Optional[Union[str, Any]] = Field(
         default=None, description="Calculated accumulator for phantom revocations"
     )
     accum_fixed: Optional[Union[str, Any]] = Field(
         default=None, description="Applied ledger transaction to fix revocations"
     )
@@ -77,15 +77,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RevRegWalletUpdatedResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/rev_regs_created.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/rev_regs_created.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RevRegsCreated(BaseModel):
     """
     RevRegsCreated
-    """
+    """  # noqa: E501
 
     rev_reg_ids: Optional[List[Annotated[str, Field(strict=True)]]] = None
     __properties: ClassVar[List[str]] = ["rev_reg_ids"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RevRegsCreated from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/revoke_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/revoke_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RevokeRequest(BaseModel):
     """
     RevokeRequest
-    """
+    """  # noqa: E501
 
     comment: Optional[StrictStr] = Field(
         default=None,
         description="Optional comment to include in revocation notification",
     )
     connection_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None,
@@ -173,15 +173,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RevokeRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/route_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/route_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class RouteRecord(BaseModel):
     """
     RouteRecord
-    """
+    """  # noqa: E501
 
     connection_id: Optional[StrictStr] = None
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     recipient_key: StrictStr
     record_id: Optional[StrictStr] = None
@@ -117,15 +117,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of RouteRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_get_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_get_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SchemaGetResult(BaseModel):
     """
     SchemaGetResult
-    """
+    """  # noqa: E501
 
     var_schema: Optional[ModelSchema] = Field(default=None, alias="schema")
     __properties: ClassVar[List[str]] = ["schema"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of var_schema
         if self.var_schema:
             _dict["schema"] = self.var_schema.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SchemaGetResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_input_descriptor.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_input_descriptor.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SchemaInputDescriptor(BaseModel):
     """
     SchemaInputDescriptor
-    """
+    """  # noqa: E501
 
     required: Optional[StrictBool] = Field(default=None, description="Required")
     uri: Optional[StrictStr] = Field(default=None, description="URI")
     __properties: ClassVar[List[str]] = ["required", "uri"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SchemaInputDescriptor from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_send_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_send_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SchemaSendRequest(BaseModel):
     """
     SchemaSendRequest
-    """
+    """  # noqa: E501
 
     attributes: List[StrictStr] = Field(description="List of schema attributes")
     schema_name: StrictStr = Field(description="Schema name")
     schema_version: Annotated[str, Field(strict=True)] = Field(
         description="Schema version"
     )
     __properties: ClassVar[List[str]] = ["attributes", "schema_name", "schema_version"]
@@ -78,15 +78,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SchemaSendRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schema_send_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schema_send_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SchemaSendResult(BaseModel):
     """
     SchemaSendResult
-    """
+    """  # noqa: E501
 
     var_schema: Optional[ModelSchema] = Field(default=None, alias="schema")
     schema_id: Annotated[str, Field(strict=True)] = Field(
         description="Schema identifier"
     )
     __properties: ClassVar[List[str]] = ["schema", "schema_id"]
 
@@ -86,15 +86,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of var_schema
         if self.var_schema:
             _dict["schema"] = self.var_schema.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SchemaSendResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schemas_created_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/verify_request.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,46 +14,49 @@
 
 from __future__ import annotations
 
 import json
 import pprint
 from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, Field
-from typing_extensions import Annotated
+from pydantic import BaseModel, Field, StrictStr
 
+from aries_cloudcontroller.models.signed_doc import SignedDoc
 from aries_cloudcontroller.util import DEFAULT_PYDANTIC_MODEL_CONFIG
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class SchemasCreatedResult(BaseModel):
-    """
-    SchemasCreatedResult
+class VerifyRequest(BaseModel):
     """
+    VerifyRequest
+    """  # noqa: E501
 
-    schema_ids: Optional[List[Annotated[str, Field(strict=True)]]] = None
-    __properties: ClassVar[List[str]] = ["schema_ids"]
+    doc: Dict[str, Any]
+    verkey: Optional[StrictStr] = Field(
+        default=None, description="Verkey to use for doc verification"
+    )
+    __properties: ClassVar[List[str]] = ["doc", "verkey"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of SchemasCreatedResult from a JSON string"""
+        """Create an instance of VerifyRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -66,17 +69,24 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of SchemasCreatedResult from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of VerifyRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
-        _obj = cls.model_validate({"schema_ids": obj.get("schema_ids")})
+        _obj = cls.model_validate(
+            {
+                "doc": SignedDoc.from_dict(obj.get("doc"))
+                if obj.get("doc") is not None
+                else None,
+                "verkey": obj.get("verkey"),
+            }
+        )
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/schemas_input_descriptor_filter.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/schemas_input_descriptor_filter.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SchemasInputDescriptorFilter(BaseModel):
     """
     SchemasInputDescriptorFilter
-    """
+    """  # noqa: E501
 
     oneof_filter: Optional[StrictBool] = Field(default=None, description="oneOf")
     uri_groups: Optional[List[List[SchemaInputDescriptor]]] = None
     __properties: ClassVar[List[str]] = ["oneof_filter", "uri_groups"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -80,15 +80,15 @@
                             if _inner_item is not None
                         ]
                     )
             _dict["uri_groups"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SchemasInputDescriptorFilter from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/send_menu.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/send_menu.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SendMenu(BaseModel):
     """
     SendMenu
-    """
+    """  # noqa: E501
 
     menu: MenuJson
     __properties: ClassVar[List[str]] = ["menu"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of menu
         if self.menu:
             _dict["menu"] = self.menu.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SendMenu from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/send_message.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/send_message.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SendMessage(BaseModel):
     """
     SendMessage
-    """
+    """  # noqa: E501
 
     content: Optional[StrictStr] = Field(default=None, description="Message content")
     __properties: ClassVar[List[str]] = ["content"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SendMessage from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/service_decorator.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/service_decorator.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class ServiceDecorator(BaseModel):
     """
     ServiceDecorator
-    """
+    """  # noqa: E501
 
     recipient_keys: Optional[List[Annotated[str, Field(strict=True)]]] = Field(
         default=None, description="List of recipient keys", alias="recipientKeys"
     )
     routing_keys: Optional[List[Annotated[str, Field(strict=True)]]] = Field(
         default=None, description="List of routing keys", alias="routingKeys"
     )
@@ -80,15 +80,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of ServiceDecorator from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/sign_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/sign_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SignRequest(BaseModel):
     """
     SignRequest
-    """
+    """  # noqa: E501
 
     doc: Doc
     verkey: StrictStr = Field(description="Verkey to use for signing")
     __properties: ClassVar[List[str]] = ["doc", "verkey"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -70,15 +70,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of doc
         if self.doc:
             _dict["doc"] = self.doc.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SignRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/sign_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/sign_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SignResponse(BaseModel):
     """
     SignResponse
-    """
+    """  # noqa: E501
 
     error: Optional[StrictStr] = Field(default=None, description="Error text")
     signed_doc: Optional[Union[str, Any]] = Field(
         default=None, description="Signed document"
     )
     __properties: ClassVar[List[str]] = ["error", "signed_doc"]
 
@@ -68,15 +68,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SignResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/signature_options.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/signature_options.py`

 * *Files 13% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SignatureOptions(BaseModel):
     """
     SignatureOptions
-    """
+    """  # noqa: E501
 
     challenge: Optional[StrictStr] = None
     domain: Optional[StrictStr] = None
     proof_purpose: StrictStr = Field(alias="proofPurpose")
     type: Optional[StrictStr] = None
     verification_method: StrictStr = Field(alias="verificationMethod")
     __properties: ClassVar[List[str]] = [
@@ -75,15 +75,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SignatureOptions from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/signed_doc.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/signed_doc.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SignedDoc(BaseModel):
     """
     SignedDoc
-    """
+    """  # noqa: E501
 
     proof: SignatureOptions
     __properties: ClassVar[List[str]] = ["proof"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of proof
         if self.proof:
             _dict["proof"] = self.proof.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SignedDoc from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/submission_requirements.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/submission_requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class SubmissionRequirements(BaseModel):
     """
     SubmissionRequirements
-    """
+    """  # noqa: E501
 
     count: Optional[StrictInt] = Field(default=None, description="Count Value")
     var_from: Optional[StrictStr] = Field(
         default=None, description="From", alias="from"
     )
     from_nested: Optional[List[SubmissionRequirements]] = None
     max: Optional[StrictInt] = Field(default=None, description="Max Value")
@@ -100,15 +100,15 @@
             for _item in self.from_nested:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["from_nested"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of SubmissionRequirements from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
@@ -128,13 +128,9 @@
                 "purpose": obj.get("purpose"),
                 "rule": obj.get("rule"),
             }
         )
         return _obj
 
 
-from typing import TYPE_CHECKING
-
-if TYPE_CHECKING:
-    # TODO: pydantic v2
-    # SubmissionRequirements.model_rebuild()
-    pass
+# TODO: Rewrite to not use raise_errors
+SubmissionRequirements.model_rebuild(raise_errors=False)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_accept.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_record.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,37 +24,37 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class TAAAccept(BaseModel):
-    """
-    TAAAccept
+class TAARecord(BaseModel):
     """
+    TAARecord
+    """  # noqa: E501
 
-    mechanism: Optional[StrictStr] = None
+    digest: Optional[StrictStr] = None
     text: Optional[StrictStr] = None
     version: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["mechanism", "text", "version"]
+    __properties: ClassVar[List[str]] = ["digest", "text", "version"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TAAAccept from a JSON string"""
+        """Create an instance of TAARecord from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,23 +67,23 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of TAAAccept from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of TAARecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "mechanism": obj.get("mechanism"),
+                "digest": obj.get("digest"),
                 "text": obj.get("text"),
                 "version": obj.get("version"),
             }
         )
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_acceptance.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_acceptance.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TAAAcceptance(BaseModel):
     """
     TAAAcceptance
-    """
+    """  # noqa: E501
 
     mechanism: Optional[StrictStr] = None
     time: Optional[
         Annotated[int, Field(le=18446744073709551615, strict=True, ge=0)]
     ] = None
     __properties: ClassVar[List[str]] = ["mechanism", "time"]
 
@@ -69,15 +69,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TAAAcceptance from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_info.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TAAInfo(BaseModel):
     """
     TAAInfo
-    """
+    """  # noqa: E501
 
     aml_record: Optional[AMLRecord] = None
     taa_accepted: Optional[TAAAcceptance] = None
     taa_record: Optional[TAARecord] = None
     taa_required: Optional[StrictBool] = None
     __properties: ClassVar[List[str]] = [
         "aml_record",
@@ -85,15 +85,15 @@
             _dict["taa_accepted"] = self.taa_accepted.to_dict()
         # override the default output from pydantic by calling `to_dict()` of taa_record
         if self.taa_record:
             _dict["taa_record"] = self.taa_record.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TAAInfo from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_accept.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,37 +24,37 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class TAARecord(BaseModel):
-    """
-    TAARecord
+class TAAAccept(BaseModel):
     """
+    TAAAccept
+    """  # noqa: E501
 
-    digest: Optional[StrictStr] = None
+    mechanism: Optional[StrictStr] = None
     text: Optional[StrictStr] = None
     version: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["digest", "text", "version"]
+    __properties: ClassVar[List[str]] = ["mechanism", "text", "version"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of TAARecord from a JSON string"""
+        """Create an instance of TAAAccept from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -67,23 +67,23 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of TAARecord from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of TAAAccept from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "digest": obj.get("digest"),
+                "mechanism": obj.get("mechanism"),
                 "text": obj.get("text"),
                 "version": obj.get("version"),
             }
         )
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/taa_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/taa_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TAAResult(BaseModel):
     """
     TAAResult
-    """
+    """  # noqa: E501
 
     result: Optional[TAAInfo] = None
     __properties: ClassVar[List[str]] = ["result"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of result
         if self.result:
             _dict["result"] = self.result.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TAAResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/tails_delete_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/tails_delete_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TailsDeleteResponse(BaseModel):
     """
     TailsDeleteResponse
-    """
+    """  # noqa: E501
 
     message: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["message"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TailsDeleteResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/transaction_jobs.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/transaction_jobs.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TransactionJobs(BaseModel):
     """
     TransactionJobs
-    """
+    """  # noqa: E501
 
     transaction_my_job: Optional[StrictStr] = Field(
         default=None, description="My transaction related job"
     )
     transaction_their_job: Optional[StrictStr] = Field(
         default=None, description="Their transaction related job"
     )
@@ -94,15 +94,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TransactionJobs from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/transaction_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/transaction_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TransactionList(BaseModel):
     """
     TransactionList
-    """
+    """  # noqa: E501
 
     results: Optional[List[TransactionRecord]] = Field(
         default=None, description="List of transaction records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -75,15 +75,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TransactionList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/transaction_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/transaction_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TransactionRecord(BaseModel):
     """
     TransactionRecord
-    """
+    """  # noqa: E501
 
     type: Optional[StrictStr] = Field(
         default=None, description="Transaction type", alias="_type"
     )
     connection_id: Optional[StrictStr] = Field(
         default=None,
         description="The connection identifier for thie particular transaction record",
@@ -146,15 +146,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TransactionRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_credential_definition_send_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_credential_definition_send_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TxnOrCredentialDefinitionSendResult(BaseModel):
     """
     TxnOrCredentialDefinitionSendResult
-    """
+    """  # noqa: E501
 
     sent: Optional[CredentialDefinitionSendResult] = None
     txn: Optional[TransactionRecord] = None
     __properties: ClassVar[List[str]] = ["sent", "txn"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -76,15 +76,15 @@
             _dict["sent"] = self.sent.to_dict()
         # override the default output from pydantic by calling `to_dict()` of txn
         if self.txn:
             _dict["txn"] = self.txn.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TxnOrCredentialDefinitionSendResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_publish_revocations_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_publish_revocations_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TxnOrPublishRevocationsResult(BaseModel):
     """
     TxnOrPublishRevocationsResult
-    """
+    """  # noqa: E501
 
     sent: Optional[PublishRevocations] = None
     txn: Optional[TransactionRecord] = None
     __properties: ClassVar[List[str]] = ["sent", "txn"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["sent"] = self.sent.to_dict()
         # override the default output from pydantic by calling `to_dict()` of txn
         if self.txn:
             _dict["txn"] = self.txn.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TxnOrPublishRevocationsResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_register_ledger_nym_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_register_ledger_nym_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TxnOrRegisterLedgerNymResponse(BaseModel):
     """
     TxnOrRegisterLedgerNymResponse
-    """
+    """  # noqa: E501
 
     success: Optional[StrictBool] = Field(
         default=None, description="Success of nym registration operation"
     )
     txn: Optional[TransactionRecord] = None
     __properties: ClassVar[List[str]] = ["success", "txn"]
 
@@ -72,15 +72,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of txn
         if self.txn:
             _dict["txn"] = self.txn.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TxnOrRegisterLedgerNymResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_rev_reg_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_rev_reg_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TxnOrRevRegResult(BaseModel):
     """
     TxnOrRevRegResult
-    """
+    """  # noqa: E501
 
     sent: Optional[RevRegResult] = None
     txn: Optional[TransactionRecord] = None
     __properties: ClassVar[List[str]] = ["sent", "txn"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["sent"] = self.sent.to_dict()
         # override the default output from pydantic by calling `to_dict()` of txn
         if self.txn:
             _dict["txn"] = self.txn.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TxnOrRevRegResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/txn_or_schema_send_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/txn_or_schema_send_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class TxnOrSchemaSendResult(BaseModel):
     """
     TxnOrSchemaSendResult
-    """
+    """  # noqa: E501
 
     sent: Optional[SchemaSendResult] = None
     txn: Optional[TransactionRecord] = None
     __properties: ClassVar[List[str]] = ["sent", "txn"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["sent"] = self.sent.to_dict()
         # override the default output from pydantic by calling `to_dict()` of txn
         if self.txn:
             _dict["txn"] = self.txn.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of TxnOrSchemaSendResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/update_profile_settings.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/update_profile_settings.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class UpdateProfileSettings(BaseModel):
     """
     UpdateProfileSettings
-    """
+    """  # noqa: E501
 
     extra_settings: Optional[Union[str, Any]] = Field(
         default=None, description="Agent config key-value pairs"
     )
     __properties: ClassVar[List[str]] = ["extra_settings"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of UpdateProfileSettings from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/update_wallet_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/update_wallet_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class UpdateWalletRequest(BaseModel):
     """
     UpdateWalletRequest
-    """
+    """  # noqa: E501
 
     extra_settings: Optional[Union[str, Any]] = Field(
         default=None, description="Agent config key-value pairs"
     )
     image_url: Optional[StrictStr] = Field(
         default=None,
         description="Image url for this wallet. This image url is publicized            (self-attested) to other agents as part of forming a connection.",
@@ -98,15 +98,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of UpdateWalletRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_bound_offer_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_bound_offer_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialBoundOfferRequest(BaseModel):
     """
     V10CredentialBoundOfferRequest
-    """
+    """  # noqa: E501
 
     counter_proposal: Optional[CredentialProposal] = None
     __properties: ClassVar[List[str]] = ["counter_proposal"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of counter_proposal
         if self.counter_proposal:
             _dict["counter_proposal"] = self.counter_proposal.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialBoundOfferRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_conn_free_offer_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_conn_free_offer_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialConnFreeOfferRequest(BaseModel):
     """
     V10CredentialConnFreeOfferRequest
-    """
+    """  # noqa: E501
 
     auto_issue: Optional[StrictBool] = Field(
         default=None,
         description="Whether to respond automatically to credential requests, creating and issuing requested credentials",
     )
     auto_remove: Optional[StrictBool] = Field(
         default=None,
@@ -113,15 +113,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialConnFreeOfferRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_create.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_create.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialCreate(BaseModel):
     """
     V10CredentialCreate
-    """
+    """  # noqa: E501
 
     auto_remove: Optional[StrictBool] = Field(
         default=None,
         description="Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting)",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -184,15 +184,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialCreate from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_exchange.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_exchange.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialExchange(BaseModel):
     """
     V10CredentialExchange
-    """
+    """  # noqa: E501
 
     auto_issue: Optional[StrictBool] = Field(
         default=None,
         description="Issuer choice to issue to request in this credential exchange",
     )
     auto_offer: Optional[StrictBool] = Field(
         default=None,
@@ -266,15 +266,15 @@
             _dict["credential_request"] = self.credential_request.to_dict()
         # override the default output from pydantic by calling `to_dict()` of raw_credential
         if self.raw_credential:
             _dict["raw_credential"] = self.raw_credential.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialExchange from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_exchange_list_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_exchange_list_result.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialExchangeListResult(BaseModel):
     """
     V10CredentialExchangeListResult
-    """
+    """  # noqa: E501
 
     results: Optional[List[V10CredentialExchange]] = Field(
         default=None, description="Aries#0036 v1.0 credential exchange records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -75,15 +75,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialExchangeListResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_free_offer_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_free_offer_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialFreeOfferRequest(BaseModel):
     """
     V10CredentialFreeOfferRequest
-    """
+    """  # noqa: E501
 
     auto_issue: Optional[StrictBool] = Field(
         default=None,
         description="Whether to respond automatically to credential requests, creating and issuing requested credentials",
     )
     auto_remove: Optional[StrictBool] = Field(
         default=None,
@@ -115,15 +115,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialFreeOfferRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_issue_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_issue_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class V10CredentialIssueRequest(BaseModel):
-    """
-    V10CredentialIssueRequest
+class V20CredIssueRequest(BaseModel):
     """
+    V20CredIssueRequest
+    """  # noqa: E501
 
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
     )
     __properties: ClassVar[List[str]] = ["comment"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -46,15 +46,15 @@
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V10CredentialIssueRequest from a JSON string"""
+        """Create an instance of V20CredIssueRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,16 +72,16 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V10CredentialIssueRequest from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of V20CredIssueRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({"comment": obj.get("comment")})
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_problem_report_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_problem_report_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialProblemReportRequest(BaseModel):
     """
     V10CredentialProblemReportRequest
-    """
+    """  # noqa: E501
 
     description: StrictStr
     __properties: ClassVar[List[str]] = ["description"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialProblemReportRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_proposal_request_mand.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_proposal_request_mand.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialProposalRequestMand(BaseModel):
     """
     V10CredentialProposalRequestMand
-    """
+    """  # noqa: E501
 
     auto_remove: Optional[StrictBool] = Field(
         default=None,
         description="Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting)",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -186,15 +186,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialProposalRequestMand from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_proposal_request_opt.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_proposal_request_opt.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialProposalRequestOpt(BaseModel):
     """
     V10CredentialProposalRequestOpt
-    """
+    """  # noqa: E501
 
     auto_remove: Optional[StrictBool] = Field(
         default=None,
         description="Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting)",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -186,15 +186,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialProposalRequestOpt from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_credential_store_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_store_request.py`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10CredentialStoreRequest(BaseModel):
     """
     V10CredentialStoreRequest
-    """
+    """  # noqa: E501
 
     credential_id: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["credential_id"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10CredentialStoreRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_discovery_exchange_list_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10DiscoveryExchangeListResult(BaseModel):
     """
     V10DiscoveryExchangeListResult
-    """
+    """  # noqa: E501
 
     results: Optional[List[V10DiscoveryRecord]] = None
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -73,15 +73,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10DiscoveryExchangeListResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_discovery_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_discovery_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10DiscoveryRecord(BaseModel):
     """
     V10DiscoveryRecord
-    """
+    """  # noqa: E501
 
     connection_id: Optional[StrictStr] = Field(
         default=None, description="Connection identifier"
     )
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
@@ -136,15 +136,15 @@
             _dict["disclose"] = self.disclose.to_dict()
         # override the default output from pydantic by calling `to_dict()` of query_msg
         if self.query_msg:
             _dict["query_msg"] = self.query_msg.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10DiscoveryRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_create_request_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_create_request_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10PresentationCreateRequestRequest(BaseModel):
     """
     V10PresentationCreateRequestRequest
-    """
+    """  # noqa: E501
 
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
     )
     comment: Optional[StrictStr] = None
     proof_request: IndyProofRequest
     trace: Optional[StrictBool] = Field(
@@ -86,15 +86,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10PresentationCreateRequestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_exchange.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_exchange.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10PresentationExchange(BaseModel):
     """
     V10PresentationExchange
-    """
+    """  # noqa: E501
 
     auto_present: Optional[StrictBool] = Field(
         default=None,
         description="Prover choice to auto-present proof as verifier requests",
     )
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
@@ -209,15 +209,15 @@
         if self.presentation_request_dict:
             _dict[
                 "presentation_request_dict"
             ] = self.presentation_request_dict.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10PresentationExchange from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_exchange_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_exchange_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10PresentationExchangeList(BaseModel):
     """
     V10PresentationExchangeList
-    """
+    """  # noqa: E501
 
     results: Optional[List[V10PresentationExchange]] = Field(
         default=None, description="Aries RFC 37 v1.0 presentation exchange records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -77,15 +77,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10PresentationExchangeList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_problem_report_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_problem_report_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10PresentationProblemReportRequest(BaseModel):
     """
     V10PresentationProblemReportRequest
-    """
+    """  # noqa: E501
 
     description: StrictStr
     __properties: ClassVar[List[str]] = ["description"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10PresentationProblemReportRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_proposal_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_proposal_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10PresentationProposalRequest(BaseModel):
     """
     V10PresentationProposalRequest
-    """
+    """  # noqa: E501
 
     auto_present: Optional[StrictBool] = Field(
         default=None,
         description="Whether to respond automatically to presentation requests, building and presenting requested proof",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -91,15 +91,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10PresentationProposalRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_send_request_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_send_request_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10PresentationSendRequestRequest(BaseModel):
     """
     V10PresentationSendRequestRequest
-    """
+    """  # noqa: E501
 
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
     )
     comment: Optional[StrictStr] = None
     connection_id: StrictStr = Field(description="Connection identifier")
     proof_request: IndyProofRequest
@@ -88,15 +88,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10PresentationSendRequestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v10_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_presentation_send_request_to_proposal.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V10PresentationSendRequestToProposal(BaseModel):
     """
     V10PresentationSendRequestToProposal
-    """
+    """  # noqa: E501
 
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
     )
     trace: Optional[StrictBool] = Field(
         default=None, description="Whether to trace event (default false)"
     )
@@ -70,15 +70,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V10PresentationSendRequestToProposal from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_attr_spec.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_attr_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredAttrSpec(BaseModel):
     """
     V20CredAttrSpec
-    """
+    """  # noqa: E501
 
     mime_type: Optional[StrictStr] = Field(
         default=None,
         description="MIME type: omit for (null) default",
         alias="mime-type",
     )
     name: StrictStr = Field(description="Attribute name")
@@ -78,15 +78,15 @@
         # and model_fields_set contains the field
         if self.mime_type is None and "mime_type" in self.model_fields_set:
             _dict["mime-type"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredAttrSpec from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_bound_offer_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_bound_offer_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredBoundOfferRequest(BaseModel):
     """
     V20CredBoundOfferRequest
-    """
+    """  # noqa: E501
 
     counter_preview: Optional[V20CredPreview] = None
     filter: Optional[V20CredFilter] = None
     __properties: ClassVar[List[str]] = ["counter_preview", "filter"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["counter_preview"] = self.counter_preview.to_dict()
         # override the default output from pydantic by calling `to_dict()` of filter
         if self.filter:
             _dict["filter"] = self.filter.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredBoundOfferRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_free.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_free.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredExFree(BaseModel):
     """
     V20CredExFree
-    """
+    """  # noqa: E501
 
     auto_remove: Optional[StrictBool] = Field(
         default=None,
         description="Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting)",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -120,15 +120,15 @@
             and "verification_method" in self.model_fields_set
         ):
             _dict["verification_method"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredExFree from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -37,15 +37,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredExRecord(BaseModel):
     """
     V20CredExRecord
-    """
+    """  # noqa: E501
 
     auto_issue: Optional[StrictBool] = Field(
         default=None,
         description="Issuer choice to issue to request in this credential exchange",
     )
     auto_offer: Optional[StrictBool] = Field(
         default=None,
@@ -239,15 +239,15 @@
             _dict["cred_proposal"] = self.cred_proposal.to_dict()
         # override the default output from pydantic by calling `to_dict()` of cred_request
         if self.cred_request:
             _dict["cred_request"] = self.cred_request.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredExRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_by_format.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_by_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredExRecordByFormat(BaseModel):
     """
     V20CredExRecordByFormat
-    """
+    """  # noqa: E501
 
     cred_issue: Optional[Union[str, Any]] = None
     cred_offer: Optional[Union[str, Any]] = None
     cred_proposal: Optional[Union[str, Any]] = None
     cred_request: Optional[Union[str, Any]] = None
     __properties: ClassVar[List[str]] = [
         "cred_issue",
@@ -73,15 +73,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredExRecordByFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_detail.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_detail.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredExRecordDetail(BaseModel):
     """
     V20CredExRecordDetail
-    """
+    """  # noqa: E501
 
     cred_ex_record: Optional[V20CredExRecord] = None
     indy: Optional[V20CredExRecordIndy] = None
     ld_proof: Optional[V20CredExRecordLDProof] = None
     __properties: ClassVar[List[str]] = ["cred_ex_record", "indy", "ld_proof"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -81,15 +81,15 @@
             _dict["indy"] = self.indy.to_dict()
         # override the default output from pydantic by calling `to_dict()` of ld_proof
         if self.ld_proof:
             _dict["ld_proof"] = self.ld_proof.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredExRecordDetail from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_indy.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_indy.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredExRecordIndy(BaseModel):
     """
     V20CredExRecordIndy
-    """
+    """  # noqa: E501
 
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     cred_ex_id: Optional[StrictStr] = Field(
         default=None,
         description="Corresponding v2.0 credential exchange record identifier",
@@ -158,15 +158,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredExRecordIndy from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_ld_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_ld_proof.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredExRecordLDProof(BaseModel):
     """
     V20CredExRecordLDProof
-    """
+    """  # noqa: E501
 
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     cred_ex_id: Optional[StrictStr] = Field(
         default=None,
         description="Corresponding v2.0 credential exchange record identifier",
@@ -120,15 +120,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredExRecordLDProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_ex_record_list_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_ex_record_list_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredExRecordListResult(BaseModel):
     """
     V20CredExRecordListResult
-    """
+    """  # noqa: E501
 
     results: Optional[List[V20CredExRecordDetail]] = Field(
         default=None,
         description="Credential exchange records and corresponding detail records",
     )
     __properties: ClassVar[List[str]] = ["results"]
 
@@ -76,15 +76,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredExRecordListResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_filter.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredFilter(BaseModel):
     """
     V20CredFilter
-    """
+    """  # noqa: E501
 
     indy: Optional[V20CredFilterIndy] = None
     ld_proof: Optional[LDProofVCDetail] = None
     __properties: ClassVar[List[str]] = ["indy", "ld_proof"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["indy"] = self.indy.to_dict()
         # override the default output from pydantic by calling `to_dict()` of ld_proof
         if self.ld_proof:
             _dict["ld_proof"] = self.ld_proof.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredFilter from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_filter_indy.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_filter_indy.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredFilterIndy(BaseModel):
     """
     V20CredFilterIndy
-    """
+    """  # noqa: E501
 
     cred_def_id: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential definition identifier"
     )
     issuer_did: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Credential issuer DID"
     )
@@ -159,15 +159,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredFilterIndy from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_filter_ld_proof.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_filter_ld_proof.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredFilterLDProof(BaseModel):
     """
     V20CredFilterLDProof
-    """
+    """  # noqa: E501
 
     ld_proof: LDProofVCDetail
     __properties: ClassVar[List[str]] = ["ld_proof"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -69,15 +69,15 @@
         )
         # override the default output from pydantic by calling `to_dict()` of ld_proof
         if self.ld_proof:
             _dict["ld_proof"] = self.ld_proof.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredFilterLDProof from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_format.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredFormat(BaseModel):
     """
     V20CredFormat
-    """
+    """  # noqa: E501
 
     attach_id: StrictStr = Field(description="Attachment identifier")
     format: StrictStr = Field(description="Attachment format specifier")
     __properties: ClassVar[List[str]] = ["attach_id", "format"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_issue.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_issue.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredIssue(BaseModel):
     """
     V20CredIssue
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -112,15 +112,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredIssue from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_issue_problem_report_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_problem_report_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class V20CredIssueProblemReportRequest(BaseModel):
-    """
-    V20CredIssueProblemReportRequest
+class V20PresProblemReportRequest(BaseModel):
     """
+    V20PresProblemReportRequest
+    """  # noqa: E501
 
     description: StrictStr
     __properties: ClassVar[List[str]] = ["description"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -44,15 +44,15 @@
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V20CredIssueProblemReportRequest from a JSON string"""
+        """Create an instance of V20PresProblemReportRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,16 +65,16 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V20CredIssueProblemReportRequest from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of V20PresProblemReportRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({"description": obj.get("description")})
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_issue_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v10_credential_issue_request.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class V20CredIssueRequest(BaseModel):
-    """
-    V20CredIssueRequest
+class V10CredentialIssueRequest(BaseModel):
     """
+    V10CredentialIssueRequest
+    """  # noqa: E501
 
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
     )
     __properties: ClassVar[List[str]] = ["comment"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -46,15 +46,15 @@
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V20CredIssueRequest from a JSON string"""
+        """Create an instance of V10CredentialIssueRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -72,16 +72,16 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V20CredIssueRequest from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of V10CredentialIssueRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({"comment": obj.get("comment")})
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_offer.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_offer.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredOffer(BaseModel):
     """
     V20CredOffer
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -118,15 +118,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredOffer from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_offer_conn_free_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_offer_conn_free_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredOfferConnFreeRequest(BaseModel):
     """
     V20CredOfferConnFreeRequest
-    """
+    """  # noqa: E501
 
     auto_issue: Optional[StrictBool] = Field(
         default=None,
         description="Whether to respond automatically to credential requests, creating and issuing requested credentials",
     )
     auto_remove: Optional[StrictBool] = Field(
         default=None,
@@ -111,15 +111,15 @@
         # and model_fields_set contains the field
         if self.replacement_id is None and "replacement_id" in self.model_fields_set:
             _dict["replacement_id"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredOfferConnFreeRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_offer_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_offer_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredOfferRequest(BaseModel):
     """
     V20CredOfferRequest
-    """
+    """  # noqa: E501
 
     auto_issue: Optional[StrictBool] = Field(
         default=None,
         description="Whether to respond automatically to credential requests, creating and issuing requested credentials",
     )
     auto_remove: Optional[StrictBool] = Field(
         default=None,
@@ -113,15 +113,15 @@
         # and model_fields_set contains the field
         if self.replacement_id is None and "replacement_id" in self.model_fields_set:
             _dict["replacement_id"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredOfferRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_preview.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_preview.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredPreview(BaseModel):
     """
     V20CredPreview
-    """
+    """  # noqa: E501
 
     type: Optional[StrictStr] = Field(
         default=None, description="Message type identifier", alias="@type"
     )
     attributes: List[V20CredAttrSpec]
     __properties: ClassVar[List[str]] = ["@type", "attributes"]
 
@@ -76,15 +76,15 @@
             for _item in self.attributes:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["attributes"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredPreview from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_proposal.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_proposal.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredProposal(BaseModel):
     """
     V20CredProposal
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -114,15 +114,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredProposal from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredRequest(BaseModel):
     """
     V20CredRequest
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -107,15 +107,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_request_free.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_request_free.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredRequestFree(BaseModel):
     """
     V20CredRequestFree
-    """
+    """  # noqa: E501
 
     auto_remove: Optional[StrictBool] = Field(
         default=None,
         description="Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting)",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -101,15 +101,15 @@
         # and model_fields_set contains the field
         if self.holder_did is None and "holder_did" in self.model_fields_set:
             _dict["holder_did"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredRequestFree from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_request_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_request_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredRequestRequest(BaseModel):
     """
     V20CredRequestRequest
-    """
+    """  # noqa: E501
 
     holder_did: Optional[StrictStr] = Field(
         default=None,
         description="Holder DID to substitute for the credentialSubject.id",
     )
     __properties: ClassVar[List[str]] = ["holder_did"]
 
@@ -73,15 +73,15 @@
         # and model_fields_set contains the field
         if self.holder_did is None and "holder_did" in self.model_fields_set:
             _dict["holder_did"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredRequestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_cred_store_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_store_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20CredStoreRequest(BaseModel):
     """
     V20CredStoreRequest
-    """
+    """  # noqa: E501
 
     credential_id: Optional[StrictStr] = None
     __properties: ClassVar[List[str]] = ["credential_id"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -65,15 +65,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20CredStoreRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_discovery_exchange_list_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_discovery_exchange_list_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20DiscoveryExchangeListResult(BaseModel):
     """
     V20DiscoveryExchangeListResult
-    """
+    """  # noqa: E501
 
     results: Optional[List[V20DiscoveryRecord]] = None
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -73,15 +73,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20DiscoveryExchangeListResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_discovery_exchange_result.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/vc_record_list.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,44 +16,44 @@
 
 import json
 import pprint
 from typing import Any, ClassVar, Dict, List, Optional
 
 from pydantic import BaseModel
 
-from aries_cloudcontroller.models.v20_discovery_record import V20DiscoveryRecord
+from aries_cloudcontroller.models.vc_record import VCRecord
 from aries_cloudcontroller.util import DEFAULT_PYDANTIC_MODEL_CONFIG
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class V20DiscoveryExchangeResult(BaseModel):
-    """
-    V20DiscoveryExchangeResult
+class VCRecordList(BaseModel):
     """
+    VCRecordList
+    """  # noqa: E501
 
-    results: Optional[V20DiscoveryRecord] = None
+    results: Optional[List[VCRecord]] = None
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V20DiscoveryExchangeResult from a JSON string"""
+        """Create an instance of VCRecordList from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -63,29 +63,33 @@
           are ignored.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of results
+        # override the default output from pydantic by calling `to_dict()` of each item in results (list)
+        _items = []
         if self.results:
-            _dict["results"] = self.results.to_dict()
+            for _item in self.results:
+                if _item:
+                    _items.append(_item.to_dict())
+            _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V20DiscoveryExchangeResult from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of VCRecordList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "results": V20DiscoveryRecord.from_dict(obj.get("results"))
+                "results": [VCRecord.from_dict(_item) for _item in obj.get("results")]
                 if obj.get("results") is not None
                 else None
             }
         )
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_discovery_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_discovery_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20DiscoveryRecord(BaseModel):
     """
     V20DiscoveryRecord
-    """
+    """  # noqa: E501
 
     connection_id: Optional[StrictStr] = Field(
         default=None, description="Connection identifier"
     )
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
@@ -136,15 +136,15 @@
             _dict["disclosures"] = self.disclosures.to_dict()
         # override the default output from pydantic by calling `to_dict()` of queries_msg
         if self.queries_msg:
             _dict["queries_msg"] = self.queries_msg.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20DiscoveryRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_issue_cred_schema_core.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_issue_cred_schema_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20IssueCredSchemaCore(BaseModel):
     """
     V20IssueCredSchemaCore
-    """
+    """  # noqa: E501
 
     auto_remove: Optional[StrictBool] = Field(
         default=None,
         description="Whether to remove the credential exchange record on completion (overrides --preserve-exchange-records configuration setting)",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -106,15 +106,15 @@
         # and model_fields_set contains the field
         if self.replacement_id is None and "replacement_id" in self.model_fields_set:
             _dict["replacement_id"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20IssueCredSchemaCore from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20Pres(BaseModel):
     """
     V20Pres
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -105,15 +105,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20Pres from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_create_request_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_create_request_request.py`

 * *Files 3% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresCreateRequestRequest(BaseModel):
     """
     V20PresCreateRequestRequest
-    """
+    """  # noqa: E501
 
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
     )
     comment: Optional[StrictStr] = None
     presentation_request: V20PresRequestByFormat
     trace: Optional[StrictBool] = Field(
@@ -88,15 +88,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresCreateRequestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_ex_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_ex_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresExRecord(BaseModel):
     """
     V20PresExRecord
-    """
+    """  # noqa: E501
 
     auto_present: Optional[StrictBool] = Field(
         default=None,
         description="Prover choice to auto-present proof as verifier requests",
     )
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
@@ -229,15 +229,15 @@
             _dict["pres_proposal"] = self.pres_proposal.to_dict()
         # override the default output from pydantic by calling `to_dict()` of pres_request
         if self.pres_request:
             _dict["pres_request"] = self.pres_request.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresExRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_ex_record_by_format.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_ex_record_by_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresExRecordByFormat(BaseModel):
     """
     V20PresExRecordByFormat
-    """
+    """  # noqa: E501
 
     pres: Optional[Union[str, Any]] = None
     pres_proposal: Optional[Union[str, Any]] = None
     pres_request: Optional[Union[str, Any]] = None
     __properties: ClassVar[List[str]] = ["pres", "pres_proposal", "pres_request"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -67,15 +67,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresExRecordByFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_ex_record_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_ex_record_list.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresExRecordList(BaseModel):
     """
     V20PresExRecordList
-    """
+    """  # noqa: E501
 
     results: Optional[List[V20PresExRecord]] = Field(
         default=None, description="Presentation exchange records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -75,15 +75,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresExRecordList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_format.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresFormat(BaseModel):
     """
     V20PresFormat
-    """
+    """  # noqa: E501
 
     attach_id: StrictStr = Field(description="Attachment identifier")
     format: StrictStr = Field(description="Attachment format specifier")
     __properties: ClassVar[List[str]] = ["attach_id", "format"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_problem_report_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_cred_issue_problem_report_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,18 +24,18 @@
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class V20PresProblemReportRequest(BaseModel):
-    """
-    V20PresProblemReportRequest
+class V20CredIssueProblemReportRequest(BaseModel):
     """
+    V20CredIssueProblemReportRequest
+    """  # noqa: E501
 
     description: StrictStr
     __properties: ClassVar[List[str]] = ["description"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
@@ -44,15 +44,15 @@
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of V20PresProblemReportRequest from a JSON string"""
+        """Create an instance of V20CredIssueProblemReportRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,16 +65,16 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of V20PresProblemReportRequest from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of V20CredIssueProblemReportRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({"description": obj.get("description")})
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_proposal.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_proposal.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresProposal(BaseModel):
     """
     V20PresProposal
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -103,15 +103,15 @@
             for _item in self.proposalsattach:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["proposals~attach"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresProposal from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_proposal_by_format.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_proposal_by_format.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresProposalByFormat(BaseModel):
     """
     V20PresProposalByFormat
-    """
+    """  # noqa: E501
 
     dif: Optional[DIFProofProposal] = None
     indy: Optional[IndyProofRequest] = None
     __properties: ClassVar[List[str]] = ["dif", "indy"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["dif"] = self.dif.to_dict()
         # override the default output from pydantic by calling `to_dict()` of indy
         if self.indy:
             _dict["indy"] = self.indy.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresProposalByFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_proposal_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_proposal_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresProposalRequest(BaseModel):
     """
     V20PresProposalRequest
-    """
+    """  # noqa: E501
 
     auto_present: Optional[StrictBool] = Field(
         default=None,
         description="Whether to respond automatically to presentation requests, building and presenting requested proof",
     )
     comment: Optional[StrictStr] = Field(
         default=None, description="Human-readable comment"
@@ -93,15 +93,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresProposalRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresRequest(BaseModel):
     """
     V20PresRequest
-    """
+    """  # noqa: E501
 
     id: Optional[StrictStr] = Field(
         default=None, description="Message identifier", alias="@id"
     )
     type: Optional[StrictStr] = Field(
         default=None, description="Message type", alias="@type"
     )
@@ -107,15 +107,15 @@
             for _item in self.request_presentationsattach:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["request_presentations~attach"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_request_by_format.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_request_by_format.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresRequestByFormat(BaseModel):
     """
     V20PresRequestByFormat
-    """
+    """  # noqa: E501
 
     dif: Optional[DIFProofRequest] = None
     indy: Optional[IndyProofRequest] = None
     __properties: ClassVar[List[str]] = ["dif", "indy"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -74,15 +74,15 @@
             _dict["dif"] = self.dif.to_dict()
         # override the default output from pydantic by calling `to_dict()` of indy
         if self.indy:
             _dict["indy"] = self.indy.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresRequestByFormat from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_send_request_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_send_request_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -30,15 +30,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresSendRequestRequest(BaseModel):
     """
     V20PresSendRequestRequest
-    """
+    """  # noqa: E501
 
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
     )
     comment: Optional[StrictStr] = None
     connection_id: StrictStr = Field(description="Connection identifier")
     presentation_request: V20PresRequestByFormat
@@ -90,15 +90,15 @@
         # and model_fields_set contains the field
         if self.comment is None and "comment" in self.model_fields_set:
             _dict["comment"] = None
 
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresSendRequestRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_pres_spec_by_format_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_pres_spec_by_format_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresSpecByFormatRequest(BaseModel):
     """
     V20PresSpecByFormatRequest
-    """
+    """  # noqa: E501
 
     dif: Optional[DIFPresSpec] = None
     indy: Optional[IndyPresSpec] = None
     trace: Optional[StrictBool] = Field(
         default=None,
         description="Record trace information, based on agent configuration",
     )
@@ -78,15 +78,15 @@
             _dict["dif"] = self.dif.to_dict()
         # override the default output from pydantic by calling `to_dict()` of indy
         if self.indy:
             _dict["indy"] = self.indy.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresSpecByFormatRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/v20_presentation_send_request_to_proposal.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/v20_presentation_send_request_to_proposal.py`

 * *Files 5% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class V20PresentationSendRequestToProposal(BaseModel):
     """
     V20PresentationSendRequestToProposal
-    """
+    """  # noqa: E501
 
     auto_verify: Optional[StrictBool] = Field(
         default=None, description="Verifier choice to auto-verify proof presentation"
     )
     trace: Optional[StrictBool] = Field(
         default=None, description="Whether to trace event (default false)"
     )
@@ -70,15 +70,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of V20PresentationSendRequestToProposal from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/vc_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/vc_record.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class VCRecord(BaseModel):
     """
     VCRecord
-    """
+    """  # noqa: E501
 
     contexts: Optional[List[Annotated[str, Field(strict=True)]]] = None
     cred_tags: Optional[Dict[str, StrictStr]] = None
     cred_value: Optional[Union[str, Any]] = Field(
         default=None, description="(JSON-serializable) credential value"
     )
     expanded_types: Optional[List[StrictStr]] = None
@@ -94,15 +94,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of VCRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/vc_record_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/did_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -16,44 +16,44 @@
 
 import json
 import pprint
 from typing import Any, ClassVar, Dict, List, Optional
 
 from pydantic import BaseModel
 
-from aries_cloudcontroller.models.vc_record import VCRecord
+from aries_cloudcontroller.models.did import DID
 from aries_cloudcontroller.util import DEFAULT_PYDANTIC_MODEL_CONFIG
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class VCRecordList(BaseModel):
-    """
-    VCRecordList
+class DIDResult(BaseModel):
     """
+    DIDResult
+    """  # noqa: E501
 
-    results: Optional[List[VCRecord]] = None
-    __properties: ClassVar[List[str]] = ["results"]
+    result: Optional[DID] = None
+    __properties: ClassVar[List[str]] = ["result"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of VCRecordList from a JSON string"""
+        """Create an instance of DIDResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -63,33 +63,29 @@
           are ignored.
         """
         _dict = self.model_dump(
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
-        # override the default output from pydantic by calling `to_dict()` of each item in results (list)
-        _items = []
-        if self.results:
-            for _item in self.results:
-                if _item:
-                    _items.append(_item.to_dict())
-            _dict["results"] = _items
+        # override the default output from pydantic by calling `to_dict()` of result
+        if self.result:
+            _dict["result"] = self.result.to_dict()
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of VCRecordList from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of DIDResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate(
             {
-                "results": [VCRecord.from_dict(_item) for _item in obj.get("results")]
-                if obj.get("results") is not None
+                "result": DID.from_dict(obj.get("result"))
+                if obj.get("result") is not None
                 else None
             }
         )
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/verify_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/write_ledger_request.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,49 +14,45 @@
 
 from __future__ import annotations
 
 import json
 import pprint
 from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, Field, StrictStr
+from pydantic import BaseModel, StrictStr
 
-from aries_cloudcontroller.models.signed_doc import SignedDoc
 from aries_cloudcontroller.util import DEFAULT_PYDANTIC_MODEL_CONFIG
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class VerifyRequest(BaseModel):
-    """
-    VerifyRequest
+class WriteLedgerRequest(BaseModel):
     """
+    WriteLedgerRequest
+    """  # noqa: E501
 
-    doc: Dict[str, Any]
-    verkey: Optional[StrictStr] = Field(
-        default=None, description="Verkey to use for doc verification"
-    )
-    __properties: ClassVar[List[str]] = ["doc", "verkey"]
+    ledger_id: Optional[StrictStr] = None
+    __properties: ClassVar[List[str]] = ["ledger_id"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of VerifyRequest from a JSON string"""
+        """Create an instance of WriteLedgerRequest from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -69,24 +65,17 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of VerifyRequest from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of WriteLedgerRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
-        _obj = cls.model_validate(
-            {
-                "doc": SignedDoc.from_dict(obj.get("doc"))
-                if obj.get("doc") is not None
-                else None,
-                "verkey": obj.get("verkey"),
-            }
-        )
+        _obj = cls.model_validate({"ledger_id": obj.get("ledger_id")})
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/verify_response.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/verify_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class VerifyResponse(BaseModel):
     """
     VerifyResponse
-    """
+    """  # noqa: E501
 
     error: Optional[StrictStr] = Field(default=None, description="Error text")
     valid: StrictBool
     __properties: ClassVar[List[str]] = ["error", "valid"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
@@ -66,15 +66,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of VerifyResponse from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/w3_c_credentials_list_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/w3_c_credentials_list_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class W3CCredentialsListRequest(BaseModel):
     """
     W3CCredentialsListRequest
-    """
+    """  # noqa: E501
 
     contexts: Optional[List[Annotated[str, Field(strict=True)]]] = None
     given_id: Optional[StrictStr] = Field(
         default=None, description="Given credential id to match"
     )
     issuer_id: Optional[StrictStr] = Field(
         default=None, description="Credential issuer identifier to match"
@@ -96,15 +96,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of W3CCredentialsListRequest from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_list.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class WalletList(BaseModel):
     """
     WalletList
-    """
+    """  # noqa: E501
 
     results: Optional[List[WalletRecord]] = Field(
         default=None, description="List of wallet records"
     )
     __properties: ClassVar[List[str]] = ["results"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
@@ -75,15 +75,15 @@
             for _item in self.results:
                 if _item:
                     _items.append(_item.to_dict())
             _dict["results"] = _items
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of WalletList from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_list_with_groups.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_list_with_groups.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from typing_extensions import Self
 
 
 class WalletListWithGroups(WalletList):
     results: Optional[List[WalletRecordWithGroups]] = None
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of WalletListWithGroups from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_record.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_record.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 except ImportError:
     from typing_extensions import Self
 
 
 class WalletRecord(BaseModel):
     """
     WalletRecord
-    """
+    """  # noqa: E501
 
     created_at: Optional[Annotated[str, Field(strict=True)]] = Field(
         default=None, description="Time of record creation"
     )
     key_management_mode: StrictStr = Field(
         description="Mode regarding management of wallet key"
     )
@@ -124,15 +124,15 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of WalletRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/wallet_record_with_groups.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/wallet_record_with_groups.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     from typing_extensions import Self
 
 
 class WalletRecordWithGroups(WalletRecord):
     group_id: Optional[str] = Field(None, examples=["SomeGroupId"])
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
+    def from_dict(cls, obj: Dict) -> Self:
         """Create an instance of WalletRecord from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller/models/write_ledger_request.py` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller/models/cred_revoked_result.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,45 +14,47 @@
 
 from __future__ import annotations
 
 import json
 import pprint
 from typing import Any, ClassVar, Dict, List, Optional
 
-from pydantic import BaseModel, StrictStr
+from pydantic import BaseModel, Field, StrictBool
 
 from aries_cloudcontroller.util import DEFAULT_PYDANTIC_MODEL_CONFIG
 
 try:
     from typing import Self
 except ImportError:
     from typing_extensions import Self
 
 
-class WriteLedgerRequest(BaseModel):
-    """
-    WriteLedgerRequest
+class CredRevokedResult(BaseModel):
     """
+    CredRevokedResult
+    """  # noqa: E501
 
-    ledger_id: Optional[StrictStr] = None
-    __properties: ClassVar[List[str]] = ["ledger_id"]
+    revoked: Optional[StrictBool] = Field(
+        default=None, description="Whether credential is revoked on the ledger"
+    )
+    __properties: ClassVar[List[str]] = ["revoked"]
 
     model_config = DEFAULT_PYDANTIC_MODEL_CONFIG
 
     def to_str(self) -> str:
         """Returns the string representation of the model using alias"""
         return pprint.pformat(self.model_dump(by_alias=True))
 
     def to_json(self) -> str:
         """Returns the JSON representation of the model using alias"""
         return self.model_dump_json(by_alias=True, exclude_unset=True)
 
     @classmethod
     def from_json(cls, json_str: str) -> Self:
-        """Create an instance of WriteLedgerRequest from a JSON string"""
+        """Create an instance of CredRevokedResult from a JSON string"""
         return cls.from_dict(json.loads(json_str))
 
     def to_dict(self) -> Dict[str, Any]:
         """Return the dictionary representation of the model using alias.
 
         This has the following differences from calling pydantic's
         `self.model_dump(by_alias=True)`:
@@ -65,17 +67,17 @@
             by_alias=True,
             exclude={},
             exclude_none=True,
         )
         return _dict
 
     @classmethod
-    def from_dict(cls, obj: dict) -> Self:
-        """Create an instance of WriteLedgerRequest from a dict"""
+    def from_dict(cls, obj: Dict) -> Self:
+        """Create an instance of CredRevokedResult from a dict"""
         if obj is None:
             return None
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
-        _obj = cls.model_validate({"ledger_id": obj.get("ledger_id")})
+        _obj = cls.model_validate({"revoked": obj.get("revoked")})
         return _obj
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/PKG-INFO` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,23 @@
 Metadata-Version: 2.1
 Name: aries-cloudcontroller
-Version: 0.9.0.post1
+Version: 0.9.0.post2
 Summary: A simple python client for controlling an ACA-Py agent
 Home-page: https://github.com/didx-xyz/aries-cloudcontroller-python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: aiohttp~=3.9.0
+Requires-Dist: pydantic~=2.5.1
+Requires-Dist: python-dateutil~=2.8.2
+Requires-Dist: typing-extensions~=4.8.0
+Requires-Dist: urllib3~=2.1.0
 
 <p align="center">
   <br />
   <img
     alt="Hyperledger Aries logo"
     src="https://raw.githubusercontent.com/didx-xyz/aries-cloudcontroller-python/main/assets/aries-logo.png"
     height="250px"
```

#### html2text {}

```diff
@@ -1,13 +1,16 @@
-Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.9.0.post1 Summary:
+Metadata-Version: 2.1 Name: aries-cloudcontroller Version: 0.9.0.post2 Summary:
 A simple python client for controlling an ACA-Py agent Home-page: https://
 github.com/didx-xyz/aries-cloudcontroller-python Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: Apache Software
 License Classifier: Operating System :: OS Independent Requires-Python: >=3.9
-Description-Content-Type: text/markdown License-File: LICENSE
+Description-Content-Type: text/markdown License-File: LICENSE Requires-Dist:
+aiohttp~=3.9.0 Requires-Dist: pydantic~=2.5.1 Requires-Dist: python-
+dateutil~=2.8.2 Requires-Dist: typing-extensions~=4.8.0 Requires-Dist:
+urllib3~=2.1.0
 
                            [Hyperledger Aries logo]
                   ************ AArriieess CClloouudd CCoonnttrroolllleerr PPyytthhoonn ************
        [Pipeline Status]_[_a_r_i_e_s_-_c_l_o_u_d_c_o_n_t_r_o_l_l_e_r_ _v_e_r_s_i_o_n_]_[_L_i_c_e_n_s_e_]_[_P_y_t_h_o_n_]
 
       _F_e_a_t_u_r_e_s  |  _U_s_a_g_e  |  _A_v_a_i_l_a_b_l_e_ _A_P_I_s  |  _C_o_n_t_r_i_b_u_t_i_n_g  |  _L_i_c_e_n_s_e
 The Aries CloudController is a client library, written in Python, for
```

### Comparing `aries_cloudcontroller-0.9.0.post1/aries_cloudcontroller.egg-info/SOURCES.txt` & `aries_cloudcontroller-0.9.0.post2/aries_cloudcontroller.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/setup.py` & `aries_cloudcontroller-0.9.0.post2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     lineiter = (line.strip() for line in open(filename))
     return [line for line in lineiter if line and not line.startswith("#")]
 
 
 if __name__ == "__main__":
     setup(
         name=PACKAGE_NAME,
-        version="0.9.0-rev1",
+        version="0.9.0-rev2",
         description="A simple python client for controlling an ACA-Py agent",
         long_description=long_description,
         long_description_content_type="text/markdown",
         url="https://github.com/didx-xyz/aries-cloudcontroller-python",
         packages=find_packages(),
         include_package_data=True,
         package_data={
```

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/client/test_acapy_client.py` & `aries_cloudcontroller-0.9.0.post2/tests/client/test_acapy_client.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_attach_decorator_data.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_attach_decorator_data.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_credential_definition.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_credential_definition.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_credential_offer.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_credential_offer.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_did.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_did.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_filter.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_filter.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_invitation.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_invitation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_presentation.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_presentation.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_v20_cred_ex_record.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_v20_cred_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/model/test_v20_pres_ex_record.py` & `aries_cloudcontroller-0.9.0.post2/tests/model/test_v20_pres_ex_record.py`

 * *Files identical despite different names*

### Comparing `aries_cloudcontroller-0.9.0.post1/tests/util/compare_dicts.py` & `aries_cloudcontroller-0.9.0.post2/tests/util/compare_dicts.py`

 * *Files identical despite different names*

