# Comparing `tmp/ckanext_files-0.2.5.tar.gz` & `tmp/ckanext_files-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ckanext_files-0.2.5.tar", last modified: Sat Apr 20 10:44:36 2024, max compression
+gzip compressed data, was "ckanext_files-0.2.6.tar", last modified: Wed Apr 24 11:53:12 2024, max compression
```

## Comparing `ckanext_files-0.2.5.tar` & `ckanext_files-0.2.6.tar`

### file list

```diff
@@ -1,107 +1,108 @@
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.742362 ckanext_files-0.2.5/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/LICENSE
--rw-r--r--   0 sergey    (1000) sergey    (1000)      204 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/MANIFEST.in
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-20 10:44:36.742362 ckanext_files-0.2.5/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14070 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/README.md
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.712363 ckanext_files-0.2.5/ckanext/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/ckanext/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.712363 ckanext_files-0.2.5/ckanext/file_manager/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext_files-0.2.5/ckanext/file_manager/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/file_manager/collection.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/file_manager/plugin.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/file_manager/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.715696 ckanext_files-0.2.5/ckanext/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/ckanext/files/__init__.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.715696 ckanext_files-0.2.5/ckanext/files/assets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2024-04-09 01:54:26.000000 ckanext_files-0.2.5/ckanext/files/assets/resource.config
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.719029 ckanext_files-0.2.5/ckanext/files/assets/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     8237 2024-04-15 14:21:37.000000 ckanext_files-0.2.5/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    37143 2024-04-15 14:21:37.000000 ckanext_files-0.2.5/ckanext/files/assets/scripts/files--modules.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.5/ckanext/files/assets/scripts/files--shared-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)    44969 2024-04-15 14:21:37.000000 ckanext_files-0.2.5/ckanext/files/assets/scripts/files--shared.js
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.719029 ckanext_files-0.2.5/ckanext/files/assets/styles/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      197 2024-04-09 02:46:04.000000 ckanext_files-0.2.5/ckanext/files/assets/styles/files--style.css
--rw-r--r--   0 sergey    (1000) sergey    (1000)      360 2024-04-09 01:54:34.000000 ckanext_files-0.2.5/ckanext/files/assets/webassets.yml
--rw-r--r--   0 sergey    (1000) sergey    (1000)    14339 2024-04-15 14:22:47.000000 ckanext_files-0.2.5/ckanext/files/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/cli.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1355 2024-04-07 14:32:45.000000 ckanext_files-0.2.5/ckanext/files/command.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4998 2024-04-20 10:44:26.000000 ckanext_files-0.2.5/ckanext/files/exceptions.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/helpers.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/interfaces.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.719029 ckanext_files-0.2.5/ckanext/files/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/ckanext/files/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     9785 2024-04-20 10:44:26.000000 ckanext_files-0.2.5/ckanext/files/logic/action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3907 2024-04-07 14:32:45.000000 ckanext_files-0.2.5/ckanext/files/logic/auth.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2875 2024-04-07 16:20:32.000000 ckanext_files-0.2.5/ckanext/files/logic/schema.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1098 2024-04-15 14:22:08.000000 ckanext_files-0.2.5/ckanext/files/logic/validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.709029 ckanext_files-0.2.5/ckanext/files/migration/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.722363 ckanext_files-0.2.5/ckanext/files/migration/files/
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/ckanext/files/migration/files/alembic.ini
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/migration/files/env.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/ckanext/files/migration/files/script.py.mako
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.725696 ckanext_files-0.2.5/ckanext/files/migration/files/versions/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-07 14:32:45.000000 ckanext_files-0.2.5/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.725696 ckanext_files-0.2.5/ckanext/files/model/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/model/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/model/base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2472 2024-04-07 14:32:45.000000 ckanext_files-0.2.5/ckanext/files/model/file.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/model/owner.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/plugin.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.709029 ckanext_files-0.2.5/ckanext/files/public/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.709029 ckanext_files-0.2.5/ckanext/files/public/ckanext-files/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.729029 ckanext_files-0.2.5/ckanext/files/public/ckanext-files/scripts/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.5/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js
--rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/shared.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.729029 ckanext_files-0.2.5/ckanext/files/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7410 2024-04-09 11:03:43.000000 ckanext_files-0.2.5/ckanext/files/storage/fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11028 2024-04-20 10:44:26.000000 ckanext_files-0.2.5/ckanext/files/storage/google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4719 2024-04-15 14:21:38.000000 ckanext_files-0.2.5/ckanext/files/storage/redis.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.729029 ckanext_files-0.2.5/ckanext/files/templates/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.709029 ckanext_files-0.2.5/ckanext/files/templates/files/
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.732362 ckanext_files-0.2.5/ckanext/files/templates/files/snippets/
--rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/templates/files/snippets/_asset.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/templates/files/snippets/_resource.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5167 2024-04-09 03:20:53.000000 ckanext_files-0.2.5/ckanext/files/templates/files/snippets/file_table.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2451 2024-04-09 05:48:11.000000 ckanext_files-0.2.5/ckanext/files/templates/files/snippets/uploader_v1.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.732362 ckanext_files-0.2.5/ckanext/files/templates/files/user/
--rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/templates/files/user/delete.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      847 2024-04-09 05:48:21.000000 ckanext_files-0.2.5/ckanext/files/templates/files/user/index.html
--rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/templates/page.html
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.735696 ckanext_files-0.2.5/ckanext/files/tests/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/ckanext/files/tests/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3442 2024-04-07 16:20:32.000000 ckanext_files-0.2.5/ckanext/files/tests/conftest.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.735696 ckanext_files-0.2.5/ckanext/files/tests/logic/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/ckanext/files/tests/logic/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/logic/test_action.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/logic/test_validators.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.739029 ckanext_files-0.2.5/ckanext/files/tests/storage/
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/storage/__init__.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/storage/test_fs.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    10311 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/storage/test_google_cloud.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/storage/test_redis.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)    11805 2024-04-09 11:08:13.000000 ckanext_files-0.2.5/ckanext/files/tests/test_base.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/test_config.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/tests/test_utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/ckanext/files/types.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     5490 2024-04-15 14:21:38.000000 ckanext_files-0.2.5/ckanext/files/utils.py
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4522 2024-04-20 10:44:26.000000 ckanext_files-0.2.5/ckanext/files/views.py
-drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-20 10:44:36.739029 ckanext_files-0.2.5/ckanext_files.egg-info/
--rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-20 10:44:36.000000 ckanext_files-0.2.5/ckanext_files.egg-info/PKG-INFO
--rw-r--r--   0 sergey    (1000) sergey    (1000)     3113 2024-04-20 10:44:36.000000 ckanext_files-0.2.5/ckanext_files.egg-info/SOURCES.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-20 10:44:36.000000 ckanext_files-0.2.5/ckanext_files.egg-info/dependency_links.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      241 2024-04-20 10:44:36.000000 ckanext_files-0.2.5/ckanext_files.egg-info/entry_points.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-20 10:44:36.000000 ckanext_files-0.2.5/ckanext_files.egg-info/namespace_packages.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-04-20 10:44:36.000000 ckanext_files-0.2.5/ckanext_files.egg-info/requires.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-20 10:44:36.000000 ckanext_files-0.2.5/ckanext_files.egg-info/top_level.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-04-01 12:19:47.000000 ckanext_files-0.2.5/pyproject.toml
--rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/requirements.txt
--rw-r--r--   0 sergey    (1000) sergey    (1000)     2000 2024-04-20 10:44:36.742362 ckanext_files-0.2.5/setup.cfg
--rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext_files-0.2.5/setup.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.384065 ckanext_files-0.2.6/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    34517 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/LICENSE
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-24 11:51:24.000000 ckanext_files-0.2.6/MANIFEST.in
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-24 11:53:12.384065 ckanext_files-0.2.6/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14070 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/README.md
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.357399 ckanext_files-0.2.6/ckanext/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      221 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.360732 ckanext_files-0.2.6/ckanext/file_manager/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-02-04 13:46:59.000000 ckanext_files-0.2.6/ckanext/file_manager/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4162 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/file_manager/collection.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1423 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/file_manager/plugin.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3519 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/file_manager/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/__init__.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/assets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      187 2024-04-09 01:54:26.000000 ckanext_files-0.2.6/ckanext/files/assets/resource.config
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/assets/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     8237 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    37143 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--modules.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    44969 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared.js
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.367399 ckanext_files-0.2.6/ckanext/files/assets/styles/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      197 2024-04-09 02:46:04.000000 ckanext_files-0.2.6/ckanext/files/assets/styles/files--style.css
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      360 2024-04-09 01:54:34.000000 ckanext_files-0.2.6/ckanext/files/assets/webassets.yml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    14339 2024-04-15 14:22:47.000000 ckanext_files-0.2.6/ckanext/files/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      840 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/cli.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1355 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/command.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1245 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      373 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/config_declaration.yaml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4998 2024-04-20 10:44:26.000000 ckanext_files-0.2.6/ckanext/files/exceptions.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1031 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/helpers.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      564 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/interfaces.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.370732 ckanext_files-0.2.6/ckanext/files/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     9785 2024-04-22 16:49:03.000000 ckanext_files-0.2.6/ckanext/files/logic/action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3907 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/logic/auth.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2875 2024-04-07 16:20:32.000000 ckanext_files-0.2.6/ckanext/files/logic/schema.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1098 2024-04-15 14:22:08.000000 ckanext_files-0.2.6/ckanext/files/logic/validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.354066 ckanext_files-0.2.6/ckanext/files/migration/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.370732 ckanext_files-0.2.6/ckanext/files/migration/files/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1774 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/migration/files/alembic.ini
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2228 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/env.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      494 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/migration/files/script.py.mako
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.374065 ckanext_files-0.2.6/ckanext/files/migration/files/versions/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      595 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      921 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      849 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1019 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      484 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/76fdef67f479_add_access_column_to_owner_table.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      883 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.374065 ckanext_files-0.2.6/ckanext/files/model/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       77 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/model/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      211 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/model/base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2472 2024-04-07 14:32:45.000000 ckanext_files-0.2.6/ckanext/files/model/file.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1547 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/model/owner.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4614 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/plugin.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.354066 ckanext_files-0.2.6/ckanext/files/public/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.354066 ckanext_files-0.2.6/ckanext/files/public/ckanext-files/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.374065 ckanext_files-0.2.6/ckanext/files/public/ckanext-files/scripts/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      797 2024-04-15 14:21:37.000000 ckanext_files-0.2.6/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      363 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/shared.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      312 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7410 2024-04-09 11:03:43.000000 ckanext_files-0.2.6/ckanext/files/storage/fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11028 2024-04-20 10:44:26.000000 ckanext_files-0.2.6/ckanext/files/storage/google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4719 2024-04-15 14:21:38.000000 ckanext_files-0.2.6/ckanext/files/storage/redis.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/templates/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.357399 ckanext_files-0.2.6/ckanext/files/templates/files/
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       59 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/_asset.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)       29 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/_resource.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5167 2024-04-09 03:20:53.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/file_table.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2451 2024-04-09 05:48:11.000000 ckanext_files-0.2.6/ckanext/files/templates/files/snippets/uploader_v1.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.377399 ckanext_files-0.2.6/ckanext/files/templates/files/user/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      550 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/files/user/delete.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      847 2024-04-22 16:49:06.000000 ckanext_files-0.2.6/ckanext/files/templates/files/user/index.html
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      274 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/templates/page.html
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.380732 ckanext_files-0.2.6/ckanext/files/tests/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/tests/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3442 2024-04-07 16:20:32.000000 ckanext_files-0.2.6/ckanext/files/tests/conftest.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.380732 ckanext_files-0.2.6/ckanext/files/tests/logic/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/ckanext/files/tests/logic/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1506 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/logic/test_action.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1725 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/logic/test_validators.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.380732 ckanext_files-0.2.6/ckanext/files/tests/storage/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/__init__.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     7502 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/test_fs.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    10311 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/test_google_cloud.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3814 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/storage/test_redis.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    11805 2024-04-09 11:08:13.000000 ckanext_files-0.2.6/ckanext/files/tests/test_base.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3061 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/test_config.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     6777 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/tests/test_utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     1128 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/ckanext/files/types.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     5490 2024-04-15 14:21:38.000000 ckanext_files-0.2.6/ckanext/files/utils.py
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4522 2024-04-20 10:44:26.000000 ckanext_files-0.2.6/ckanext/files/views.py
+drwxr-xr-x   0 sergey    (1000) sergey    (1000)        0 2024-04-24 11:53:12.384065 ckanext_files-0.2.6/ckanext_files.egg-info/
+-rw-r--r--   0 sergey    (1000) sergey    (1000)    15608 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/PKG-INFO
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     3151 2024-04-24 11:53:12.000000 ckanext_files-0.2.6/ckanext_files.egg-info/SOURCES.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        1 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/dependency_links.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      241 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/entry_points.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/namespace_packages.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      359 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/requires.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        8 2024-04-24 11:53:11.000000 ckanext_files-0.2.6/ckanext_files.egg-info/top_level.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     4286 2024-04-01 12:19:47.000000 ckanext_files-0.2.6/pyproject.toml
+-rw-r--r--   0 sergey    (1000) sergey    (1000)        0 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/requirements.txt
+-rw-r--r--   0 sergey    (1000) sergey    (1000)     2000 2024-04-24 11:53:12.387399 ckanext_files-0.2.6/setup.cfg
+-rw-r--r--   0 sergey    (1000) sergey    (1000)      262 2024-01-28 01:59:52.000000 ckanext_files-0.2.6/setup.py
```

### Comparing `ckanext_files-0.2.5/LICENSE` & `ckanext_files-0.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/PKG-INFO` & `ckanext_files-0.2.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext_files-0.2.5/README.md` & `ckanext_files-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/file_manager/collection.py` & `ckanext_files-0.2.6/ckanext/file_manager/collection.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/file_manager/plugin.py` & `ckanext_files-0.2.6/ckanext/file_manager/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/file_manager/views.py` & `ckanext_files-0.2.6/ckanext/file_manager/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js` & `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--google-cloud-storage-uploader.js`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/assets/scripts/files--modules.js` & `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--modules.js`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/assets/scripts/files--shared-uploader.js` & `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared-uploader.js`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/assets/scripts/files--shared.js` & `ckanext_files-0.2.6/ckanext/files/assets/scripts/files--shared.js`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/base.py` & `ckanext_files-0.2.6/ckanext/files/base.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/cli.py` & `ckanext_files-0.2.6/ckanext/files/cli.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/command.py` & `ckanext_files-0.2.6/ckanext/files/command.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/config.py` & `ckanext_files-0.2.6/ckanext/files/config.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/exceptions.py` & `ckanext_files-0.2.6/ckanext/files/exceptions.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/helpers.py` & `ckanext_files-0.2.6/ckanext/files/helpers.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/interfaces.py` & `ckanext_files-0.2.6/ckanext/files/interfaces.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/logic/action.py` & `ckanext_files-0.2.6/ckanext/files/logic/action.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/logic/auth.py` & `ckanext_files-0.2.6/ckanext/files/logic/auth.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/logic/schema.py` & `ckanext_files-0.2.6/ckanext/files/logic/schema.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/logic/validators.py` & `ckanext_files-0.2.6/ckanext/files/logic/validators.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/alembic.ini` & `ckanext_files-0.2.6/ckanext/files/migration/files/alembic.ini`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/env.py` & `ckanext_files-0.2.6/ckanext/files/migration/files/env.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py` & `ckanext_files-0.2.6/ckanext/files/migration/files/versions/2c5f1f90888c_add_file_last_access_field.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py` & `ckanext_files-0.2.6/ckanext/files/migration/files/versions/2fbd30a1b364_create_owner_table.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py` & `ckanext_files-0.2.6/ckanext/files/migration/files/versions/3c69eb68cecd_create_upload_table.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py` & `ckanext_files-0.2.6/ckanext/files/migration/files/versions/5851e09b7ca3_remove_path_rename_kind_add_stats.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py` & `ckanext_files-0.2.6/ckanext/files/migration/files/versions/64ca007bf3eb_merge_upload_and_file_models.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py` & `ckanext_files-0.2.6/ckanext/files/migration/files/versions/cc1a832108c5_create_files_table.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/model/file.py` & `ckanext_files-0.2.6/ckanext/files/model/file.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/model/owner.py` & `ckanext_files-0.2.6/ckanext/files/model/owner.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/plugin.py` & `ckanext_files-0.2.6/ckanext/files/plugin.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js` & `ckanext_files-0.2.6/ckanext/files/public/ckanext-files/scripts/files--shared-uploader.js`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/storage/fs.py` & `ckanext_files-0.2.6/ckanext/files/storage/fs.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/storage/google_cloud.py` & `ckanext_files-0.2.6/ckanext/files/storage/google_cloud.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/storage/redis.py` & `ckanext_files-0.2.6/ckanext/files/storage/redis.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/templates/files/snippets/file_table.html` & `ckanext_files-0.2.6/ckanext/files/templates/files/snippets/file_table.html`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/templates/files/snippets/uploader_v1.html` & `ckanext_files-0.2.6/ckanext/files/templates/files/snippets/uploader_v1.html`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/templates/files/user/delete.html` & `ckanext_files-0.2.6/ckanext/files/templates/files/user/delete.html`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/templates/files/user/index.html` & `ckanext_files-0.2.6/ckanext/files/templates/files/user/index.html`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/conftest.py` & `ckanext_files-0.2.6/ckanext/files/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/logic/test_action.py` & `ckanext_files-0.2.6/ckanext/files/tests/logic/test_action.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/logic/test_validators.py` & `ckanext_files-0.2.6/ckanext/files/tests/logic/test_validators.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/storage/test_fs.py` & `ckanext_files-0.2.6/ckanext/files/tests/storage/test_fs.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/storage/test_google_cloud.py` & `ckanext_files-0.2.6/ckanext/files/tests/storage/test_google_cloud.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/storage/test_redis.py` & `ckanext_files-0.2.6/ckanext/files/tests/storage/test_redis.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/test_base.py` & `ckanext_files-0.2.6/ckanext/files/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/test_config.py` & `ckanext_files-0.2.6/ckanext/files/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/tests/test_utils.py` & `ckanext_files-0.2.6/ckanext/files/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/types.py` & `ckanext_files-0.2.6/ckanext/files/types.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/utils.py` & `ckanext_files-0.2.6/ckanext/files/utils.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext/files/views.py` & `ckanext_files-0.2.6/ckanext/files/views.py`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/ckanext_files.egg-info/PKG-INFO` & `ckanext_files-0.2.6/ckanext_files.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ckanext-files
-Version: 0.2.5
+Version: 0.2.6
 Home-page: https://github.com/DataShades/ckanext-files
 Author: Sergey Motornyuk
 Author-email: sergey.motornyuk@linkdigital.com.au
 License: AGPL
 Keywords: CKAN
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

### Comparing `ckanext_files-0.2.5/ckanext_files.egg-info/SOURCES.txt` & `ckanext_files-0.2.6/ckanext_files.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 ckanext/file_manager/plugin.py
 ckanext/file_manager/views.py
 ckanext/files/__init__.py
 ckanext/files/base.py
 ckanext/files/cli.py
 ckanext/files/command.py
 ckanext/files/config.py
+ckanext/files/config_declaration.yaml
 ckanext/files/exceptions.py
 ckanext/files/helpers.py
 ckanext/files/interfaces.py
 ckanext/files/plugin.py
 ckanext/files/shared.py
 ckanext/files/types.py
 ckanext/files/utils.py
```

### Comparing `ckanext_files-0.2.5/pyproject.toml` & `ckanext_files-0.2.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `ckanext_files-0.2.5/setup.cfg` & `ckanext_files-0.2.6/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ckanext-files
-version = 0.2.5
+version = 0.2.6
 description = 
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/DataShades/ckanext-files
 author = Sergey Motornyuk
 author_email = sergey.motornyuk@linkdigital.com.au
 license = AGPL
```

