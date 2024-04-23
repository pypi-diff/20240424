# Comparing `tmp/affixapi-1.1.62.tar.gz` & `tmp/affixapi-1.1.63.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "affixapi-1.1.62.tar", last modified: Mon Apr 22 21:54:35 2024, max compression
+gzip compressed data, was "affixapi-1.1.63.tar", last modified: Mon Apr 22 23:16:58 2024, max compression
```

## Comparing `affixapi-1.1.62.tar` & `affixapi-1.1.63.tar`

### file list

```diff
@@ -1,158 +1,156 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.877404 affixapi-1.1.62/
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-22 21:54:32.000000 affixapi-1.1.62/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    21929 2024-04-22 21:54:35.877404 affixapi-1.1.62/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    21577 2024-04-22 21:54:32.000000 affixapi-1.1.62/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.877404 affixapi-1.1.62/affixapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    21929 2024-04-22 21:54:35.000000 affixapi-1.1.62/affixapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5850 2024-04-22 21:54:35.000000 affixapi-1.1.62/affixapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 21:54:35.000000 affixapi-1.1.62/affixapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 21:54:35.000000 affixapi-1.1.62/affixapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 21:54:35.000000 affixapi-1.1.62/affixapi.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.853404 affixapi-1.1.62/openapi_client/
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.853404 affixapi-1.1.62/openapi_client/api/
--rw-r--r--   0 runner    (1001) docker     (127)    53338 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/api/2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/api/core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/api/management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    53353 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/api/xhr__vertically_integrated_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.853404 affixapi-1.1.62/openapi_client/apis/
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/apis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.865404 affixapi-1.1.62/openapi_client/model/
--rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18293 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16613 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employment_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    16583 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employment_status_not_null.py
--rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model/work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/model_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.865404 affixapi-1.1.62/openapi_client/models/
--rw-r--r--   0 runner    (1001) docker     (127)     5096 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-22 21:54:32.000000 affixapi-1.1.62/openapi_client/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 21:54:35.877404 affixapi-1.1.62/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 21:54:32.000000 affixapi-1.1.62/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 21:54:35.877404 affixapi-1.1.62/test/
--rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_2023_03_01_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_address_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_address_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_client_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_client_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_companies20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_company_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_core_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_create_employee_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_create_employee_request_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_create_employee_request_dependents.py
--rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_create_employee_request_emergency_contacts.py
--rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_create_employee_request_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_currency_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_currency_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_disconnect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employee_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employee_response_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employees20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employment_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employment_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employment_status.py
--rw-r--r--   0 runner    (1001) docker     (127)    10366 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employment_status_not_null.py
--rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employment_status_not_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_employment_status_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_group_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_group_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_groups20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_groups_no_null_enum_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_id_and_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_identity_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_inline_response400.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_inline_response401.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_inline_response409.py
--rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_introspect_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_location_no_non_null_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_location_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_management_api.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_message_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_mode_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_mode_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payrun_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payruns20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payslip_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payslip_response_contributions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payslip_response_deductions.py
--rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payslip_response_earnings.py
--rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payslip_response_taxes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_payslips20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_provider_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_provider_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_providers_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_scopes_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_scopes_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_time_off_balance_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_time_off_balances20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_time_off_entries20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_time_off_entry_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_timesheet_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_timesheets20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_token_request.py
--rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_token_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_tokens_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_work_locations20230301_response.py
--rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-22 21:54:32.000000 affixapi-1.1.62/test/test_xhr__vertically_integrated_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.683570 affixapi-1.1.63/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-22 23:16:55.000000 affixapi-1.1.63/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    21927 2024-04-22 23:16:58.683570 affixapi-1.1.63/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    21575 2024-04-22 23:16:55.000000 affixapi-1.1.63/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.683570 affixapi-1.1.63/affixapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    21927 2024-04-22 23:16:58.000000 affixapi-1.1.63/affixapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5803 2024-04-22 23:16:58.000000 affixapi-1.1.63/affixapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-22 23:16:58.000000 affixapi-1.1.63/affixapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-22 23:16:58.000000 affixapi-1.1.63/affixapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-22 23:16:58.000000 affixapi-1.1.63/affixapi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.659569 affixapi-1.1.63/openapi_client/
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.659569 affixapi-1.1.63/openapi_client/api/
+-rw-r--r--   0 runner    (1001) docker     (127)    53384 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/api/2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      219 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14368 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/api/core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35533 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/api/management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53399 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/api/xhr__vertically_integrated_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46350 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.659569 affixapi-1.1.63/openapi_client/apis/
+-rw-r--r--   0 runner    (1001) docker     (127)      672 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/apis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27003 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14609 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.671569 affixapi-1.1.63/openapi_client/model/
+-rw-r--r--   0 runner    (1001) docker     (127)      348 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18281 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18293 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17178 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17416 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16480 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17198 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24128 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16862 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16299 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17045 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16825 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16485 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16517 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16360 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16953 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16487 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18034 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16580 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16597 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16629 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16766 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16776 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16493 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16561 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16285 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16640 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16204 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17703 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16690 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17253 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17205 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17138 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16053 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16418 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16420 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17525 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16469 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19501 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16235 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16229 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16434 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16478 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18880 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16463 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18962 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18964 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17983 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16543 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18715 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17690 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16496 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17797 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17631 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16457 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16527 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model/work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    84300 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/model_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.671569 affixapi-1.1.63/openapi_client/models/
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22042 2024-04-22 23:16:55.000000 affixapi-1.1.63/openapi_client/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-22 23:16:58.683570 affixapi-1.1.63/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1008 2024-04-22 23:16:55.000000 affixapi-1.1.63/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-22 23:16:58.683570 affixapi-1.1.63/test/
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_2023_03_01_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10367 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_address_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_address_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_client_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_client_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10491 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_companies20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_company_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10217 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_core_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11877 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_create_employee_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10430 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_create_employee_request_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10422 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_create_employee_request_dependents.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10472 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_create_employee_request_emergency_contacts.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10401 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_create_employee_request_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_currency_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_currency_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10329 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_disconnect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11678 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employee_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employee_response_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10495 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employees20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10538 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employment_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10446 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employment_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10445 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employment_status_not_null_not_nullable.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10416 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employment_status_not_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10372 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_employment_status_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_group_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_group_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10462 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_groups20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10511 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_groups_no_null_enum_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_id_and_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_identity_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_inline_response400.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_inline_response401.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_inline_response409.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10656 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_introspect_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_location_no_non_null_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10428 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_location_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10871 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_management_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_message_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10280 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_mode_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_mode_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payrun_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10473 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payruns20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10908 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payslip_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10400 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payslip_response_contributions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10379 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payslip_response_deductions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10365 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payslip_response_earnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10344 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payslip_response_taxes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10484 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_payslips20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_provider_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10315 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_provider_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_providers_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10294 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_scopes_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_scopes_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10359 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_time_off_balance_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10565 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_time_off_balances20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10550 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_time_off_entries20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10345 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_time_off_entry_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10322 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_timesheet_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10506 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_timesheets20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10287 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_token_request.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10621 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_token_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10301 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_tokens_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10524 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_work_locations20230301_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11711 2024-04-22 23:16:55.000000 affixapi-1.1.63/test/test_xhr__vertically_integrated_api.py
```

### Comparing `affixapi-1.1.62/LICENSE` & `affixapi-1.1.63/LICENSE`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/PKG-INFO` & `affixapi-1.1.63/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.62
+Version: 1.1.63
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -268,15 +268,15 @@
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
-from openapi_client.model.employment_status_not_null import EmploymentStatusNotNull
+from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -366,16 +366,15 @@
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
- - [EmploymentStatus](docs/EmploymentStatus.md)
- - [EmploymentStatusNotNull](docs/EmploymentStatusNotNull.md)
+ - [EmploymentStatusNotNullNotNullable](docs/EmploymentStatusNotNullNotNullable.md)
  - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
  - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
  - [IdAndMessageResponse](docs/IdAndMessageResponse.md)
```

### Comparing `affixapi-1.1.62/README.md` & `affixapi-1.1.63/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -254,15 +254,15 @@
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
-from openapi_client.model.employment_status_not_null import EmploymentStatusNotNull
+from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -352,16 +352,15 @@
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
- - [EmploymentStatus](docs/EmploymentStatus.md)
- - [EmploymentStatusNotNull](docs/EmploymentStatusNotNull.md)
+ - [EmploymentStatusNotNullNotNullable](docs/EmploymentStatusNotNullNotNullable.md)
  - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
  - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
  - [IdAndMessageResponse](docs/IdAndMessageResponse.md)
```

### Comparing `affixapi-1.1.62/affixapi.egg-info/PKG-INFO` & `affixapi-1.1.63/affixapi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: affixapi
-Version: 1.1.62
+Version: 1.1.63
 Summary: Affix API
 Home-page: 
 Author: OpenAPI Generator community
 Author-email: developers@affixapi.com
 Keywords: OpenAPI,OpenAPI-Generator,Affix API
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
@@ -268,15 +268,15 @@
 
 import time
 import openapi_client
 from pprint import pprint
 from openapi_client.api import 2023_03_01_api
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
-from openapi_client.model.employment_status_not_null import EmploymentStatusNotNull
+from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -366,16 +366,15 @@
  - [CurrencyResponse](docs/CurrencyResponse.md)
  - [DisconnectResponse](docs/DisconnectResponse.md)
  - [EmployeeResponse](docs/EmployeeResponse.md)
  - [EmployeeResponseManager](docs/EmployeeResponseManager.md)
  - [Employees20230301Response](docs/Employees20230301Response.md)
  - [EmploymentNoNullEnumRequest](docs/EmploymentNoNullEnumRequest.md)
  - [EmploymentResponse](docs/EmploymentResponse.md)
- - [EmploymentStatus](docs/EmploymentStatus.md)
- - [EmploymentStatusNotNull](docs/EmploymentStatusNotNull.md)
+ - [EmploymentStatusNotNullNotNullable](docs/EmploymentStatusNotNullNotNullable.md)
  - [EmploymentStatusNotNullRequest](docs/EmploymentStatusNotNullRequest.md)
  - [EmploymentStatusResponse](docs/EmploymentStatusResponse.md)
  - [GroupNoNullEnumRequest](docs/GroupNoNullEnumRequest.md)
  - [GroupResponse](docs/GroupResponse.md)
  - [Groups20230301Response](docs/Groups20230301Response.md)
  - [GroupsNoNullEnumRequest](docs/GroupsNoNullEnumRequest.md)
  - [IdAndMessageResponse](docs/IdAndMessageResponse.md)
```

### Comparing `affixapi-1.1.62/affixapi.egg-info/SOURCES.txt` & `affixapi-1.1.63/affixapi.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -35,16 +35,15 @@
 openapi_client/model/currency_response.py
 openapi_client/model/disconnect_response.py
 openapi_client/model/employee_response.py
 openapi_client/model/employee_response_manager.py
 openapi_client/model/employees20230301_response.py
 openapi_client/model/employment_no_null_enum_request.py
 openapi_client/model/employment_response.py
-openapi_client/model/employment_status.py
-openapi_client/model/employment_status_not_null.py
+openapi_client/model/employment_status_not_null_not_nullable.py
 openapi_client/model/employment_status_not_null_request.py
 openapi_client/model/employment_status_response.py
 openapi_client/model/group_no_null_enum_request.py
 openapi_client/model/group_response.py
 openapi_client/model/groups20230301_response.py
 openapi_client/model/groups_no_null_enum_request.py
 openapi_client/model/id_and_message_response.py
@@ -99,16 +98,15 @@
 test/test_currency_response.py
 test/test_disconnect_response.py
 test/test_employee_response.py
 test/test_employee_response_manager.py
 test/test_employees20230301_response.py
 test/test_employment_no_null_enum_request.py
 test/test_employment_response.py
-test/test_employment_status.py
-test/test_employment_status_not_null.py
+test/test_employment_status_not_null_not_nullable.py
 test/test_employment_status_not_null_request.py
 test/test_employment_status_response.py
 test/test_group_no_null_enum_request.py
 test/test_group_response.py
 test/test_groups20230301_response.py
 test/test_groups_no_null_enum_request.py
 test/test_id_and_message_response.py
```

### Comparing `affixapi-1.1.62/openapi_client/__init__.py` & `affixapi-1.1.63/openapi_client/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/api/2023_03_01_api.py` & `affixapi-1.1.63/openapi_client/api/2023_03_01_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
-from openapi_client.model.employment_status_not_null import EmploymentStatusNotNull
+from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -167,15 +167,15 @@
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.xhr_employees20230301(async_req=True)
             >>> result = thread.get()
 
 
             Keyword Args:
-                employment_status (EmploymentStatusNotNull): Enable server-side filtering of the `employment_status` attribute. Will only include individuals with that attribute explicitly set (ie if an individuals has a `null`, it will not be returned if this parameter is set) . [optional]
+                employment_status (EmploymentStatusNotNullNotNullable): Enable server-side filtering of the `employment_status` attribute. Will only include individuals with that attribute explicitly set (ie if an individuals has a `null`, it will not be returned if this parameter is set) . [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (float/tuple): timeout setting for this request. If one
                     number provided, it will be total request timeout. It can also
@@ -244,15 +244,15 @@
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'employment_status':
-                        (EmploymentStatusNotNull,),
+                        (EmploymentStatusNotNullNotNullable,),
                 },
                 'attribute_map': {
                     'employment_status': 'employment_status',
                 },
                 'location_map': {
                     'employment_status': 'query',
                 },
```

### Comparing `affixapi-1.1.62/openapi_client/api/core_api.py` & `affixapi-1.1.63/openapi_client/api/core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/api/management_api.py` & `affixapi-1.1.63/openapi_client/api/management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/api/xhr__vertically_integrated_api.py` & `affixapi-1.1.63/openapi_client/api/xhr__vertically_integrated_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     datetime,
     file_type,
     none_type,
     validate_and_convert_types
 )
 from openapi_client.model.companies20230301_response import Companies20230301Response
 from openapi_client.model.employees20230301_response import Employees20230301Response
-from openapi_client.model.employment_status_not_null import EmploymentStatusNotNull
+from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.identity_response import IdentityResponse
 from openapi_client.model.inline_response401 import InlineResponse401
 from openapi_client.model.message_response import MessageResponse
 from openapi_client.model.payruns20230301_response import Payruns20230301Response
 from openapi_client.model.payslips20230301_response import Payslips20230301Response
 from openapi_client.model.time_off_balances20230301_response import TimeOffBalances20230301Response
@@ -167,15 +167,15 @@
             asynchronous HTTP request, please pass async_req=True
 
             >>> thread = api.xhr_employees20230301(async_req=True)
             >>> result = thread.get()
 
 
             Keyword Args:
-                employment_status (EmploymentStatusNotNull): Enable server-side filtering of the `employment_status` attribute. Will only include individuals with that attribute explicitly set (ie if an individuals has a `null`, it will not be returned if this parameter is set) . [optional]
+                employment_status (EmploymentStatusNotNullNotNullable): Enable server-side filtering of the `employment_status` attribute. Will only include individuals with that attribute explicitly set (ie if an individuals has a `null`, it will not be returned if this parameter is set) . [optional]
                 _return_http_data_only (bool): response data without head status
                     code and headers. Default is True.
                 _preload_content (bool): if False, the urllib3.HTTPResponse object
                     will be returned without reading/decoding response data.
                     Default is True.
                 _request_timeout (float/tuple): timeout setting for this request. If one
                     number provided, it will be total request timeout. It can also
@@ -244,15 +244,15 @@
             root_map={
                 'validations': {
                 },
                 'allowed_values': {
                 },
                 'openapi_types': {
                     'employment_status':
-                        (EmploymentStatusNotNull,),
+                        (EmploymentStatusNotNullNotNullable,),
                 },
                 'attribute_map': {
                     'employment_status': 'employment_status',
                 },
                 'location_map': {
                     'employment_status': 'query',
                 },
```

### Comparing `affixapi-1.1.62/openapi_client/api_client.py` & `affixapi-1.1.63/openapi_client/api_client.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/apis/__init__.py` & `affixapi-1.1.63/openapi_client/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/configuration.py` & `affixapi-1.1.63/openapi_client/configuration.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/exceptions.py` & `affixapi-1.1.63/openapi_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/address_no_non_null_request.py` & `affixapi-1.1.63/openapi_client/model/address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/address_response.py` & `affixapi-1.1.63/openapi_client/model/address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/client_request.py` & `affixapi-1.1.63/openapi_client/model/client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/client_response.py` & `affixapi-1.1.63/openapi_client/model/client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/companies20230301_response.py` & `affixapi-1.1.63/openapi_client/model/companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/company_response.py` & `affixapi-1.1.63/openapi_client/model/company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/create_employee_request.py` & `affixapi-1.1.63/openapi_client/model/create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/create_employee_request_bank_account.py` & `affixapi-1.1.63/openapi_client/model/create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/create_employee_request_dependents.py` & `affixapi-1.1.63/openapi_client/model/create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/create_employee_request_emergency_contacts.py` & `affixapi-1.1.63/openapi_client/model/create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/create_employee_request_manager.py` & `affixapi-1.1.63/openapi_client/model/create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/currency_not_null_request.py` & `affixapi-1.1.63/openapi_client/model/currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/currency_response.py` & `affixapi-1.1.63/openapi_client/model/currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/disconnect_response.py` & `affixapi-1.1.63/openapi_client/model/disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/employee_response.py` & `affixapi-1.1.63/openapi_client/model/employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/employee_response_manager.py` & `affixapi-1.1.63/openapi_client/model/employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/employees20230301_response.py` & `affixapi-1.1.63/openapi_client/model/employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/employment_no_null_enum_request.py` & `affixapi-1.1.63/openapi_client/model/employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/employment_response.py` & `affixapi-1.1.63/openapi_client/model/employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/employment_status.py` & `affixapi-1.1.63/openapi_client/model/employment_status_not_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class EmploymentStatus(ModelSimple):
+class EmploymentStatusNotNullRequest(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -47,15 +47,14 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
             'None': None,
-            'NULL': "null",
             'ACTIVE': "active",
             'INACTIVE': "inactive",
             'PENDING': "pending",
             'LEAVE': "leave",
         },
     }
 
@@ -96,23 +95,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """EmploymentStatus - a model defined in OpenAPI
+        """EmploymentStatusNotNullRequest - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["null", "active", "inactive", "pending", "leave", ]  # noqa: E501
+            args[0] (str):, must be one of ["active", "inactive", "pending", "leave", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["null", "active", "inactive", "pending", "leave", ]  # noqa: E501
+            value (str):, must be one of ["active", "inactive", "pending", "leave", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.62/openapi_client/model/employment_status_not_null.py` & `affixapi-1.1.63/openapi_client/model/employment_status_not_null_not_nullable.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class EmploymentStatusNotNull(ModelSimple):
+class EmploymentStatusNotNullNotNullable(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -46,28 +46,27 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'None': None,
             'ACTIVE': "active",
             'INACTIVE': "inactive",
             'PENDING': "pending",
             'LEAVE': "leave",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
-    _nullable = True
+    _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
@@ -95,15 +94,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """EmploymentStatusNotNull - a model defined in OpenAPI
+        """EmploymentStatusNotNullNotNullable - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
             args[0] (str):, must be one of ["active", "inactive", "pending", "leave", ]  # noqa: E501
 
         Keyword Args:
```

### Comparing `affixapi-1.1.62/openapi_client/model/employment_status_not_null_request.py` & `affixapi-1.1.63/openapi_client/model/employment_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class EmploymentStatusNotNullRequest(ModelSimple):
+class EmploymentStatusResponse(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -47,14 +47,15 @@
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
             'None': None,
+            'NULL': "null",
             'ACTIVE': "active",
             'INACTIVE': "inactive",
             'PENDING': "pending",
             'LEAVE': "leave",
         },
     }
 
@@ -95,23 +96,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """EmploymentStatusNotNullRequest - a model defined in OpenAPI
+        """EmploymentStatusResponse - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["active", "inactive", "pending", "leave", ]  # noqa: E501
+            args[0] (str):, must be one of ["null", "active", "inactive", "pending", "leave", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["active", "inactive", "pending", "leave", ]  # noqa: E501
+            value (str):, must be one of ["null", "active", "inactive", "pending", "leave", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.62/openapi_client/model/employment_status_response.py` & `affixapi-1.1.63/openapi_client/model/mode_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 
-class EmploymentStatusResponse(ModelSimple):
+class ModeResponse(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -46,29 +46,25 @@
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
         ('value',): {
-            'None': None,
-            'NULL': "null",
-            'ACTIVE': "active",
-            'INACTIVE': "inactive",
-            'PENDING': "pending",
-            'LEAVE': "leave",
+            'OFFICIAL': "official",
+            'XHR': "xhr",
         },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
-    _nullable = True
+    _nullable = False
 
     @cached_property
     def openapi_types():
         """
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
@@ -96,23 +92,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """EmploymentStatusResponse - a model defined in OpenAPI
+        """ModeResponse - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["null", "active", "inactive", "pending", "leave", ]  # noqa: E501
+            args[0] (str):, must be one of ["official", "xhr", ]  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["null", "active", "inactive", "pending", "leave", ]  # noqa: E501
+            value (str):, must be one of ["official", "xhr", ]  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.62/openapi_client/model/group_no_null_enum_request.py` & `affixapi-1.1.63/openapi_client/model/group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/group_response.py` & `affixapi-1.1.63/openapi_client/model/group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/groups20230301_response.py` & `affixapi-1.1.63/openapi_client/model/groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/groups_no_null_enum_request.py` & `affixapi-1.1.63/openapi_client/model/groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/id_and_message_response.py` & `affixapi-1.1.63/openapi_client/model/id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/identity_response.py` & `affixapi-1.1.63/openapi_client/model/identity_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/inline_response400.py` & `affixapi-1.1.63/openapi_client/model/inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/inline_response401.py` & `affixapi-1.1.63/openapi_client/model/inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/inline_response409.py` & `affixapi-1.1.63/openapi_client/model/inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/introspect_response.py` & `affixapi-1.1.63/openapi_client/model/introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/location_no_non_null_request.py` & `affixapi-1.1.63/openapi_client/model/location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/location_response.py` & `affixapi-1.1.63/openapi_client/model/location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/message_response.py` & `affixapi-1.1.63/openapi_client/model/message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/mode_request.py` & `affixapi-1.1.63/openapi_client/model/mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/mode_response.py` & `affixapi-1.1.63/openapi_client/model/timesheets20230301_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,20 @@
     date,
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
+def lazy_import():
+    from openapi_client.model.timesheet_response import TimesheetResponse
+    globals()['TimesheetResponse'] = TimesheetResponse
 
-class ModeResponse(ModelSimple):
+
+class Timesheets20230301Response(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -45,18 +49,14 @@
           min_items, exclusive_maximum, inclusive_maximum, exclusive_minimum,
           inclusive_minimum, and regex.
       additional_properties_type (tuple): A tuple of classes accepted
           as additional properties values.
     """
 
     allowed_values = {
-        ('value',): {
-            'OFFICIAL': "official",
-            'XHR': "xhr",
-        },
     }
 
     validations = {
     }
 
     additional_properties_type = None
 
@@ -68,16 +68,17 @@
         This must be a method because a model may have properties that are
         of type self, this must run after the class is loaded
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
+        lazy_import()
         return {
-            'value': (str,),
+            'value': ([TimesheetResponse],),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -92,23 +93,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """ModeResponse - a model defined in OpenAPI
+        """Timesheets20230301Response - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] (str):, must be one of ["official", "xhr", ]  # noqa: E501
+            args[0] ([TimesheetResponse]):  # noqa: E501
 
         Keyword Args:
-            value (str):, must be one of ["official", "xhr", ]  # noqa: E501
+            value ([TimesheetResponse]):  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.62/openapi_client/model/payrun_response.py` & `affixapi-1.1.63/openapi_client/model/payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/payruns20230301_response.py` & `affixapi-1.1.63/openapi_client/model/payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/payslip_response.py` & `affixapi-1.1.63/openapi_client/model/payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/payslip_response_contributions.py` & `affixapi-1.1.63/openapi_client/model/payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/payslip_response_deductions.py` & `affixapi-1.1.63/openapi_client/model/payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/payslip_response_earnings.py` & `affixapi-1.1.63/openapi_client/model/payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/payslip_response_taxes.py` & `affixapi-1.1.63/openapi_client/model/payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/payslips20230301_response.py` & `affixapi-1.1.63/openapi_client/model/payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/provider_request.py` & `affixapi-1.1.63/openapi_client/model/provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/provider_response.py` & `affixapi-1.1.63/openapi_client/model/provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/providers_response.py` & `affixapi-1.1.63/openapi_client/model/providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/scopes_request.py` & `affixapi-1.1.63/openapi_client/model/scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/scopes_response.py` & `affixapi-1.1.63/openapi_client/model/scopes_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/time_off_balance_response.py` & `affixapi-1.1.63/openapi_client/model/time_off_balance_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/time_off_balances20230301_response.py` & `affixapi-1.1.63/openapi_client/model/time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/time_off_entries20230301_response.py` & `affixapi-1.1.63/openapi_client/model/time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/time_off_entry_response.py` & `affixapi-1.1.63/openapi_client/model/time_off_entry_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/timesheet_response.py` & `affixapi-1.1.63/openapi_client/model/timesheet_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/timesheets20230301_response.py` & `affixapi-1.1.63/openapi_client/model/work_locations20230301_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,19 +24,19 @@
     datetime,
     file_type,
     none_type,
     validate_get_composed_info,
 )
 
 def lazy_import():
-    from openapi_client.model.timesheet_response import TimesheetResponse
-    globals()['TimesheetResponse'] = TimesheetResponse
+    from openapi_client.model.location_response import LocationResponse
+    globals()['LocationResponse'] = LocationResponse
 
 
-class Timesheets20230301Response(ModelSimple):
+class WorkLocations20230301Response(ModelSimple):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -70,15 +70,15 @@
 
         Returns
             openapi_types (dict): The key is attribute name
                 and the value is attribute type.
         """
         lazy_import()
         return {
-            'value': ([TimesheetResponse],),
+            'value': ([LocationResponse],),
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -93,23 +93,23 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):
-        """Timesheets20230301Response - a model defined in OpenAPI
+        """WorkLocations20230301Response - a model defined in OpenAPI
 
         Note that value can be passed either in args or in kwargs, but not in both.
 
         Args:
-            args[0] ([TimesheetResponse]):  # noqa: E501
+            args[0] ([LocationResponse]): Work locations.  # noqa: E501
 
         Keyword Args:
-            value ([TimesheetResponse]):  # noqa: E501
+            value ([LocationResponse]): Work locations.  # noqa: E501
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
                                 drill down to the model in received_data
                                 when deserializing a response
```

### Comparing `affixapi-1.1.62/openapi_client/model/token_request.py` & `affixapi-1.1.63/openapi_client/model/token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/token_response.py` & `affixapi-1.1.63/openapi_client/model/token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model/tokens_response.py` & `affixapi-1.1.63/openapi_client/model/tokens_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/model_utils.py` & `affixapi-1.1.63/openapi_client/model_utils.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/openapi_client/models/__init__.py` & `affixapi-1.1.63/openapi_client/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,16 +24,15 @@
 from openapi_client.model.currency_response import CurrencyResponse
 from openapi_client.model.disconnect_response import DisconnectResponse
 from openapi_client.model.employee_response import EmployeeResponse
 from openapi_client.model.employee_response_manager import EmployeeResponseManager
 from openapi_client.model.employees20230301_response import Employees20230301Response
 from openapi_client.model.employment_no_null_enum_request import EmploymentNoNullEnumRequest
 from openapi_client.model.employment_response import EmploymentResponse
-from openapi_client.model.employment_status import EmploymentStatus
-from openapi_client.model.employment_status_not_null import EmploymentStatusNotNull
+from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
 from openapi_client.model.employment_status_response import EmploymentStatusResponse
 from openapi_client.model.group_no_null_enum_request import GroupNoNullEnumRequest
 from openapi_client.model.group_response import GroupResponse
 from openapi_client.model.groups20230301_response import Groups20230301Response
 from openapi_client.model.groups_no_null_enum_request import GroupsNoNullEnumRequest
 from openapi_client.model.id_and_message_response import IdAndMessageResponse
```

### Comparing `affixapi-1.1.62/openapi_client/rest.py` & `affixapi-1.1.63/openapi_client/rest.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/setup.py` & `affixapi-1.1.63/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 ## -> generated (previously)
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "affixapi"
-VERSION = "1.1.62"
+VERSION = "1.1.63"
 
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `affixapi-1.1.62/test/test_2023_03_01_api.py` & `affixapi-1.1.63/test/test_2023_03_01_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_address_no_non_null_request.py` & `affixapi-1.1.63/test/test_address_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_address_response.py` & `affixapi-1.1.63/test/test_address_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_client_request.py` & `affixapi-1.1.63/test/test_client_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_client_response.py` & `affixapi-1.1.63/test/test_client_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_companies20230301_response.py` & `affixapi-1.1.63/test/test_companies20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_company_response.py` & `affixapi-1.1.63/test/test_company_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_core_api.py` & `affixapi-1.1.63/test/test_core_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_create_employee_request.py` & `affixapi-1.1.63/test/test_create_employee_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_create_employee_request_bank_account.py` & `affixapi-1.1.63/test/test_create_employee_request_bank_account.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_create_employee_request_dependents.py` & `affixapi-1.1.63/test/test_create_employee_request_dependents.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_create_employee_request_emergency_contacts.py` & `affixapi-1.1.63/test/test_create_employee_request_emergency_contacts.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_create_employee_request_manager.py` & `affixapi-1.1.63/test/test_create_employee_request_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_currency_not_null_request.py` & `affixapi-1.1.63/test/test_currency_not_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_currency_response.py` & `affixapi-1.1.63/test/test_currency_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_disconnect_response.py` & `affixapi-1.1.63/test/test_disconnect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_employee_response.py` & `affixapi-1.1.63/test/test_employee_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_employee_response_manager.py` & `affixapi-1.1.63/test/test_employee_response_manager.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_employees20230301_response.py` & `affixapi-1.1.63/test/test_employees20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_employment_no_null_enum_request.py` & `affixapi-1.1.63/test/test_employment_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_employment_response.py` & `affixapi-1.1.63/test/test_employment_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_employment_status.py` & `affixapi-1.1.63/test/test_employment_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.employment_status import EmploymentStatus
+from openapi_client.model.employment_status_response import EmploymentStatusResponse
 
 
-class TestEmploymentStatus(unittest.TestCase):
-    """EmploymentStatus unit test stubs"""
+class TestEmploymentStatusResponse(unittest.TestCase):
+    """EmploymentStatusResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentStatus(self):
-        """Test EmploymentStatus"""
+    def testEmploymentStatusResponse(self):
+        """Test EmploymentStatusResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentStatus()  # noqa: E501
+        # model = EmploymentStatusResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_employment_status_not_null.py` & `affixapi-1.1.63/test/test_employment_status_not_null_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.employment_status_not_null import EmploymentStatusNotNull
+from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
 
 
-class TestEmploymentStatusNotNull(unittest.TestCase):
-    """EmploymentStatusNotNull unit test stubs"""
+class TestEmploymentStatusNotNullRequest(unittest.TestCase):
+    """EmploymentStatusNotNullRequest unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentStatusNotNull(self):
-        """Test EmploymentStatusNotNull"""
+    def testEmploymentStatusNotNullRequest(self):
+        """Test EmploymentStatusNotNullRequest"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentStatusNotNull()  # noqa: E501
+        # model = EmploymentStatusNotNullRequest()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_employment_status_not_null_request.py` & `affixapi-1.1.63/test/test_message_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.employment_status_not_null_request import EmploymentStatusNotNullRequest
+from openapi_client.model.message_response import MessageResponse
 
 
-class TestEmploymentStatusNotNullRequest(unittest.TestCase):
-    """EmploymentStatusNotNullRequest unit test stubs"""
+class TestMessageResponse(unittest.TestCase):
+    """MessageResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentStatusNotNullRequest(self):
-        """Test EmploymentStatusNotNullRequest"""
+    def testMessageResponse(self):
+        """Test MessageResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentStatusNotNullRequest()  # noqa: E501
+        # model = MessageResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_employment_status_response.py` & `affixapi-1.1.63/test/test_identity_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.employment_status_response import EmploymentStatusResponse
+from openapi_client.model.identity_response import IdentityResponse
 
 
-class TestEmploymentStatusResponse(unittest.TestCase):
-    """EmploymentStatusResponse unit test stubs"""
+class TestIdentityResponse(unittest.TestCase):
+    """IdentityResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testEmploymentStatusResponse(self):
-        """Test EmploymentStatusResponse"""
+    def testIdentityResponse(self):
+        """Test IdentityResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = EmploymentStatusResponse()  # noqa: E501
+        # model = IdentityResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_group_no_null_enum_request.py` & `affixapi-1.1.63/test/test_group_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_group_response.py` & `affixapi-1.1.63/test/test_group_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_groups20230301_response.py` & `affixapi-1.1.63/test/test_groups20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_groups_no_null_enum_request.py` & `affixapi-1.1.63/test/test_groups_no_null_enum_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_id_and_message_response.py` & `affixapi-1.1.63/test/test_id_and_message_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_identity_response.py` & `affixapi-1.1.63/test/test_time_off_balance_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.identity_response import IdentityResponse
+from openapi_client.model.time_off_balance_response import TimeOffBalanceResponse
 
 
-class TestIdentityResponse(unittest.TestCase):
-    """IdentityResponse unit test stubs"""
+class TestTimeOffBalanceResponse(unittest.TestCase):
+    """TimeOffBalanceResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testIdentityResponse(self):
-        """Test IdentityResponse"""
+    def testTimeOffBalanceResponse(self):
+        """Test TimeOffBalanceResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = IdentityResponse()  # noqa: E501
+        # model = TimeOffBalanceResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_inline_response400.py` & `affixapi-1.1.63/test/test_inline_response400.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_inline_response401.py` & `affixapi-1.1.63/test/test_inline_response401.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_inline_response409.py` & `affixapi-1.1.63/test/test_inline_response409.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_introspect_response.py` & `affixapi-1.1.63/test/test_introspect_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_location_no_non_null_request.py` & `affixapi-1.1.63/test/test_location_no_non_null_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_location_response.py` & `affixapi-1.1.63/test/test_location_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_management_api.py` & `affixapi-1.1.63/test/test_management_api.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_message_response.py` & `affixapi-1.1.63/test/test_scopes_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.message_response import MessageResponse
+from openapi_client.model.scopes_response import ScopesResponse
 
 
-class TestMessageResponse(unittest.TestCase):
-    """MessageResponse unit test stubs"""
+class TestScopesResponse(unittest.TestCase):
+    """ScopesResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMessageResponse(self):
-        """Test MessageResponse"""
+    def testScopesResponse(self):
+        """Test ScopesResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = MessageResponse()  # noqa: E501
+        # model = ScopesResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_mode_request.py` & `affixapi-1.1.63/test/test_mode_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_mode_response.py` & `affixapi-1.1.63/test/test_mode_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payrun_response.py` & `affixapi-1.1.63/test/test_payrun_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payruns20230301_response.py` & `affixapi-1.1.63/test/test_payruns20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payslip_response.py` & `affixapi-1.1.63/test/test_payslip_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payslip_response_contributions.py` & `affixapi-1.1.63/test/test_payslip_response_contributions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payslip_response_deductions.py` & `affixapi-1.1.63/test/test_payslip_response_deductions.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payslip_response_earnings.py` & `affixapi-1.1.63/test/test_payslip_response_earnings.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payslip_response_taxes.py` & `affixapi-1.1.63/test/test_payslip_response_taxes.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_payslips20230301_response.py` & `affixapi-1.1.63/test/test_payslips20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_provider_request.py` & `affixapi-1.1.63/test/test_provider_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_provider_response.py` & `affixapi-1.1.63/test/test_provider_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_providers_response.py` & `affixapi-1.1.63/test/test_providers_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_scopes_request.py` & `affixapi-1.1.63/test/test_scopes_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_scopes_response.py` & `affixapi-1.1.63/test/test_timesheet_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.scopes_response import ScopesResponse
+from openapi_client.model.timesheet_response import TimesheetResponse
 
 
-class TestScopesResponse(unittest.TestCase):
-    """ScopesResponse unit test stubs"""
+class TestTimesheetResponse(unittest.TestCase):
+    """TimesheetResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testScopesResponse(self):
-        """Test ScopesResponse"""
+    def testTimesheetResponse(self):
+        """Test TimesheetResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = ScopesResponse()  # noqa: E501
+        # model = TimesheetResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_time_off_balance_response.py` & `affixapi-1.1.63/test/test_time_off_entry_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.time_off_balance_response import TimeOffBalanceResponse
+from openapi_client.model.time_off_entry_response import TimeOffEntryResponse
 
 
-class TestTimeOffBalanceResponse(unittest.TestCase):
-    """TimeOffBalanceResponse unit test stubs"""
+class TestTimeOffEntryResponse(unittest.TestCase):
+    """TimeOffEntryResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTimeOffBalanceResponse(self):
-        """Test TimeOffBalanceResponse"""
+    def testTimeOffEntryResponse(self):
+        """Test TimeOffEntryResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TimeOffBalanceResponse()  # noqa: E501
+        # model = TimeOffEntryResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_time_off_balances20230301_response.py` & `affixapi-1.1.63/test/test_time_off_balances20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_time_off_entries20230301_response.py` & `affixapi-1.1.63/test/test_time_off_entries20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_time_off_entry_response.py` & `affixapi-1.1.63/test/test_tokens_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.time_off_entry_response import TimeOffEntryResponse
+from openapi_client.model.tokens_response import TokensResponse
 
 
-class TestTimeOffEntryResponse(unittest.TestCase):
-    """TimeOffEntryResponse unit test stubs"""
+class TestTokensResponse(unittest.TestCase):
+    """TokensResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTimeOffEntryResponse(self):
-        """Test TimeOffEntryResponse"""
+    def testTokensResponse(self):
+        """Test TokensResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TimeOffEntryResponse()  # noqa: E501
+        # model = TokensResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_timesheet_response.py` & `affixapi-1.1.63/test/test_employment_status_not_null_not_nullable.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,28 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.timesheet_response import TimesheetResponse
+from openapi_client.model.employment_status_not_null_not_nullable import EmploymentStatusNotNullNotNullable
 
 
-class TestTimesheetResponse(unittest.TestCase):
-    """TimesheetResponse unit test stubs"""
+class TestEmploymentStatusNotNullNotNullable(unittest.TestCase):
+    """EmploymentStatusNotNullNotNullable unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTimesheetResponse(self):
-        """Test TimesheetResponse"""
+    def testEmploymentStatusNotNullNotNullable(self):
+        """Test EmploymentStatusNotNullNotNullable"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TimesheetResponse()  # noqa: E501
+        # model = EmploymentStatusNotNullNotNullable()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_timesheets20230301_response.py` & `affixapi-1.1.63/test/test_timesheets20230301_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_token_request.py` & `affixapi-1.1.63/test/test_token_request.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_token_response.py` & `affixapi-1.1.63/test/test_token_response.py`

 * *Files identical despite different names*

### Comparing `affixapi-1.1.62/test/test_tokens_response.py` & `affixapi-1.1.63/test/test_work_locations20230301_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,28 +9,30 @@
 """
 
 
 import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.tokens_response import TokensResponse
+from openapi_client.model.location_response import LocationResponse
+globals()['LocationResponse'] = LocationResponse
+from openapi_client.model.work_locations20230301_response import WorkLocations20230301Response
 
 
-class TestTokensResponse(unittest.TestCase):
-    """TokensResponse unit test stubs"""
+class TestWorkLocations20230301Response(unittest.TestCase):
+    """WorkLocations20230301Response unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTokensResponse(self):
-        """Test TokensResponse"""
+    def testWorkLocations20230301Response(self):
+        """Test WorkLocations20230301Response"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = TokensResponse()  # noqa: E501
+        # model = WorkLocations20230301Response()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `affixapi-1.1.62/test/test_work_locations20230301_response.py` & `affixapi-1.1.63/test/test_xhr__vertically_integrated_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -5,34 +5,95 @@
 
     The version of the OpenAPI document: 2023-03-01
     Contact: developers@affixapi.com
     Generated by: https://openapi-generator.tech
 """
 
 
-import sys
 import unittest
 
 import openapi_client
-from openapi_client.model.location_response import LocationResponse
-globals()['LocationResponse'] = LocationResponse
-from openapi_client.model.work_locations20230301_response import WorkLocations20230301Response
+from openapi_client.api.xhr__vertically_integrated_api import XHRVerticallyIntegratedApi  # noqa: E501
 
 
-class TestWorkLocations20230301Response(unittest.TestCase):
-    """WorkLocations20230301Response unit test stubs"""
+class TestXHRVerticallyIntegratedApi(unittest.TestCase):
+    """XHRVerticallyIntegratedApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = XHRVerticallyIntegratedApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testWorkLocations20230301Response(self):
-        """Test WorkLocations20230301Response"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = WorkLocations20230301Response()  # noqa: E501
+    def test_xhr_companies20230301(self):
+        """Test case for xhr_companies20230301
+
+        Company  # noqa: E501
+        """
+        pass
+
+    def test_xhr_employees20230301(self):
+        """Test case for xhr_employees20230301
+
+        Employees  # noqa: E501
+        """
+        pass
+
+    def test_xhr_groups20230301(self):
+        """Test case for xhr_groups20230301
+
+        Groups  # noqa: E501
+        """
+        pass
+
+    def test_xhr_identity20230301(self):
+        """Test case for xhr_identity20230301
+
+        Identity  # noqa: E501
+        """
+        pass
+
+    def test_xhr_payruns20230301(self):
+        """Test case for xhr_payruns20230301
+
+        Payruns  # noqa: E501
+        """
+        pass
+
+    def test_xhr_payslips20230301(self):
+        """Test case for xhr_payslips20230301
+
+        Payslips  # noqa: E501
+        """
+        pass
+
+    def test_xhr_time_off_balances20230301(self):
+        """Test case for xhr_time_off_balances20230301
+
+        Time off balances  # noqa: E501
+        """
+        pass
+
+    def test_xhr_time_off_entries20230301(self):
+        """Test case for xhr_time_off_entries20230301
+
+        Time off entries  # noqa: E501
+        """
+        pass
+
+    def test_xhr_timesheets20230301(self):
+        """Test case for xhr_timesheets20230301
+
+        Timesheets  # noqa: E501
+        """
+        pass
+
+    def test_xhr_work_locations20230301(self):
+        """Test case for xhr_work_locations20230301
+
+        Work locations  # noqa: E501
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

