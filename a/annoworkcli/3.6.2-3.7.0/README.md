# Comparing `tmp/annoworkcli-3.6.2.tar.gz` & `tmp/annoworkcli-3.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "annoworkcli-3.6.2.tar", max compression
+gzip compressed data, was "annoworkcli-3.7.0.tar", max compression
```

## Comparing `annoworkcli-3.6.2.tar` & `annoworkcli-3.7.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0     2107 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/README.md
--rw-r--r--   0        0        0       71 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/__init__.py
--rw-r--r--   0        0        0     3579 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/__main__.py
--rw-r--r--   0        0        0      131 2024-03-01 06:06:16.996025 annoworkcli-3.6.2/annoworkcli/__version__.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/account/__init__.py
--rw-r--r--   0        0        0     2865 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/account/list_external_linkage_info.py
--rw-r--r--   0        0        0     2362 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/account/put_external_linkage_info.py
--rw-r--r--   0        0        0      879 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/account/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/actual_working_time/__init__.py
--rw-r--r--   0        0        0     7578 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/actual_working_time/delete_actual_working_time.py
--rw-r--r--   0        0        0    14505 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
--rw-r--r--   0        0        0    13256 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    15193 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/actual_working_time/list_actual_working_time.py
--rw-r--r--   0        0        0     1408 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/actual_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/__init__.py
--rw-r--r--   0        0        0     9053 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/list_job_with_annofab_project.py
--rw-r--r--   0        0        0    24219 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/list_working_hours.py
--rw-r--r--   0        0        0     5703 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/put_account_external_linkage_info.py
--rw-r--r--   0        0        0     4479 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/put_job_from_annofab_project.py
--rw-r--r--   0        0        0    52341 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/reshape_working_hours.py
--rw-r--r--   0        0        0     1515 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/subcommand.py
--rw-r--r--   0        0        0     2268 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/utils.py
--rw-r--r--   0        0        0    11928 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/annofab/visualize_statistics.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/common/__init__.py
--rw-r--r--   0        0        0      812 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/common/annofab.py
--rw-r--r--   0        0        0    11606 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/common/cli.py
--rw-r--r--   0        0        0      222 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/common/exeptions.py
--rw-r--r--   0        0        0       43 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/common/job.py
--rw-r--r--   0        0        0     4364 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/common/utils.py
--rw-r--r--   0        0        0      889 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/common/workspace_tag.py
--rw-r--r--   0        0        0      829 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/data/logging.yaml
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/expected_working_time/__init__.py
--rw-r--r--   0        0        0     3822 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/expected_working_time/delete_expected_working_time.py
--rw-r--r--   0        0        0     6703 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/expected_working_time/list_expected_working_time.py
--rw-r--r--   0        0        0     8741 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
--rw-r--r--   0        0        0     5875 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
--rw-r--r--   0        0        0     1296 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/expected_working_time/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/job/__init__.py
--rw-r--r--   0        0        0     4002 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/job/change_job_properties.py
--rw-r--r--   0        0        0     3290 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/job/delete_job.py
--rw-r--r--   0        0        0     6248 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/job/list_job.py
--rw-r--r--   0        0        0      885 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/job/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/my/__init__.py
--rw-r--r--   0        0        0     1368 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/my/get_my_account.py
--rw-r--r--   0        0        0     2361 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/my/list_my_workspace_member.py
--rw-r--r--   0        0        0      816 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/my/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/schedule/__init__.py
--rw-r--r--   0        0        0     9013 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/schedule/list_assigned_hours_daily.py
--rw-r--r--   0        0        0     9178 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
--rw-r--r--   0        0        0    10988 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/schedule/list_schedule.py
--rw-r--r--   0        0        0      995 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/schedule/subcommand.py
--rw-r--r--   0        0        0     3240 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace/list_workspace.py
--rw-r--r--   0        0        0     2105 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace/put_workspace.py
--rw-r--r--   0        0        0      847 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/__init__.py
--rw-r--r--   0        0        0     5012 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/append_tag_to_workspace_member.py
--rw-r--r--   0        0        0     4565 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/change_workspace_member_properties.py
--rw-r--r--   0        0        0     2861 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/delete_workspace_member.py
--rw-r--r--   0        0        0     6212 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/list_workspace_member.py
--rw-r--r--   0        0        0     4689 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/put_workspace_member.py
--rw-r--r--   0        0        0     5043 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
--rw-r--r--   0        0        0     1518 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_member/subcommand.py
--rw-r--r--   0        0        0        0 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_tag/__init__.py
--rw-r--r--   0        0        0     2645 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_tag/list_workspace_tag.py
--rw-r--r--   0        0        0     2540 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_tag/put_workspace_tag.py
--rw-r--r--   0        0        0      877 2024-03-01 06:06:07.288033 annoworkcli-3.6.2/annoworkcli/workspace_tag/subcommand.py
--rw-r--r--   0        0        0     2245 2024-03-01 06:06:16.992025 annoworkcli-3.6.2/pyproject.toml
--rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 annoworkcli-3.6.2/PKG-INFO
+-rw-r--r--   0        0        0     2107 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/README.md
+-rw-r--r--   0        0        0       71 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/__init__.py
+-rw-r--r--   0        0        0     3608 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/__main__.py
+-rw-r--r--   0        0        0      131 2024-03-15 05:41:20.537249 annoworkcli-3.7.0/annoworkcli/__version__.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/account/__init__.py
+-rw-r--r--   0        0        0     2922 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/account/list_external_linkage_info.py
+-rw-r--r--   0        0        0     2406 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/account/put_external_linkage_info.py
+-rw-r--r--   0        0        0      881 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/account/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/actual_working_time/__init__.py
+-rw-r--r--   0        0        0     7666 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/actual_working_time/delete_actual_working_time.py
+-rw-r--r--   0        0        0    14647 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/actual_working_time/list_actual_working_hours_daily.py
+-rw-r--r--   0        0        0    13329 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    15180 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/actual_working_time/list_actual_working_time.py
+-rw-r--r--   0        0        0     1410 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/actual_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/__init__.py
+-rw-r--r--   0        0        0     9042 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/list_job_with_annofab_project.py
+-rw-r--r--   0        0        0    24006 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/list_working_hours.py
+-rw-r--r--   0        0        0     5763 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/put_account_external_linkage_info.py
+-rw-r--r--   0        0        0     4507 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/put_job_from_annofab_project.py
+-rw-r--r--   0        0        0    51925 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/reshape_working_hours.py
+-rw-r--r--   0        0        0     1517 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/subcommand.py
+-rw-r--r--   0        0        0     2256 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/utils.py
+-rw-r--r--   0        0        0    12048 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/annofab/visualize_statistics.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/common/__init__.py
+-rw-r--r--   0        0        0      828 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/common/annofab.py
+-rw-r--r--   0        0        0    11711 2024-03-15 05:41:11.209281 annoworkcli-3.7.0/annoworkcli/common/cli.py
+-rw-r--r--   0        0        0      222 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/common/exeptions.py
+-rw-r--r--   0        0        0       43 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/common/job.py
+-rw-r--r--   0        0        0     4488 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/common/utils.py
+-rw-r--r--   0        0        0      889 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/common/workspace_tag.py
+-rw-r--r--   0        0        0      829 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/data/logging.yaml
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/expected_working_time/__init__.py
+-rw-r--r--   0        0        0     3851 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/expected_working_time/delete_expected_working_time.py
+-rw-r--r--   0        0        0     6724 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/expected_working_time/list_expected_working_time.py
+-rw-r--r--   0        0        0     8795 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py
+-rw-r--r--   0        0        0     5840 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/expected_working_time/list_expected_working_time_weekly.py
+-rw-r--r--   0        0        0     1298 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/expected_working_time/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/job/__init__.py
+-rw-r--r--   0        0        0     4030 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/job/change_job_properties.py
+-rw-r--r--   0        0        0     3348 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/job/delete_job.py
+-rw-r--r--   0        0        0     6283 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/job/list_job.py
+-rw-r--r--   0        0        0      887 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/job/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/my/__init__.py
+-rw-r--r--   0        0        0     1426 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/my/get_my_account.py
+-rw-r--r--   0        0        0     2404 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/my/list_my_workspace_member.py
+-rw-r--r--   0        0        0      818 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/my/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/schedule/__init__.py
+-rw-r--r--   0        0        0     5800 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/schedule/delete_schedule.py
+-rw-r--r--   0        0        0     9074 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/schedule/list_assigned_hours_daily.py
+-rw-r--r--   0        0        0     9244 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py
+-rw-r--r--   0        0        0    10998 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/schedule/list_schedule.py
+-rw-r--r--   0        0        0     1105 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/schedule/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace/__init__.py
+-rw-r--r--   0        0        0     3297 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace/list_workspace.py
+-rw-r--r--   0        0        0     2163 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace/put_workspace.py
+-rw-r--r--   0        0        0      849 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/__init__.py
+-rw-r--r--   0        0        0     5015 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/append_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     4530 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/change_workspace_member_properties.py
+-rw-r--r--   0        0        0     2881 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/delete_workspace_member.py
+-rw-r--r--   0        0        0     6269 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/list_workspace_member.py
+-rw-r--r--   0        0        0     4746 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/put_workspace_member.py
+-rw-r--r--   0        0        0     5046 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/remove_tag_to_workspace_member.py
+-rw-r--r--   0        0        0     1520 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_member/subcommand.py
+-rw-r--r--   0        0        0        0 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_tag/__init__.py
+-rw-r--r--   0        0        0     2702 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_tag/list_workspace_tag.py
+-rw-r--r--   0        0        0     2576 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_tag/put_workspace_tag.py
+-rw-r--r--   0        0        0      879 2024-03-15 05:41:11.213281 annoworkcli-3.7.0/annoworkcli/workspace_tag/subcommand.py
+-rw-r--r--   0        0        0     4474 2024-03-15 05:41:20.537249 annoworkcli-3.7.0/pyproject.toml
+-rw-r--r--   0        0        0     3199 1970-01-01 00:00:00.000000 annoworkcli-3.7.0/PKG-INFO
```

### Comparing `annoworkcli-3.6.2/README.md` & `annoworkcli-3.7.0/README.md`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.6.2/annoworkcli/__main__.py` & `annoworkcli-3.7.0/annoworkcli/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import copy
 import logging
 import sys
-from typing import Optional, Sequence
+from collections.abc import Sequence
+from typing import Optional
 
 import pandas
 
 import annoworkcli
 import annoworkcli.account.subcommand
 import annoworkcli.actual_working_time.subcommand
 import annoworkcli.annofab.subcommand
@@ -31,17 +32,15 @@
     """
     major, minor, _ = pandas.__version__.split(".")
     if int(major) >= 2 and int(minor) >= 2:
         pandas.options.mode.copy_on_write = "warn"
 
 
 def create_parser() -> argparse.ArgumentParser:
-    parser = argparse.ArgumentParser(
-        description="Command Line Interface for Annowork", formatter_class=PrettyHelpFormatter, allow_abbrev=False
-    )
+    parser = argparse.ArgumentParser(description="Command Line Interface for Annowork", formatter_class=PrettyHelpFormatter, allow_abbrev=False)
     parser.add_argument("--version", action="version", version=f"annoworkcli {annoworkcli.__version__}")
     parser.set_defaults(command_help=parser.print_help)
 
     subparsers = parser.add_subparsers(dest="command_name")
 
     annoworkcli.account.subcommand.add_parser(subparsers)
     annoworkcli.actual_working_time.subcommand.add_parser(subparsers)
@@ -67,15 +66,15 @@
             index = tmp_argv.index(masked_option)
             tmp_argv[index + 1] = "***"
         except ValueError:
             continue
     return tmp_argv
 
 
-def main(arguments: Optional[Sequence[str]] = None):
+def main(arguments: Optional[Sequence[str]] = None):  # noqa: ANN201
     """
     annoworkcli コマンドのメイン処理
 
     Args:
         arguments: コマンドライン引数。テストコード用
 
     """
```

### Comparing `annoworkcli-3.6.2/annoworkcli/account/list_external_linkage_info.py` & `annoworkcli-3.7.0/annoworkcli/account/list_external_linkage_info.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,51 +10,51 @@
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListExternalLinkageInfo:
-    def __init__(self, annowork_service: AnnoworkResource):
+    def __init__(self, annowork_service: AnnoworkResource):  # noqa: ANN204
         self.annowork_service = annowork_service
 
-    def main(self, user_id_list: list[str], output: Optional[Path], output_format: OutputFormat):
+    def main(self, user_id_list: list[str], output: Optional[Path], output_format: OutputFormat):  # noqa: ANN201
         logger.info(f"{len(user_id_list)} 件のアカウント外部連携情報を取得します。")
 
         results = []
         for user_id in user_id_list:
             info = self.annowork_service.wrapper.get_account_external_linkage_info_or_none(user_id)
             if info is None:
                 logger.warning(f"user_id={user_id} のアカウント外部連携情報は存在しません。")
             info["user_id"] = user_id
             results.append(info)
 
         if len(results) == 0:
-            logger.warning(f"アカウント外部連携情報は0件なので、出力しません。")
+            logger.warning("アカウント外部連携情報は0件なので、出力しません。")
             return
 
         logger.info(f"{len(results)} 件のアカウント外部連携情報を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(results, is_pretty=True, output=output)
         else:
             df = pandas.json_normalize(results)
             print_csv(df, output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     assert user_id_list is not None
     ListExternalLinkageInfo(annowork_service=annowork_service).main(
         user_id_list=user_id_list, output=args.output, output_format=OutputFormat(args.format)
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-u",
         "--user_id",
         type=str,
         nargs="+",
         required=True,
         help="出力対象ユーザのuser_id",
@@ -73,12 +73,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_external_linkage_info"
     subcommand_help = "アカウント外部連携情報取得の一覧を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/account/put_external_linkage_info.py` & `annoworkcli-3.7.0/annoworkcli/account/put_external_linkage_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,41 +8,39 @@
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, get_json_from_args
 
 logger = logging.getLogger(__name__)
 
 
 class PutExternalLinkageInfo:
-    def __init__(self, annowork_service: AnnoworkResource):
+    def __init__(self, annowork_service: AnnoworkResource):  # noqa: ANN204
         self.annowork_service = annowork_service
 
-    def main(self, user_id: str, external_linkage_info: dict[str, Any]):
+    def main(self, user_id: str, external_linkage_info: dict[str, Any]):  # noqa: ANN201
         old_info = self.annowork_service.wrapper.get_account_external_linkage_info_or_none(user_id)
         if old_info is None:
             logger.warning(f"user_id={user_id} のアカウント外部連携情報は存在しません。")
             return
 
         request_body = {
             "external_linkage_info": external_linkage_info,
             "last_updated_datetime": old_info["updated_datetime"],
         }
 
         self.annowork_service.api.put_account_external_linkage_info(user_id, request_body=request_body)
         logger.info(f"{user_id=} のユーザの外部連携情報を設定しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     external_linkage_info = get_json_from_args(args.external_linkage_info)
-    PutExternalLinkageInfo(annowork_service=annowork_service).main(
-        user_id=args.user_id, external_linkage_info=external_linkage_info
-    )
+    PutExternalLinkageInfo(annowork_service=annowork_service).main(user_id=args.user_id, external_linkage_info=external_linkage_info)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-u",
         "--user_id",
         type=str,
         required=True,
         help="登録対象ユーザのuser_id",
     )
@@ -59,12 +57,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "put_external_linkage_info"
     subcommand_help = "アカウント外部連携情報取得を更新します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/account/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/account/subcommand.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 from typing import Optional
 
 import annoworkcli
 import annoworkcli.account.list_external_linkage_info
 import annoworkcli.account.put_external_linkage_info
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     annoworkcli.account.list_external_linkage_info.add_parser(subparsers)
     annoworkcli.account.put_external_linkage_info.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "account"
     subcommand_help = "ユーザアカウントに関するサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/actual_working_time/delete_actual_working_time.py` & `annoworkcli-3.7.0/annoworkcli/actual_working_time/delete_actual_working_time.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     prompt_yesnoall,
 )
 
 logger = logging.getLogger(__name__)
 
 
 class DeleteActualWorkingTime:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         annowork_service: AnnoworkResource,
         workspace_id: str,
         *,
         timezone_offset_hours: Optional[float],
         all_yes: bool,
     ):
@@ -33,47 +33,47 @@
             annowork_service=annowork_service,
             workspace_id=workspace_id,
             timezone_offset_hours=timezone_offset_hours,
         )
 
         self.all_yes = all_yes
 
-    def delete_actual_working_times(self, actual_working_times: list[dict[str, Any]]):
+    def delete_actual_working_times(self, actual_working_times: list[dict[str, Any]]):  # noqa: ANN201
         success_count = 0
         for index, actual in enumerate(actual_working_times):
             try:
                 if not self.all_yes:
                     message = (
                         f"job_name={actual['job_name']}, user_id={actual['user_id']}, "
-                        f"start_datetime={actual['start_datetime']}, end_datetime={actual['end_datetime']} のジョブを削除しますか？"
+                        f"start_datetime={actual['start_datetime']}, end_datetime={actual['end_datetime']} の実績作業時間情報を削除しますか？"
                         f" :: actual_working_time_id={actual['actual_working_time_id']}"
                     )
                     is_yes, all_yes = prompt_yesnoall(message)
                     if not is_yes:
                         continue
                     if all_yes:
                         self.all_yes = all_yes
 
-                actual = self.annowork_service.api.delete_actual_working_time_by_workspace_member(
+                actual2 = self.annowork_service.api.delete_actual_working_time_by_workspace_member(
                     self.workspace_id,
                     workspace_member_id=actual["workspace_member_id"],
                     actual_working_time_id=actual["actual_working_time_id"],
                 )
-                logger.debug(f"{index+1} 件目: 実績作業時間を削除しました。:: {actual}")
+                logger.debug(f"{index+1} 件目: 実績作業時間を削除しました。:: {actual2}")
                 success_count += 1
-            except Exception as e:
-                logger.warning(f"{index+1} 件目: 実績作業時間の削除に失敗しました。{e}")
+            except Exception:
+                logger.warning(f"{index+1} 件目: 実績作業時間の削除に失敗しました。", exc_info=True)
                 continue
             finally:
                 if (index + 1) % 100 == 0:
                     logger.debug(f"{index+1} 件 実績作業時間情報を削除しました。")
 
         logger.info(f"{success_count} / {len(actual_working_times)} 件の実績作業時間を削除しました。")
 
-    def get_actual_working_times(
+    def get_actual_working_times(  # noqa: ANN201
         self,
         *,
         start_date: str,
         end_date: str,
         job_id: Optional[str],
         user_id: Optional[str],
         actual_working_time_id_list: Optional[list[str]],
@@ -83,21 +83,19 @@
             job_ids=[job_id] if job_id is not None else None,
             start_date=start_date,
             end_date=end_date,
             is_set_additional_info=True,
         )
 
         if actual_working_time_id_list is not None:
-            get_actual_working_times = [
-                e for e in get_actual_working_times if e["actual_working_time_id"] in set(actual_working_time_id_list)
-            ]
+            get_actual_working_times = [e for e in get_actual_working_times if e["actual_working_time_id"] in set(actual_working_time_id_list)]
 
         return get_actual_working_times
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         *,
         job_id: Optional[str],
         user_id: Optional[str],
         start_date: str,
         end_date: str,
         actual_working_time_id_list: Optional[list[str]],
@@ -107,20 +105,19 @@
             end_date=end_date,
             job_id=job_id,
             user_id=user_id,
             actual_working_time_id_list=actual_working_time_id_list,
         )
 
         if len(actual_working_times) == 0:
-            logger.info(f"削除する実績作業時間情報はありませんでした。")
+            logger.info("削除する実績作業時間情報はありませんでした。")
             return
 
         message = (
-            f"実績作業時間情報 {len(actual_working_times)} 件を削除します。よろしいですか？ :: "
-            f"start_date={start_date}, end_date={end_date}, "
+            f"実績作業時間情報 {len(actual_working_times)} 件を削除します。よろしいですか？ :: " f"start_date={start_date}, end_date={end_date}, "
         )
         if job_id is not None:
             job = self.annowork_service.api.get_job(self.workspace_id, job_id)
             message += f"job_id={job_id}, job_name={job['job_name']}, "
         if user_id is not None:
             message += f"user_id={user_id}, "
 
@@ -130,15 +127,15 @@
                 return
             if all_yes:
                 self.all_yes = all_yes
 
         self.delete_actual_working_times(actual_working_times)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
 
     if args.job_id is None and args.user_id is None:
         print("--job_id または --user_id を指定してください。", file=sys.stderr)
         sys.exit(COMMAND_LINE_ERROR_STATUS_CODE)
 
     actual_working_time_id_list = get_list_from_args(args.actual_working_time_id)
@@ -152,15 +149,15 @@
         user_id=args.user_id,
         actual_working_time_id_list=actual_working_time_id_list,
         start_date=args.start_date,
         end_date=args.end_date,
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -168,15 +165,17 @@
     parser.add_argument("--start_date", type=str, required=True, help="削除したい実績作業時間情報の開始日(YYYY-mm-dd)を指定してください。")
     parser.add_argument("--end_date", type=str, required=True, help="削除したい実績作業時間情報の終了日(YYYY-mm-dd)を指定してください。")
 
     parser.add_argument("-j", "--job_id", type=str, required=False, help="削除したい実績作業時間情報に紐づくjob_idを指定してください。")
     parser.add_argument("-u", "--user_id", type=str, required=False, help="削除したい実績作業時間情報に紐づくuser_idを指定してください。")
 
     parser.add_argument(
-        "--timezone_offset", type=float, help="日付に対するタイムゾーンのオフセット時間を指定します。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。"
+        "--timezone_offset",
+        type=float,
+        help="日付に対するタイムゾーンのオフセット時間を指定します。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。",
     )
 
     parser.add_argument(
         "--actual_working_time_id",
         type=str,
         nargs="+",
         required=False,
@@ -188,12 +187,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "delete"
     subcommand_help = "実績作業時間を削除します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/actual_working_time/list_actual_working_hours_daily.py` & `annoworkcli-3.7.0/annoworkcli/actual_working_time/list_actual_working_hours_daily.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 import argparse
 import datetime
 import json
 import logging
 import typing
 from collections import defaultdict
+from collections.abc import Sequence
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Sequence, Tuple
+from typing import Any, Dict, List, Optional, Tuple  # noqa: UP035
 
 import pandas
 from annoworkapi.job import get_parent_job_id_from_job_tree
 from annoworkapi.resource import Resource as AnnoworkResource
 from annoworkapi.utils import str_to_datetime
 from dataclasses_json import DataClassJsonMixin
 
 import annoworkcli
 from annoworkcli.actual_working_time.list_actual_working_time import ListActualWorkingTime
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
-ActualWorkingHoursDict = Dict[Tuple[datetime.date, str, str], float]
+ActualWorkingHoursDict = Dict[Tuple[datetime.date, str, str], float]  # noqa: UP006
 """実績作業時間の日ごとの情報を格納する辞書
 key: (date, workspace_member_id, job_id), value: 実績作業時間
 """
 
-ActualWorkingTimeNoteDict = Dict[Tuple[datetime.date, str, str], List[str]]
+ActualWorkingTimeNoteDict = Dict[Tuple[datetime.date, str, str], List[str]]  # noqa: UP006
 """実績作業の備考を格納する辞書
 key: (date, workspace_member_id, job_id), value: 備考のlist
 dateは実績のstart_datetimeから算出する
 """
 
 
 @dataclass
@@ -40,15 +41,15 @@
     job_name: str
     workspace_member_id: str
     user_id: str
     username: str
     actual_working_hours: float
     # listでなくtyping.Listを使っている理由：`list`だとPython3.8でデコード時にエラーが発生するため
     # https://qiita.com/yuji38kwmt/items/ce49efc91bb9b6430437
-    notes: Optional[typing.List[str]]
+    notes: Optional[typing.List[str]]  # noqa: UP006
 
 
 @dataclass
 class ActualWorkingHoursDailyWithParentJob(ActualWorkingHoursDaily):
     parent_job_id: Optional[str]
     parent_job_name: Optional[str]
 
@@ -80,17 +81,15 @@
         results_dict[(dt_local_start_datetime.date(), workspace_member_id, job_id)] = actual_working_hours
     else:
         dt_tmp_local_start_datetime = dt_local_start_datetime
 
         # 実績作業時間が24時間を超えることはないが、24時間を超えても計算できるような処理にする
         while dt_tmp_local_start_datetime.date() < dt_local_end_datetime.date():
             dt_next_date = dt_tmp_local_start_datetime.date() + datetime.timedelta(days=1)
-            dt_tmp_local_end_datetime = datetime.datetime(
-                year=dt_next_date.year, month=dt_next_date.month, day=dt_next_date.day, tzinfo=tzinfo
-            )
+            dt_tmp_local_end_datetime = datetime.datetime(year=dt_next_date.year, month=dt_next_date.month, day=dt_next_date.day, tzinfo=tzinfo)
             actual_working_hours = (dt_tmp_local_end_datetime - dt_tmp_local_start_datetime).total_seconds() / 3600
             results_dict[(dt_tmp_local_start_datetime.date(), workspace_member_id, job_id)] = actual_working_hours
             dt_tmp_local_start_datetime = dt_tmp_local_end_datetime
 
         actual_working_hours = (dt_local_end_datetime - dt_tmp_local_start_datetime).total_seconds() / 3600
         results_dict[(dt_local_end_datetime.date(), workspace_member_id, job_id)] = actual_working_hours
 
@@ -108,15 +107,15 @@
     job_dict: dict[str, SimpleJob] = {}
     member_dict: dict[str, SimpleworkspaceMember] = {}
 
     # none 判定
     if timezone_offset_hours is not None:
         tzinfo = datetime.timezone(datetime.timedelta(hours=timezone_offset_hours))
     else:
-        tzinfo = datetime.datetime.now().astimezone().tzinfo  # type: ignore
+        tzinfo = datetime.datetime.now().astimezone().tzinfo  # type: ignore[assignment]
 
     for actual in actual_working_time_list:
         tmp_results = _create_actual_working_hours_dict(actual, tzinfo=tzinfo)
 
         for key, value in tmp_results.items():
             results_dict[key] += value
 
@@ -200,21 +199,19 @@
             result = result and elm.date <= end_date
         return result
 
     return [e for e in actual_daily_list if is_match(e)]
 
 
 class ListActualWorkingHoursDaily:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-    def add_parent_job_info(
-        self, daily_list: Sequence[ActualWorkingHoursDaily]
-    ) -> list[ActualWorkingHoursDailyWithParentJob]:
+    def add_parent_job_info(self, daily_list: Sequence[ActualWorkingHoursDaily]) -> list[ActualWorkingHoursDailyWithParentJob]:
         all_job_list = self.annowork_service.api.get_jobs(self.workspace_id)
         all_job_dict = {e["job_id"]: e for e in all_job_list}
         parent_job_id_set = {get_parent_job_id_from_job_tree(e["job_tree"]) for e in all_job_list}
         if None in parent_job_id_set:
             parent_job_id_set.remove(None)
 
         result = []
@@ -255,25 +252,26 @@
             "actual_working_hours",
             "notes",
         ]
 
     return required_columns
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     parent_job_id_list = get_list_from_args(args.parent_job_id)
     user_id_list = get_list_from_args(args.user_id)
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     if all(v is None for v in [job_id_list, parent_job_id_list, user_id_list, start_date, end_date]):
         logger.warning(
-            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。" "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。"
+            "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
         )
 
     main_obj = ListActualWorkingHoursDaily(annowork_service, args.workspace_id)
 
     list_actual_working_time_obj = ListActualWorkingTime(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
@@ -293,36 +291,36 @@
     result: Sequence[ActualWorkingHoursDaily] = create_actual_working_hours_daily_list(
         actual_working_time_list, timezone_offset_hours=args.timezone_offset, show_notes=True
     )
 
     result = filter_actual_daily_list(result, start_date=start_date, end_date=end_date)
 
     if len(result) == 0:
-        logger.warning(f"日ごとの実績作業時間情報は0件なので、出力しません。")
+        logger.warning("日ごとの実績作業時間情報は0件なので、出力しません。")
         return
 
     show_parent_job: bool = args.show_parent_job
     if show_parent_job:
         result = main_obj.add_parent_job_info(result)
 
     if OutputFormat(args.format) == OutputFormat.JSON:
         # `.schema().dump(many=True)`を使わない理由：使うと警告が発生するから
         # https://qiita.com/yuji38kwmt/items/a3625b2011aff1d9901b
         dict_result = []
         for elm in result:
-            dict_result.append(elm.to_dict())
+            dict_result.append(elm.to_dict())  # noqa: PERF401
 
         print_json(dict_result, is_pretty=True, output=args.output)
     else:
         df = pandas.DataFrame(result)
         required_columns = get_required_columns(show_parent_job)
         print_csv(df[required_columns], output=args.output)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     required_group = parser.add_mutually_exclusive_group(required=True)
 
     required_group.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         help="対象のワークスペースID",
@@ -334,15 +332,17 @@
     job_id_group.add_argument("-j", "--job_id", type=str, nargs="+", required=False, help="絞り込み対象のジョブID")
     job_id_group.add_argument("-pj", "--parent_job_id", type=str, nargs="+", required=False, help="絞り込み対象の親のジョブID")
 
     parser.add_argument("--start_date", type=str, required=False, help="集計開始日(YYYY-mm-dd)")
     parser.add_argument("--end_date", type=str, required=False, help="集計終了日(YYYY-mm-dd)")
 
     parser.add_argument(
-        "--timezone_offset", type=float, help="日付に対するタイムゾーンのオフセット時間。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。"
+        "--timezone_offset",
+        type=float,
+        help="日付に対するタイムゾーンのオフセット時間。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。",
     )
 
     parser.add_argument(
         "--show_parent_job",
         action="store_true",
         help="親のジョブ情報も出力します。",
     )
@@ -361,12 +361,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_daily"
     subcommand_help = "実績作業時間を日ごとに集約した情報を一覧として出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py` & `annoworkcli-3.7.0/annoworkcli/actual_working_time/list_actual_working_hours_daily_groupby_tag.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import logging
 from collections import defaultdict
+from collections.abc import Collection, Sequence
 from pathlib import Path
-from typing import Any, Collection, Optional, Sequence
+from typing import Any, Optional
 
 import pandas
 from annoworkapi.job import get_parent_job_id_from_job_tree
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.actual_working_time.list_actual_working_hours_daily import (
@@ -18,20 +19,20 @@
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListActualWorkingTimeGroupbyTag:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str, timezone_offset_hours: int):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str, timezone_offset_hours: int):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
         self.timezone_offset_hours = timezone_offset_hours
 
-    def add_parent_job_info(self, daily_list: list[dict[str, Any]]):
+    def add_parent_job_info(self, daily_list: list[dict[str, Any]]):  # noqa: ANN201
         """引数daily_listに、parent_job情報を追加する。"""
         all_job_list = self.annowork_service.api.get_jobs(self.workspace_id)
         all_job_dict = {e["job_id"]: e for e in all_job_list}
         parent_job_id_set = {get_parent_job_id_from_job_tree(e["job_tree"]) for e in all_job_list}
         if None in parent_job_id_set:
             parent_job_id_set.remove(None)
 
@@ -72,17 +73,15 @@
 
         # keyはtuple[date, job_id, org_tag]のdict
         dict_hours: dict[tuple[str, str, str], float] = defaultdict(float)
 
         # ワークスペースタグごと日毎の時間を集計する
         for workspace_tag in workspace_tags:
             workspace_tag_name = workspace_tag["workspace_tag_name"]
-            members = self.annowork_service.api.get_workspace_tag_members(
-                self.workspace_id, workspace_tag["workspace_tag_id"]
-            )
+            members = self.annowork_service.api.get_workspace_tag_members(self.workspace_id, workspace_tag["workspace_tag_id"])
             member_ids = {e["workspace_member_id"] for e in members}
             for elm in actual_working_hours_daily:
                 if elm.workspace_member_id in member_ids:
                     dict_hours[(elm.date, elm.job_id, workspace_tag_name)] += elm.actual_working_hours
 
         # 全体の時間を日毎に集計する
 
@@ -132,20 +131,18 @@
         )
 
         logger.debug(f"{len(actual_working_time_list)} 件の実績作業時間情報を日ごとに集約します。")
         actual_working_hours_daily_list: Sequence[ActualWorkingHoursDaily] = create_actual_working_hours_daily_list(
             actual_working_time_list, timezone_offset_hours=self.timezone_offset_hours, show_notes=False
         )
 
-        actual_working_hours_daily_list = filter_actual_daily_list(
-            actual_working_hours_daily_list, start_date=start_date, end_date=end_date
-        )
+        actual_working_hours_daily_list = filter_actual_daily_list(actual_working_hours_daily_list, start_date=start_date, end_date=end_date)
         return actual_working_hours_daily_list
 
-    def main(
+    def main(  # noqa: ANN201, PLR0913
         self,
         *,
         output: Path,
         output_format: OutputFormat,
         job_ids: Optional[Collection[str]] = None,
         parent_job_ids: Optional[Collection[str]] = None,
         user_ids: Optional[Collection[str]] = None,
@@ -155,15 +152,15 @@
         target_workspace_tag_names: Optional[Collection[str]] = None,
         show_parent_job: bool = False,
     ):
         actual_working_hours_daily_list = self.get_actual_working_hours_daily(
             job_ids=job_ids, parent_job_ids=parent_job_ids, user_ids=user_ids, start_date=start_date, end_date=end_date
         )
         if len(actual_working_hours_daily_list) == 0:
-            logger.warning(f"日ごとの実績作業時間情報は0件なので、出力しません。")
+            logger.warning("日ごとの実績作業時間情報は0件なので、出力しません。")
             return
 
         results = self.get_actual_working_times_groupby_tag(
             actual_working_hours_daily_list,
             target_workspace_tag_ids=target_workspace_tag_ids,
             target_workspace_tag_names=target_workspace_tag_names,
             show_parent_job=show_parent_job,
@@ -195,25 +192,25 @@
 
             remaining_columns = list(set(df.columns) - set(required_columns))
             columns = required_columns + sorted(remaining_columns)
 
             print_csv(df[columns], output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     parent_job_id_list = get_list_from_args(args.parent_job_id)
     user_id_list = get_list_from_args(args.user_id)
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     if all(v is None for v in [job_id_list, parent_job_id_list, user_id_list, start_date, end_date]):
         logger.warning(
-            f"'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
         )
 
     workspace_tag_id_list = get_list_from_args(args.workspace_tag_id)
     workspace_tag_name_list = get_list_from_args(args.workspace_tag_name)
 
     ListActualWorkingTimeGroupbyTag(
         annowork_service=annowork_service,
@@ -229,15 +226,15 @@
         target_workspace_tag_names=workspace_tag_name_list,
         output=args.output,
         output_format=OutputFormat(args.format),
         show_parent_job=args.show_parent_job,
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     required_group = parser.add_mutually_exclusive_group(required=True)
 
     required_group.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         help="対象のワークスペースID",
@@ -266,15 +263,17 @@
         "--workspace_tag_name",
         type=str,
         nargs="+",
         help="出力対象のワークスペースタグ名。未指定の場合は全てのワークスペースタグを出力します。",
     )
 
     parser.add_argument(
-        "--timezone_offset", type=float, help="日付に対するタイムゾーンのオフセット時間。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。"
+        "--timezone_offset",
+        type=float,
+        help="日付に対するタイムゾーンのオフセット時間。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。",
     )
 
     parser.add_argument(
         "--show_parent_job",
         action="store_true",
         help="親のジョブ情報も出力します。",
     )
@@ -293,12 +292,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_daily_groupby_tag"
     subcommand_help = "日ごとの実績作業時間を、ワークスペースタグで集計した値を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/actual_working_time/list_actual_working_time.py` & `annoworkcli-3.7.0/annoworkcli/actual_working_time/list_actual_working_time.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import argparse
 import datetime
 import logging
+from collections.abc import Collection
 from pathlib import Path
-from typing import Any, Collection, Optional
+from typing import Any, Optional
 
 import pandas
 from annoworkapi.actual_working_time import get_term_start_end_from_date_for_actual_working_time
 from annoworkapi.job import get_parent_job_id_from_job_tree
 from annoworkapi.resource import Resource as AnnoworkResource
 from annoworkapi.utils import str_to_datetime
 
@@ -14,43 +15,37 @@
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListActualWorkingTime:
-    def __init__(
-        self, annowork_service: AnnoworkResource, workspace_id: str, *, timezone_offset_hours: Optional[float]
-    ):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str, *, timezone_offset_hours: Optional[float]):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-        self.workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+        self.workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
 
         # none 判定
         if timezone_offset_hours is not None:
             tzinfo = datetime.timezone(datetime.timedelta(hours=timezone_offset_hours))
         else:
-            tzinfo = datetime.datetime.now().astimezone().tzinfo  # type: ignore
+            tzinfo = datetime.datetime.now().astimezone().tzinfo  # type: ignore[assignment]
         self.tzinfo = tzinfo
         """日付に対するタイムゾーン"""
 
     def get_actual_working_times_by_workspace_member(
         self,
         workspace_member_id_list: list[str],
         *,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
     ) -> list[dict[str, Any]]:
         query_params = {}
-        term_start, term_end = get_term_start_end_from_date_for_actual_working_time(
-            start_date, end_date, tzinfo=self.tzinfo
-        )
+        term_start, term_end = get_term_start_end_from_date_for_actual_working_time(start_date, end_date, tzinfo=self.tzinfo)
         if term_start is not None:
             query_params["term_start"] = term_start
         if term_end is not None:
             query_params["term_end"] = term_end
 
         result = []
         for workspace_member_id in workspace_member_id_list:
@@ -65,17 +60,15 @@
         self,
         *,
         job_id_list: Optional[Collection[str]] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
     ) -> list[dict[str, Any]]:
         query_params = {}
-        term_start, term_end = get_term_start_end_from_date_for_actual_working_time(
-            start_date, end_date, tzinfo=self.tzinfo
-        )
+        term_start, term_end = get_term_start_end_from_date_for_actual_working_time(start_date, end_date, tzinfo=self.tzinfo)
         if term_start is not None:
             query_params["term_start"] = term_start
         if term_end is not None:
             query_params["term_end"] = term_end
 
         if job_id_list is not None:
             result = []
@@ -87,22 +80,18 @@
             return result
         else:
             logger.debug(f"実績時間情報を取得します。{query_params=}")
             return self.annowork_service.api.get_actual_working_times(self.workspace_id, query_params=query_params)
 
     @staticmethod
     def get_actual_working_hours(actual_working_time: dict[str, Any]) -> float:
-        delta = str_to_datetime(actual_working_time["end_datetime"]) - str_to_datetime(
-            actual_working_time["start_datetime"]
-        )
+        delta = str_to_datetime(actual_working_time["end_datetime"]) - str_to_datetime(actual_working_time["start_datetime"])
         return delta.total_seconds() / 3600
 
-    def set_additional_info_to_actual_working_time(
-        self, actual_working_time_list: list[dict[str, Any]], is_add_parent_job_info: bool = False
-    ):
+    def set_additional_info_to_actual_working_time(self, actual_working_time_list: list[dict[str, Any]], is_add_parent_job_info: bool = False):  # noqa: ANN201
         """workspace_member_id, job_idに紐づく情報を付与する。
 
         Args:
             actual_working_time_list (list[dict[str,Any]]): (IN/OUT) 実績作業時間のリスト
         """
         workspace_member_dict = {e["workspace_member_id"]: e for e in self.workspace_members}
         job_list = self.annowork_service.api.get_jobs(self.workspace_id)
@@ -125,17 +114,15 @@
             actual["actual_working_hours"] = self.get_actual_working_hours(actual)
             actual["user_id"] = member["user_id"]
             actual["username"] = member["username"]
 
             job_id = actual["job_id"]
             job = job_dict.get(job_id)
             if job is None:
-                logger.warning(
-                    f"{job_id=} であるジョブは存在しません。 " f":: actual_working_time_id= '{actual['actual_working_time_id']}' "
-                )
+                logger.warning(f"{job_id=} であるジョブは存在しません。 " f":: actual_working_time_id= '{actual['actual_working_time_id']}' ")
                 continue
             actual["job_name"] = job["job_name"]
             if is_add_parent_job_info:
                 parent_job_id = get_parent_job_id_from_job_tree(job["job_tree"])
                 actual["parent_job_id"] = parent_job_id
                 if parent_job_id is not None:
                     parent_job = job_dict[parent_job_id]
@@ -207,15 +194,15 @@
         else:
             result = self.get_actual_working_times_by_job(job_id_list=job_ids, start_date=start_date, end_date=end_date)
 
         if is_set_additional_info is not None:
             self.set_additional_info_to_actual_working_time(result, is_add_parent_job_info=is_add_parent_job_info)
         return result
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         *,
         output: Path,
         output_format: OutputFormat,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         job_id_list: Optional[list[str]] = None,
@@ -229,15 +216,15 @@
             job_ids=job_id_list,
             parent_job_ids=parent_job_id_list,
             user_ids=user_id_list,
             is_set_additional_info=True,
             is_add_parent_job_info=is_add_parent_job_info,
         )
         if len(result) == 0:
-            logger.warning(f"実績作業時間情報は0件なので、出力しません。")
+            logger.warning("実績作業時間情報は0件なので、出力しません。")
             return
 
         logger.info(f"{len(result)} 件の実績作業時間情報を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(result, is_pretty=True, output=output)
         else:
@@ -273,25 +260,26 @@
                     "note",
                 ]
             remaining_columns = list(set(df.columns) - set(required_columns))
             columns = required_columns + remaining_columns
             print_csv(df[columns], output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     parent_job_id_list = get_list_from_args(args.parent_job_id)
     user_id_list = get_list_from_args(args.user_id)
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     if all(v is None for v in [job_id_list, parent_job_id_list, user_id_list, start_date, end_date]):
         logger.warning(
-            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。" "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。"
+            "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
         )
 
     ListActualWorkingTime(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
         timezone_offset_hours=args.timezone_offset,
     ).main(
@@ -302,15 +290,15 @@
         end_date=end_date,
         is_add_parent_job_info=args.show_parent_job,
         output=args.output,
         output_format=OutputFormat(args.format),
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -328,15 +316,17 @@
     parser.add_argument(
         "--show_parent_job",
         action="store_true",
         help="親のジョブ情報も出力します。",
     )
 
     parser.add_argument(
-        "--timezone_offset", type=float, help="日付に対するタイムゾーンのオフセット時間を指定します。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。"
+        "--timezone_offset",
+        type=float,
+        help="日付に対するタイムゾーンのオフセット時間を指定します。例えばJSTなら '9' です。指定しない場合はローカルのタイムゾーンを参照します。",
     )
 
     parser.add_argument("-o", "--output", type=Path, help="出力先")
 
     parser.add_argument(
         "-f",
         "--format",
@@ -349,12 +339,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list"
     subcommand_help = "実績作業時間情報の一覧を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/actual_working_time/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/actual_working_time/subcommand.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,27 +4,25 @@
 import annoworkcli
 import annoworkcli.actual_working_time.delete_actual_working_time
 import annoworkcli.actual_working_time.list_actual_working_hours_daily
 import annoworkcli.actual_working_time.list_actual_working_hours_daily_groupby_tag
 import annoworkcli.actual_working_time.list_actual_working_time
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     # 実績作業時間の削除は間違って削除してしまったときの影響が大きいので、有効にしない。
     # annoworkcli.actual_working_time.delete_actual_working_time.add_parser(subparsers)
     annoworkcli.actual_working_time.list_actual_working_time.add_parser(subparsers)
     annoworkcli.actual_working_time.list_actual_working_hours_daily.add_parser(subparsers)
     annoworkcli.actual_working_time.list_actual_working_hours_daily_groupby_tag.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "actual_working_time"
     subcommand_help = "実績作業時間関係のサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/list_job_with_annofab_project.py` & `annoworkcli-3.7.0/annoworkcli/annofab/list_job_with_annofab_project.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         if af_project_id is None:
             continue
         af_project_id_set.add(af_project_id)
     return af_project_id_set
 
 
 class ListJobWithAnnofabProject:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         *,
         annowork_service: AnnoworkResource,
         workspace_id: str,
         annofab_service: AnnofabResource,
         parallelism: Optional[int] = None,
     ):
@@ -109,30 +109,28 @@
             af_project_id = get_annofab_project_id_from_url(external_linkage_info_url)
             if af_project_id is None:
                 job["annofab"] = None
                 continue
 
             af_project = af_project_dict.get(af_project_id)
             if af_project is None:
-                logger.warning(
-                    f"annofab_project_id='{af_project_id}' のAnnofabプロジェクトを取得できませんでした。:: job_id={job['job_id']}"
-                )
+                logger.warning(f"annofab_project_id='{af_project_id}' のAnnofabプロジェクトを取得できませんでした。:: job_id={job['job_id']}")
                 job["annofab"] = None
                 continue
 
             job["annofab"] = {
                 "project_id": af_project["project_id"],
                 "project_title": af_project["title"],
                 "project_status": af_project["project_status"],
                 "input_data_type": af_project["input_data_type"],
             }
         return job_list
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     parent_job_id_list = get_list_from_args(args.parent_job_id)
     annofab_project_id_list = get_list_from_args(args.annofab_project_id)
 
     main_obj = ListJobWithAnnofabProject(
         annowork_service=annowork_service,
@@ -148,27 +146,27 @@
         job_id_list=job_id_list,
         parent_job_id_list=parent_job_id_list,
         annofab_project_id_list=annofab_project_id_list,
         is_show_parent_job=args.show_parent_job,
     )
 
     if len(job_list) == 0:
-        logger.warning(f"ジョブの一覧が0件なので、出力しません。")
+        logger.warning("ジョブの一覧が0件なので、出力しません。")
         return
 
     logger.info(f"{len(job_list)} 件のジョブの一覧を出力します。")
 
     if OutputFormat(args.format) == OutputFormat.JSON:
         print_json(job_list, is_pretty=True, output=args.output)
     else:
         df = pandas.json_normalize(job_list)
         print_csv(df, output=args.output)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -203,28 +201,24 @@
         "--show_parent_job",
         action="store_true",
         help="親のジョブ情報も出力します。",
     )
 
     parser.add_argument("-o", "--output", type=Path, help="出力先")
 
-    parser.add_argument(
-        "-f", "--format", type=str, choices=[e.value for e in OutputFormat], help="出力先", default=OutputFormat.CSV.value
-    )
+    parser.add_argument("-f", "--format", type=str, choices=[e.value for e in OutputFormat], help="出力先", default=OutputFormat.CSV.value)
 
     parser.add_argument("--parallelism", type=int, required=False, help="並列度。指定しない場合は、逐次的に処理します。")
 
     parser.add_argument("--annofab_mfa_code", type=str, help="Annofabにログインする際のMFAコード")
     parser.add_argument("--annofab_user_id", type=str, help="Annofabにログインする際のユーザID")
     parser.add_argument("--annofab_password", type=str, help="Annofabにログインする際のパスワード")
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_job"
     subcommand_help = "ジョブとジョブに紐づくAnnofabプロジェクトの情報を一緒に出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/list_working_hours.py` & `annoworkcli-3.7.0/annoworkcli/annofab/list_working_hours.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import argparse
 import functools
 import itertools
 import logging
 import multiprocessing
+from collections.abc import Collection
 from pathlib import Path
-from typing import Any, Collection, Optional
+from typing import Any, Optional
 
 import pandas
 import requests
 from annofabapi.resource import Resource as AnnofabResource
 from annoworkapi.job import get_parent_job_id_from_job_tree
 from annoworkapi.resource import Resource as AnnoworkResource
 
@@ -40,33 +41,27 @@
     Args:
         df_actual_working_hours: 実績作業時間情報
         df_user_and_af_account: ユーザ情報とAnnofabアカウント情報
         df_job_and_af_project: ジョブ情報とAnnofabプロジェクト情報
         df_af_working_hours: Annofabの作業時間情報
     """
     # annowork側の作業時間情報
-    df_aw_working_hours = df_actual_working_hours.merge(
-        df_user_and_af_account[["user_id", "annofab_account_id"]], how="left", on="user_id"
-    ).merge(
+    df_aw_working_hours = df_actual_working_hours.merge(df_user_and_af_account[["user_id", "annofab_account_id"]], how="left", on="user_id").merge(
         df_job_and_af_project[["job_id", "annofab_project_id"]],
         how="left",
         on="job_id",
     )
 
-    df_merged = df_aw_working_hours.merge(
-        df_af_working_hours, how="outer", on=["date", "annofab_project_id", "annofab_account_id"]
-    )
+    df_merged = df_aw_working_hours.merge(df_af_working_hours, how="outer", on=["date", "annofab_project_id", "annofab_account_id"])
 
     TMP_SUFFIX = "_tmp"
     # df_merged は outer joinしているため、左側にも欠損値ができる。
     # それを埋めるために、以前に user情報, job情報の一意な dataframe を生成して、欠損値を埋める
     USER_COLUMNS = ["workspace_member_id", "user_id", "username"]
-    df_merged = df_merged.merge(
-        df_user_and_af_account, how="left", on="annofab_account_id", suffixes=(None, TMP_SUFFIX)
-    )
+    df_merged = df_merged.merge(df_user_and_af_account, how="left", on="annofab_account_id", suffixes=(None, TMP_SUFFIX))
     for user_column in USER_COLUMNS:
         df_merged[user_column] = df_merged[user_column].fillna(df_merged[f"{user_column}{TMP_SUFFIX}"])
 
     # job_id, job_nameの欠損値を、df_job_and_af_project を使って埋める
     # af_projectに紐付いているジョブとaf_projectのDataFrameを生成して、それを使って欠損値を埋める
     # drop_duplicatesの理由: AnnoworkのジョブとAnnofabのプロジェクトが1対1で紐づくときだけ、df_mergeのjob_idとjob_nameの欠損値を埋めるようにするため
     df_job_id_af_project = df_job_and_af_project[df_job_and_af_project["annofab_project_id"].notna()].drop_duplicates(
@@ -78,43 +73,43 @@
         on=["annofab_project_id"],
         suffixes=(None, TMP_SUFFIX),
     )
     df_merged["job_id"] = df_merged["job_id"].fillna(df_merged[f"job_id{TMP_SUFFIX}"])
     df_merged["job_name"] = df_merged["job_name"].fillna(df_merged[f"job_name{TMP_SUFFIX}"])
 
     # annofab_project_titleを結合するために、annofab_projectだけのDataFrameを生成する
-    df_af_project = df_job_and_af_project.drop_duplicates(subset=["annofab_project_id"])[
-        ["annofab_project_id", "annofab_project_title"]
-    ]
+    df_af_project = df_job_and_af_project.drop_duplicates(subset=["annofab_project_id"])[["annofab_project_id", "annofab_project_title"]]
     df_merged = df_merged.merge(df_af_project, on="annofab_project_id", how="left")
 
     df_merged.fillna(
         {
             "actual_working_hours": 0,
             "annofab_working_hours": 0,
         },
         inplace=True,
     )
 
     return df_merged[
-        ["date", "job_id", "job_name"]
-        + USER_COLUMNS
-        + [
+        [
+            "date",
+            "job_id",
+            "job_name",
+            *USER_COLUMNS,
             "actual_working_hours",
             "annofab_project_id",
             "annofab_project_title",
             "annofab_account_id",
             "annofab_working_hours",
             "notes",
         ]
     ]
 
 
 class ListWorkingHoursWithAnnofab:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         *,
         annowork_service: AnnoworkResource,
         workspace_id: str,
         annofab_service: AnnofabResource,
         parallelism: Optional[int] = None,
     ):
@@ -124,17 +119,15 @@
         self.parallelism = parallelism
 
         self.all_jobs = self.annowork_service.api.get_jobs(self.workspace_id)
         self.all_workspace_members = self.annowork_service.api.get_workspace_members(
             self.workspace_id, query_params={"includes_inactive_members": True}
         )
 
-        self.list_actual_working_time_obj = ListActualWorkingTime(
-            annowork_service, workspace_id, timezone_offset_hours=TIMEZONE_OFFSET_HOURS
-        )
+        self.list_actual_working_time_obj = ListActualWorkingTime(annowork_service, workspace_id, timezone_offset_hours=TIMEZONE_OFFSET_HOURS)
 
     def get_actual_working_hours_daily(
         self,
         *,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         job_ids: Optional[Collection[str]] = None,
@@ -147,17 +140,15 @@
             user_ids=user_ids,
             start_date=start_date,
             end_date=end_date,
             is_set_additional_info=False,
         )
         self.list_actual_working_time_obj.set_additional_info_to_actual_working_time(actual_working_time_list)
 
-        result = create_actual_working_hours_daily_list(
-            actual_working_time_list, timezone_offset_hours=TIMEZONE_OFFSET_HOURS
-        )
+        result = create_actual_working_hours_daily_list(actual_working_time_list, timezone_offset_hours=TIMEZONE_OFFSET_HOURS)
         result = filter_actual_daily_list(result, start_date=start_date, end_date=end_date)
         return result
 
     def _get_df_user_and_af_account(self, user_ids: Collection[str]) -> pandas.DataFrame:
         """ユーザ情報とAnnofabのアカウント情報格納されたpandas.DataFrameを返します。
         以下の列を持ちます。
         * user_id
@@ -199,32 +190,24 @@
             return project["title"]
 
         all_job_dict = {e["job_id"]: e for e in self.all_jobs}
 
         df_job = pandas.DataFrame(self.all_jobs)
 
         df_af_project = pandas.DataFrame({"job_id": list(job_ids)})
-        df_af_project["annofab_project_id"] = df_af_project["job_id"].apply(
-            lambda e: get_annofab_project_id_from_job(all_job_dict[e])
-        )
+        df_af_project["annofab_project_id"] = df_af_project["job_id"].apply(lambda e: get_annofab_project_id_from_job(all_job_dict[e]))
         df_af_project["annofab_project_title"] = df_af_project["annofab_project_id"].apply(get_project_title)
 
         df = df_job.merge(df_af_project, how="inner", on="job_id")
         return df[["job_id", "job_name", "annofab_project_id", "annofab_project_title"]]
 
-    def _get_af_working_hours_from_af_project(
-        self, af_project_id: str, start_date: Optional[str], end_date: Optional[str]
-    ) -> list[dict[str, Any]]:
+    def _get_af_working_hours_from_af_project(self, af_project_id: str, start_date: Optional[str], end_date: Optional[str]) -> list[dict[str, Any]]:
         try:
-            logger.debug(
-                f"annofab_project_id= '{af_project_id}' のAnnofabプロジェクトの作業時間を取得します。:: {start_date=}, {end_date=}"
-            )
-            account_statistics = self.annofab_service.wrapper.get_account_daily_statistics(
-                af_project_id, from_date=start_date, to_date=end_date
-            )
+            logger.debug(f"annofab_project_id= '{af_project_id}' のAnnofabプロジェクトの作業時間を取得します。:: {start_date=}, {end_date=}")
+            account_statistics = self.annofab_service.wrapper.get_account_daily_statistics(af_project_id, from_date=start_date, to_date=end_date)
         except requests.exceptions.HTTPError as e:
             if e.response.status_code == requests.codes.not_found:
                 logger.warning(f"annofab_project_id= '{af_project_id}' は存在しません。")
             else:
                 logger.warning(f"annofab_project_id= '{af_project_id}' の作業時間を取得できませんでした。:: {e}")
             return []
 
@@ -241,17 +224,15 @@
                             "annofab_account_id": af_account_id,
                             "date": history["date"],
                             "annofab_working_hours": working_hours,
                         }
                     )
         return result
 
-    def _get_af_working_hours(
-        self, af_project_ids: Collection[str], start_date: Optional[str], end_date: Optional[str]
-    ) -> pandas.DataFrame:
+    def _get_af_working_hours(self, af_project_ids: Collection[str], start_date: Optional[str], end_date: Optional[str]) -> pandas.DataFrame:
         """Annofabの作業時間情報が格納されたDataFrameを返す。
 
         返すDataFrameには以下の列が存在します。
         * date
         * annofab_project_id
         * annofab_account_id
         * annofab_working_hours
@@ -268,44 +249,40 @@
             )
             with multiprocessing.Pool(self.parallelism) as pool:
                 tmp_result = pool.map(partial_func, af_project_ids)
                 result = list(itertools.chain.from_iterable(tmp_result))
 
         else:
             for af_project_id in af_project_ids:
-                result.extend(
-                    self._get_af_working_hours_from_af_project(af_project_id, start_date=start_date, end_date=end_date)
-                )
+                result.extend(self._get_af_working_hours_from_af_project(af_project_id, start_date=start_date, end_date=end_date))
 
         if len(result) > 0:
             return pandas.DataFrame(result)
 
         df = pandas.DataFrame(columns=["date", "annofab_project_id", "annofab_account_id", "annofab_working_hours"])
-        # `astype()`を使用する理由：後続の処理で`fillna()`を実行した際に、「Downcasting object dtype arrays ～」というFutureWarningを発生させないようにするため
+        # `astype()`を使用する理由：後続の処理で`fillna()`を実行した際に、「Downcasting object dtype arrays ～」というFutureWarningを発生させないようにするため  # noqa: E501
         # https://qiita.com/yuji38kwmt/items/ba07a25924cfda363e42
         df = df.astype({"annofab_working_hours": "float64"})
         return df
 
     def _get_df_job_parent_job(self) -> pandas.DataFrame:
         """job_id, parent_job_id, parent_job_nameが格納されたpandas.DataFrameを返します。"""
         all_job_dict = {e["job_id"]: e for e in self.all_jobs}
 
         df_job = pandas.DataFrame(self.all_jobs)
         df_job["parent_job_id"] = df_job["job_tree"].apply(get_parent_job_id_from_job_tree)
 
         df_parent_job = pandas.DataFrame({"parent_job_id": df_job["parent_job_id"].unique()})
-        df_parent_job["parent_job_name"] = df_parent_job["parent_job_id"].apply(
-            lambda e: all_job_dict[e]["job_name"] if e is not None else None
-        )
+        df_parent_job["parent_job_name"] = df_parent_job["parent_job_id"].apply(lambda e: all_job_dict[e]["job_name"] if e is not None else None)
 
         df = df_job.merge(df_parent_job, how="left", on="parent_job_id")
         return df[["job_id", "parent_job_id", "parent_job_name"]]
 
     @staticmethod
-    def _get_required_columns(is_show_parent_job: bool):
+    def _get_required_columns(is_show_parent_job: bool) -> list[str]:
         job_columns = [
             "job_id",
             "job_name",
         ]
         user_columns = [
             "workspace_member_id",
             "user_id",
@@ -314,19 +291,17 @@
         annofab_columns = ["annofab_project_id", "annofab_project_title", "annofab_account_id", "annofab_working_hours"]
 
         if is_show_parent_job:
             parent_job_columns = [
                 "parent_job_id",
                 "parent_job_name",
             ]
-            required_columns = (
-                ["date"] + job_columns + parent_job_columns + user_columns + ["actual_working_hours"] + annofab_columns
-            )
+            required_columns = ["date"] + job_columns + parent_job_columns + user_columns + ["actual_working_hours"] + annofab_columns  # noqa: RUF005
         else:
-            required_columns = ["date"] + job_columns + user_columns + ["actual_working_hours"] + annofab_columns
+            required_columns = ["date"] + job_columns + user_columns + ["actual_working_hours"] + annofab_columns  # noqa: RUF005
 
         required_columns.append("notes")
         return required_columns
 
     def get_df_working_hours(
         self,
         *,
@@ -350,15 +325,15 @@
             """
             df = df.drop_duplicates(subset=["annofab_project_id", "annofab_project_title"])
             # 補足：
             #  * annofab_project_idがnaのとき：Annofabプロジェクトに紐付いていないジョブ
             #  * annofab_project_titleがnaのとき：アクセスできないAnnofabプロジェクトに紐付いているジョブ
             df = df[df["annofab_project_id"].notna() & df["annofab_project_title"].notna()]
             # `unique()`を実行する理由：前述の`drop_duplicates`でannofab_project_idはユニークなはずだが、念の為`unique()`を実行した。
-            return list(e for e in df["annofab_project_id"].unique())
+            return list(df["annofab_project_id"].unique())
 
         def _get_start_date(df: pandas.DataFrame) -> Optional[str]:
             min_date = df["date"].min() if len(df) > 0 else None
             if start_date is None:
                 return min_date
             if min_date is not None:
                 return min(start_date, min_date)
@@ -422,46 +397,40 @@
             df = df.merge(df_job_parent_job, how="left", on="job_id")
 
         df.sort_values(["date", "job_id", "user_id"], inplace=True)
         required_columns = self._get_required_columns(is_show_parent_job)
         return df[required_columns]
 
     def get_job_id_list_from_parent_job_id_list(self, parent_job_id_list: Collection[str]) -> list[str]:
-        return [
-            e["job_id"]
-            for e in self.all_jobs
-            if get_parent_job_id_from_job_tree(e["job_tree"]) in set(parent_job_id_list)
-        ]
+        return [e["job_id"] for e in self.all_jobs if get_parent_job_id_from_job_tree(e["job_tree"]) in set(parent_job_id_list)]
 
     def get_job_id_list_from_annofab_project_id_list(self, annofab_project_id_list: list[str]) -> list[str]:
         annofab_project_id_set = set(annofab_project_id_list)
 
         def _match_job(job: dict[str, Any]) -> bool:
             af_project_id = get_annofab_project_id_from_job(job)
             if af_project_id is None:
                 return False
             return af_project_id in annofab_project_id_set
 
         return [e["job_id"] for e in self.all_jobs if _match_job(e)]
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     job_id_list = get_list_from_args(args.job_id)
     parent_job_id_list = get_list_from_args(args.parent_job_id)
     annofab_project_id_list = get_list_from_args(args.annofab_project_id)
     user_id_list = get_list_from_args(args.user_id)
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
-    if all(
-        v is None
-        for v in [job_id_list, parent_job_id_list, annofab_project_id_list, user_id_list, start_date, end_date]
-    ):
+    if all(v is None for v in [job_id_list, parent_job_id_list, annofab_project_id_list, user_id_list, start_date, end_date]):
         logger.warning(
-            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。" "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。"
+            "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
         )
 
     main_obj = ListWorkingHoursWithAnnofab(
         annowork_service=build_annoworkapi(args),
         workspace_id=args.workspace_id,
         annofab_service=build_annofabapi_resource_and_login(
             annofab_login_user_id=args.annofab_user_id,
@@ -482,26 +451,26 @@
         end_date=end_date,
         job_ids=job_id_list,
         user_ids=user_id_list,
         is_show_parent_job=args.show_parent_job,
     )
 
     if len(df) == 0:
-        logger.warning(f"作業時間情報は0件なので、出力しません。")
+        logger.warning("作業時間情報は0件なので、出力しません。")
         return
 
     logger.info(f"{len(df)} 件の作業時間情報を出力します。")
 
     if OutputFormat(args.format) == OutputFormat.JSON:
         print_json(df.to_dict("records"), is_pretty=True, output=args.output)
     else:
         print_csv(df, output=args.output)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -550,12 +519,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_working_hours"
     subcommand_help = "日ごとの実績作業時間と、ジョブに紐づくAnnofabプロジェクトの作業時間を一緒に出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/put_account_external_linkage_info.py` & `annoworkcli-3.7.0/annoworkcli/annofab/put_account_external_linkage_info.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
     if "account_id" not in external_linkage_info["annofab"]:
         return None
     return external_linkage_info["annofab"]["account_id"]
 
 
 class PutAnnofabAccountId:
-    def __init__(self, *, annowork_service: AnnoworkResource, annofab_service: AnnofabResource, overwrite: bool):
+    def __init__(self, *, annowork_service: AnnoworkResource, annofab_service: AnnofabResource, overwrite: bool):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.annofab_service = annofab_service
         self.overwrite = overwrite
 
     def put_account_annofab_info_for_user(self, user_id: str, af_account_id: str) -> bool:
         content = self.annowork_service.wrapper.get_account_external_linkage_info_or_none(user_id)
         if content is None:
@@ -49,19 +49,17 @@
             request_body["last_updated_datetime"] = last_updated_datetime
 
         logger.debug(f"{request_body=}")
         self.annowork_service.api.put_account_external_linkage_info(user_id, request_body=request_body)
         logger.debug(f"{user_id=}: アカウントの外部連携情報に {af_account_id=} を設定しました。")
         return True
 
-    def main(self, af_workspace_name: str, user_id_list: list[str]):
+    def main(self, af_workspace_name: str, user_id_list: list[str]):  # noqa: ANN201
         af_workspace_member_list = self.annofab_service.wrapper.get_all_organization_members(af_workspace_name)
-        af_user_id_account_id_dict: dict[str, str] = {
-            member["user_id"]: member["account_id"] for member in af_workspace_member_list
-        }
+        af_user_id_account_id_dict: dict[str, str] = {member["user_id"]: member["account_id"] for member in af_workspace_member_list}
 
         success_count = 0
         for user_id in user_id_list:
             af_account_id = af_user_id_account_id_dict.get(user_id)
             if af_account_id is None:
                 logger.warning(f"Annofabのワークスペース '{af_workspace_name}' に {user_id=} のユーザは存在しないので、スキップします。")
                 continue
@@ -72,29 +70,29 @@
                     success_count += 1
             except Exception as e:
                 logger.warning(f"{user_id=}: アカウントの外部連携情報の設定に失敗しました。:: {e}")
 
         logger.info(f"{success_count} / {len(user_id_list)} 件、アカウントの外部連携情報の設定しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     annofab_service = build_annofabapi_resource_and_login(
         annofab_login_user_id=args.annofab_user_id,
         annofab_login_password=args.annofab_password,
         mfa_code=args.annofab_mfa_code,
     )
     user_id_list = get_list_from_args(args.user_id)
     assert user_id_list is not None
-    PutAnnofabAccountId(
-        annowork_service=annowork_service, annofab_service=annofab_service, overwrite=args.overwrite
-    ).main(af_workspace_name=args.annofab_workspace_name, user_id_list=user_id_list)
+    PutAnnofabAccountId(annowork_service=annowork_service, annofab_service=annofab_service, overwrite=args.overwrite).main(
+        af_workspace_name=args.annofab_workspace_name, user_id_list=user_id_list
+    )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-u",
         "--user_id",
         type=str,
         nargs="+",
         required=True,
         help="外部連携情報を設定するユーザのuser_id。",
@@ -119,14 +117,15 @@
     parser.add_argument("--annofab_password", type=str, help="Annofabにログインする際のパスワード")
 
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "put_account_external_linkage_info"
-    subcommand_help = "アカウントの外部連携情報に、Annofabから取得したaccount_idを設定します。\n" "Annofabのuser_idはAnnoworkのuser_idと一致している必要があります。"
-
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
+    subcommand_help = (
+        "アカウントの外部連携情報に、Annofabから取得したaccount_idを設定します。\n"
+        "Annofabのuser_idはAnnoworkのuser_idと一致している必要があります。"
     )
+
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/put_job_from_annofab_project.py` & `annoworkcli-3.7.0/annoworkcli/annofab/put_job_from_annofab_project.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,28 +9,26 @@
 from annoworkcli.annofab.utils import build_annofabapi_resource_and_login
 from annoworkcli.common.cli import build_annoworkapi
 
 logger = logging.getLogger(__name__)
 
 
 class PutJobFromAnnofabProject:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         *,
         annowork_service: AnnoworkResource,
         workspace_id: str,
         annofab_service: AnnofabResource,
     ):
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
         self.annofab_service = annofab_service
 
-    def put_job_from_annofab_project(
-        self, parent_job_id: str, annofab_project_id: str, job_id: Optional[str] = None
-    ) -> bool:
+    def put_job_from_annofab_project(self, parent_job_id: str, annofab_project_id: str, job_id: Optional[str] = None) -> bool:
         af_project = self.annofab_service.wrapper.get_project_or_none(annofab_project_id)
         if af_project is None:
             logger.warning(f"{annofab_project_id=} にアクセスできません。ジョブの登録処理をスキップします。")
             return False
 
         new_job_id = job_id if job_id is not None else annofab_project_id
 
@@ -48,31 +46,29 @@
         }
 
         new_job = self.annowork_service.api.put_job(self.workspace_id, new_job_id, request_body=request_body)
         logger.debug(f"annofab_project_id={annofab_project_id} に対応するジョブを作成しました。 :: {new_job}")
         return True
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     main_obj = PutJobFromAnnofabProject(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
         annofab_service=build_annofabapi_resource_and_login(
             annofab_login_user_id=args.annofab_user_id,
             annofab_login_password=args.annofab_password,
             mfa_code=args.annofab_mfa_code,
         ),
     )
-    main_obj.put_job_from_annofab_project(
-        parent_job_id=args.parent_job_id, annofab_project_id=args.annofab_project_id, job_id=args.job_id
-    )
+    main_obj.put_job_from_annofab_project(parent_job_id=args.parent_job_id, annofab_project_id=args.annofab_project_id, job_id=args.job_id)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/reshape_working_hours.py` & `annoworkcli-3.7.0/annoworkcli/annofab/reshape_working_hours.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # pylint: disable=too-many-lines
 
 
 import argparse
 import json
 import logging
+from collections.abc import Collection
 from enum import Enum
 from pathlib import Path
-from typing import Any, Collection, Optional
+from typing import Any, Optional
 
 import numpy
 import pandas
 from annofabapi.resource import Resource as AnnofabResource
 from annoworkapi.job import get_parent_job_id_from_job_tree
 from annoworkapi.resource import Resource as AnnoworkResource
 
@@ -51,15 +52,15 @@
     LIST_BY_DATE_USER_PARENT_JOB = "list_by_date_user_parent_job"
     """作業時間の一覧を、日付, ユーザ, 親ジョブ単位で出力する。アサイン時間と比較しても意味のある情報にならないので、アサイン時間は含まない。"""
 
     LIST_BY_DATE_USER_JOB = "list_by_date_user_job"
     """作業時間の一覧を、日付, ユーザ, ジョブ単位で出力する。アサイン対象のジョブと比較できないので、アサイン時間は含まない。"""
 
 
-def filter_df(
+def filter_df(  # noqa: ANN201
     df: pandas.DataFrame,
     *,
     job_ids: Optional[Collection[str]] = None,
     user_ids: Optional[Collection[str]] = None,
     start_date: Optional[str] = None,
     end_date: Optional[str] = None,
 ):
@@ -215,27 +216,25 @@
             df_job_parent_job: job_id, parent_job_id, parent_job_name 列が格納されたDataFrame。
                 指定されなければ、parent_job_id, parent_job_nameは格納しません。
 
         Notes:
             アサイン時間はparent_jobに対して指定するので、アサイン時間情報は参照しない。
         """
         # dropna=Falseを指定する理由: 複数のジョブが同じAnnofabプロジェクトを参照している場合、ジョブを特定できないためjob_idが空になるときがあるため
-        df_sum_actual = df_actual.groupby("job_id", dropna=False)[
-            ["actual_working_hours", "annofab_working_hours"]
-        ].sum()
+        df_sum_actual = df_actual.groupby("job_id", dropna=False)[["actual_working_hours", "annofab_working_hours"]].sum()
         # df_sum_actual が0件のときは、列がないので追加する
         if "actual_working_hours" not in df_sum_actual.columns:
             df_sum_actual["actual_working_hours"] = 0
         if "annofab_working_hours" not in df_sum_actual.columns:
             df_sum_actual["annofab_working_hours"] = 0
 
         # job_id, job_name, parent_job_id, parent_job_name, annofab_project_id 列を持つ列
-        df_job = df_actual.drop_duplicates(subset=["job_id"])[
-            ["job_id", "job_name", "annofab_project_id", "annofab_project_title"]
-        ].set_index("job_id")
+        df_job = df_actual.drop_duplicates(subset=["job_id"])[["job_id", "job_name", "annofab_project_id", "annofab_project_title"]].set_index(
+            "job_id"
+        )
         if df_job_parent_job is not None:
             df_job = df_job.join(df_job_parent_job.set_index("job_id"), how="left")
 
         df = df_sum_actual.join(df_job, how="left")
 
         df.fillna(
             {
@@ -256,15 +255,15 @@
         if df_job_parent_job is not None:
             extension_columns = [
                 "parent_job_id",
                 "parent_job_name",
             ]
 
         columns = (
-            [
+            [  # noqa: RUF005
                 "job_id",
                 "job_name",
             ]
             + extension_columns
             + [
                 "annofab_project_id",
                 "annofab_project_title",
@@ -284,17 +283,15 @@
         df_job_parent_job: pandas.DataFrame,
         df_parent_job: pandas.DataFrame,
     ) -> pandas.DataFrame:
         """`--shape_type total_by_parent_job`に対応するDataFrameを生成する。"""
 
         df_tmp_actual = df_actual.merge(df_job_parent_job, how="left", on="job_id", suffixes=("_tmp", None))
         # dropna=Falseを指定する理由: 複数のジョブが同じAnnofabプロジェクトを参照している場合、ジョブを特定できないためjob_idが空になるときがあるため
-        df_sum_actual = df_tmp_actual.groupby("parent_job_id", dropna=False)[
-            ["actual_working_hours", "annofab_working_hours"]
-        ].sum()
+        df_sum_actual = df_tmp_actual.groupby("parent_job_id", dropna=False)[["actual_working_hours", "annofab_working_hours"]].sum()
         df_sum_actual.reset_index(inplace=True)
         # df_sum_actual が0件のときは、列がないので追加する
         if "actual_working_hours" not in df_sum_actual.columns:
             df_sum_actual["actual_working_hours"] = 0
         if "annofab_working_hours" not in df_sum_actual.columns:
             df_sum_actual["annofab_working_hours"] = 0
 
@@ -354,25 +351,17 @@
         `--shape_type total_by_user_parent_job`に対応するDataFrameを生成する。
 
         Args:
             df_job_parent_job: job_id, parent_job_id 列を持つDataFrame
 
         """
         # groupbyをjob_id, parent_job_idの2回に分けている理由：join/mergeするときの行数を減らすため
-        df_sum_actual_groupby_job_id = df_actual.groupby(["user_id", "job_id"])[
-            ["actual_working_hours", "annofab_working_hours"]
-        ].sum()
-        df_sum_actual_groupby_job_id = df_sum_actual_groupby_job_id.join(
-            df_job_parent_job.set_index("job_id"), how="left"
-        )
-        df_sum_actual = (
-            df_sum_actual_groupby_job_id.reset_index(level="user_id")
-            .groupby(by=["user_id", "parent_job_id"])
-            .sum(numeric_only=True)
-        )
+        df_sum_actual_groupby_job_id = df_actual.groupby(["user_id", "job_id"])[["actual_working_hours", "annofab_working_hours"]].sum()
+        df_sum_actual_groupby_job_id = df_sum_actual_groupby_job_id.join(df_job_parent_job.set_index("job_id"), how="left")
+        df_sum_actual = df_sum_actual_groupby_job_id.reset_index(level="user_id").groupby(by=["user_id", "parent_job_id"]).sum(numeric_only=True)
 
         # df_sum_actual が0件のときは、列がないので追加する
         # TODO 必要か？
         if "actual_working_hours" not in df_sum_actual.columns:
             df_sum_actual["actual_working_hours"] = 0
         if "annofab_working_hours" not in df_sum_actual.columns:
             df_sum_actual["annofab_working_hours"] = 0
@@ -440,17 +429,15 @@
         `--shape_type total_by_user_job`に対応するDataFrameを生成する。
 
         Args:
             df_job_parent_job: job_id, parent_job_id, parent_job_name 列を持つDataFrame
 
         """
         # groupbyをjob_id, parent_job_idの2回に分けている理由：join/mergeするときの行数を減らすため
-        df_sum_actual = df_actual.groupby(["user_id", "job_id"])[
-            ["actual_working_hours", "annofab_working_hours"]
-        ].sum()
+        df_sum_actual = df_actual.groupby(["user_id", "job_id"])[["actual_working_hours", "annofab_working_hours"]].sum()
 
         # df_sum_actual が0件のときは、列がないので追加する
         if "actual_working_hours" not in df_sum_actual.columns:
             df_sum_actual["actual_working_hours"] = 0
         if "annofab_working_hours" not in df_sum_actual.columns:
             df_sum_actual["annofab_working_hours"] = 0
 
@@ -485,15 +472,15 @@
         if df_job_parent_job is not None:
             extension_columns = [
                 "parent_job_id",
                 "parent_job_name",
             ]
 
         columns = (
-            [
+            [  # noqa: RUF005
                 "user_id",
                 "username",
                 "job_id",
                 "job_name",
             ]
             + extension_columns
             + [
@@ -552,17 +539,15 @@
                     "monitored_working_hours",
                     "monitor_rate",
                     "monitor_diff",
                 ]
             ]
         )
 
-    def get_df_list_by_date_user_job(
-        self, df_actual: pandas.DataFrame, df_job_parent_job: Optional[pandas.DataFrame] = None
-    ) -> pandas.DataFrame:
+    def get_df_list_by_date_user_job(self, df_actual: pandas.DataFrame, df_job_parent_job: Optional[pandas.DataFrame] = None) -> pandas.DataFrame:
         """
         `--shape_type list_by_date_user_job`に対応するDataFrameを生成する。
 
         Args:
             df_job_parent_job: job_id, parent_job_id, parent_job_name 列が格納されたDataFrame。
                 指定されなければ、parent_job_id, parent_job_nameは格納しません。
 
@@ -581,15 +566,15 @@
         if df_job_parent_job is not None:
             extension_columns = [
                 "parent_job_id",
                 "parent_job_name",
             ]
 
         columns = (
-            [
+            [  # noqa: RUF005
                 "date",
                 "user_id",
                 "username",
                 "job_id",
                 "job_name",
             ]
             + extension_columns
@@ -658,42 +643,32 @@
         )
         if len(df) == 0:
             return pandas.DataFrame()
 
         df.rename(columns={"annofab_working_hours": "monitored_working_hours"}, inplace=True)
 
         if insert_sum_column:
-            df_sum_by_date = df.groupby(["date"])[
-                ["actual_working_hours", "monitored_working_hours", "assigned_working_hours"]
-            ].sum()
+            df_sum_by_date = df.groupby(["date"])[["actual_working_hours", "monitored_working_hours", "assigned_working_hours"]].sum()
             # 列名が"総合計"になるように、indexを変更する
             df_sum_by_date.index = [(date, SUM_COLUMN_NAME) for date in df_sum_by_date.index]
 
             df = pandas.concat([df, df_sum_by_date])
 
         # ヘッダが [user_id, value] になるように設定する
-        df2 = df.stack().unstack([1, 2])
+        df2 = df.stack().unstack([1, 2])  # noqa: PD010, PD013
 
         # DataFrameのindexの日付が連続になるようにする
-        not_exists_date_set = {
-            str(e.date()) for e in pandas.date_range(start=min(df2.index), end=max(df2.index))
-        } - set(df2.index)
+        not_exists_date_set = {str(e.date()) for e in pandas.date_range(start=min(df2.index), end=max(df2.index))} - set(df2.index)
 
-        df_not_exists_date = pandas.DataFrame(
-            [pandas.Series(name=date, dtype="float64") for date in not_exists_date_set]
-        )
+        df_not_exists_date = pandas.DataFrame([pandas.Series(name=date, dtype="float64") for date in not_exists_date_set])
         df2 = pandas.concat([df2, df_not_exists_date])
         df2.sort_index(inplace=True)
         # 作業時間がNaNの場合は0に置換する
         df2.replace(
-            {
-                col: {numpy.nan: 0}
-                for col in df2.columns
-                if col[1] in ["actual_working_hours", "monitored_working_hours", "assigned_working_hours"]
-            },
+            {col: {numpy.nan: 0} for col in df2.columns if col[1] in ["actual_working_hours", "monitored_working_hours", "assigned_working_hours"]},
             inplace=True,
         )
 
         # user_idの辞書順（大文字小文字区別しない）のユーザのDataFrameを生成する。
         df_user = (
             pandas.concat(
                 [
@@ -703,15 +678,15 @@
             )
             .drop_duplicates()
             .sort_index(key=lambda x: x.str.lower())
         )
 
         username_list = list(df_user["username"])
         if insert_sum_column:
-            username_list = [SUM_COLUMN_NAME] + username_list
+            username_list = [SUM_COLUMN_NAME] + username_list  # noqa: RUF005
 
         if insert_sum_row:
             # 先頭行に合計を追加する
             tmp_sum_row = df2.sum()
             tmp_sum_row.name = SUM_ROW_NAME
             df2 = pandas.concat([pandas.DataFrame([tmp_sum_row]), df2])
 
@@ -770,15 +745,15 @@
     elif input_file.suffix.lower() == ".csv":
         return pandas.read_csv(str(input_file))
 
     return pandas.DataFrame()
 
 
 class ReshapeWorkingHours:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         *,
         annowork_service: AnnoworkResource,
         workspace_id: str,
         parallelism: Optional[int] = None,
     ):
         self.annowork_service = annowork_service
@@ -793,15 +768,15 @@
             af_project_id = get_annofab_project_id_from_job(job)
             if af_project_id is None:
                 return False
             return af_project_id in annofab_project_id_set
 
         return [e["job_id"] for e in self.all_jobs if _match_job(e)]
 
-    def get_df_actual(
+    def get_df_actual(  # noqa: ANN201
         self,
         annofab_service: AnnofabResource,
         *,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         user_ids: Optional[Collection[str]] = None,
         parent_job_ids: Optional[Collection[str]] = None,
@@ -819,30 +794,26 @@
             annofab_service=annofab_service,
             parallelism=self.parallelism,
         )
 
         if parent_job_ids is not None:
             job_ids = list_actual_obj.get_job_id_list_from_parent_job_id_list(parent_job_ids)
 
-        df = list_actual_obj.get_df_working_hours(
-            start_date=start_date, end_date=end_date, job_ids=job_ids, user_ids=user_ids
-        )
+        df = list_actual_obj.get_df_working_hours(start_date=start_date, end_date=end_date, job_ids=job_ids, user_ids=user_ids)
         return df
 
-    def get_df_assigned(
+    def get_df_assigned(  # noqa: ANN201
         self,
         *,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         parent_job_ids: Optional[Collection[str]] = None,
         user_ids: Optional[Collection[str]] = None,
     ):
-        list_assigned_obj = ListAssignedHoursDaily(
-            annowork_service=self.annowork_service, workspace_id=self.workspace_id
-        )
+        list_assigned_obj = ListAssignedHoursDaily(annowork_service=self.annowork_service, workspace_id=self.workspace_id)
         result = list_assigned_obj.get_assigned_hours_daily_list(
             start_date=start_date,
             end_date=end_date,
             job_ids=parent_job_ids,
             user_ids=user_ids,
         )
         return pandas.DataFrame(result)
@@ -881,15 +852,15 @@
         df_job = pandas.DataFrame(self.all_jobs)
         df_job["is_parent"] = df_job["job_tree"].apply(lambda e: get_parent_job_id_from_job_tree(e) is None)
 
         df = df_job[df_job["is_parent"]][["job_id", "job_name"]]
         df.rename(columns={"job_name": "parent_job_name", "job_id": "parent_job_id"}, inplace=True)
         return df
 
-    def get_df_output(
+    def get_df_output(  # noqa: PLR0912
         self,
         df_actual: pandas.DataFrame,
         df_assigned: pandas.DataFrame,
         shape_type: ShapeType,
         show_parent_job: bool = False,
     ) -> pandas.DataFrame:
         """実績時間DataFrameとアサイン時間のDataFrameから、shape_typeに従ったDataFrameを生成します。
@@ -908,17 +879,15 @@
         # 見やすくするため、小数点以下2桁になるように四捨五入する
         reshape_obj = ReshapeDataFrame(round_decimals=2)
         if shape_type == ShapeType.DETAILS:
             df_output = reshape_obj.get_df_details(df_actual=df_actual, df_assigned=df_assigned)
 
         elif shape_type == ShapeType.TOTAL_BY_USER:
             df_user_company = self.get_df_user_company()
-            df_output = reshape_obj.get_df_total_by_user(
-                df_actual=df_actual, df_assigned=df_assigned, df_user_company=df_user_company
-            )
+            df_output = reshape_obj.get_df_total_by_user(df_actual=df_actual, df_assigned=df_assigned, df_user_company=df_user_company)
 
         elif shape_type == ShapeType.TOTAL_BY_JOB:
             if show_parent_job:
                 df_job_parent_job = self.get_df_job_parent_job()
                 df_parent_job = self.get_df_parent_job()
                 df_job_parent_job = df_job_parent_job.merge(df_parent_job, on="parent_job_id", how="left")
             else:
@@ -969,17 +938,15 @@
             if show_parent_job:
                 df_job_parent_job = self.get_df_job_parent_job()
                 df_parent_job = self.get_df_parent_job()
                 df_job_parent_job = df_job_parent_job.merge(df_parent_job, on="parent_job_id", how="left")
             else:
                 df_job_parent_job = None
 
-            df_output = reshape_obj.get_df_list_by_date_user_job(
-                df_actual=df_actual, df_job_parent_job=df_job_parent_job
-            )
+            df_output = reshape_obj.get_df_list_by_date_user_job(df_actual=df_actual, df_job_parent_job=df_job_parent_job)
 
         elif shape_type == ShapeType.LIST_BY_DATE_USER_PARENT_JOB:
             df_job_parent_job = self.get_df_job_parent_job()
             df_parent_job = self.get_df_parent_job()
             df_output = reshape_obj.get_df_list_by_date_user_parent_job(
                 df_actual=df_actual, df_job_parent_job=df_job_parent_job, df_parent_job=df_parent_job
             )
@@ -1008,35 +975,25 @@
 
         Returns:
             tuple[pandas.DataFrame, pandas.DataFrame]: 絞り込まれたdf_actual, df_assigned
         """
         child_job_ids: Optional[Collection] = None
 
         if parent_job_ids is not None:
-            child_job_ids = {
-                e["job_id"]
-                for e in self.all_jobs
-                if get_parent_job_id_from_job_tree(e["job_tree"]) in set(parent_job_ids)
-            }
-            df_actual = filter_df(
-                df_actual, job_ids=child_job_ids, user_ids=user_ids, start_date=start_date, end_date=end_date
-            )
+            child_job_ids = {e["job_id"] for e in self.all_jobs if get_parent_job_id_from_job_tree(e["job_tree"]) in set(parent_job_ids)}
+            df_actual = filter_df(df_actual, job_ids=child_job_ids, user_ids=user_ids, start_date=start_date, end_date=end_date)
         else:
-            df_actual = filter_df(
-                df_actual, job_ids=job_ids, user_ids=user_ids, start_date=start_date, end_date=end_date
-            )
+            df_actual = filter_df(df_actual, job_ids=job_ids, user_ids=user_ids, start_date=start_date, end_date=end_date)
 
         if job_ids is not None:
             # アサインは親ジョブに紐付けているため、job_idに対応するアサインはない。したがって、0件にする。
             df_assigned = pandas.DataFrame(columns=df_assigned.columns)
         else:
             # df_assignedのjob_idがparent_job_idになるので、job_ids にはparent_job_idsを渡している
-            df_assigned = filter_df(
-                df_assigned, job_ids=parent_job_ids, user_ids=user_ids, start_date=start_date, end_date=end_date
-            )
+            df_assigned = filter_df(df_assigned, job_ids=parent_job_ids, user_ids=user_ids, start_date=start_date, end_date=end_date)
         return (df_actual, df_assigned)
 
 
 def get_empty_df_actual() -> pandas.DataFrame:
     return pandas.DataFrame(
         columns=[
             "date",
@@ -1063,15 +1020,15 @@
             "user_id",
             "username",
             "assigned_working_hours",
         ]
     )
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     main_obj = ReshapeWorkingHours(
         annowork_service=build_annoworkapi(args),
         workspace_id=args.workspace_id,
         parallelism=args.parallelism,
     )
 
     parent_job_id_list = get_list_from_args(args.parent_job_id)
@@ -1080,15 +1037,16 @@
     user_id_list = get_list_from_args(args.user_id)
     start_date = args.start_date
     end_date = args.end_date
 
     if args.actual_file is None or args.assigned_file is None:
         if all(v is None for v in [job_id_list, parent_job_id_list, user_id_list, start_date, end_date]):
             logger.warning(
-                "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。" "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+                "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。"
+                "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
             )
 
     # "--job_id"と"--annofab_project_id"は排他的なので、job_id_listは上書きする
     if annofab_project_id_list is not None:
         job_id_list = main_obj.get_job_id_list_from_af_project_id(annofab_project_id_list)
 
     shape_type = ShapeType(args.shape_type)
@@ -1111,58 +1069,53 @@
             user_ids=user_id_list,
         )
         if len(df_actual) == 0:
             df_actual = get_empty_df_actual()
 
     if args.assigned_file is not None:
         df_assigned = get_dataframe_from_input_file(args.assigned_file)
+    elif (
+        shape_type
+        in {
+            ShapeType.TOTAL_BY_JOB,
+            ShapeType.LIST_BY_DATE_USER_JOB,
+            ShapeType.LIST_BY_DATE_USER_PARENT_JOB,
+        }
+        or job_id_list is not None
+    ):
+        # このshape_typeのときは、df_assignedが不要なので、空のDataFrameを生成する
+        # job_idが指定されたときも、アサインを取得できないので、空のDataFrameを生成する
+        df_assigned = get_empty_df_assigned()
     else:
-        if (
-            shape_type
-            in {
-                ShapeType.TOTAL_BY_JOB,
-                ShapeType.LIST_BY_DATE_USER_JOB,
-                ShapeType.LIST_BY_DATE_USER_PARENT_JOB,
-            }
-            or job_id_list is not None
-        ):
-            # このshape_typeのときは、df_assignedが不要なので、空のDataFrameを生成する
-            # job_idが指定されたときも、アサインを取得できないので、空のDataFrameを生成する
+        df_assigned = main_obj.get_df_assigned(start_date=start_date, end_date=end_date, parent_job_ids=parent_job_id_list, user_ids=user_id_list)
+        if len(df_assigned) == 0:
             df_assigned = get_empty_df_assigned()
-        else:
-            df_assigned = main_obj.get_df_assigned(
-                start_date=start_date, end_date=end_date, parent_job_ids=parent_job_id_list, user_ids=user_id_list
-            )
-            if len(df_assigned) == 0:
-                df_assigned = get_empty_df_assigned()
 
     df_actual, df_assigned = main_obj.filter_df(
         df_actual=df_actual,
         df_assigned=df_assigned,
         start_date=args.start_date,
         end_date=args.end_date,
         user_ids=user_id_list,
         parent_job_ids=parent_job_id_list,
         job_ids=job_id_list,
     )
 
-    df_output = main_obj.get_df_output(
-        df_actual=df_actual, df_assigned=df_assigned, shape_type=shape_type, show_parent_job=args.show_parent_job
-    )
+    df_output = main_obj.get_df_output(df_actual=df_actual, df_assigned=df_assigned, shape_type=shape_type, show_parent_job=args.show_parent_job)
 
     output_path: Optional[Path] = args.output
 
     if len(df_output) == 0:
         logger.warning(f"出力対象のデータは0件なので、'{output_path if output_path is not None else '標準出力'}'に出力しません。")
         return
 
     print_csv(df_output, output=args.output)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -1232,15 +1185,17 @@
             "* list_by_date_user_parent_job: 作業時間の一覧を日付、ユーザ、親ジョブ単位で出力します。 ``--assigned_file`` は不要です。 \n"
         ),
     )
 
     parser.add_argument(
         "--show_parent_job",
         action="store_true",
-        help="親のジョブ情報も出力します。``--shape_type`` に以下の値を渡したときに有効なオプションです。\n" "* total_by_job" "* list_by_date_user_job",
+        help="親のジョブ情報も出力します。``--shape_type`` に以下の値を渡したときに有効なオプションです。\n"
+        "* total_by_job"
+        "* list_by_date_user_job",
     )
 
     parser.add_argument("--parallelism", type=int, required=False, help="並列度。指定しない場合は、逐次的に処理します。")
 
     parser.add_argument("-o", "--output", type=Path, help="出力先")
     parser.add_argument("--annofab_mfa_code", type=str, help="Annofabにログインする際のMFAコード")
     parser.add_argument("--annofab_user_id", type=str, help="Annofabにログインする際のユーザID")
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/annofab/subcommand.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import annoworkcli.annofab.list_working_hours
 import annoworkcli.annofab.put_account_external_linkage_info
 import annoworkcli.annofab.put_job_from_annofab_project
 import annoworkcli.annofab.reshape_working_hours
 import annoworkcli.annofab.visualize_statistics
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     annoworkcli.annofab.list_job_with_annofab_project.add_parser(subparsers)
     annoworkcli.annofab.list_working_hours.add_parser(subparsers)
     annoworkcli.annofab.visualize_statistics.add_parser(subparsers)
     annoworkcli.annofab.reshape_working_hours.add_parser(subparsers)
@@ -23,12 +23,10 @@
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "annofab"
     subcommand_help = "Annofabにアクセスするサブコマンド"
     description = "Annofabにアクセスするサブコマンド\n" "Annofabの認証情報を事前に設定しておく必要があります。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=description, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=description, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/utils.py` & `annoworkcli-3.7.0/annoworkcli/annofab/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,18 +20,15 @@
     login_password = ""
     while login_password == "":
         login_password = getpass.getpass("Enter Annofab Password: ")
     return login_password
 
 
 def build_annofabapi_resource_and_login(
-    *,
-    annofab_login_user_id: Optional[str] = None,
-    annofab_login_password: Optional[str] = None,
-    mfa_code: Optional[str] = None
+    *, annofab_login_user_id: Optional[str] = None, annofab_login_password: Optional[str] = None, mfa_code: Optional[str] = None
 ) -> annofabapi.Resource:
     """
     annofabapi.Resourceインスタンスを生成したあと、ログインする。
 
     Args:
         args: コマンドライン引数の情報
```

### Comparing `annoworkcli-3.6.2/annoworkcli/annofab/visualize_statistics.py` & `annoworkcli-3.7.0/annoworkcli/annofab/visualize_statistics.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import datetime
 import logging
 import subprocess
 import tempfile
 from collections import defaultdict
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Dict, Optional, Tuple
+from typing import Dict, Optional, Tuple  # noqa: UP035
 
 import pandas
 from annoworkapi.resource import Resource as AnnoworkResource
 from dataclasses_json import DataClassJsonMixin
 
 import annoworkcli
 from annoworkcli.actual_working_time.list_actual_working_hours_daily import create_actual_working_hours_daily_list
@@ -18,15 +18,15 @@
 from annoworkcli.common.annofab import TIMEZONE_OFFSET_HOURS, get_annofab_project_id_from_job
 from annoworkcli.common.cli import build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv
 
 logger = logging.getLogger(__name__)
 
 
-ActualWorkingHoursDict = Dict[Tuple[datetime.date, str, str], float]
+ActualWorkingHoursDict = Dict[Tuple[datetime.date, str, str], float]  # noqa: UP006
 """実績作業時間の日ごとの情報を格納する辞書
 key: (date, workspace_member_id, job_id), value: 実績作業時間
 """
 
 
 @dataclass
 class AnnofabLabor(DataClassJsonMixin):
@@ -34,74 +34,72 @@
 
     date: str
     account_id: str
     project_id: str
     actual_worktime_hour: float
 
 
-JobIdAnnofabProjectIdDict = Dict[str, str]
+JobIdAnnofabProjectIdDict = Dict[str, str]  # noqa: UP006
 """key:job_id, value:annofab_project_idのdict
 """
 
 
 class ListLabor:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
         self.all_job_list = self.annowork_service.api.get_jobs(self.workspace_id)
 
         # Annofabが日本時間に固定されているので、それに合わせて timezone_offset_hours を指定する。
         self.list_actual_working_time_obj = ListActualWorkingTime(
             annowork_service=annowork_service,
             workspace_id=workspace_id,
             timezone_offset_hours=TIMEZONE_OFFSET_HOURS,
         )
 
-    def get_job_id_annofab_project_id_dict_from_annofab_project_id(
-        self, annofab_project_id_list: list[str]
-    ) -> JobIdAnnofabProjectIdDict:
+    def get_job_id_annofab_project_id_dict_from_annofab_project_id(self, annofab_project_id_list: list[str]) -> JobIdAnnofabProjectIdDict:
         # オーダを減らすため、事前にdictを作成する
         annofab_project_id_dict: dict[str, list[str]] = defaultdict(list)
         for job in self.all_job_list:
             af_project_id = get_annofab_project_id_from_job(job)
             if af_project_id is not None:
                 annofab_project_id_dict[af_project_id].append(job["job_id"])
 
         result = {}
         for annofab_project_id in annofab_project_id_list:
             job_id_list = annofab_project_id_dict.get(annofab_project_id)
             if job_id_list is None:
-                logger.warning(f"ジョブの外部連携情報に、AnnofabのプロジェクトID '{annofab_project_id}' を表すURLが設定されたジョブは見つかりませんでした。")
+                logger.warning(
+                    f"ジョブの外部連携情報に、AnnofabのプロジェクトID '{annofab_project_id}' を表すURLが設定されたジョブは見つかりませんでした。"
+                )
                 continue
 
             for job_id in job_id_list:
                 result[job_id] = annofab_project_id
 
         return result
 
     def get_job_id_annofab_project_id_dict_from_job_id(self, job_id_list: list[str]) -> JobIdAnnofabProjectIdDict:
         job_id_dict = {
-            job["job_id"]: get_annofab_project_id_from_job(job)
-            for job in self.all_job_list
-            if get_annofab_project_id_from_job(job) is not None
+            job["job_id"]: get_annofab_project_id_from_job(job) for job in self.all_job_list if get_annofab_project_id_from_job(job) is not None
         }
 
         result = {}
         for job_id in job_id_list:
             annofab_project_id = job_id_dict.get(job_id)
             if annofab_project_id is None:
                 logger.warning(f"{job_id=} のジョブの外部連携情報にAnnofabのプロジェクトを表すURLは設定されていませんでした。")
                 continue
 
             result[job_id] = annofab_project_id
 
         return result
 
-    def get_user_id_annofab_account_id_dict(self, user_id_set) -> dict[str, str]:
+    def get_user_id_annofab_account_id_dict(self, user_id_set) -> dict[str, str]:  # noqa: ANN001
         result = {}
         for user_id in user_id_set:
             annofab_account_id = self.annowork_service.wrapper.get_annofab_account_id_from_user_id(user_id)
             if annofab_account_id is None:
                 logger.warning(f"{user_id=} の外部連携情報にAnnofabのaccount_idが設定されていません。")
                 continue
             result[user_id] = annofab_account_id
@@ -120,36 +118,32 @@
             job_id_annofab_project_id_dict = self.get_job_id_annofab_project_id_dict_from_job_id(job_id_list)
 
             actual_working_time_list = self.list_actual_working_time_obj.get_actual_working_times(
                 job_ids=job_id_list, start_date=start_date, end_date=end_date, is_set_additional_info=True
             )
 
         elif annofab_project_id_list is not None:
-            job_id_annofab_project_id_dict = self.get_job_id_annofab_project_id_dict_from_annofab_project_id(
-                annofab_project_id_list
-            )
+            job_id_annofab_project_id_dict = self.get_job_id_annofab_project_id_dict_from_annofab_project_id(annofab_project_id_list)
             actual_working_time_list = self.list_actual_working_time_obj.get_actual_working_times(
                 job_ids=job_id_annofab_project_id_dict.keys(),
                 start_date=start_date,
                 end_date=end_date,
                 is_set_additional_info=True,
             )
 
         if len(actual_working_time_list) == 0:
             return []
 
         # annofabのデータは日本時間に固定されているので、日本時間を指定する
-        daily_list = create_actual_working_hours_daily_list(
-            actual_working_time_list, timezone_offset_hours=TIMEZONE_OFFSET_HOURS
-        )
+        daily_list = create_actual_working_hours_daily_list(actual_working_time_list, timezone_offset_hours=TIMEZONE_OFFSET_HOURS)
 
         user_id_set = {elm.user_id for elm in daily_list}
         user_id_annofab_account_id_dict = self.get_user_id_annofab_account_id_dict(user_id_set)
         if len(user_id_set) != len(user_id_annofab_account_id_dict):
-            raise RuntimeError(f"アカウント外部連携情報にAnnofabのaccount_idが設定されていないユーザがいます。")
+            raise RuntimeError("アカウント外部連携情報にAnnofabのaccount_idが設定されていないユーザがいます。")
 
         result = []
         for elm in daily_list:
             annofab_project_id = job_id_annofab_project_id_dict.get(elm.job_id)
             if annofab_project_id is None:
                 # annofabプロジェクトに紐付いていないジョブの場合に通る
                 continue
@@ -162,15 +156,15 @@
                     project_id=annofab_project_id,
                     actual_worktime_hour=elm.actual_working_hours,
                 )
             )
         return result
 
 
-def visualize_statistics(temp_dir: Path, args):
+def visualize_statistics(temp_dir: Path, args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     annofab_project_id_list = get_list_from_args(args.annofab_project_id)
     main_obj = ListLabor(annowork_service, args.workspace_id)
     annofab_labor_list = main_obj.get_annofab_labor_list(
         job_id_list=job_id_list,
         annofab_project_id_list=annofab_project_id_list,
@@ -190,21 +184,21 @@
         "statistics",
         "visualize",
         "--labor_csv",
         str(annofab_labor_csv),
     ]
 
     if annofab_project_id_list is not None:
-        command.extend(["--project_id"] + annofab_project_id_list)
+        command.extend(["--project_id"] + annofab_project_id_list)  # noqa: RUF005
     elif job_id_list is not None:
         job_id_annofab_project_id_dict = main_obj.get_job_id_annofab_project_id_dict_from_job_id(job_id_list)
         if len(job_id_annofab_project_id_dict) == 0:
             logger.error("Annofabプロジェクトに紐づくジョブが0件なので、終了します。")
             return
-        command.extend(["--project_id"] + list(job_id_annofab_project_id_dict.values()))
+        command.extend(["--project_id"] + list(job_id_annofab_project_id_dict.values()))  # noqa: RUF005
 
     if args.start_date is not None:
         command.extend(["--start_date", args.start_date])
 
     if args.end_date is not None:
         command.extend(["--end_date", args.end_date])
 
@@ -224,23 +218,23 @@
         command.extend(args.annofabcli_options)
 
     str_command = " ".join(command)
     logger.debug(f"run command: {str_command}")
     subprocess.run(command, check=True)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     if args.temp_dir is not None:
         visualize_statistics(args.temp_dir, args)
     else:
         with tempfile.TemporaryDirectory() as str_temp_dir:
             visualize_statistics(Path(str_temp_dir), args)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
```

### Comparing `annoworkcli-3.6.2/annoworkcli/common/annofab.py` & `annoworkcli-3.7.0/annoworkcli/common/annofab.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,15 +16,15 @@
     url = job["external_linkage_info"].get("url")
     if url is None:
         return None
 
     return get_annofab_project_id_from_url(url)
 
 
-def isoduration_to_hour(duration) -> float:
+def isoduration_to_hour(duration) -> float:  # noqa: ANN001
     """
     ISO 8601 duration を 時間に変換する
     Args:
         duration (str): ISO 8601 Durationの文字
 
     Returns:
         変換後の時間。
```

### Comparing `annoworkcli-3.6.2/annoworkcli/common/cli.py` & `annoworkcli-3.7.0/annoworkcli/common/cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 """
 import argparse
 import getpass
 import json
 import logging
 import os
 from enum import Enum
-from typing import Any, List, Optional, Tuple
+from typing import Any, List, Optional, Tuple  # noqa: UP035
 
 import annoworkapi
 from annoworkapi.api import DEFAULT_ENDPOINT_URL
 from annoworkapi.exceptions import CredentialsNotFoundError
 from more_itertools import first_true
 
 from annoworkcli.common.exeptions import CommandLineArgumentError
@@ -27,40 +27,40 @@
     JSON = "json"
 
 
 class PrettyHelpFormatter(argparse.RawTextHelpFormatter, argparse.ArgumentDefaultsHelpFormatter):
     def _format_action(self, action: argparse.Action) -> str:
         return super()._format_action(action) + "\n"
 
-    def _get_help_string(self, action):
+    def _get_help_string(self, action):  # noqa: ANN001, ANN202
         """引数説明用のメッセージを生成する。
         不要なデフォルト値（--debug や オプショナルな引数）を表示させないようにする.
         `argparse.ArgumentDefaultsHelpFormatter._get_help_string` をオーバライドしている。
 
         Args:
             action ([type]): [description]
 
         Returns:
             [type]: [description]
         """
         # ArgumentDefaultsHelpFormatter._get_help_string の中身を、そのまま持ってきた。
         # https://qiita.com/yuji38kwmt/items/c7c4d487e3188afd781e 参照
 
         # 必須な引数には、引数の説明の後ろに"(required)"を付ける
-        help = action.help  # pylint: disable=redefined-builtin
+        help = action.help  # pylint: disable=redefined-builtin  # noqa: A001
         if action.required:
-            help += " (required)"
+            help += " (required)"  # noqa: A001
 
         if "%(default)" not in action.help:
             if action.default is not argparse.SUPPRESS:
                 defaulting_nargs = [argparse.OPTIONAL, argparse.ZERO_OR_MORE]
                 if action.option_strings or action.nargs in defaulting_nargs:
                     # 以下の条件だけ、annoworkcli独自の設定
                     if action.default is not None and not action.const:
-                        help += " (default: %(default)s)"
+                        help += " (default: %(default)s)"  # noqa: A001
         return help
 
 
 def add_parser(
     subparsers: Optional[argparse._SubParsersAction],
     command_name: str,
     command_help: str,
@@ -87,15 +87,17 @@
 
     def create_parent_parser() -> argparse.ArgumentParser:
         """
         共通の引数セットを生成する。
         """
         parent_parser = argparse.ArgumentParser(add_help=False, allow_abbrev=False)
         group = parent_parser.add_argument_group(GLOBAL_OPTIONAL_ARGUMENTS_TITLE)
-        group.add_argument("--debug", action="store_true", help="HTTPリクエストの内容やレスポンスのステータスコードなど、デバッグ用のログが出力されます。")
+        group.add_argument(
+            "--debug", action="store_true", help="HTTPリクエストの内容やレスポンスのステータスコードなど、デバッグ用のログが出力されます。"
+        )
 
         group.add_argument(
             "--annowork_user_id",
             type=str,
             help="Annoworkにログインする際のユーザーIDを指定します。",
         )
         group.add_argument(
@@ -123,30 +125,28 @@
         description=description if description is not None else command_help,
         help=command_help,
         epilog=epilog,
         formatter_class=PrettyHelpFormatter,
     )
     parser.set_defaults(command_help=parser.print_help)
 
-    # 引数グループに"global optional group"がある場合は、"--help"オプションをデフォルトの"optional"グループから、"global optional arguments"グループに移動する
+    # 引数グループに"global optional group"がある場合は、"--help"オプションをデフォルトの"optional"グループから、"global optional arguments"グループに移動する  # noqa: E501
     # https://ja.stackoverflow.com/a/57313/19524
-    global_optional_argument_group = first_true(
-        parser._action_groups, pred=lambda e: e.title == GLOBAL_OPTIONAL_ARGUMENTS_TITLE
-    )
+    global_optional_argument_group = first_true(parser._action_groups, pred=lambda e: e.title == GLOBAL_OPTIONAL_ARGUMENTS_TITLE)
     if global_optional_argument_group is not None:
         # optional グループの 0番目が help なので取り出す
         help_action = parser._optionals._group_actions.pop(0)
         assert help_action.dest == "help"
         # global optional group の 先頭にhelpを追加
         global_optional_argument_group._group_actions.insert(0, help_action)
 
     return parser
 
 
-def get_list_from_args(str_list: Optional[List[str]] = None) -> Optional[List[str]]:
+def get_list_from_args(str_list: Optional[List[str]] = None) -> Optional[List[str]]:  # noqa: UP006
     """
     文字列のListのサイズが1で、プレフィックスが`file://`ならば、ファイルパスとしてファイルを読み込み、行をListとして返す。
     そうでなければ、引数の値をそのまま返す。
 
     Args:
         str_list: コマンドライン引数で指定されたリスト、またはfileスキームのURL
 
@@ -163,15 +163,15 @@
     path = get_file_scheme_path(str_value)
     if path is not None:
         return read_lines_except_blank_line(path)
     else:
         return str_list
 
 
-def get_json_from_args(target: Optional[str] = None) -> Any:
+def get_json_from_args(target: Optional[str] = None) -> Any:  # noqa: ANN401
     """
     JSON形式をPythonオブジェクトに変換する。
     プレフィックスが`file://`ならば、ファイルパスとしてファイルを読み込み、Pythonオブジェクトを返す。
     """
 
     if target is None:
         return None
@@ -199,15 +199,15 @@
         if choice == "y":
             return True
 
         elif choice == "N":
             return False
 
 
-def prompt_yesnoall(msg: str) -> Tuple[bool, bool]:
+def prompt_yesnoall(msg: str) -> Tuple[bool, bool]:  # noqa: UP006
     """
     標準入力で yes, no, all(すべてyes)を選択できるようにする。
     Args:
         msg: 確認メッセージ
 
     Returns:
         Tuple[yesno, is_all]. yesno:Trueならyes. is_all: Trueならall.
@@ -276,24 +276,20 @@
     endpoint_url = _get_endpoint_url_from_args_or_envvar(args)
 
     # エンドポイントURLがデフォルトでない場合は、気付けるようにするためログに出力する
     if endpoint_url != annoworkapi.api.DEFAULT_ENDPOINT_URL:
         logger.info(f"endpoint_url='{endpoint_url}'")
 
     if args.annowork_user_id is not None and args.annowork_password is not None:
-        return annoworkapi.build(
-            login_user_id=args.annowork_user_id, login_password=args.annowork_password, endpoint_url=endpoint_url
-        )
+        return annoworkapi.build(login_user_id=args.annowork_user_id, login_password=args.annowork_password, endpoint_url=endpoint_url)
 
     elif args.annowork_user_id is not None and args.annowork_password is None:
         # コマンドライン引数でユーザーIDのみ指定された場合は、パスワードを標準入力から取得する
         login_password = _get_annowork_password_from_stdin()
-        return annoworkapi.build(
-            login_user_id=args.annowork_user_id, login_password=login_password, endpoint_url=endpoint_url
-        )
+        return annoworkapi.build(login_user_id=args.annowork_user_id, login_password=login_password, endpoint_url=endpoint_url)
 
     elif args.annowork_user_id is None and args.annowork_password is not None:
         # コマンドライン引数でパスワードのみ指定された場合は、エラーにする
         raise CommandLineArgumentError("`--annowork_password`を指定する際は、`--annowork_user_id`も指定してください。")
 
     # コマンドライン引数でユーザーID、パスワードが指定されていない場合
     try:
```

### Comparing `annoworkcli-3.6.2/annoworkcli/common/utils.py` & `annoworkcli-3.7.0/annoworkcli/common/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 import copy
 import datetime
 import json
 import logging.config
 import pkgutil
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, TypeVar
+from typing import Any, Dict, List, Optional, TypeVar  # noqa: UP035
 
 import isodate
 import pandas
 import yaml
 
 DEFAULT_CSV_FORMAT = {"encoding": "utf_8_sig", "index": False}
 DATETIME_FORMAT = "%Y-%m-%dT%H:%M:%S.%fZ"
 
 logger = logging.getLogger(__name__)
 
 T = TypeVar("T")  # Can be anything
 
 
-def read_lines(filepath: str) -> List[str]:
+def read_lines(filepath: str) -> List[str]:  # noqa: UP006
     """ファイルを行単位で読み込む。改行コードを除く"""
 
     # BOM付きUTF-8のファイルも読み込めるようにする
     # annoworkが出力するCSVはデフォルトでBOM付きUTF-8。これを加工してannoworkcliに読み込ませる場合もあるので、BOM付きUTF-8に対応させた
     with open(filepath, encoding="utf-8-sig") as f:
         lines = f.readlines()
     return [e.rstrip("\r\n") for e in lines]
 
 
-def read_lines_except_blank_line(filepath: str) -> List[str]:
+def read_lines_except_blank_line(filepath: str) -> List[str]:  # noqa: UP006
     """ファイルを行単位で読み込む。ただし、改行コード、空行を除く"""
     lines = read_lines(filepath)
     return [line for line in lines if line != ""]
 
 
 def output_string(target: str, output: Optional[Path] = None) -> None:
     """
@@ -48,15 +48,15 @@
     else:
         output.parent.mkdir(parents=True, exist_ok=True)
         with output.open(mode="w", encoding="utf_8") as f:
             f.write(target)
             logger.info(f"{output} に出力しました。")
 
 
-def print_json(target: Any, is_pretty: bool = False, output: Optional[Path] = None) -> None:
+def print_json(target: Any, is_pretty: bool = False, output: Optional[Path] = None) -> None:  # noqa: ANN401
     """
     JSONを出力する。
 
     Args:
         target: 出力対象のJSON
         is_pretty: 人が見やすいJSONを出力するか
         output: 出力先。Noneなら標準出力に出力する。
@@ -64,18 +64,18 @@
     """
     if is_pretty:
         output_string(json.dumps(target, indent=2, ensure_ascii=False), output)
     else:
         output_string(json.dumps(target, ensure_ascii=False), output)
 
 
-def print_csv(
+def print_csv(  # noqa: ANN201
     df: pandas.DataFrame,
     output: Optional[Path] = None,
-    to_csv_kwargs: Optional[Dict[str, Any]] = None,
+    to_csv_kwargs: Optional[Dict[str, Any]] = None,  # noqa: UP006
 ):
     if output is not None:
         output.parent.mkdir(parents=True, exist_ok=True)
 
     path_or_buf = sys.stdout if output is None else str(output)
 
     kwargs = copy.deepcopy(DEFAULT_CSV_FORMAT)
@@ -104,15 +104,15 @@
     """
     if is_file_scheme(str_value):
         return str_value[len("file://") :]
     else:
         return None
 
 
-def isoduration_to_hour(duration) -> float:
+def isoduration_to_hour(duration) -> float:  # noqa: ANN001
     """
     ISO 8601 duration を 時間に変換する
     Args:
         duration (str): ISO 8601 Durationの文字
 
     Returns:
         変換後の時間。
@@ -121,15 +121,15 @@
     return isodate.parse_duration(duration).total_seconds() / 3600
 
 
 def to_iso8601_string(dt: datetime.datetime) -> str:
     return dt.astimezone(datetime.timezone.utc).strftime(DATETIME_FORMAT)
 
 
-def set_default_logger(is_debug_mode: bool = False):
+def set_default_logger(is_debug_mode: bool = False):  # noqa: ANN201
     """
     デフォルトのロガーを設定する。パッケージ内のlogging.yamlを読み込む。
     """
     # 事前にログ出力先のディレクトリを作成する。
     Path(".log").mkdir(exist_ok=True, parents=True)
     data = pkgutil.get_data("annoworkcli", "data/logging.yaml")
     if data is None:
```

### Comparing `annoworkcli-3.6.2/annoworkcli/common/workspace_tag.py` & `annoworkcli-3.7.0/annoworkcli/common/workspace_tag.py`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.6.2/annoworkcli/data/logging.yaml` & `annoworkcli-3.7.0/annoworkcli/data/logging.yaml`

 * *Files identical despite different names*

### Comparing `annoworkcli-3.6.2/annoworkcli/expected_working_time/delete_expected_working_time.py` & `annoworkcli-3.7.0/annoworkcli/expected_working_time/delete_expected_working_time.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,30 +8,28 @@
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, prompt_yesno
 
 logger = logging.getLogger(__name__)
 
 
 class DeleteExpectedWorkingTime:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-    def delete_expected_working_times(self, expected_working_times: list[dict[str, Any]]):
+    def delete_expected_working_times(self, expected_working_times: list[dict[str, Any]]):  # noqa: ANN201
         for expected in expected_working_times:
             self.annowork_service.api.delete_expected_working_time_by_workspace_member(
                 self.workspace_id,
                 workspace_member_id=expected["workspace_member_id"],
                 date=expected["date"],
             )
 
     def get_expected_working_times(self, *, user_id: str, start_date: str, end_date: str) -> list[dict[str, Any]]:
-        workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+        workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
         member = more_itertools.first_true(workspace_members, pred=lambda e: e["user_id"] == user_id)
         if member is None:
             logger.warning(f"{user_id=} のユーザはワークスペースメンバに存在しませんでした。")
             return []
 
         query_params = {
             "term_start": start_date,
@@ -39,40 +37,38 @@
         }
         workspace_member_id = member["workspace_member_id"]
         logger.debug(f"予定稼働情報を取得します。{workspace_member_id=}, {query_params=}")
         return self.annowork_service.api.get_expected_working_times_by_workspace_member(
             self.workspace_id, workspace_member_id=workspace_member_id, query_params=query_params
         )
 
-    def main(self, *, user_id: str, start_date: str, end_date: str):
-        expected_working_times = self.get_expected_working_times(
-            user_id=user_id, start_date=start_date, end_date=end_date
-        )
+    def main(self, *, user_id: str, start_date: str, end_date: str):  # noqa: ANN201
+        expected_working_times = self.get_expected_working_times(user_id=user_id, start_date=start_date, end_date=end_date)
         if len(expected_working_times) == 0:
-            logger.info(f"削除する予定稼働時間情報はありませんでした。")
+            logger.info("削除する予定稼働時間情報はありませんでした。")
             return
 
         yesno = prompt_yesno(
             f"user_id={user_id}, start_date={start_date}, end_date={end_date} の"
             f"予定稼働時間情報 {len(expected_working_times)} 件を削除します。よろしいですか？"
         )
         if yesno:
             self.delete_expected_working_times(expected_working_times)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     DeleteExpectedWorkingTime(annowork_service=annowork_service, workspace_id=args.workspace_id).main(
         user_id=args.user_id,
         start_date=args.start_date,
         end_date=args.end_date,
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -84,12 +80,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "delete"
     subcommand_help = "予定稼働時間を削除します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/expected_working_time/list_expected_working_time.py` & `annoworkcli-3.7.0/annoworkcli/expected_working_time/list_expected_working_time.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,20 +11,18 @@
 from annoworkcli.common.cli import COMMAND_LINE_ERROR_STATUS_CODE, OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListExpectedWorkingTime:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
-        self.workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+        self.workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
 
     def get_expected_working_times_by_user_id(
         self, user_id_list: list[str], *, start_date: Optional[str] = None, end_date: Optional[str] = None
     ) -> list[dict[str, Any]]:
         workspace_member_dict = {e["user_id"]: e["workspace_member_id"] for e in self.workspace_members}
 
         query_params = {}
@@ -58,15 +56,15 @@
             query_params["term_start"] = start_date
         if end_date is not None:
             query_params["term_end"] = end_date
 
         logger.debug(f"予定稼働時間情報を取得します。{query_params=}")
         return self.annowork_service.api.get_expected_working_times(self.workspace_id, query_params=query_params)
 
-    def set_member_info_to_working_times(self, working_times: list[dict[str, Any]]):
+    def set_member_info_to_working_times(self, working_times: list[dict[str, Any]]):  # noqa: ANN201
         workspace_member_dict = {e["workspace_member_id"]: e for e in self.workspace_members}
         for elm in working_times:
             workspace_member_id = elm["workspace_member_id"]
             member = workspace_member_dict.get(workspace_member_id)
             if member is None:
                 logger.warning(f"{workspace_member_id=} であるワークスペースメンバは存在しません。 :: date={elm['date']}")
                 continue
@@ -74,34 +72,32 @@
             elm.update(
                 {
                     "user_id": member["user_id"],
                     "username": member["username"],
                 }
             )
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         *,
         output: Path,
         output_format: OutputFormat,
         user_id_list: Optional[list[str]] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
     ):
         if user_id_list is not None:
-            result = self.get_expected_working_times_by_user_id(
-                user_id_list=user_id_list, start_date=start_date, end_date=end_date
-            )
+            result = self.get_expected_working_times_by_user_id(user_id_list=user_id_list, start_date=start_date, end_date=end_date)
         else:
             result = self.get_expected_working_times(start_date=start_date, end_date=end_date)
 
         self.set_member_info_to_working_times(result)
 
         if len(result) == 0:
-            logger.warning(f"予定稼働時間情報0件なので、出力しません。")
+            logger.warning("予定稼働時間情報0件なので、出力しません。")
             return
 
         logger.info(f"{len(result)} 件の予定稼働時間情報を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(result, is_pretty=True, output=output)
         else:
@@ -116,15 +112,15 @@
             ]
             remaining_columns = list(set(df.columns) - set(required_columns))
             columns = required_columns + remaining_columns
 
             print_csv(df[columns], output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     command = " ".join(sys.argv[0:3])
     if all(v is None for v in [user_id_list, start_date, end_date]):
@@ -136,15 +132,15 @@
         start_date=args.start_date,
         end_date=args.end_date,
         output=args.output,
         output_format=OutputFormat(args.format),
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -167,12 +163,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list"
     subcommand_help = "予定稼働時間の一覧を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py` & `annoworkcli-3.7.0/annoworkcli/expected_working_time/list_expected_working_time_groupby_tag.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import argparse
 import logging
 import sys
 from collections import defaultdict
+from collections.abc import Collection
 from pathlib import Path
-from typing import Any, Collection, Optional
+from typing import Any, Optional
 
 import pandas
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import COMMAND_LINE_ERROR_STATUS_CODE, OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 from annoworkcli.expected_working_time.list_expected_working_time import ListExpectedWorkingTime
 
 logger = logging.getLogger(__name__)
 
 
 class ListExpectedWorkingTimeGroupbyTag:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
     def get_expected_working_times_groupby_tag(
         self,
         expected_working_times: list[dict[str, Any]],
         target_workspace_tag_ids: Optional[Collection[str]] = None,
@@ -56,17 +57,15 @@
                 )
 
         dict_hours: dict[tuple[str, str], float] = defaultdict(float)
 
         # ワークスペースタグごと日毎の時間を集計する
         for workspace_tag in workspace_tags:
             workspace_tag_name = workspace_tag["workspace_tag_name"]
-            members = self.annowork_service.api.get_workspace_tag_members(
-                self.workspace_id, workspace_tag["workspace_tag_id"]
-            )
+            members = self.annowork_service.api.get_workspace_tag_members(self.workspace_id, workspace_tag["workspace_tag_id"])
             member_ids = {e["workspace_member_id"] for e in members}
             for elm in expected_working_times:
                 if elm["workspace_member_id"] in member_ids:
                     dict_hours[elm["date"], workspace_tag_name] += elm["expected_working_hours"]
 
         # 全体の時間を日毎に集計する
         for elm in expected_working_times:
@@ -81,15 +80,15 @@
         for date, value in dict_date.items():
             elm = {"date": date, "expected_working_hours": value}
             results.append(elm)
 
         results.sort(key=lambda e: (e["date"]))
         return results
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         *,
         output: Path,
         output_format: OutputFormat,
         user_id_list: Optional[list[str]] = None,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
@@ -101,15 +100,15 @@
             expected_working_times = list_obj.get_expected_working_times_by_user_id(
                 user_id_list=user_id_list, start_date=start_date, end_date=end_date
             )
         else:
             expected_working_times = list_obj.get_expected_working_times(start_date=start_date, end_date=end_date)
 
         if len(expected_working_times) == 0:
-            logger.warning(f"予定稼働時間情報0件なので、出力しません。")
+            logger.warning("予定稼働時間情報0件なので、出力しません。")
             return
 
         results = self.get_expected_working_times_groupby_tag(
             expected_working_times,
             target_workspace_tag_ids=target_workspace_tag_ids,
             target_workspace_tag_names=target_workspace_tag_names,
         )
@@ -127,15 +126,15 @@
             ]
             remaining_columns = list(set(df.columns) - set(required_columns))
             columns = required_columns + sorted(remaining_columns)
 
             print_csv(df[columns], output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     command = " ".join(sys.argv[0:3])
     if all(v is None for v in [user_id_list, start_date, end_date]):
@@ -152,15 +151,15 @@
         output=args.output,
         target_workspace_tag_ids=workspace_tag_id_list,
         target_workspace_tag_names=workspace_tag_name_list,
         output_format=OutputFormat(args.format),
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -199,12 +198,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_groupby_tag"
     subcommand_help = "ワークスペースタグで集計した予定稼働時間の一覧を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/expected_working_time/list_expected_working_time_weekly.py` & `annoworkcli-3.7.0/annoworkcli/expected_working_time/list_expected_working_time_weekly.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 from annoworkcli.common.cli import COMMAND_LINE_ERROR_STATUS_CODE, OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 from annoworkcli.expected_working_time.list_expected_working_time import ListExpectedWorkingTime
 
 logger = logging.getLogger(__name__)
 
 
-def get_weekly_expected_working_hours_df(
-    expected_working_times: list[dict[str, Any]], workspace_members: list[dict[str, Any]]
-) -> pandas.DataFrame:
+def get_weekly_expected_working_hours_df(expected_working_times: list[dict[str, Any]], workspace_members: list[dict[str, Any]]) -> pandas.DataFrame:
     """週単位の予定稼働時間が格納されたDataFrameを生成します。
 
     Args:
         expected_working_times: 予定稼働時間情報。date, workspace_member_id, expected_working_hours を参照します。
         workspace_members: ワークスペースメンバ情報。workspace_member_id, user_id, username を参照します。
 
     Returns:
@@ -30,19 +28,17 @@
     df = pandas.DataFrame(expected_working_times)
     # 1週間ごとに集計する（日曜日始まり, 日曜日がindexになっている）
     df["date"] = pandas.to_datetime(df["date"])
 
     df_weekly = (
         # `include_groups=False`を指定する理由：pandas2.2.0で以下の警告が出ないようにするため
         # DeprecationWarning: DataFrameGroupBy.resample operated on the grouping columns.
-        # This behavior is deprecated, and in a future version of pandas the grouping columns will be excluded from the operation.  # noqa: E501
+        # This behavior is deprecated, and in a future version of pandas the grouping columns will be excluded from the operation.
         # Either pass `include_groups=False` to exclude the groupings or explicitly select the grouping columns after groupby to silence this warning.  # noqa: E501
-        df.groupby("workspace_member_id")
-        .resample("W", on="date", label="left", closed="left", include_groups=False)
-        .sum(numeric_only=True)
+        df.groupby("workspace_member_id").resample("W", on="date", label="left", closed="left", include_groups=False).sum(numeric_only=True)
     )
     df_weekly.reset_index(inplace=True)
 
     # 1週間の始まり（日曜日）と終わり（土曜日）の日付列を設定
     df_weekly.rename(columns={"date": "start_date"}, inplace=True)
     df_weekly["end_date"] = df_weekly["start_date"] + pandas.Timedelta(days=6)
     # pandas.Timestamp型をstr型に変換する
@@ -56,36 +52,34 @@
 
     df = df_weekly.merge(df_workspace_member, on="workspace_member_id", how="left")
     df.sort_values(["user_id", "start_date"], inplace=True)
 
     return df[["workspace_member_id", "user_id", "username", "start_date", "end_date", "expected_working_hours"]]
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     command = " ".join(sys.argv[0:3])
     if all(v is None for v in [user_id_list, start_date, end_date]):
         print(f"{command}: error: '--start_date'や'--user_id'などの絞り込み条件を1つ以上指定してください。", file=sys.stderr)
         sys.exit(COMMAND_LINE_ERROR_STATUS_CODE)
 
     main_obj = ListExpectedWorkingTime(annowork_service=annowork_service, workspace_id=args.workspace_id)
 
     if user_id_list is not None:
-        expected_working_times = main_obj.get_expected_working_times_by_user_id(
-            user_id_list=user_id_list, start_date=start_date, end_date=end_date
-        )
+        expected_working_times = main_obj.get_expected_working_times_by_user_id(user_id_list=user_id_list, start_date=start_date, end_date=end_date)
     else:
         expected_working_times = main_obj.get_expected_working_times(start_date=start_date, end_date=end_date)
 
     if len(expected_working_times) == 0:
-        logger.warning(f"予定稼働時間情報0件なので、出力しません。")
+        logger.warning("予定稼働時間情報0件なので、出力しません。")
         return
 
     df = get_weekly_expected_working_hours_df(expected_working_times, main_obj.workspace_members)
 
     logger.info(f"{len(df)} 件の週単位の予定稼働時間情報を出力します。")
 
     if OutputFormat(args.format) == OutputFormat.CSV:
@@ -93,15 +87,15 @@
 
     elif OutputFormat(args.format) == OutputFormat.JSON:
         print_json(df.to_dict("records"), is_pretty=True, output=args.output)
     else:
         logger.error("`--format`が対象外でした。")
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -124,12 +118,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_weekly"
     subcommand_help = "予定稼働時間の一覧を週ごと（日曜日始まり）に出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/expected_working_time/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/expected_working_time/subcommand.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,26 +4,24 @@
 import annoworkcli
 import annoworkcli.expected_working_time.delete_expected_working_time
 import annoworkcli.expected_working_time.list_expected_working_time
 import annoworkcli.expected_working_time.list_expected_working_time_groupby_tag
 import annoworkcli.expected_working_time.list_expected_working_time_weekly
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     annoworkcli.expected_working_time.delete_expected_working_time.add_parser(subparsers)
     annoworkcli.expected_working_time.list_expected_working_time.add_parser(subparsers)
     annoworkcli.expected_working_time.list_expected_working_time_groupby_tag.add_parser(subparsers)
     annoworkcli.expected_working_time.list_expected_working_time_weekly.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "expected_working_time"
     subcommand_help = "予定稼働時間関係のサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/job/change_job_properties.py` & `annoworkcli-3.7.0/annoworkcli/job/change_job_properties.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,29 +7,27 @@
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, get_list_from_args, prompt_yesnoall
 
 logger = logging.getLogger(__name__)
 
 
 class ChangeJobProperties:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str, *, all_yes: bool):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str, *, all_yes: bool):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
         self.all_yes = all_yes
 
     def change_job_status(self, job_id: str, status: str) -> bool:
         job = self.annowork_service.wrapper.get_job_or_none(self.workspace_id, job_id)
         if job is None:
             logger.warning(f"{job_id=} のジョブは存在しませんでした。")
             return False
 
         if not self.all_yes:
-            is_yes, all_yes = prompt_yesnoall(
-                f"job_id={job_id}, job_name={job['job_name']}" f" のジョブのステータスを '{status}' に変更しますか？"
-            )
+            is_yes, all_yes = prompt_yesnoall(f"job_id={job_id}, job_name={job['job_name']}" f" のジョブのステータスを '{status}' に変更しますか？")
             if not is_yes:
                 return False
             if all_yes:
                 self.all_yes = all_yes
 
         request_body = {"job_name": job["job_name"], "status": status, "last_updated_datetime": job["updated_datetime"]}
         if job["note"] is not None:
@@ -39,39 +37,39 @@
         if job["external_linkage_info"] is not None:
             request_body["external_linkage_info"] = job["external_linkage_info"]
 
         new_job = self.annowork_service.api.put_job(self.workspace_id, job_id, request_body=request_body)
         logger.debug(f"ジョブのステータスを変更しました。 :: {new_job}")
         return True
 
-    def main(self, *, job_id_list: list[str], status: str):
+    def main(self, *, job_id_list: list[str], status: str):  # noqa: ANN201
         logger.info(f"{len(job_id_list)} 件のジョブのステータスを変更します。")
         success_count = 0
         for job_id in job_id_list:
             try:
                 result = self.change_job_status(job_id, status=status)
                 if result:
                     success_count += 1
             except Exception as e:
                 logger.warning(f"{job_id=} のジョブのステータスの変更に失敗しました。{e}")
 
         logger.info(f"{success_count} / {len(job_id_list)} 件のジョブのステータスを変更しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     assert job_id_list is not None
 
     ChangeJobProperties(annowork_service=annowork_service, workspace_id=args.workspace_id, all_yes=args.yes).main(
         job_id_list=job_id_list, status=args.status
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -98,12 +96,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "change"
     subcommand_help = "ジョブの情報（ステータスなど）を変更します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/job/delete_job.py` & `annoworkcli-3.7.0/annoworkcli/job/delete_job.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, prompt_yesnoall
 
 logger = logging.getLogger(__name__)
 
 
 class DeleteJob:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str, *, all_yes: bool):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str, *, all_yes: bool):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
         self.all_yes = all_yes
 
     def delete_job(self, job_id: str) -> bool:
         job = self.annowork_service.wrapper.get_job_or_none(self.workspace_id, job_id)
         if job is None:
@@ -33,15 +33,15 @@
             if all_yes:
                 self.all_yes = all_yes
 
         self.annowork_service.api.delete_job(self.workspace_id, job_id)
         logger.debug(f"ジョブを削除しました。 :: {job}")
         return True
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         job_id_list: list[str],
     ):
         logger.info(f"{len(job_id_list)} 件のジョブを削除します。")
         success_count = 0
         for job_id in job_id_list:
             try:
@@ -49,24 +49,24 @@
                 if result:
                     success_count += 1
             except Exception as e:
                 logger.warning(f"{job_id=} のジョブの削除に失敗しました。{e}", e)
         logger.info(f"{success_count} / {len(job_id_list)} 件のジョブを削除しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = [args.job_id]
 
     DeleteJob(annowork_service=annowork_service, workspace_id=args.workspace_id, all_yes=args.yes).main(
         job_id_list,
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -85,12 +85,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "delete"
     subcommand_help = "ジョブを削除します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/job/list_job.py` & `annoworkcli-3.7.0/annoworkcli/job/list_job.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,17 +10,15 @@
 import annoworkcli
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
-def filter_job_list_with_external_linkage_info_url(
-    job_list: list[dict[str, Any]], external_linkage_info_url_list: list[str]
-) -> list[dict[str, Any]]:
+def filter_job_list_with_external_linkage_info_url(job_list: list[dict[str, Any]], external_linkage_info_url_list: list[str]) -> list[dict[str, Any]]:
     result = []
     for job in job_list:
         url = job["external_linkage_info"].get("url")
         if url is None:
             continue
         url = url.strip()
         for target_url in external_linkage_info_url_list:
@@ -28,15 +26,15 @@
             if url.startswith(target_url):
                 result.append(job)
                 break
     return result
 
 
 class ListJob:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         annowork_service: AnnoworkResource,
         workspace_id: str,
     ):
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
@@ -50,17 +48,15 @@
     ) -> list[dict[str, Any]]:
         all_job_list = self.annowork_service.api.get_jobs(self.workspace_id)
         job_list = all_job_list
         if job_id_list is not None:
             job_list = [job for job in job_list if job["job_id"] in set(job_id_list)]
 
         if parent_job_id_list is not None:
-            job_list = [
-                job for job in job_list if get_parent_job_id_from_job_tree(job["job_tree"]) in set(parent_job_id_list)
-            ]
+            job_list = [job for job in job_list if get_parent_job_id_from_job_tree(job["job_tree"]) in set(parent_job_id_list)]
 
         if external_linkage_info_url_list is not None:
             job_list = filter_job_list_with_external_linkage_info_url(job_list, external_linkage_info_url_list)
 
         # 親のジョブ情報を追加する
         if is_add_parent_job_info:
             all_job_dict = {job["job_id"]: job for job in all_job_list}
@@ -72,15 +68,15 @@
                     job["parent_job_name"] = parent_job["job_name"]
                 else:
                     job["parent_job_id"] = None
                     job["parent_job_name"] = None
 
         return job_list
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         output: Path,
         output_format: OutputFormat,
         *,
         job_id_list: Optional[list[str]],
         parent_job_id_list: Optional[list[str]],
         external_linkage_info_url_list: Optional[list[str]],
@@ -89,27 +85,27 @@
         job_list = self.get_job_list(
             job_id_list=job_id_list,
             parent_job_id_list=parent_job_id_list,
             external_linkage_info_url_list=external_linkage_info_url_list,
             is_add_parent_job_info=is_add_parent_job_info,
         )
         if len(job_list) == 0:
-            logger.warning(f"ジョブ情報は0件なので、出力しません。")
+            logger.warning("ジョブ情報は0件なので、出力しません。")
             return
 
         logger.debug(f"{len(job_list)} 件のジョブ一覧を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(job_list, is_pretty=True, output=output)
         else:
             df = pandas.json_normalize(job_list)
             print_csv(df, output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
 
     job_id_list = get_list_from_args(args.job_id)
     parent_job_id_list = get_list_from_args(args.parent_job_id)
     external_linkage_info_url_list = get_list_from_args(args.external_linkage_info_url)
 
     ListJob(annowork_service=annowork_service, workspace_id=args.workspace_id).main(
@@ -118,15 +114,15 @@
         job_id_list=job_id_list,
         parent_job_id_list=parent_job_id_list,
         external_linkage_info_url_list=external_linkage_info_url_list,
         is_add_parent_job_info=args.show_parent_job,
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
```

### Comparing `annoworkcli-3.6.2/annoworkcli/job/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/job/subcommand.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,25 +3,23 @@
 
 import annoworkcli
 import annoworkcli.job.change_job_properties
 import annoworkcli.job.delete_job
 import annoworkcli.job.list_job
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     annoworkcli.job.change_job_properties.add_parser(subparsers)
     annoworkcli.job.delete_job.add_parser(subparsers)
     annoworkcli.job.list_job.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "job"
     subcommand_help = "ジョブ関係のサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/my/get_my_account.py` & `annoworkcli-3.7.0/annoworkcli/my/get_my_account.py`

 * *Files 17% similar despite different names*

```diff
@@ -9,42 +9,40 @@
 from annoworkcli.common.cli import build_annoworkapi
 from annoworkcli.common.utils import print_json
 
 logger = logging.getLogger(__name__)
 
 
 class GetMyAccount:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         annowork_service: AnnoworkResource,
     ):
         self.annowork_service = annowork_service
 
-    def main(self, output: Optional[Path]):
+    def main(self, output: Optional[Path]):  # noqa: ANN201
         my_account = self.annowork_service.api.get_my_account()
         print_json(my_account, output=output, is_pretty=True)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
 
     GetMyAccount(
         annowork_service=annowork_service,
     ).main(output=args.output)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-o", "--output", type=Path, required=False, help="出力先")
 
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "get"
     subcommand_help = "ログイン中のアカウント情報を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
 
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/my/list_my_workspace_member.py` & `annoworkcli-3.7.0/annoworkcli/my/list_my_workspace_member.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,45 +10,43 @@
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListWorkspaceMember:
-    def __init__(self, annowork_service: AnnoworkResource):
+    def __init__(self, annowork_service: AnnoworkResource):  # noqa: ANN204
         self.annowork_service = annowork_service
 
-    def main(self, output: Optional[Path], output_format: OutputFormat, workspace_id: Optional[str] = None):
+    def main(self, output: Optional[Path], output_format: OutputFormat, workspace_id: Optional[str] = None):  # noqa: ANN201
         query_params = {}
         if workspace_id is not None:
             query_params[workspace_id] = workspace_id
 
         my_workspace_members = self.annowork_service.api.get_my_workspace_members(query_params=query_params)
 
         if len(my_workspace_members) == 0:
-            logger.warning(f"ワークスペースメンバ情報は0件なので、出力しません。")
+            logger.warning("ワークスペースメンバ情報は0件なので、出力しません。")
             return
 
         logger.debug(f"{len(my_workspace_members)} 件のワークスペースメンバ一覧を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(my_workspace_members, is_pretty=True, output=output)
         else:
             df = pandas.json_normalize(my_workspace_members)
             print_csv(df, output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
-    ListWorkspaceMember(annowork_service=annowork_service).main(
-        output=args.output, output_format=OutputFormat(args.format)
-    )
+    ListWorkspaceMember(annowork_service=annowork_service).main(output=args.output, output_format=OutputFormat(args.format))
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument("-o", "--output", type=Path, help="出力先")
     parser.add_argument(
         "-f",
         "--format",
         type=str,
         choices=[e.value for e in OutputFormat],
         help="出力先のフォーマット",
@@ -58,12 +56,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_workspace_member"
     subcommand_help = "自身のワークスペースメンバの一覧を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/my/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/my/subcommand.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 from typing import Optional
 
 import annoworkcli
 import annoworkcli.my.get_my_account
 import annoworkcli.my.list_my_workspace_member
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     annoworkcli.my.get_my_account.add_parser(subparsers)
     annoworkcli.my.list_my_workspace_member.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "my"
     subcommand_help = "自分自身に関するサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/schedule/list_assigned_hours_daily.py` & `annoworkcli-3.7.0/annoworkcli/schedule/list_assigned_hours_daily.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import argparse
 import logging
 from collections import defaultdict
+from collections.abc import Collection
 from dataclasses import dataclass
 from pathlib import Path
-from typing import Any, Collection, Dict, Optional, Tuple
+from typing import Any, Dict, Optional, Tuple  # noqa: UP035
 
 import pandas
 from annoworkapi.resource import Resource as AnnoworkResource
 from dataclasses_json import DataClassJsonMixin
 
 import annoworkcli
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
@@ -33,15 +34,15 @@
     job_name: Optional[str]
     workspace_member_id: str
     user_id: Optional[str]
     username: Optional[str]
     assigned_working_hours: float
 
 
-AssignedHoursDict = Dict[Tuple[str, str, str], float]
+AssignedHoursDict = Dict[Tuple[str, str, str], float]  # noqa: UP006
 """アサイン時間の日ごとの情報を格納する辞書
 key: (date, workspace_member_id, job_id), value: アサイン時間
 """
 
 
 def _get_min_max_date_from_schedule_list(schedule_list: list[dict[str, Any]]) -> tuple[str, str]:
     min_date = "9999-99-99"
@@ -49,39 +50,35 @@
     for schedule in schedule_list:
         min_date = min(min_date, schedule["start_date"])
         max_date = max(max_date, schedule["end_date"])
     return min_date, max_date
 
 
 class ListAssignedHoursDaily:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
         self.list_schedule_obj = ListSchedule(annowork_service, workspace_id)
 
     def get_expected_working_hours_dict(self, schedule_list: list[dict[str, Any]]) -> ExpectedWorkingHoursDict:
         min_date, max_date = _get_min_max_date_from_schedule_list(schedule_list)
         query_params = {"term_start": min_date, "term_end": max_date}
         logger.debug(f"予定稼働時間を取得します。 :: {query_params=}")
-        expected_working_times = self.annowork_service.api.get_expected_working_times(
-            self.workspace_id, query_params=query_params
-        )
+        expected_working_times = self.annowork_service.api.get_expected_working_times(self.workspace_id, query_params=query_params)
         return {(e["date"], e["workspace_member_id"]): e["expected_working_hours"] for e in expected_working_times}
 
     def get_assigned_hours_daily_list(
         self,
         *,
         start_date: Optional[str] = None,
         end_date: Optional[str] = None,
         job_ids: Optional[Collection[str]] = None,
         user_ids: Optional[Collection[str]] = None,
     ) -> list[AssignedHoursDaily]:
-        schedule_list = self.list_schedule_obj.get_schedules(
-            start_date=start_date, end_date=end_date, job_ids=job_ids, user_ids=user_ids
-        )
+        schedule_list = self.list_schedule_obj.get_schedules(start_date=start_date, end_date=end_date, job_ids=job_ids, user_ids=user_ids)
 
         if len(schedule_list) == 0:
             return []
 
         result_dict: AssignedHoursDict = defaultdict(float)
         expected_working_hours_dict = self.get_expected_working_hours_dict(schedule_list)
 
@@ -107,17 +104,15 @@
             if start_date is not None and not date >= start_date:
                 continue
             if end_date is not None and not date <= end_date:
                 continue
 
             job = all_jobs_dict.get(job_id)
             if job is None:
-                logger.warning(
-                    f"{job_id=} であるジョブは存在しません。 " f":: date='{date}', workspace_member_id='{workspace_member_id}'"
-                )
+                logger.warning(f"{job_id=} であるジョブは存在しません。 " f":: date='{date}', workspace_member_id='{workspace_member_id}'")
 
             member = all_members_dict.get(workspace_member_id)
             if member is None:
                 logger.warning(f"{workspace_member_id=} であるメンバーは存在しません。 " f":: date='{date}', job_id='{job_id}'")
 
             result_list.append(
                 AssignedHoursDaily(
@@ -129,15 +124,15 @@
                     user_id=member["user_id"] if member is not None else None,
                     username=member["username"] if member is not None else None,
                 )
             )
 
         return result_list
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         *,
         output: Path,
         output_format: OutputFormat,
         start_date: Optional[str],
         end_date: Optional[str],
         job_id_list: Optional[list[str]],
@@ -146,43 +141,44 @@
         result = self.get_assigned_hours_daily_list(
             start_date=start_date,
             end_date=end_date,
             job_ids=job_id_list,
             user_ids=user_id_list,
         )
         if len(result) == 0:
-            logger.warning(f"アサイン時間情報は0件なので、出力しません。")
+            logger.warning("アサイン時間情報は0件なので、出力しません。")
             return
 
         result.sort(key=lambda e: e.date)
         logger.info(f"{len(result)} 件のアサイン時間情報を出力します。")
 
         if output_format == OutputFormat.JSON:
             # `.schema().dump(many=True)`を使わない理由：使うと警告が発生するから
             # https://qiita.com/yuji38kwmt/items/a3625b2011aff1d9901b
             dict_result = []
             for elm in result:
-                dict_result.append(elm.to_dict())
+                dict_result.append(elm.to_dict())  # noqa: PERF401
             print_json(dict_result, is_pretty=True, output=output)
         else:
             df = pandas.DataFrame(result)
             print_csv(df, output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     user_id_list = get_list_from_args(args.user_id)
 
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     if all(v is None for v in [job_id_list, user_id_list, start_date, end_date]):
         logger.warning(
-            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。" "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。"
+            "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
         )
 
     ListAssignedHoursDaily(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
     ).main(
         job_id_list=job_id_list,
@@ -190,15 +186,15 @@
         start_date=start_date,
         end_date=end_date,
         output=args.output,
         output_format=OutputFormat(args.format),
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -224,12 +220,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_daily"
     subcommand_help = "作業計画から求めたアサイン時間を日ごとに出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py` & `annoworkcli-3.7.0/annoworkcli/schedule/list_assigned_hours_daily_groupby_tag.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 import argparse
 import logging
 from collections import defaultdict
+from collections.abc import Collection
 from pathlib import Path
-from typing import Any, Collection, Optional
+from typing import Any, Optional
 
 import pandas
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 from annoworkcli.schedule.list_assigned_hours_daily import AssignedHoursDaily, ListAssignedHoursDaily
 from annoworkcli.schedule.list_schedule import ListSchedule
 
 logger = logging.getLogger(__name__)
 
 
 class ListAssignedHoursDailyGroupbyTag:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
         self.list_schedule_obj = ListSchedule(annowork_service, workspace_id)
 
     def get_assigned_hours_groupby_tag(
         self,
         assigned_hours_list: list[AssignedHoursDaily],
@@ -51,17 +52,15 @@
 
         # dictのkeyはtuple[date, job_id, workspace_tag_name]
         dict_hours: dict[tuple[str, str, str], float] = defaultdict(float)
 
         # ワークスペースタグごと日毎の時間を集計する
         for workspace_tag in workspace_tags:
             workspace_tag_name = workspace_tag["workspace_tag_name"]
-            members = self.annowork_service.api.get_workspace_tag_members(
-                self.workspace_id, workspace_tag["workspace_tag_id"]
-            )
+            members = self.annowork_service.api.get_workspace_tag_members(self.workspace_id, workspace_tag["workspace_tag_id"])
             member_ids = {e["workspace_member_id"] for e in members}
             for elm in assigned_hours_list:
                 if elm.workspace_member_id in member_ids:
                     dict_hours[elm.date, elm.job_id, workspace_tag_name] += elm.assigned_working_hours
 
         # 全体の時間を日毎に集計する
 
@@ -80,15 +79,15 @@
         for (date, job_id), value in dict_date.items():
             e = {"date": date, "job_id": job_id, "job_name": job_dict.get(job_id), "assigned_working_hours": value}
             results.append(e)
 
         results.sort(key=lambda e: (e["date"], e["job_id"]))
         return results
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         *,
         output: Path,
         output_format: OutputFormat,
         start_date: Optional[str],
         end_date: Optional[str],
         job_id_list: Optional[list[str]],
@@ -100,15 +99,15 @@
         assigned_hours_list = list_obj.get_assigned_hours_daily_list(
             start_date=start_date,
             end_date=end_date,
             job_ids=job_id_list,
             user_ids=user_id_list,
         )
         if len(assigned_hours_list) == 0:
-            logger.warning(f"アサイン時間情報は0件なので、出力しません。")
+            logger.warning("アサイン時間情報は0件なので、出力しません。")
             return
 
         results = self.get_assigned_hours_groupby_tag(
             assigned_hours_list,
             target_workspace_tag_ids=target_workspace_tag_ids,
             target_workspace_tag_names=target_workspace_tag_names,
         )
@@ -127,25 +126,26 @@
             ]
             remaining_columns = list(set(df.columns) - set(required_columns))
             columns = required_columns + sorted(remaining_columns)
 
             print_csv(df[columns], output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     user_id_list = get_list_from_args(args.user_id)
 
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     if all(v is None for v in [job_id_list, user_id_list, start_date, end_date]):
         logger.warning(
-            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。" "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。"
+            "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
         )
 
     workspace_tag_id_list = get_list_from_args(args.workspace_tag_id)
     workspace_tag_name_list = get_list_from_args(args.workspace_tag_name)
 
     ListAssignedHoursDailyGroupbyTag(
         annowork_service=annowork_service,
@@ -158,15 +158,15 @@
         output=args.output,
         output_format=OutputFormat(args.format),
         target_workspace_tag_ids=workspace_tag_id_list,
         target_workspace_tag_names=workspace_tag_name_list,
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -208,12 +208,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list_daily_groupby_tag"
     subcommand_help = "日ごとのアサイン時間を、ワークスペースタグで集計した値を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/schedule/list_schedule.py` & `annoworkcli-3.7.0/annoworkcli/schedule/list_schedule.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 import argparse
 import logging
+from collections.abc import Collection
 from pathlib import Path
-from typing import Any, Collection, Dict, Optional, Tuple
+from typing import Any, Dict, Optional, Tuple  # noqa: UP035
 
 import pandas
 from annoworkapi.enums import ScheduleType
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
-ExpectedWorkingHoursDict = Dict[Tuple[str, str], float]
+ExpectedWorkingHoursDict = Dict[Tuple[str, str], float]  # noqa: UP006
 """keyがtuple(date, workspace_member_id), valueが予定稼働時間のdict
 """
 
 
-def create_assigned_hours_dict(
-    schedule: dict[str, Any], expected_working_hours_dict: ExpectedWorkingHoursDict
-) -> dict[str, float]:
+def create_assigned_hours_dict(schedule: dict[str, Any], expected_working_hours_dict: ExpectedWorkingHoursDict) -> dict[str, float]:
     """作業計画情報からアサインされた時間の辞書（key:日付, value:アサイン時間）を返す。
 
     Args:
         schedule (dict[str,Any]): １つの作業計画情報
         expected_working_hours_dict (ExpectedWorkingHoursDict): 予定稼働時間情報のdict
 
     Returns:
@@ -45,36 +44,30 @@
             expected_working_hours = expected_working_hours_dict.get((date, schedule["workspace_member_id"]), 0)
             result[date] = expected_working_hours * schedule["value"] * 0.01
 
     return result
 
 
 class ListSchedule:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-        self.workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+        self.workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
 
-    def _set_assigned_hours(self, schedule_list: list[dict[str, Any]], min_date: str, max_date: str):
+    def _set_assigned_hours(self, schedule_list: list[dict[str, Any]], min_date: str, max_date: str):  # noqa: ANN202
         query_params = {"term_start": min_date, "term_end": max_date}
         logger.debug(f"予定稼働時間を取得します。 :: {query_params=}")
-        expected_working_times = self.annowork_service.api.get_expected_working_times(
-            self.workspace_id, query_params=query_params
-        )
-        expected_working_hours_dict = {
-            (e["date"], e["workspace_member_id"]): e["expected_working_hours"] for e in expected_working_times
-        }
+        expected_working_times = self.annowork_service.api.get_expected_working_times(self.workspace_id, query_params=query_params)
+        expected_working_hours_dict = {(e["date"], e["workspace_member_id"]): e["expected_working_hours"] for e in expected_working_times}
         for schedule in schedule_list:
             assigned_hours_dict = create_assigned_hours_dict(schedule, expected_working_hours_dict)
             schedule["assigned_working_hours"] = sum(assigned_hours_dict.values())
 
-    def set_additional_info_to_schedule(self, schedule_list: list[dict[str, Any]]):
+    def set_additional_info_to_schedule(self, schedule_list: list[dict[str, Any]]):  # noqa: ANN201
         """workspace_member_id, job_idに紐づく情報, アサインされた時間を付与する。
 
         Args:
             schedule_list (list[dict[str,Any]]): (IN/OUT) 実績作業時間のリスト
         """
         if len(schedule_list) == 0:
             return
@@ -90,17 +83,15 @@
         for schedule in schedule_list:
             min_date = min(min_date, schedule["start_date"])
             max_date = max(max_date, schedule["end_date"])
 
             workspace_member_id = schedule["workspace_member_id"]
             member = workspace_member_dict.get(schedule["workspace_member_id"])
             if member is None:
-                logger.warning(
-                    f"{workspace_member_id=} であるワークスペースメンバは存在しません。 " f":: schedule_id= '{schedule['schedule_id']}' "
-                )
+                logger.warning(f"{workspace_member_id=} であるワークスペースメンバは存在しません。 " f":: schedule_id= '{schedule['schedule_id']}' ")
                 continue
 
             schedule["user_id"] = member["user_id"]
             schedule["username"] = member["username"]
 
             job_id = schedule["job_id"]
             job = job_dict.get(job_id)
@@ -148,30 +139,28 @@
         }
 
         schedule_list = []
         if job_ids is not None:
             for job_id in job_ids:
                 query_params["job_id"] = job_id
                 logger.debug(f"作業計画を取得します。 :: {query_params=}")
-                schedule_list.extend(
-                    self.annowork_service.api.get_schedules(self.workspace_id, query_params=query_params)
-                )
+                schedule_list.extend(self.annowork_service.api.get_schedules(self.workspace_id, query_params=query_params))
         else:
             logger.debug(f"作業計画を取得します。 :: {query_params=}")
             schedule_list.extend(self.annowork_service.api.get_schedules(self.workspace_id, query_params=query_params))
 
         if user_ids is not None:
             workspace_member_id_list = self.get_workspace_member_id_list_from_user_id(user_ids)
             schedule_list = [e for e in schedule_list if e["workspace_member_id"] in set(workspace_member_id_list)]
 
         if is_set_additional_info is not None:
             self.set_additional_info_to_schedule(schedule_list)
         return schedule_list
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         *,
         output: Path,
         output_format: OutputFormat,
         start_date: Optional[str],
         end_date: Optional[str],
         job_id_list: Optional[list[str]],
@@ -181,15 +170,15 @@
             start_date=start_date,
             end_date=end_date,
             job_ids=job_id_list,
             user_ids=user_id_list,
             is_set_additional_info=True,
         )
         if len(result) == 0:
-            logger.warning(f"作業計画情報は0件なので、出力しません。")
+            logger.warning("作業計画情報は0件なので、出力しません。")
             return
 
         logger.info(f"{len(result)} 件の作業計画情報を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(result, is_pretty=True, output=output)
         else:
@@ -210,25 +199,26 @@
             ]
             remaining_columns = list(set(df.columns) - set(required_columns))
             columns = required_columns + remaining_columns
 
             print_csv(df[columns], output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     job_id_list = get_list_from_args(args.job_id)
     user_id_list = get_list_from_args(args.user_id)
 
     start_date: Optional[str] = args.start_date
     end_date: Optional[str] = args.end_date
 
     if all(v is None for v in [job_id_list, user_id_list, start_date, end_date]):
         logger.warning(
-            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。" "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
+            "'--start_date'や'--job_id'などの絞り込み条件が1つも指定されていません。"
+            "WebAPIから取得するデータ量が多すぎて、WebAPIのリクエストが失敗するかもしれません。"
         )
 
     ListSchedule(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
     ).main(
         job_id_list=job_id_list,
@@ -236,15 +226,15 @@
         start_date=start_date,
         end_date=end_date,
         output=args.output,
         output_format=OutputFormat(args.format),
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -270,12 +260,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list"
     subcommand_help = "作業計画の一覧を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/schedule/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/schedule/subcommand.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 import argparse
 from typing import Optional
 
 import annoworkcli
+import annoworkcli.schedule.delete_schedule
 import annoworkcli.schedule.list_assigned_hours_daily
 import annoworkcli.schedule.list_assigned_hours_daily_groupby_tag
 import annoworkcli.schedule.list_schedule
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
+    annoworkcli.schedule.delete_schedule.add_parser(subparsers)
     annoworkcli.schedule.list_schedule.add_parser(subparsers)
     annoworkcli.schedule.list_assigned_hours_daily.add_parser(subparsers)
     annoworkcli.schedule.list_assigned_hours_daily_groupby_tag.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "schedule"
     subcommand_help = "作業計画関係のサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace/list_workspace.py` & `annoworkcli-3.7.0/annoworkcli/workspace/list_workspace.py`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListWorkspace:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         annowork_service: AnnoworkResource,
     ):
         self.annowork_service = annowork_service
 
     def get_workspace_list(
         self,
@@ -32,44 +32,44 @@
             org = self.annowork_service.wrapper.get_workspace_or_none(workspace_id)
             if org is None:
                 logger.warning(f"{workspace_id=} であるワークスペースは存在しませんでした。")
                 continue
             workspace_list.append(org)
         return workspace_list
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         output: Path,
         output_format: OutputFormat,
         *,
         workspace_id_list: Optional[list[str]],
     ):
         workspace_list = self.get_workspace_list(workspace_id_list)
         if len(workspace_list) == 0:
-            logger.warning(f"ワークスペース情報は0件なので、出力しません。")
+            logger.warning("ワークスペース情報は0件なので、出力しません。")
             return
 
         logger.debug(f"{len(workspace_list)} 件のワークスペース一覧を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(workspace_list, is_pretty=True, output=output)
         else:
             df = pandas.DataFrame(workspace_list)
             print_csv(df, output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     workspace_id_list = get_list_from_args(args.workspace_id)
     ListWorkspace(
         annowork_service=annowork_service,
     ).main(output=args.output, output_format=OutputFormat(args.format), workspace_id_list=workspace_id_list)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         nargs="+",
         required=False,
         help="対象のワークスペースIDを指定してください。未指定の場合は、自身の所属しているワークスペース一覧を出力します。",
@@ -89,12 +89,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list"
     subcommand_help = "ワークスペースの一覧を取得します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace/put_workspace.py` & `annoworkcli-3.7.0/annoworkcli/workspace/put_workspace.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,44 +7,44 @@
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi
 
 logger = logging.getLogger(__name__)
 
 
 class PutWorkspace:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         annowork_service: AnnoworkResource,
     ):
         self.annowork_service = annowork_service
 
-    def main(self, workspace_id: str, workspace_name: str, email: str):
+    def main(self, workspace_id: str, workspace_name: str, email: str):  # noqa: ANN201
         org = self.annowork_service.wrapper.get_workspace_or_none(workspace_id)
 
         request_body = {
             "workspace_name": workspace_name,
             "email": email,
         }
         if org is not None:
             request_body["last_updated_datetime"] = org["updated_datetime"]
 
         self.annowork_service.api.put_workspace(workspace_id, request_body=request_body)
 
         logger.info(f"ワークスペース {workspace_id} を作成/更新しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
 
     PutWorkspace(
         annowork_service=annowork_service,
     ).main(workspace_id=args.workspace_id, workspace_name=args.workspace_name, email=args.email)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -66,12 +66,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "put"
     subcommand_help = "ワークスペースを登録/更新します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/workspace/subcommand.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,22 +3,20 @@
 
 import annoworkcli
 import annoworkcli.workspace.list_workspace
 import annoworkcli.workspace.put_workspace
 from annoworkcli.common.cli import add_parser as add_root_parser
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
     annoworkcli.workspace.list_workspace.add_parser(subparsers)
     annoworkcli.workspace.put_workspace.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "workspace"
     subcommand_help = "ワークスペース関係のサブコマンド"
 
-    parser = add_root_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = add_root_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_member/append_tag_to_workspace_member.py` & `annoworkcli-3.7.0/annoworkcli/workspace_member/append_tag_to_workspace_member.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import argparse
 import logging
-from typing import Any, Collection, Optional
+from collections.abc import Collection
+from typing import Any, Optional
 
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, get_list_from_args
 
 logger = logging.getLogger(__name__)
 
 
 class AppendTagToWorkspaceMember:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         *,
         annowork_service: AnnoworkResource,
         workspace_id: str,
     ):
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
@@ -34,36 +35,30 @@
         # request_bodyにuser_idを指定しない理由: user_idを指定すると、脱退済のユーザーが組織に招待されてしまうため
         request_body: dict[str, Any] = {
             "role": old_member["role"],
             "workspace_tags": new_workspace_tags,
             "last_updated_datetime": old_member["updated_datetime"],
         }
 
-        new_member = self.annowork_service.api.put_workspace_member(
-            self.workspace_id, workspace_member_id, request_body=request_body
-        )
+        new_member = self.annowork_service.api.put_workspace_member(self.workspace_id, workspace_member_id, request_body=request_body)
         logger.debug(f"{user_id=} :: ワークスペースメンバにワークスペースタグを追加しました。 :: username='{new_member['username']}'")
         return True
 
-    def main(self, user_id_list: list[str], workspace_tag_ids: Collection[str]):
-        workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+    def main(self, user_id_list: list[str], workspace_tag_ids: Collection[str]):  # noqa: ANN201
+        workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
         member_dict: dict[str, dict[str, Any]] = {m["user_id"]: m for m in workspace_members}
         success_count = 0
         for user_id in user_id_list:
             try:
                 old_member = member_dict.get(user_id)
                 if old_member is None:
                     logger.warning(f"{user_id=} のユーザはワークスペースメンバに存在しないので、スキップします。")
                     continue
 
-                old_tags = self.annowork_service.api.get_workspace_member_tags(
-                    self.workspace_id, old_member["workspace_member_id"]
-                )
+                old_tags = self.annowork_service.api.get_workspace_member_tags(self.workspace_id, old_member["workspace_member_id"])
                 old_workspace_tag_ids = {e["workspace_tag_id"] for e in old_tags}
                 diff_tags = set(workspace_tag_ids) - old_workspace_tag_ids
                 if len(diff_tags) == 0:
                     logger.warning(f"{user_id=} には、すでにワークスペースタグ {workspace_tag_ids} が設定されているので、スキップします。")
                     continue
 
                 result = self.put_workspace_member(
@@ -77,27 +72,27 @@
             except Exception as e:
                 logger.warning(f"{user_id=}: ワークスペースタグの付与に失敗しました。{e}", e)
                 continue
 
         logger.info(f"{success_count}/{len(user_id_list)} 件のユーザにワークスペースタグを付与しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     workspace_tag_id_list = get_list_from_args(args.workspace_tag_id)
     assert user_id_list is not None
     assert workspace_tag_id_list is not None
     AppendTagToWorkspaceMember(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
     ).main(user_id_list=user_id_list, workspace_tag_ids=workspace_tag_id_list)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -123,12 +118,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "append_tag"
     subcommand_help = "ワークスペースメンバにワークスペースタグを追加します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_member/change_workspace_member_properties.py` & `annoworkcli-3.7.0/annoworkcli/workspace_member/change_workspace_member_properties.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 import argparse
 import logging
-from typing import Any, Collection, Optional
+from collections.abc import Collection
+from typing import Any, Optional
 
 from annoworkapi.enums import Role
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, get_list_from_args
 
 logger = logging.getLogger(__name__)
 
 
 class ChangeWorkspaceMemberProperties:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         *,
         annowork_service: AnnoworkResource,
         workspace_id: str,
     ):
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
@@ -34,65 +35,57 @@
         # request_bodyにuser_idを指定しない理由: user_idを指定すると、脱退済のユーザーが組織に招待されてしまうため
         request_body: dict[str, Any] = {
             "role": role,
             "workspace_tags": list(old_workspace_tag_ids),
             "last_updated_datetime": old_member["updated_datetime"],
         }
 
-        new_member = self.annowork_service.api.put_workspace_member(
-            self.workspace_id, workspace_member_id, request_body=request_body
-        )
+        new_member = self.annowork_service.api.put_workspace_member(self.workspace_id, workspace_member_id, request_body=request_body)
         logger.debug(f"{user_id=}, {workspace_member_id=}: ワークスペースメンバのロールを変更しました。 :: {new_member}")
         return True
 
-    def main(self, user_id_list: list[str], role: str):
-        workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+    def main(self, user_id_list: list[str], role: str):  # noqa: ANN201
+        workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
         member_dict: dict[str, dict[str, Any]] = {m["user_id"]: m for m in workspace_members}
         success_count = 0
         for user_id in user_id_list:
             try:
                 old_member = member_dict.get(user_id)
                 if old_member is None:
                     logger.warning(f"{user_id=} のユーザはワークスペースメンバに存在しないので、スキップします。")
                     continue
 
                 if old_member["role"] == role:
                     logger.warning(f"{user_id=} のロールは '{role}' なので、ロールを変更する必要はありません。スキップします。")
                     continue
 
-                old_tags = self.annowork_service.api.get_workspace_member_tags(
-                    self.workspace_id, old_member["workspace_member_id"]
-                )
+                old_tags = self.annowork_service.api.get_workspace_member_tags(self.workspace_id, old_member["workspace_member_id"])
                 old_workspace_tag_ids = {e["workspace_tag_id"] for e in old_tags}
 
-                result = self.put_workspace_member(
-                    user_id, role=role, old_workspace_tag_ids=old_workspace_tag_ids, old_member=old_member
-                )
+                result = self.put_workspace_member(user_id, role=role, old_workspace_tag_ids=old_workspace_tag_ids, old_member=old_member)
                 if result:
                     success_count += 1
             except Exception as e:
                 logger.warning(f"{user_id=}: ワークスペースメンバの登録に失敗しました。{e}")
                 continue
 
         logger.info(f"{success_count}/{len(user_id_list)} 件のユーザをワークスペースメンバに登録しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     assert user_id_list is not None
     ChangeWorkspaceMemberProperties(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
     ).main(user_id_list=user_id_list, role=args.role)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -117,12 +110,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "change"
     subcommand_help = "ワークスペースメンバの情報（ロールなど）を変更します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_member/delete_workspace_member.py` & `annoworkcli-3.7.0/annoworkcli/workspace_member/delete_workspace_member.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,59 +7,57 @@
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, get_list_from_args
 
 logger = logging.getLogger(__name__)
 
 
 class DeleteWorkspaceMember:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         annowork_service: AnnoworkResource,
         workspace_id: str,
     ):
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-    def main(self, user_id_list: list[str]):
+    def main(self, user_id_list: list[str]):  # noqa: ANN201
         workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id)
         member_dict: dict[str, dict[str, Any]] = {m["user_id"]: m for m in workspace_members}
         success_count = 0
 
         logger.info(f"{len(user_id_list)} 件のユーザをワークスペースメンバから削除します。")
         for user_id in user_id_list:
             member = member_dict.get(user_id)
             if member is None:
                 logger.warning(f"{user_id=}: ユーザがワークスペースメンバに存在しません。")
                 continue
 
             try:
                 workspace_member_id = member["workspace_member_id"]
-                self.annowork_service.api.delete_workspace_member(
-                    self.workspace_id, workspace_member_id=workspace_member_id
-                )
+                self.annowork_service.api.delete_workspace_member(self.workspace_id, workspace_member_id=workspace_member_id)
                 success_count += 1
             except Exception as e:
                 logger.warning(f"{user_id=}: ワークスペースメンバの削除に失敗しました。{e}")
                 continue
 
         logger.info(f"{success_count}/{len(user_id_list)} 件のユーザをワークスペースメンバから削除しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
 
     user_id_list = get_list_from_args(args.user_id)
     assert user_id_list is not None
     DeleteWorkspaceMember(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
     ).main(user_id_list=user_id_list)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -76,12 +74,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "delete"
     subcommand_help = "ワークスペースメンバを削除します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_member/list_workspace_member.py` & `annoworkcli-3.7.0/annoworkcli/workspace_member/list_workspace_member.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,94 +1,90 @@
 import argparse
 import logging
+from collections.abc import Collection
 from pathlib import Path
-from typing import Any, Collection, Optional
+from typing import Any, Optional
 
 import more_itertools
 import pandas
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi, get_list_from_args
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListWorkspace:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-    def set_additional_info(self, workspace_members: list[dict[str, Any]]):
+    def set_additional_info(self, workspace_members: list[dict[str, Any]]):  # noqa: ANN201
         logger.debug(f"{len(workspace_members)} 件のメンバのワークスペースタグ情報を取得します。")
         for member in workspace_members:
-            workspace_tags = self.annowork_service.api.get_workspace_member_tags(
-                self.workspace_id, member["workspace_member_id"]
-            )
+            workspace_tags = self.annowork_service.api.get_workspace_member_tags(self.workspace_id, member["workspace_member_id"])
             member["workspace_tag_ids"] = [e["workspace_tag_id"] for e in workspace_tags]
             member["workspace_tag_names"] = [e["workspace_tag_name"] for e in workspace_tags]
 
     def get_workspace_members_from_tags(self, workspace_tag_ids: Collection[str]) -> list[dict[str, Any]]:
         result = []
         for tag_id in workspace_tag_ids:
             tmp = self.annowork_service.api.get_workspace_tag_members(self.workspace_id, tag_id)
             result.extend(tmp)
 
         # メンバが重複している可能性があるので取り除く
         # pandasのメソッドを使うために、一時的にDataFrameにする
         return pandas.DataFrame(result).drop_duplicates().to_dict("records")
 
     @classmethod
-    def filter_member_with_user_id(
-        cls, members: list[dict[str, Any]], user_ids: Collection[str]
-    ) -> list[dict[str, Any]]:
+    def filter_member_with_user_id(cls, members: list[dict[str, Any]], user_ids: Collection[str]) -> list[dict[str, Any]]:
         """
         メンバ一覧を、指定したuser_idで絞り込みます。
 
         Args:
             members: 絞り込まれるメンバ一覧
             user_ids: 指定したuser_idで絞り込みます
 
         Returns:
             絞り込み後のメンバ一覧
         """
         result = []
         for user_id in user_ids:
             member = more_itertools.first_true(
-                members, pred=lambda e: e["user_id"] == user_id  # pylint: disable=cell-var-from-loop
+                members,
+                pred=lambda e: e["user_id"] == user_id,  # pylint: disable=cell-var-from-loop  # noqa: B023
             )
             if member is not None:
                 result.append(member)
             else:
                 logger.warning(f"{user_id=}であるメンバは存在しません。")
                 continue
         return result
 
-    def main(
+    def main(  # noqa: ANN201
         self,
         output: Path,
         output_format: OutputFormat,
         workspace_tag_ids: Optional[Collection[str]],
         user_ids: Optional[Collection[str]],
         show_workspace_tag: bool,
     ):
         # workspace_tag_idsとuser_idsは排他的
         assert workspace_tag_ids is None or user_ids is None
         if workspace_tag_ids is not None:
             workspace_members = self.get_workspace_members_from_tags(workspace_tag_ids)
         else:
-            workspace_members = self.annowork_service.api.get_workspace_members(
-                self.workspace_id, query_params={"includes_inactive_members": True}
-            )
+            workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
             if user_ids is not None:
                 workspace_members = self.filter_member_with_user_id(workspace_members, user_ids)
 
         if len(workspace_members) == 0:
-            logger.warning(f"ワークスペースメンバ情報は0件なので、出力しません。")
+            logger.warning("ワークスペースメンバ情報は0件なので、出力しません。")
             return
 
         if show_workspace_tag:
             self.set_additional_info(workspace_members)
 
         workspace_members.sort(key=lambda e: e["user_id"].lower())
 
@@ -97,28 +93,28 @@
         if output_format == OutputFormat.JSON:
             print_json(workspace_members, is_pretty=True, output=output)
         else:
             df = pandas.json_normalize(workspace_members)
             print_csv(df, output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     workspace_tag_id_list = get_list_from_args(args.workspace_tag_id)
     user_id_list = get_list_from_args(args.user_id)
     ListWorkspace(annowork_service=annowork_service, workspace_id=args.workspace_id).main(
         output=args.output,
         output_format=OutputFormat(args.format),
         workspace_tag_ids=workspace_tag_id_list,
         user_ids=user_id_list,
         show_workspace_tag=args.show_workspace_tag,
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -159,12 +155,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list"
     subcommand_help = "ワークスペースメンバの一覧を出力します。無効化されたメンバも出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_member/put_workspace_member.py` & `annoworkcli-3.7.0/annoworkcli/workspace_member/put_workspace_member.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 import argparse
 import logging
 import uuid
-from typing import Any, Collection, Optional
+from collections.abc import Collection
+from typing import Any, Optional
 
 from annoworkapi.enums import Role
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, get_list_from_args
 
 logger = logging.getLogger(__name__)
 
 
 class PutWorkspaceMember:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         annowork_service: AnnoworkResource,
         workspace_id: str,
     ):
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-    def put_workspace_member(
+    def put_workspace_member(  # noqa: ANN201
         self,
         user_id: str,
         role: str,
         workspace_tag_id_list: Optional[Collection[str]],
         old_member: Optional[dict[str, Any]],
     ):
         """[summary]
@@ -49,24 +50,20 @@
             "user_id": user_id,
             "role": role,
             "workspace_tags": workspace_tag_id_list if workspace_tag_id_list is not None else [],
         }
         if last_updated_datetime is not None:
             request_body["last_updated_datetime"] = last_updated_datetime
 
-        new_member = self.annowork_service.api.put_workspace_member(
-            self.workspace_id, workspace_member_id, request_body=request_body
-        )
+        new_member = self.annowork_service.api.put_workspace_member(self.workspace_id, workspace_member_id, request_body=request_body)
         logger.debug(f"{user_id=} :: ワークスペースメンバを追加しました。 :: username='{new_member['username']}', {workspace_member_id=}")
         return True
 
-    def main(self, user_id_list: list[str], role: str, workspace_tag_id_list: Optional[Collection[str]]):
-        workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+    def main(self, user_id_list: list[str], role: str, workspace_tag_id_list: Optional[Collection[str]]):  # noqa: ANN201
+        workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
         member_dict: dict[str, dict[str, Any]] = {m["user_id"]: m for m in workspace_members}
         success_count = 0
         for user_id in user_id_list:
             try:
                 result = self.put_workspace_member(
                     user_id,
                     role,
@@ -78,26 +75,26 @@
             except Exception:
                 logger.warning(f"{user_id=}: ワークスペースメンバの登録に失敗しました。", exc_info=True)
                 continue
 
         logger.info(f"{success_count}/{len(user_id_list)} 件のユーザをワークスペースメンバに登録しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     workspace_tag_id_list = get_list_from_args(args.workspace_tag_id)
     assert user_id_list is not None
     PutWorkspaceMember(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
     ).main(user_id_list=user_id_list, role=args.role, workspace_tag_id_list=workspace_tag_id_list)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -131,12 +128,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "put"
     subcommand_help = "ワークスペースメンバを登録します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_member/remove_tag_to_workspace_member.py` & `annoworkcli-3.7.0/annoworkcli/workspace_member/remove_tag_to_workspace_member.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import argparse
 import logging
-from typing import Any, Collection, Optional
+from collections.abc import Collection
+from typing import Any, Optional
 
 from annoworkapi.resource import Resource as AnnoworkResource
 
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi, get_list_from_args
 
 logger = logging.getLogger(__name__)
 
 
 class RemoveTagToWorkspaceMember:
-    def __init__(
+    def __init__(  # noqa: ANN204
         self,
         *,
         annowork_service: AnnoworkResource,
         workspace_id: str,
     ):
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
@@ -34,36 +35,30 @@
         # request_bodyにuser_idを指定しない理由: user_idを指定すると、脱退済のユーザーが組織に招待されてしまうため
         request_body: dict[str, Any] = {
             "role": old_member["role"],
             "workspace_tags": new_workspace_tags,
             "last_updated_datetime": old_member["updated_datetime"],
         }
 
-        new_member = self.annowork_service.api.put_workspace_member(
-            self.workspace_id, workspace_member_id, request_body=request_body
-        )
+        new_member = self.annowork_service.api.put_workspace_member(self.workspace_id, workspace_member_id, request_body=request_body)
         logger.debug(f"{user_id=} :: ワークスペースメンバからワークスペースタグを削除しました。 :: username='{new_member['username']}'")
         return True
 
-    def main(self, user_id_list: list[str], workspace_tag_ids: Collection[str]):
-        workspace_members = self.annowork_service.api.get_workspace_members(
-            self.workspace_id, query_params={"includes_inactive_members": True}
-        )
+    def main(self, user_id_list: list[str], workspace_tag_ids: Collection[str]):  # noqa: ANN201
+        workspace_members = self.annowork_service.api.get_workspace_members(self.workspace_id, query_params={"includes_inactive_members": True})
         member_dict: dict[str, dict[str, Any]] = {m["user_id"]: m for m in workspace_members}
         success_count = 0
         for user_id in user_id_list:
             try:
                 old_member = member_dict.get(user_id)
                 if old_member is None:
                     logger.warning(f"{user_id=} のユーザはワークスペースメンバに存在しないので、スキップします。")
                     continue
 
-                old_tags = self.annowork_service.api.get_workspace_member_tags(
-                    self.workspace_id, old_member["workspace_member_id"]
-                )
+                old_tags = self.annowork_service.api.get_workspace_member_tags(self.workspace_id, old_member["workspace_member_id"])
                 old_workspace_tag_ids = {e["workspace_tag_id"] for e in old_tags}
                 diff_tags = old_workspace_tag_ids - set(workspace_tag_ids)
                 if old_workspace_tag_ids == diff_tags:
                     logger.warning(f"{user_id=} には、すでにワークスペースタグ {workspace_tag_ids} が設定されていないので、スキップします。")
                     continue
 
                 result = self.put_workspace_member(
@@ -77,28 +72,28 @@
             except Exception as e:
                 logger.warning(f"{user_id=}: ワークスペースタグの削除に失敗しました。{e}", e)
                 continue
 
         logger.info(f"{success_count}/{len(user_id_list)} 件のユーザからワークスペースタグを削除しました。")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     user_id_list = get_list_from_args(args.user_id)
     workspace_tag_id_list = get_list_from_args(args.workspace_tag_id)
     assert user_id_list is not None
     assert workspace_tag_id_list is not None
 
     RemoveTagToWorkspaceMember(
         annowork_service=annowork_service,
         workspace_id=args.workspace_id,
     ).main(user_id_list=user_id_list, workspace_tag_ids=workspace_tag_id_list)
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -124,12 +119,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "remove_tag"
     subcommand_help = "ワークスペースメンバからワークスペースタグを削除します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_member/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/workspace_member/subcommand.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import annoworkcli.workspace_member.change_workspace_member_properties
 import annoworkcli.workspace_member.delete_workspace_member
 import annoworkcli.workspace_member.list_workspace_member
 import annoworkcli.workspace_member.put_workspace_member
 import annoworkcli.workspace_member.remove_tag_to_workspace_member
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     annoworkcli.workspace_member.append_tag_to_workspace_member.add_parser(subparsers)
     annoworkcli.workspace_member.change_workspace_member_properties.add_parser(subparsers)
     annoworkcli.workspace_member.delete_workspace_member.add_parser(subparsers)
     annoworkcli.workspace_member.list_workspace_member.add_parser(subparsers)
@@ -23,12 +23,10 @@
     annoworkcli.workspace_member.remove_tag_to_workspace_member.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "workspace_member"
     subcommand_help = "ワークスペースメンバ関係のサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_tag/list_workspace_tag.py` & `annoworkcli-3.7.0/annoworkcli/workspace_tag/list_workspace_tag.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 from annoworkcli.common.cli import OutputFormat, build_annoworkapi
 from annoworkcli.common.utils import print_csv, print_json
 
 logger = logging.getLogger(__name__)
 
 
 class ListWorkspaceTag:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-    def main(self, output: Path, output_format: OutputFormat):
+    def main(self, output: Path, output_format: OutputFormat):  # noqa: ANN201
         workspace_tags = self.annowork_service.api.get_workspace_tags(self.workspace_id)
 
         if len(workspace_tags) == 0:
-            logger.warning(f"ワークスペースタグ情報は0件なので、出力しません。")
+            logger.warning("ワークスペースタグ情報は0件なので、出力しません。")
             return
 
         logger.debug(f"{len(workspace_tags)} 件のタグ一覧を出力します。")
 
         if output_format == OutputFormat.JSON:
             print_json(workspace_tags, is_pretty=True, output=output)
         else:
@@ -37,22 +37,22 @@
                 "workspace_tag_name",
             ]
             remaining_columns = list(set(df.columns) - set(required_columns))
             columns = required_columns + remaining_columns
             print_csv(df[columns], output=output)
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     ListWorkspaceTag(annowork_service=annowork_service, workspace_id=args.workspace_id).main(
         output=args.output, output_format=OutputFormat(args.format)
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -71,12 +71,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "list"
     subcommand_help = "ワークスペースタグの一覧を出力します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_tag/put_workspace_tag.py` & `annoworkcli-3.7.0/annoworkcli/workspace_tag/put_workspace_tag.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,43 +9,41 @@
 import annoworkcli
 from annoworkcli.common.cli import build_annoworkapi
 
 logger = logging.getLogger(__name__)
 
 
 class PutWorkspaceTag:
-    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):
+    def __init__(self, annowork_service: AnnoworkResource, workspace_id: str):  # noqa: ANN204
         self.annowork_service = annowork_service
         self.workspace_id = workspace_id
 
-    def main(self, workspace_tag_name: str, workspace_tag_id: Optional[str]):
+    def main(self, workspace_tag_name: str, workspace_tag_id: Optional[str]):  # noqa: ANN201
         workspace_tags = self.annowork_service.api.get_workspace_tags(self.workspace_id)
 
         if workspace_tag_id is None:
             workspace_tag_id = str(uuid.uuid4())
 
         old_workspace_tag = first_true(workspace_tags, pred=lambda e: e["workspace_tag_id"] == workspace_tag_id)
         request_body = {"workspace_tag_name": workspace_tag_name}
         if old_workspace_tag is not None:
             request_body["last_updated_datetime"] = old_workspace_tag["updated_datetime"]
 
-        content = self.annowork_service.api.put_workspace_tag(
-            self.workspace_id, workspace_tag_id, request_body=request_body
-        )
+        content = self.annowork_service.api.put_workspace_tag(self.workspace_id, workspace_tag_id, request_body=request_body)
         logger.debug(f"{workspace_tag_name=} を登録しました。{content=}")
 
 
-def main(args):
+def main(args):  # noqa: ANN001, ANN201
     annowork_service = build_annoworkapi(args)
     PutWorkspaceTag(annowork_service=annowork_service, workspace_id=args.workspace_id).main(
         workspace_tag_name=args.workspace_tag_name, workspace_tag_id=args.workspace_tag_id
     )
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     parser.add_argument(
         "-w",
         "--workspace_id",
         type=str,
         required=True,
         help="対象のワークスペースID",
     )
@@ -68,12 +66,10 @@
     parser.set_defaults(subcommand_func=main)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "put"
     subcommand_help = "ワークスペースタグを作成または更新します。"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/annoworkcli/workspace_tag/subcommand.py` & `annoworkcli-3.7.0/annoworkcli/workspace_tag/subcommand.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,24 +2,22 @@
 from typing import Optional
 
 import annoworkcli
 import annoworkcli.workspace_tag.list_workspace_tag
 import annoworkcli.workspace_tag.put_workspace_tag
 
 
-def parse_args(parser: argparse.ArgumentParser):
+def parse_args(parser: argparse.ArgumentParser):  # noqa: ANN201
     subparsers = parser.add_subparsers(dest="subcommand_name")
 
     # サブコマンドの定義
     annoworkcli.workspace_tag.list_workspace_tag.add_parser(subparsers)
     annoworkcli.workspace_tag.put_workspace_tag.add_parser(subparsers)
 
 
 def add_parser(subparsers: Optional[argparse._SubParsersAction] = None) -> argparse.ArgumentParser:
     subcommand_name = "workspace_tag"
     subcommand_help = "ワークスペースタグ関係のサブコマンド"
 
-    parser = annoworkcli.common.cli.add_parser(
-        subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False
-    )
+    parser = annoworkcli.common.cli.add_parser(subparsers, subcommand_name, subcommand_help, description=subcommand_help, is_subcommand=False)
     parse_args(parser)
     return parser
```

### Comparing `annoworkcli-3.6.2/PKG-INFO` & `annoworkcli-3.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: annoworkcli
-Version: 3.6.2
+Version: 3.7.0
 Summary: AnnoworkのCLI(Command Line Interface)
 Home-page: https://github.com/kurusugawa-computer/annowork-cli
 License: MIT
 Keywords: annowork,cli
 Author: Kurusugawa Computer Inc.
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
```

