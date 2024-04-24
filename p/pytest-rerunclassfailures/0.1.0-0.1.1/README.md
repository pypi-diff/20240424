# Comparing `tmp/pytest_rerunclassfailures-0.1.0.tar.gz` & `tmp/pytest_rerunclassfailures-0.1.1.tar.gz`

## Comparing `pytest_rerunclassfailures-0.1.0.tar` & `pytest_rerunclassfailures-0.1.1.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.flake8
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.pylintrc
--rw-r--r--   0        0        0     1038 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/CHANGELOG.md
--rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/CODE_OF_CONDUCT.md
--rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/CONTRIBUTING.md
--rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/SECURITY.md
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/TODO.md
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/mypy.ini
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/pull_request_template.md
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/pytest.ini
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/requirements.txt
--rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/setup.cfg
--rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/setup.py
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.github/dependabot.yml
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.github/workflows/linters.yml
--rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.github/workflows/master_linters.yml
--rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.github/workflows/master_tests.yml
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/.gitignore
--rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/dbnavigator.xml
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/misc.xml
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/modules.xml
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/pytest-rerunclassfailures.iml
--rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/vcs.xml
--rw-r--r--   0        0        0    21088 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/workspace.xml
--rw-r--r--   0        0        0    23457 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/copilot/chatSessions/00000000000.xd
--rw-r--r--   0        0        0     6937 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/copilot/chatSessions/xd.lck
--rw-r--r--   0        0        0        4 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/copilot/chatSessions/blobs/version
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0        0        0   206933 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/assets/pytest-rerunclassfailures.jpg
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/src/pytest_rerunclassfailures/__init__.py
--rw-r--r--   0        0        0    20660 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/src/pytest_rerunclassfailures/pytest_rerunclassfailures.py
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/src/pytest_rerunclassfailures/requirements.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/conftest.py
--rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_arguments.py
--rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_class_attributes.py
--rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_failure_stages.py
--rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_format_handling.py
--rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_ordering.py
--rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_statuses.py
--rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_units_rest.py
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_xdist.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/type_check.py
--rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_always_fails.py
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_always_pass.py
--rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_basic.py
--rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_class_fixture_attributes.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_class_with_no_class.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_dict_attributes.py
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_different_statuses.py
--rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_ext_function_fixture_attributes.py
--rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_function_attributes.py
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_function_attributes_as_fixtures.py
--rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_function_fixture_attributes.py
--rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_list_attributes.py
--rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_no_class.py
--rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_non_init_attributes.py
--rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_run_order_both.py
--rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_run_order_order.py
--rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_run_order_ordering.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_same_class_1.py
--rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_same_class_2.py
--rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_same_class_in_module.py
--rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_same_test_in_class.py
--rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_several_classes_in_module.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_call.py
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_setup.py
--rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_teardown_class.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_teardown_class_pure.py
--rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_teardown_func.py
--rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/tests/test_source/test_unpickleable_attributes.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/.gitignore
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/LICENSE
--rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/README.md
--rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     7370 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.flake8
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.pylintrc
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/CHANGELOG.md
+-rw-r--r--   0        0        0     5202 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/CODE_OF_CONDUCT.md
+-rw-r--r--   0        0        0     2864 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0      564 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/SECURITY.md
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/TODO.md
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/mypy.ini
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/pull_request_template.md
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/pytest.ini
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/requirements.txt
+-rw-r--r--   0        0        0     1730 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/setup.cfg
+-rw-r--r--   0        0        0      272 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/setup.py
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      595 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.github/workflows/linters.yml
+-rw-r--r--   0        0        0     1721 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.github/workflows/master_linters.yml
+-rw-r--r--   0        0        0     1459 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.github/workflows/master_tests.yml
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/.gitignore
+-rw-r--r--   0        0        0    20670 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/dbnavigator.xml
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/misc.xml
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/modules.xml
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/pytest-rerunclassfailures.iml
+-rw-r--r--   0        0        0      167 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/vcs.xml
+-rw-r--r--   0        0        0    22179 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/workspace.xml
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0        0        0   206933 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/assets/pytest-rerunclassfailures.jpg
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/src/pytest_rerunclassfailures/__init__.py
+-rw-r--r--   0        0        0    20794 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/src/pytest_rerunclassfailures/pytest_rerunclassfailures.py
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/src/pytest_rerunclassfailures/requirements.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0     2708 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/conftest.py
+-rw-r--r--   0        0        0    10389 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_arguments.py
+-rw-r--r--   0        0        0     6123 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_class_attributes.py
+-rw-r--r--   0        0        0     3400 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_failure_stages.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_format_handling.py
+-rw-r--r--   0        0        0     3494 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_ordering.py
+-rw-r--r--   0        0        0     3431 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_rerun_different_length.py
+-rw-r--r--   0        0        0     2649 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_statuses.py
+-rw-r--r--   0        0        0     3454 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_units_rest.py
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_xdist.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/type_check.py
+-rw-r--r--   0        0        0      221 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_always_fails.py
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_always_pass.py
+-rw-r--r--   0        0        0      326 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_basic.py
+-rw-r--r--   0        0        0     1094 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_class_fixture_attributes.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_class_with_no_class.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_dict_attributes.py
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_different_statuses.py
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_ext_function_fixture_attributes.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_failed_on_first_run.py
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_failed_on_second_run.py
+-rw-r--r--   0        0        0      843 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_function_attributes.py
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_function_attributes_as_fixtures.py
+-rw-r--r--   0        0        0     1149 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_function_fixture_attributes.py
+-rw-r--r--   0        0        0      895 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_list_attributes.py
+-rw-r--r--   0        0        0      290 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_no_class.py
+-rw-r--r--   0        0        0      740 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_non_init_attributes.py
+-rw-r--r--   0        0        0     1118 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_run_order_both.py
+-rw-r--r--   0        0        0      599 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_run_order_order.py
+-rw-r--r--   0        0        0      615 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_run_order_ordering.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_same_class_1.py
+-rw-r--r--   0        0        0      338 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_same_class_2.py
+-rw-r--r--   0        0        0      672 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_same_class_in_module.py
+-rw-r--r--   0        0        0      416 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_same_test_in_class.py
+-rw-r--r--   0        0        0      598 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_several_classes_in_module.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_call.py
+-rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_setup.py
+-rw-r--r--   0        0        0      866 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_teardown_class.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_teardown_class_pure.py
+-rw-r--r--   0        0        0      925 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_teardown_func.py
+-rw-r--r--   0        0        0     4611 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/tests/test_source/test_unpickleable_attributes.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/.gitignore
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4651 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/README.md
+-rw-r--r--   0        0        0     2491 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     7370 2020-02-02 00:00:00.000000 pytest_rerunclassfailures-0.1.1/PKG-INFO
```

### Comparing `pytest_rerunclassfailures-0.1.0/CHANGELOG.md` & `pytest_rerunclassfailures-0.1.1/CHANGELOG.md`

 * *Files 11% similar despite different names*

```diff
@@ -38,7 +38,15 @@
 
 ## [0.1.0] - 2024-03-29
 
 ### Updated
 - README.md updated
 - Added more tests to achieve 100% coverage (including non-reachable code via mocks)
 - Added coverage collection and reporting
+
+## [0.1.1] - 2024-04-24
+
+### Fixed
+- Fixed proper setting of result outcome for reruns in case of different rerun length
+
+### Updated
+- Requirements bumped to the latest versions
```

### Comparing `pytest_rerunclassfailures-0.1.0/CODE_OF_CONDUCT.md` & `pytest_rerunclassfailures-0.1.1/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/CONTRIBUTING.md` & `pytest_rerunclassfailures-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/SECURITY.md` & `pytest_rerunclassfailures-0.1.1/SECURITY.md`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/setup.cfg` & `pytest_rerunclassfailures-0.1.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pytest-rerunclassfailures
-version = attr: pytest-rerunclassfailures.0.1.0
+version = attr: pytest-rerunclassfailures.0.1.1
 author = Iliya Vereshchagin
 author_email = i.vereshchagin@gmail.com
 maintainer = Iliya Vereshchagin
 maintainer_email = i.vereshchagin@gmail.com
 url = https://github.com/wwakabobik/pytest-rerunclassfailures
 description = pytest rerun class failures plugin
 long_description = file: README.md
```

### Comparing `pytest_rerunclassfailures-0.1.0/.github/ISSUE_TEMPLATE/bug_report.md` & `pytest_rerunclassfailures-0.1.1/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/.github/ISSUE_TEMPLATE/feature_request.md` & `pytest_rerunclassfailures-0.1.1/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/.github/workflows/linters.yml` & `pytest_rerunclassfailures-0.1.1/.github/workflows/linters.yml`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/.github/workflows/master_linters.yml` & `pytest_rerunclassfailures-0.1.1/.github/workflows/master_linters.yml`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/.github/workflows/master_tests.yml` & `pytest_rerunclassfailures-0.1.1/.github/workflows/master_tests.yml`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/.github/workflows/tests.yml` & `pytest_rerunclassfailures-0.1.1/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -29,8 +29,8 @@
         pip install pytest-ordering
         pip install pytest-order
         pip install pytest-cov
     - name: Add 'src' to PYTHONPATH
       run: echo "PYTHONPATH=$PYTHONPATH:$(pwd)/src:." >> $GITHUB_ENV
     - name: Execute tests
       id: tests
-      run: pytest tests -n=auto --dist=loadfile --order-scope=module --cov-report=term --cov-fail-under=95
+      run: pytest tests -n=auto --dist=loadfile --order-scope=module --cov=src/pytest_rerunclassfailures --cov-report=term --cov-report=xml:coverage.xml --cov-fail-under=95
```

### Comparing `pytest_rerunclassfailures-0.1.0/.idea/dbnavigator.xml` & `pytest_rerunclassfailures-0.1.1/.idea/dbnavigator.xml`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/.idea/workspace.xml` & `pytest_rerunclassfailures-0.1.1/.idea/workspace.xml`

 * *Files 2% similar despite different names*

#### Comparing `pytest_rerunclassfailures-0.1.0/.idea/workspace.xml` & `pytest_rerunclassfailures-0.1.1/.idea/workspace.xml`

```diff
@@ -1,16 +1,24 @@
 <?xml version="1.0" encoding="utf-8"?>
 <project version="4">
   <component name="AutoImportSettings">
     <option name="autoReloadType" value="SELECTIVE"/>
   </component>
   <component name="BlackConnectSettings" port="45489" lineLength="120" triggerOnReformat="true" targetSpecificVersions="true" pythonTargets="py3.11"/>
   <component name="ChangeListManager">
-    <list default="true" id="38c87715-d495-43db-9d28-b8fccb0a07bb" name="Changes" comment="Update CHANGELOG.md">
-      <change beforePath="$PROJECT_DIR$/.github/workflows/master_tests.yml" beforeDir="false" afterPath="$PROJECT_DIR$/.github/workflows/master_tests.yml" afterDir="false"/>
+    <list default="true" id="38c87715-d495-43db-9d28-b8fccb0a07bb" name="Changes" comment="Update coveralls with token">
+      <change afterPath="$PROJECT_DIR$/tests/test_rerun_different_length.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/tests/test_source/test_failed_on_first_run.py" afterDir="false"/>
+      <change afterPath="$PROJECT_DIR$/tests/test_source/test_failed_on_second_run.py" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/.github/workflows/tests.yml" beforeDir="false" afterPath="$PROJECT_DIR$/.github/workflows/tests.yml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/CHANGELOG.md" beforeDir="false" afterPath="$PROJECT_DIR$/CHANGELOG.md" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/pyproject.toml" beforeDir="false" afterPath="$PROJECT_DIR$/pyproject.toml" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/requirements.txt" beforeDir="false" afterPath="$PROJECT_DIR$/requirements.txt" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/setup.cfg" beforeDir="false" afterPath="$PROJECT_DIR$/setup.cfg" afterDir="false"/>
+      <change beforePath="$PROJECT_DIR$/src/pytest_rerunclassfailures/pytest_rerunclassfailures.py" beforeDir="false" afterPath="$PROJECT_DIR$/src/pytest_rerunclassfailures/pytest_rerunclassfailures.py" afterDir="false"/>
     </list>
     <option name="SHOW_DIALOG" value="false"/>
     <option name="HIGHLIGHT_CONFLICTS" value="true"/>
     <option name="HIGHLIGHT_NON_ACTIVE_CHANGELIST" value="false"/>
     <option name="LAST_RESOLUTION" value="IGNORE"/>
   </component>
   <component name="FileTemplateManagerImpl">
@@ -31,26 +39,26 @@
   &quot;associatedIndex&quot;: 5
 }</component>
   <component name="ProjectId" id="2duM4YXLuHf59ryj47JAezCMIsn"/>
   <component name="ProjectViewState">
     <option name="hideEmptyMiddlePackages" value="true"/>
     <option name="showLibraryContents" value="true"/>
   </component>
-  <component name="PropertiesComponent">{
-  &quot;keyToString&quot;: {
-    &quot;RunOnceActivity.OpenProjectViewOnStart&quot;: &quot;true&quot;,
-    &quot;RunOnceActivity.ShowReadmeOnStart&quot;: &quot;true&quot;,
-    &quot;last_opened_file_path&quot;: &quot;/Users/ilyavereshchagin/Work/pytest-rerunclassfailures/tests&quot;,
-    &quot;settings.editor.selected.configurable&quot;: &quot;me.lensvol.blackconnect.settings&quot;
+  <component name="PropertiesComponent"><![CDATA[{
+  "keyToString": {
+    "RunOnceActivity.OpenProjectViewOnStart": "true",
+    "RunOnceActivity.ShowReadmeOnStart": "true",
+    "last_opened_file_path": "/Users/ilyavereshchagin/Work/pytest-rerunclassfailures/tests/test_source",
+    "settings.editor.selected.configurable": "com.jetbrains.python.configuration.PyActiveSdkModuleConfigurable"
   }
-}</component>
+}]]></component>
   <component name="RecentsManager">
     <key name="CopyFile.RECENT_KEYS">
-      <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/tests/test_source"/>
+      <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/.github/workflows"/>
       <recent name="$PROJECT_DIR$/src/pytest_rerunclassfailures"/>
     </key>
     <key name="MoveFile.RECENT_KEYS">
       <recent name="$PROJECT_DIR$/tests"/>
       <recent name="$PROJECT_DIR$/tests/test_source"/>
       <recent name="$PROJECT_DIR$/src"/>
@@ -61,30 +69,14 @@
     <task active="true" id="Default" summary="Default task">
       <changelist id="38c87715-d495-43db-9d28-b8fccb0a07bb" name="Changes" comment=""/>
       <created>1710853320458</created>
       <option name="number" value="Default"/>
       <option name="presentableId" value="Default"/>
       <updated>1710853320458</updated>
     </task>
-    <task id="LOCAL-00016" summary="add tests for arguments">
-      <option name="closed" value="true"/>
-      <created>1711046451945</created>
-      <option name="number" value="00016"/>
-      <option name="presentableId" value="LOCAL-00016"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1711046451945</updated>
-    </task>
-    <task id="LOCAL-00017" summary="add tests for arguments">
-      <option name="closed" value="true"/>
-      <created>1711046675141</created>
-      <option name="number" value="00017"/>
-      <option name="presentableId" value="LOCAL-00017"/>
-      <option name="project" value="LOCAL"/>
-      <updated>1711046675141</updated>
-    </task>
     <task id="LOCAL-00018" summary="add tests for arguments">
       <option name="closed" value="true"/>
       <created>1711046839713</created>
       <option name="number" value="00018"/>
       <option name="presentableId" value="LOCAL-00018"/>
       <option name="project" value="LOCAL"/>
       <updated>1711046839713</updated>
@@ -453,15 +445,31 @@
       <option name="closed" value="true"/>
       <created>1711741693185</created>
       <option name="number" value="00064"/>
       <option name="presentableId" value="LOCAL-00064"/>
       <option name="project" value="LOCAL"/>
       <updated>1711741693185</updated>
     </task>
-    <option name="localTasksCounter" value="65"/>
+    <task id="LOCAL-00065" summary="Update coveralls with token">
+      <option name="closed" value="true"/>
+      <created>1711742081039</created>
+      <option name="number" value="00065"/>
+      <option name="presentableId" value="LOCAL-00065"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1711742081039</updated>
+    </task>
+    <task id="LOCAL-00066" summary="Update coveralls with token">
+      <option name="closed" value="true"/>
+      <created>1711742163590</created>
+      <option name="number" value="00066"/>
+      <option name="presentableId" value="LOCAL-00066"/>
+      <option name="project" value="LOCAL"/>
+      <updated>1711742163590</updated>
+    </task>
+    <option name="localTasksCounter" value="67"/>
     <servers/>
   </component>
   <component name="VcsManagerConfiguration">
     <MESSAGE value="initial commit"/>
     <MESSAGE value="fixes for xdist"/>
     <MESSAGE value="add tests for arguments"/>
     <MESSAGE value="add tests for different test format"/>
@@ -474,10 +482,11 @@
     <MESSAGE value="bump to 0.0.5"/>
     <MESSAGE value="bump to 0.1.0"/>
     <MESSAGE value="Add missing coverage for unpicleable attributes"/>
     <MESSAGE value="Add missing test coverage"/>
     <MESSAGE value="Add code-coverage analysis"/>
     <MESSAGE value="Add unit tests for impossible cases"/>
     <MESSAGE value="Update CHANGELOG.md"/>
-    <option name="LAST_COMMIT_MESSAGE" value="Update CHANGELOG.md"/>
+    <MESSAGE value="Update coveralls with token"/>
+    <option name="LAST_COMMIT_MESSAGE" value="Update coveralls with token"/>
   </component>
 </project>
```

### Comparing `pytest_rerunclassfailures-0.1.0/.idea/inspectionProfiles/Project_Default.xml` & `pytest_rerunclassfailures-0.1.1/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/assets/pytest-rerunclassfailures.jpg` & `pytest_rerunclassfailures-0.1.1/assets/pytest-rerunclassfailures.jpg`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/src/pytest_rerunclassfailures/pytest_rerunclassfailures.py` & `pytest_rerunclassfailures-0.1.1/src/pytest_rerunclassfailures/pytest_rerunclassfailures.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,20 +383,22 @@
 
         :param test_class: dict with test class test results (including reruns)
         :type test_class: dict
         :return: None
         :rtype: None
         """
         self.logger.debug("Preparing reports before publication")
+        max_reruns = max(len(reruns) for reruns in test_class.values())
+
         for sibling, reruns in test_class.items():
-            if len(reruns) > 1:
-                if self.only_last:
-                    test_class[sibling] = [reruns[-1]]
-                else:
-                    for rerun in reruns[:-1]:
+            if self.only_last:
+                test_class[sibling] = [reruns[-1]] if len(reruns) == max_reruns else []
+            else:
+                for rerun_index, rerun in enumerate(reruns):
+                    if rerun_index < max_reruns - 1:
                         for report in rerun:
                             dummy_report = self._check_and_add_dummy_rerun_if_needed(report)
                             rerun.append(dummy_report) if dummy_report else None  # pylint: disable=W0106
                             report.outcome = "rerun"
 
     def _check_and_add_dummy_rerun_if_needed(self, report: TestReport) -> Union[None, TestReport]:
         """
```

### Comparing `pytest_rerunclassfailures-0.1.0/tests/conftest.py` & `pytest_rerunclassfailures-0.1.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_arguments.py` & `pytest_rerunclassfailures-0.1.1/tests/test_arguments.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_class_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_class_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_failure_stages.py` & `pytest_rerunclassfailures-0.1.1/tests/test_failure_stages.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_format_handling.py` & `pytest_rerunclassfailures-0.1.1/tests/test_format_handling.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_ordering.py` & `pytest_rerunclassfailures-0.1.1/tests/test_ordering.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_statuses.py` & `pytest_rerunclassfailures-0.1.1/tests/test_statuses.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_units_rest.py` & `pytest_rerunclassfailures-0.1.1/tests/test_units_rest.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_xdist.py` & `pytest_rerunclassfailures-0.1.1/tests/test_xdist.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_class_fixture_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_class_fixture_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_dict_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_dict_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_different_statuses.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_different_statuses.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_ext_function_fixture_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_ext_function_fixture_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_function_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_function_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_function_attributes_as_fixtures.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_function_attributes_as_fixtures.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_function_fixture_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_function_fixture_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_list_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_list_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_non_init_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_non_init_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_run_order_both.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_run_order_both.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_run_order_order.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_run_order_order.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_run_order_ordering.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_run_order_ordering.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_same_class_in_module.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_same_class_in_module.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_several_classes_in_module.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_several_classes_in_module.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_teardown_class.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_teardown_class.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_teardown_class_pure.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_teardown_class_pure.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_stages_teardown_func.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_stages_teardown_func.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/tests/test_source/test_unpickleable_attributes.py` & `pytest_rerunclassfailures-0.1.1/tests/test_source/test_unpickleable_attributes.py`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/.gitignore` & `pytest_rerunclassfailures-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/LICENSE` & `pytest_rerunclassfailures-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/README.md` & `pytest_rerunclassfailures-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pytest_rerunclassfailures-0.1.0/pyproject.toml` & `pytest_rerunclassfailures-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 src-dir = "src"
 
 [tool.hatch.build.targets.sdist]
 src-dir = "src"
 
 [project]
 name = "pytest-rerunclassfailures"
-version = "0.1.0"
+version = "0.1.1"
 keywords = ["pytest", "pytest-rerunclassfailures", "pytest-plugin", "testing", "qa", "failures", "flacky"]
 authors = [
   { name="Iliya Vereshchagin", email="i.vereshchagin@gmail.com" },
 ]
 maintainers = [
   { name="Iliya Vereshchagin", email="i.vereshchagin@gmail.com" },
 ]
```

### Comparing `pytest_rerunclassfailures-0.1.0/PKG-INFO` & `pytest_rerunclassfailures-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pytest-rerunclassfailures
-Version: 0.1.0
+Version: 0.1.1
 Summary: pytest rerun class failures plugin
 Project-URL: Homepage, https://github.com/wwakabobik/pytest-rerunclassfailures
 Project-URL: Bug Tracker, https://github.com/wwakabobik/pytest-rerunclassfailures/issues
 Author-email: Iliya Vereshchagin <i.vereshchagin@gmail.com>
 Maintainer-email: Iliya Vereshchagin <i.vereshchagin@gmail.com>
 License: MIT License
```

