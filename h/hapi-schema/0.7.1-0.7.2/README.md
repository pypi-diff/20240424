# Comparing `tmp/hapi_schema-0.7.1.tar.gz` & `tmp/hapi_schema-0.7.2.tar.gz`

## Comparing `hapi_schema-0.7.1.tar` & `hapi_schema-0.7.2.tar`

### file list

```diff
@@ -1,81 +1,81 @@
--rw-r--r--   0        0        0     1674 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/changelog.md
--rw-r--r--   0        0        0     1969 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/contributing.md
--rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/requirements.txt
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/.config/coveragerc
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/.config/pre-commit-config.yaml
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/.config/pytest.ini
--rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/.config/ruff.toml
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/.github/workflows/publish.yaml
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/.github/workflows/run-python-tests.yaml
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/__init__.py
--rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/_version.py
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_admin1.py
--rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_admin2.py
--rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_age_range.py
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_dataset.py
--rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_food_security.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_gender.py
--rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_humanitarian_needs.py
--rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_ipc_phase.py
--rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_ipc_type.py
--rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_location.py
--rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_national_risk.py
--rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_operational_presence.py
--rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_org.py
--rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_org_type.py
--rw-r--r--   0        0        0     1157 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_patches.py
--rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_population.py
--rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_population_group.py
--rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_population_status.py
--rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_resource.py
--rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/db_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/utils/__init__.py
--rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/utils/base.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/src/hapi_schema/utils/view_params.py
--rw-r--r--   0        0        0     4999 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/conftest.py
--rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_admin1.py
--rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_admin2.py
--rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_age_range.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_dataset.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_food_security.py
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_gender.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_humanitarian_needs.py
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_ipc_phase.py
--rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_ipc_type.py
--rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_location.py
--rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_national_risk.py
--rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_operational_presence.py
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_org.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_org_type.py
--rw-r--r--   0        0        0      871 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_patches.py
--rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_population.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_population_group.py
--rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_population_status.py
--rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_resource.py
--rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/test_sector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/__init__.py
--rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_admin1.py
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_admin2.py
--rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_age_range.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_dataset.py
--rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_food_security.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_gender.py
--rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_humanitarian_needs.py
--rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_ipc_phase.py
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_ipc_type.py
--rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_location.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_national_risk.py
--rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_operational_presence.py
--rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_org.py
--rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_org_type.py
--rw-r--r--   0        0        0     1193 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_patches.py
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_population.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_population_group.py
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_population_status.py
--rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_resource.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/tests/sample_data/data_sector.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/.gitignore
--rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/LICENSE
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/README.md
--rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/pyproject.toml
--rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hapi_schema-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0     1702 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/changelog.md
+-rw-r--r--   0        0        0     2580 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/contributing.md
+-rw-r--r--   0        0        0     1197 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/requirements.txt
+-rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/.config/coveragerc
+-rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/.config/pre-commit-config.yaml
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/.config/pytest.ini
+-rw-r--r--   0        0        0      420 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/.config/ruff.toml
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/.github/workflows/publish.yaml
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/.github/workflows/run-python-tests.yaml
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/_version.py
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_admin1.py
+-rw-r--r--   0        0        0     2983 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_admin2.py
+-rw-r--r--   0        0        0      630 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_age_range.py
+-rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_dataset.py
+-rw-r--r--   0        0        0     4710 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_food_security.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_gender.py
+-rw-r--r--   0        0        0     5152 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_humanitarian_needs.py
+-rw-r--r--   0        0        0      809 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_ipc_phase.py
+-rw-r--r--   0        0        0      750 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_ipc_type.py
+-rw-r--r--   0        0        0     1670 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_location.py
+-rw-r--r--   0        0        0     4369 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_national_risk.py
+-rw-r--r--   0        0        0     4857 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_operational_presence.py
+-rw-r--r--   0        0        0     2056 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_org.py
+-rw-r--r--   0        0        0      583 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_org_type.py
+-rw-r--r--   0        0        0     1431 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_patch.py
+-rw-r--r--   0        0        0     4123 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_population.py
+-rw-r--r--   0        0        0      632 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_population_group.py
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_population_status.py
+-rw-r--r--   0        0        0     2226 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_resource.py
+-rw-r--r--   0        0        0      553 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/db_sector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/utils/__init__.py
+-rw-r--r--   0        0        0      166 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/utils/base.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/src/hapi_schema/utils/view_params.py
+-rw-r--r--   0        0        0     4987 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/conftest.py
+-rw-r--r--   0        0        0     2657 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_admin1.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_admin2.py
+-rw-r--r--   0        0        0      480 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_age_range.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_dataset.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_food_security.py
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_gender.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_humanitarian_needs.py
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_ipc_phase.py
+-rw-r--r--   0        0        0      815 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_ipc_type.py
+-rw-r--r--   0        0        0     2422 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_location.py
+-rw-r--r--   0        0        0     2482 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_national_risk.py
+-rw-r--r--   0        0        0     1796 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_operational_presence.py
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_org.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_org_type.py
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_patch.py
+-rw-r--r--   0        0        0     2031 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_population.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_population_group.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_population_status.py
+-rw-r--r--   0        0        0     1836 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_resource.py
+-rw-r--r--   0        0        0      434 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/test_sector.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/__init__.py
+-rw-r--r--   0        0        0      918 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_admin1.py
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_admin2.py
+-rw-r--r--   0        0        0      113 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_age_range.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_dataset.py
+-rw-r--r--   0        0        0     1261 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_food_security.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_gender.py
+-rw-r--r--   0        0        0     1983 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_humanitarian_needs.py
+-rw-r--r--   0        0        0     1491 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_ipc_phase.py
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_ipc_type.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_location.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_national_risk.py
+-rw-r--r--   0        0        0     1308 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_operational_presence.py
+-rw-r--r--   0        0        0      853 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_org.py
+-rw-r--r--   0        0        0      170 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_org_type.py
+-rw-r--r--   0        0        0     1191 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_patch.py
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_population.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_population_group.py
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_population_status.py
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_resource.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/tests/sample_data/data_sector.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/.gitignore
+-rw-r--r--   0        0        0     1099 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/LICENSE
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/README.md
+-rw-r--r--   0        0        0     2460 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/pyproject.toml
+-rw-r--r--   0        0        0     1534 2020-02-02 00:00:00.000000 hapi_schema-0.7.2/PKG-INFO
```

### Comparing `hapi_schema-0.7.1/changelog.md` & `hapi_schema-0.7.2/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # Changelog
 
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
+## [0.7.2]
+
+### Added
+
+- Patches table
+
 ## [0.7.1]
 
 ### Changed
 
 - Removed constraint from food security
 
-## [0.7.0]
-
 ### Added
 - Missing constraints
 - Tests on the constraints
 - `hapi_updated_date` and `hapi_replaced_date` fields
 
 ### Changed
```

### Comparing `hapi_schema-0.7.1/requirements.txt` & `hapi_schema-0.7.2/requirements.txt`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/.config/pre-commit-config.yaml` & `hapi_schema-0.7.2/.config/pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/.github/workflows/publish.yaml` & `hapi_schema-0.7.2/.github/workflows/publish.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/.github/workflows/run-python-tests.yaml` & `hapi_schema-0.7.2/.github/workflows/run-python-tests.yaml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_admin1.py` & `hapi_schema-0.7.2/src/hapi_schema/db_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_admin2.py` & `hapi_schema-0.7.2/src/hapi_schema/db_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_age_range.py` & `hapi_schema-0.7.2/src/hapi_schema/db_age_range.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_dataset.py` & `hapi_schema-0.7.2/src/hapi_schema/db_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_food_security.py` & `hapi_schema-0.7.2/src/hapi_schema/db_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_gender.py` & `hapi_schema-0.7.2/src/hapi_schema/db_gender.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_humanitarian_needs.py` & `hapi_schema-0.7.2/src/hapi_schema/db_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_ipc_phase.py` & `hapi_schema-0.7.2/src/hapi_schema/db_ipc_phase.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_ipc_type.py` & `hapi_schema-0.7.2/src/hapi_schema/db_ipc_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_location.py` & `hapi_schema-0.7.2/src/hapi_schema/db_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_national_risk.py` & `hapi_schema-0.7.2/src/hapi_schema/db_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_operational_presence.py` & `hapi_schema-0.7.2/src/hapi_schema/db_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_org.py` & `hapi_schema-0.7.2/src/hapi_schema/db_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_org_type.py` & `hapi_schema-0.7.2/src/hapi_schema/db_org_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_population.py` & `hapi_schema-0.7.2/src/hapi_schema/db_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_population_group.py` & `hapi_schema-0.7.2/src/hapi_schema/db_population_group.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_population_status.py` & `hapi_schema-0.7.2/src/hapi_schema/db_population_status.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_resource.py` & `hapi_schema-0.7.2/src/hapi_schema/db_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/src/hapi_schema/db_sector.py` & `hapi_schema-0.7.2/src/hapi_schema/db_sector.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/conftest.py` & `hapi_schema-0.7.2/tests/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 from hapi_schema.db_location import DBLocation
 from hapi_schema.db_national_risk import DBNationalRisk
 from hapi_schema.db_operational_presence import (
     DBOperationalPresence,
 )
 from hapi_schema.db_org import DBOrg
 from hapi_schema.db_org_type import DBOrgType
-from hapi_schema.db_patches import DBPatches
+from hapi_schema.db_patch import DBPatch
 from hapi_schema.db_population import DBPopulation
 from hapi_schema.db_population_group import DBPopulationGroup
 from hapi_schema.db_population_status import DBPopulationStatus
 from hapi_schema.db_resource import DBResource
 from hapi_schema.db_sector import DBSector
 from hapi_schema.utils.base import Base
 from sample_data.data_admin1 import data_admin1
@@ -39,15 +39,15 @@
 from sample_data.data_ipc_phase import data_ipc_phase
 from sample_data.data_ipc_type import data_ipc_type
 from sample_data.data_location import data_location
 from sample_data.data_national_risk import data_national_risk
 from sample_data.data_operational_presence import data_operational_presence
 from sample_data.data_org import data_org
 from sample_data.data_org_type import data_org_type
-from sample_data.data_patches import data_patches
+from sample_data.data_patch import data_patch
 from sample_data.data_population import data_population
 from sample_data.data_population_group import data_population_group
 from sample_data.data_population_status import data_population_status
 from sample_data.data_resource import data_resource
 from sample_data.data_sector import data_sector
 
 
@@ -83,15 +83,15 @@
 
     session.execute(insert(DBNationalRisk), data_national_risk)
     session.execute(insert(DBPopulation), data_population)
     session.execute(insert(DBOperationalPresence), data_operational_presence)
     session.execute(insert(DBFoodSecurity), data_food_security)
     session.execute(insert(DBHumanitarianNeeds), data_humanitarian_needs)
 
-    session.execute(insert(DBPatches), data_patches)
+    session.execute(insert(DBPatch), data_patch)
 
     session.commit()
 
     return engine
 
 
 @pytest.fixture(scope="session")
```

### Comparing `hapi_schema-0.7.1/tests/test_admin1.py` & `hapi_schema-0.7.2/tests/test_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_admin2.py` & `hapi_schema-0.7.2/tests/test_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_dataset.py` & `hapi_schema-0.7.2/tests/test_dataset.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_food_security.py` & `hapi_schema-0.7.2/tests/test_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_humanitarian_needs.py` & `hapi_schema-0.7.2/tests/test_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_ipc_phase.py` & `hapi_schema-0.7.2/tests/test_ipc_phase.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_ipc_type.py` & `hapi_schema-0.7.2/tests/test_ipc_type.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_location.py` & `hapi_schema-0.7.2/tests/test_location.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_national_risk.py` & `hapi_schema-0.7.2/tests/test_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_operational_presence.py` & `hapi_schema-0.7.2/tests/test_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_org.py` & `hapi_schema-0.7.2/tests/test_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_population.py` & `hapi_schema-0.7.2/tests/test_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_population_group.py` & `hapi_schema-0.7.2/tests/test_population_group.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_population_status.py` & `hapi_schema-0.7.2/tests/test_population_status.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/test_resource.py` & `hapi_schema-0.7.2/tests/test_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_admin1.py` & `hapi_schema-0.7.2/tests/sample_data/data_admin1.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_admin2.py` & `hapi_schema-0.7.2/tests/sample_data/data_admin2.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_food_security.py` & `hapi_schema-0.7.2/tests/sample_data/data_food_security.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_humanitarian_needs.py` & `hapi_schema-0.7.2/tests/sample_data/data_humanitarian_needs.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_ipc_phase.py` & `hapi_schema-0.7.2/tests/sample_data/data_ipc_phase.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_national_risk.py` & `hapi_schema-0.7.2/tests/sample_data/data_national_risk.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_operational_presence.py` & `hapi_schema-0.7.2/tests/sample_data/data_operational_presence.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_org.py` & `hapi_schema-0.7.2/tests/sample_data/data_org.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_patches.py` & `hapi_schema-0.7.2/tests/sample_data/data_patch.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from datetime import datetime
 
-data_patches = [
+data_patch = [
     dict(
         id=1,
         patch_sequence_number=1,
         commit_hash="66e7e589a1224a1832ba7360817dda7a7d9313cf",
         commit_date=datetime(2023, 1, 1),
         patch_path="2024/01",
         permanent_download_url="https://github.com/OCHA-DAP/hapi-patch-repo/blob/66e7e589a1224a1832ba7360817dda7a7d9313cf/2024/01/hapi_patch_10_hno.json",
```

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_population.py` & `hapi_schema-0.7.2/tests/sample_data/data_population.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/tests/sample_data/data_resource.py` & `hapi_schema-0.7.2/tests/sample_data/data_resource.py`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/.gitignore` & `hapi_schema-0.7.2/.gitignore`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/LICENSE` & `hapi_schema-0.7.2/LICENSE`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/pyproject.toml` & `hapi_schema-0.7.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `hapi_schema-0.7.1/PKG-INFO` & `hapi_schema-0.7.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: hapi-schema
-Version: 0.7.1
+Version: 0.7.2
 Summary: HAPI database schema specified in SQLAlchemy
 Project-URL: Homepage, https://github.com/OCHA-DAP/hapi-schemas
 Author-email: Simon Johnson <simon.johnson@un.org>
 License: MIT
 License-File: LICENSE
 Keywords: HDX,hapi,schema
 Classifier: Intended Audience :: Developers
```

