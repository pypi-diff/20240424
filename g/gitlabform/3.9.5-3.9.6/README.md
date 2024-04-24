# Comparing `tmp/gitlabform-3.9.5.tar.gz` & `tmp/gitlabform-3.9.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gitlabform-3.9.5.tar", last modified: Fri Apr 19 16:07:33 2024, max compression
+gzip compressed data, was "gitlabform-3.9.6.tar", last modified: Wed Apr 24 09:39:20 2024, max compression
```

## Comparing `gitlabform-3.9.5.tar` & `gitlabform-3.9.6.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-19 16:07:30.000000 gitlabform-3.9.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-19 16:07:33.539098 gitlabform-3.9.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-19 16:07:30.000000 gitlabform-3.9.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.519098 gitlabform-3.9.5/gitlabform/
--rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.523098 gitlabform-3.9.5/gitlabform/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/configuration/transform.py
--rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/gitlab/
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/branches.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/commits.py
--rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/group_badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/group_ldap_links.py
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/group_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/integrations.py
--rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/merge_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/pipelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_badges.py
--rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_deploy_keys.py
--rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/project_protected_environments.py
--rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/python_gitlab.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/repositories.py
--rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/resource_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/gitlab/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/lists/
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/lists/projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/output.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/processors/
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/defining_keys.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.527098 gitlabform-3.9.5/gitlabform/processors/group/
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_ldap_links_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_members_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/group/group_variables_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/multiple_entities_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/gitlabform/processors/project/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/badges_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/branches_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/deploy_keys_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/files_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/hooks_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/integrations_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/members_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approval_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approvals.py
--rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/project_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/project_push_rules_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/project_settings_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/resource_groups_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     6815 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/schedules_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/tags_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/project/variables_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/gitlabform/processors/shared/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/shared/protected_environments_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/single_entity_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/gitlabform/processors/util/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/decorators.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/processors/util/difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-19 16:07:30.000000 gitlabform-3.9.5/gitlabform/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/gitlabform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-19 16:07:33.000000 gitlabform-3.9.5/gitlabform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-19 16:07:33.543098 gitlabform-3.9.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-19 16:07:30.000000 gitlabform-3.9.5/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.531098 gitlabform-3.9.5/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.535098 gitlabform-3.9.5/tests/acceptance/standard/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2738 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_archive_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5971 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3293 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_branches.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     8047 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys_all_projects.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10859 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files_all.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1951 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files_protected.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3059 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_files_templates.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4136 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_badges.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4129 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_members_case_insensitive.py
--rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_members_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     9639 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_members_users.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_settings.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_group_variables.py
--rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_inheritance_break.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    10353 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_integrations.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2324 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_members.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_members_add_group.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2253 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_members_enforce.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_project_group_members_case_insensitive.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_project_members_case_insensitve.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_project_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_resource_groups.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     2834 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_running.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    14216 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_schedules.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_tags.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      871 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_token_from_config.py
--rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_transfer_project.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/acceptance/standard/test_variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/tests/unit/configuration/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3042 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_case_sensitivity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_projects_and_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_skip_groups_skip_projects.py
--rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_subgroups.py
--rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/configuration/test_yaml_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:33.539098 gitlabform-3.9.5/tests/unit/processors/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/test_abstract_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/test_branch_protector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/processors/test_difference_logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/test_access_levels.py
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/test_non_empty_configs_provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-19 16:07:30.000000 gitlabform-3.9.5/tests/unit/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.742213 gitlabform-3.9.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-04-24 09:39:17.000000 gitlabform-3.9.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-24 09:39:20.742213 gitlabform-3.9.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-24 09:39:17.000000 gitlabform-3.9.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.722213 gitlabform-3.9.6/gitlabform/
+-rw-r--r--   0 runner    (1001) docker     (127)    23904 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.722213 gitlabform-3.9.6/gitlabform/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)      391 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/configuration/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12541 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/configuration/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4705 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/configuration/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2760 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/configuration/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15186 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/configuration/transform.py
+-rw-r--r--   0 runner    (1001) docker     (127)      277 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.726213 gitlabform-3.9.6/gitlabform/gitlab/
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3624 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/branches.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/commits.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11515 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1354 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/group_badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/group_ldap_links.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/integrations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2299 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1899 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/merge_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/pipelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/project_badges.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4539 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/project_deploy_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4119 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/project_merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/project_protected_environments.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8115 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/python_gitlab.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/repositories.py
+-rw-r--r--   0 runner    (1001) docker     (127)      766 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/resource_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      613 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1825 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/gitlab/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.726213 gitlabform-3.9.6/gitlabform/lists/
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/lists/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3881 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/lists/filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2571 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/lists/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9532 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/lists/projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1949 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/output.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.730213 gitlabform-3.9.6/gitlabform/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8410 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3958 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/defining_keys.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.730213 gitlabform-3.9.6/gitlabform/processors/group/
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/group/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/group/group_badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/group/group_ldap_links_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11138 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/group/group_members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/group/group_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      684 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/group/group_variables_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8955 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/multiple_entities_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.734213 gitlabform-3.9.6/gitlabform/processors/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      716 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/badges_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/branches_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      814 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/deploy_keys_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11944 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/files_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2885 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/hooks_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/integrations_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7570 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/members_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/merge_requests_approval_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/merge_requests_approvals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3669 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/project_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/project_push_rules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/project_settings_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1979 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/resource_groups_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/schedules_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/tags_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/project/variables_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.734213 gitlabform-3.9.6/gitlabform/processors/shared/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/shared/protected_environments_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/single_entity_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.734213 gitlabform-3.9.6/gitlabform/processors/util/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14003 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/util/branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1277 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/util/decorators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/processors/util/difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-24 09:39:17.000000 gitlabform-3.9.6/gitlabform/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.742213 gitlabform-3.9.6/gitlabform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-04-24 09:39:20.000000 gitlabform-3.9.6/gitlabform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5603 2024-04-24 09:39:20.000000 gitlabform-3.9.6/gitlabform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:39:20.000000 gitlabform-3.9.6/gitlabform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-24 09:39:20.000000 gitlabform-3.9.6/gitlabform.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-24 09:39:20.000000 gitlabform-3.9.6/gitlabform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 09:39:20.000000 gitlabform-3.9.6/gitlabform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-04-24 09:39:20.746213 gitlabform-3.9.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-24 09:39:17.000000 gitlabform-3.9.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.734213 gitlabform-3.9.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.734213 gitlabform-3.9.6/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (127)     8309 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11532 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.738213 gitlabform-3.9.6/tests/acceptance/standard/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2738 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_archive_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5971 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3293 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_branches.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8047 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_deploy_keys.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1224 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_deploy_keys_all_projects.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10859 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_files.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1434 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_files_all.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1951 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_files_protected.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3059 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_files_templates.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4136 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_group_badges.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4129 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_group_members_case_insensitive.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8633 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_group_members_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     9639 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_group_members_users.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      882 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_group_settings.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5622 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_group_variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11104 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_inheritance_break.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    10353 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_integrations.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2324 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_members.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2071 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_members_add_group.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2253 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_members_enforce.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2205 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_project_group_members_case_insensitive.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1391 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_project_members_case_insensitve.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      544 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_project_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1300 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_resource_groups.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2834 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_running.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    14216 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_schedules.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5433 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_tags.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      871 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_token_from_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16893 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_transfer_project.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5559 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/acceptance/standard/test_variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.738213 gitlabform-3.9.6/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.742213 gitlabform-3.9.6/tests/unit/configuration/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3042 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_case_sensitivity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_inheritance_break_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4306 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_inheritance_break_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4291 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_inheritance_break_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3902 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_projects_and_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2575 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_skip_groups_skip_projects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3614 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_subgroups.py
+-rw-r--r--   0 runner    (1001) docker     (127)      589 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/configuration/test_yaml_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:20.742213 gitlabform-3.9.6/tests/unit/processors/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/processors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/processors/test_abstract_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      875 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/processors/test_branch_protector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1042 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/processors/test_difference_logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      687 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/test_access_levels.py
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/test_non_empty_configs_provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-24 09:39:17.000000 gitlabform-3.9.6/tests/unit/test_utils.py
```

### Comparing `gitlabform-3.9.5/LICENSE` & `gitlabform-3.9.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/PKG-INFO` & `gitlabform-3.9.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.9.5
+Version: 3.9.6
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.9.5 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.9.6 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `gitlabform-3.9.5/README.md` & `gitlabform-3.9.6/README.md`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/__init__.py` & `gitlabform-3.9.6/gitlabform/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/configuration/common.py` & `gitlabform-3.9.6/gitlabform/configuration/common.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/configuration/core.py` & `gitlabform-3.9.6/gitlabform/configuration/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/configuration/groups.py` & `gitlabform-3.9.6/gitlabform/configuration/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/configuration/projects.py` & `gitlabform-3.9.6/gitlabform/configuration/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/configuration/transform.py` & `gitlabform-3.9.6/gitlabform/configuration/transform.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/__init__.py` & `gitlabform-3.9.6/gitlabform/gitlab/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/branches.py` & `gitlabform-3.9.6/gitlabform/gitlab/branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/commits.py` & `gitlabform-3.9.6/gitlabform/gitlab/commits.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/core.py` & `gitlabform-3.9.6/gitlabform/gitlab/core.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/group_badges.py` & `gitlabform-3.9.6/gitlabform/gitlab/group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/group_ldap_links.py` & `gitlabform-3.9.6/gitlabform/gitlab/group_ldap_links.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/group_variables.py` & `gitlabform-3.9.6/gitlabform/gitlab/group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/groups.py` & `gitlabform-3.9.6/gitlabform/gitlab/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/integrations.py` & `gitlabform-3.9.6/gitlabform/gitlab/integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/members.py` & `gitlabform-3.9.6/gitlabform/gitlab/members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/merge_requests.py` & `gitlabform-3.9.6/gitlabform/gitlab/merge_requests.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/pipelines.py` & `gitlabform-3.9.6/gitlabform/gitlab/pipelines.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/project_badges.py` & `gitlabform-3.9.6/gitlabform/gitlab/project_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/project_deploy_keys.py` & `gitlabform-3.9.6/gitlabform/gitlab/project_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/project_merge_requests_approvals.py` & `gitlabform-3.9.6/gitlabform/gitlab/project_merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/project_protected_environments.py` & `gitlabform-3.9.6/gitlabform/gitlab/project_protected_environments.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/projects.py` & `gitlabform-3.9.6/gitlabform/gitlab/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/python_gitlab.py` & `gitlabform-3.9.6/gitlabform/gitlab/python_gitlab.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/repositories.py` & `gitlabform-3.9.6/gitlabform/gitlab/repositories.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/resource_groups.py` & `gitlabform-3.9.6/gitlabform/gitlab/resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/users.py` & `gitlabform-3.9.6/gitlabform/gitlab/users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/gitlab/variables.py` & `gitlabform-3.9.6/gitlabform/gitlab/variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/lists/__init__.py` & `gitlabform-3.9.6/gitlabform/lists/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/lists/filter.py` & `gitlabform-3.9.6/gitlabform/lists/filter.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/lists/groups.py` & `gitlabform-3.9.6/gitlabform/lists/groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/lists/projects.py` & `gitlabform-3.9.6/gitlabform/lists/projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/output.py` & `gitlabform-3.9.6/gitlabform/output.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/__init__.py` & `gitlabform-3.9.6/gitlabform/processors/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/abstract_processor.py` & `gitlabform-3.9.6/gitlabform/processors/abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/defining_keys.py` & `gitlabform-3.9.6/gitlabform/processors/defining_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/group/__init__.py` & `gitlabform-3.9.6/gitlabform/processors/group/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/group/group_badges_processor.py` & `gitlabform-3.9.6/gitlabform/processors/group/group_badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/group/group_ldap_links_processor.py` & `gitlabform-3.9.6/gitlabform/processors/group/group_ldap_links_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/group/group_members_processor.py` & `gitlabform-3.9.6/gitlabform/processors/group/group_members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/group/group_variables_processor.py` & `gitlabform-3.9.6/gitlabform/processors/group/group_variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/multiple_entities_processor.py` & `gitlabform-3.9.6/gitlabform/processors/multiple_entities_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/__init__.py` & `gitlabform-3.9.6/gitlabform/processors/project/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/badges_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/badges_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/branches_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/branches_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/deploy_keys_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/deploy_keys_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/files_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/files_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/hooks_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/hooks_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/integrations_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/integrations_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/members_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/members_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approval_rules.py` & `gitlabform-3.9.6/gitlabform/processors/project/merge_requests_approval_rules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/merge_requests_approvals.py` & `gitlabform-3.9.6/gitlabform/processors/project/merge_requests_approvals.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/project_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/project_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/resource_groups_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/resource_groups_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/schedules_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/schedules_processor.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 
         # Remove 'enforce' key from the config so that it's not treated as a "schedule"
         if enforce_schedules:
             configured_schedules.pop("enforce")
 
         project: Project = self.gl.projects.get(project_and_group)
         existing_schedules: List[RESTObject] | RESTObjectList = (
-            project.pipelineschedules.list()
+            project.pipelineschedules.list(get_all=True)
         )
 
         schedule_ids_by_description: Dict = self._group_schedule_ids_by_description(
             existing_schedules
         )
 
         for schedule_description in sorted(configured_schedules):
```

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/tags_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/tags_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/project/variables_processor.py` & `gitlabform-3.9.6/gitlabform/processors/project/variables_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/shared/protected_environments_processor.py` & `gitlabform-3.9.6/gitlabform/processors/shared/protected_environments_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/single_entity_processor.py` & `gitlabform-3.9.6/gitlabform/processors/single_entity_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/util/branch_protector.py` & `gitlabform-3.9.6/gitlabform/processors/util/branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/util/decorators.py` & `gitlabform-3.9.6/gitlabform/processors/util/decorators.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform/processors/util/difference_logger.py` & `gitlabform-3.9.6/gitlabform/processors/util/difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/gitlabform.egg-info/PKG-INFO` & `gitlabform-3.9.6/gitlabform.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gitlabform
-Version: 3.9.5
+Version: 3.9.6
 Summary: 🏗 Specialized configuration as a code tool for GitLab projects, groups and more using hierarchical configuration written in YAML
 Home-page: https://gitlabform.github.io/gitlabform
 Author: Greg Dubicki and Contributors
 Keywords: cli,yaml,gitlab,configuration-as-code
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: gitlabform Version: 3.9.5 Summary: ð Specialized
+Metadata-Version: 2.1 Name: gitlabform Version: 3.9.6 Summary: ð Specialized
 configuration as a code tool for GitLab projects, groups and more using
 hierarchical configuration written in YAML Home-page: https://
 gitlabform.github.io/gitlabform Author: Greg Dubicki and Contributors Keywords:
 cli,yaml,gitlab,configuration-as-code Classifier: Programming Language ::
 Python :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.12 Classifier:
```

### Comparing `gitlabform-3.9.5/gitlabform.egg-info/SOURCES.txt` & `gitlabform-3.9.6/gitlabform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/setup.py` & `gitlabform-3.9.6/setup.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/__init__.py` & `gitlabform-3.9.6/tests/acceptance/__init__.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/conftest.py` & `gitlabform-3.9.6/tests/acceptance/conftest.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_archive_project.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_archive_project.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_badges.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_branches.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_branches.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_deploy_keys.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_deploy_keys_all_projects.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_deploy_keys_all_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_files.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_files.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_files_all.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_files_all.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_files_protected.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_files_protected.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_files_templates.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_files_templates.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_group_badges.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_group_badges.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_group_members_case_insensitive.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_group_members_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_group_members_groups.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_group_members_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_group_members_users.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_group_members_users.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_group_settings.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_group_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_group_variables.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_group_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_hooks.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_hooks.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_inheritance_break.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_inheritance_break.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_integrations.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_integrations.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_members.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_members.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_members_add_group.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_members_add_group.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_members_enforce.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_members_enforce.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_project_group_members_case_insensitive.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_project_group_members_case_insensitive.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_project_members_case_insensitve.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_project_members_case_insensitve.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_project_settings.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_project_settings.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_resource_groups.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_resource_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_running.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_running.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_schedules.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_schedules.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_tags.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_tags.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_token_from_config.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_token_from_config.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_transfer_project.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_transfer_project.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/acceptance/standard/test_variables.py` & `gitlabform-3.9.6/tests/acceptance/standard/test_variables.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_case_sensitivity.py` & `gitlabform-3.9.6/tests/unit/configuration/test_case_sensitivity.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_projects_and_groups.py` & `gitlabform-3.9.6/tests/unit/configuration/test_inheritance_break_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_subgroups.py` & `gitlabform-3.9.6/tests/unit/configuration/test_inheritance_break_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_inheritance_break_validation.py` & `gitlabform-3.9.6/tests/unit/configuration/test_inheritance_break_validation.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_projects_and_groups.py` & `gitlabform-3.9.6/tests/unit/configuration/test_projects_and_groups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_skip_groups_skip_projects.py` & `gitlabform-3.9.6/tests/unit/configuration/test_skip_groups_skip_projects.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_subgroups.py` & `gitlabform-3.9.6/tests/unit/configuration/test_subgroups.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/configuration/test_yaml_version.py` & `gitlabform-3.9.6/tests/unit/configuration/test_yaml_version.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/processors/test_abstract_processor.py` & `gitlabform-3.9.6/tests/unit/processors/test_abstract_processor.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/processors/test_branch_protector.py` & `gitlabform-3.9.6/tests/unit/processors/test_branch_protector.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/processors/test_difference_logger.py` & `gitlabform-3.9.6/tests/unit/processors/test_difference_logger.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/test_access_levels.py` & `gitlabform-3.9.6/tests/unit/test_access_levels.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/test_non_empty_configs_provider.py` & `gitlabform-3.9.6/tests/unit/test_non_empty_configs_provider.py`

 * *Files identical despite different names*

### Comparing `gitlabform-3.9.5/tests/unit/test_utils.py` & `gitlabform-3.9.6/tests/unit/test_utils.py`

 * *Files identical despite different names*

