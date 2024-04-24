# Comparing `tmp/girder-5.0.0a2.tar.gz` & `tmp/girder-5.0.0a2.dev10.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-5.0.0a2.tar", last modified: Fri Apr 12 16:28:57 2024, max compression
+gzip compressed data, was "girder-5.0.0a2.dev10.tar", last modified: Fri Apr 12 16:12:21 2024, max compression
```

## Comparing `girder-5.0.0a2.tar` & `girder-5.0.0a2.dev10.tar`

### file list

```diff
@@ -1,487 +1,487 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.739801 girder-5.0.0a2/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.631800 girder-5.0.0a2/.circleci/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1098 2024-04-12 16:27:17.000000 girder-5.0.0a2/.circleci/Dockerfile
--rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2024-04-12 16:27:17.000000 girder-5.0.0a2/.circleci/build_plugins.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13158 2024-04-12 16:27:17.000000 girder-5.0.0a2/.circleci/config.yml
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      316 2024-04-12 16:27:17.000000 girder-5.0.0a2/.circleci/generatePyEnvChecksum.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      980 2024-04-12 16:27:17.000000 girder-5.0.0a2/.circleci/publish_npm.sh
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      417 2024-04-12 16:27:17.000000 girder-5.0.0a2/.circleci/publish_pypi.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-04-12 16:27:17.000000 girder-5.0.0a2/.codecov.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-04-12 16:27:17.000000 girder-5.0.0a2/.dockerignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2024-04-12 16:27:17.000000 girder-5.0.0a2/.editorconfig
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-04-12 16:27:17.000000 girder-5.0.0a2/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-04-12 16:27:17.000000 girder-5.0.0a2/.readthedocs.yml
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20024 2024-04-12 16:27:17.000000 girder-5.0.0a2/CHANGELOG.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      729 2024-04-12 16:27:17.000000 girder-5.0.0a2/CMakeLists.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4925 2024-04-12 16:27:17.000000 girder-5.0.0a2/CONTRIBUTING.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2024-04-12 16:27:17.000000 girder-5.0.0a2/Dockerfile
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-12 16:27:17.000000 girder-5.0.0a2/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)      491 2024-04-12 16:27:17.000000 girder-5.0.0a2/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2024-04-12 16:28:57.739801 girder-5.0.0a2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2024-04-12 16:27:17.000000 girder-5.0.0a2/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.623800 girder-5.0.0a2/clients/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.631800 girder-5.0.0a2/clients/python/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-04-12 16:27:17.000000 girder-5.0.0a2/clients/python/README.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.631800 girder-5.0.0a2/clients/python/girder_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-04-12 16:27:17.000000 girder-5.0.0a2/clients/python/girder_client/__init__.py
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-04-12 16:27:17.000000 girder-5.0.0a2/clients/python/girder_client/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-04-12 16:27:17.000000 girder-5.0.0a2/clients/python/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      395 2024-04-12 16:27:17.000000 girder-5.0.0a2/docker-compose.yml
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.639800 girder-5.0.0a2/docs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/admin-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5217 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/api-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/build-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/changelog.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2379 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/conf.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2137 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/configuration.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5131 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/dependencies.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2047 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/deployment.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/dev-installation.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22931 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/developer-cookbook.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/developer-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13030 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15086 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/favicon.ico
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.639800 girder-5.0.0a2/docs/images/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   803025 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/images/dicom-viewer.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5181 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/index.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/license.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36997 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/migration-guide.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/mount.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    38303 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/plugin-development.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21669 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/plugins.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10504 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/python-client.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/requirements-docs.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5707 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/security.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1640 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/sftp.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/user-docs.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2024-04-12 16:27:17.000000 girder-5.0.0a2/docs/user-guide.rst
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.639800 girder-5.0.0a2/girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.643800 girder-5.0.0a2/girder/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4349 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/access.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1341 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/api_docs.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/api_main.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    32888 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/describe.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5216 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/docs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3483 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/filter_logging.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    51167 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7285 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/sftp.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.643800 girder-5.0.0a2/girder/api/v1/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/assetstore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19091 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21532 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/folder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15915 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4577 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/notification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17147 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/resource.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18817 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/system.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2065 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19063 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/api/v1/user.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.647801 girder-5.0.0a2/girder/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      358 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24760 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/cli/mount.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2452 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/cli/serve.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1367 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/cli/sftpd.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1750 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/cli/shell.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5954 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/events.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.647801 girder-5.0.0a2/girder/mail_templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/mail_templates/_footer.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/mail_templates/_header.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      306 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/mail_templates/accountApproval.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/mail_templates/accountApproved.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/mail_templates/emailVerification.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/mail_templates/groupInvite.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/mail_templates/temporaryAccess.mako
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.647801 girder-5.0.0a2/girder/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4825 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/api_key.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/assetstore.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16104 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/collection.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20130 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/file.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    36301 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/folder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15676 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/group.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21461 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/item.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    65727 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/model_base.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8257 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/notification.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/setting.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4697 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22202 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/upload.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24605 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6465 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14634 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/settings.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.651800 girder-5.0.0a2/girder/utility/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6482 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3111 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/_cache.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/_hash_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17371 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/abstract_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    16381 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/acl_mixin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2310 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/assetstore_utilities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/config.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/error.mako
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18688 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/filesystem_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6280 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/mail_utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2752 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/model_importer.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6735 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/path.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4435 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/progress.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    26957 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/s3_assetstore_adapter.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2440 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/search.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3589 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/server.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2946 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/setting_utilities.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6845 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/system.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2857 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/webroot.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8124 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/utility/ziputil.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.651800 girder-5.0.0a2/girder/web/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/.env.development
--rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/.gitignore
--rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/.prettierrc.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2069 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.655800 girder-5.0.0a2/girder/web/dist/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-04-12 16:27:55.000000 girder-5.0.0a2/girder/web/dist/Girder_Favicon.png
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7590 2024-04-12 16:27:55.000000 girder-5.0.0a2/girder/web/dist/Girder_Mark.png
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.663801 girder-5.0.0a2/girder/web/dist/assets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)   127292 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/fontello-00cea317.ttf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    72868 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/fontello-13e61b43.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)   183888 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/fontello-2d6e9725.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)    58716 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/fontello-98c6b1f2.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)   127460 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/fontello-e418b5b2.eot
--rw-r--r--   0 circleci  (1001) circleci  (1002)    20127 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-13634da8.eot
--rw-r--r--   0 circleci  (1001) circleci  (1002)   108738 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-42f60659.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23424 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-a26394f7.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    45404 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-e3950440.ttf
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18028 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-fe185d11.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)   215659 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/index-269c82d1.css
--rw-r--r--   0 circleci  (1001) circleci  (1002)  1984729 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/index-41ef1ab1.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)  5812987 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/index-41ef1ab1.js.map
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35955 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/jsoneditor-icons-25c04e58.svg
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18668 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300-6e8a28a0.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14932 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300-f677ee2d.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13860 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300italic-453e6eb2.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17668 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300italic-5bb07410.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18100 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400-81f0ec27.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14380 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400-9c50a96c.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17440 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400italic-39ec493a.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13780 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400italic-da407a15.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14880 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600-1491de1b.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18696 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600-57c79375.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13852 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600italic-10879c90.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17492 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600italic-bb878389.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15056 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700-74201a4b.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18900 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700-ea20e5db.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17452 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700italic-1e742589.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13880 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700italic-d8505544.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    19072 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800-35eb714d.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15088 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800-75db6959.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800italic-49512fd4.woff2
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17788 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800italic-49b6274b.woff
--rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/index.html
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.667801 girder-5.0.0a2/girder/web/dist/src/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2938 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/src/auth.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.671801 girder-5.0.0a2/girder/web/dist/src/collections/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/collections/ApiKeyCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/collections/AssetstoreCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10660 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/collections/Collection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/collections/CollectionCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/src/collections/FileCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/src/collections/FolderCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/src/collections/GroupCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/src/collections/ItemCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/src/collections/UserCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-04-12 16:28:01.000000 girder-5.0.0a2/girder/web/dist/src/collections/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/constants.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4733 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/dialog.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/events.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/index.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/main.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6698 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/misc.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.675801 girder-5.0.0a2/girder/web/dist/src/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2841 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/AccessControlledModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/ApiKeyModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/AssetstoreModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/CollectionCreationPolicyModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/CollectionModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10910 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/FileModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      882 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/FolderModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6427 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/GroupModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2284 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/ItemModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2964 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/MetadataMixin.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5688 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/Model.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5467 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/UserModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/models/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/pluginUtils.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7243 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/rest.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/router.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7074 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.623800 girder-5.0.0a2/girder/web/dist/src/stylesheets/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.675801 girder-5.0.0a2/girder/web/dist/src/stylesheets/apidocs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      831 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/apidocs/apidocs.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.679801 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/adminConsole.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/assetstores.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      697 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/collectionList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/collectionPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      939 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/frontPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/groupList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2127 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/groupPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1370 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/itemPage.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/plugins.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/searchResultsList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/systemConfig.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/userAccount.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/userList.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/body/userPage.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.679801 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/footer.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/global.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/globalNav.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/header.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/headerUser.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1320 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/layout.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/layoutVars.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      622 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/loading.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/progressArea.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.683801 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1788 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/accessWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/browserWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/hierarchyWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/markdownWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1662 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/metadataWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/searchFieldWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/taskProgress.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/timelineWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/uploadWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3818 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/userOtpManagementWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.623800 girder-5.0.0a2/girder/web/dist/src/templates/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.687801 girder-5.0.0a2/girder/web/dist/src/templates/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/adminConsole.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3503 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/assetstores.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/collectionList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/collectionPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/filesystemImport.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2974 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/frontPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/groupList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3962 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/groupPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1836 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/itemPage.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      949 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/plugins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/s3Import.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/searchResults.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/searchResultsType.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10326 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/systemConfiguration.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/userAccount.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/userList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/body/userPage.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.687801 girder-5.0.0a2/girder/web/dist/src/templates/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/alert.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/layout.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/layoutFooter.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/layoutGlobalNav.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/layoutHeader.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      796 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/layoutHeaderUser.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/layoutProgressArea.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/loginDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1719 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/registerDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/layout/resetPasswordDialog.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.703801 girder-5.0.0a2/girder/web/dist/src/templates/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/accessEditor.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/accessEditorMixins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/accessEditorNonModal.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/accessEntry.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1918 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/apiKeyList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/browserWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/checkedActionsMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1273 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/collectionInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      565 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/confirmDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/dateTimeRangeWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/dateTimeWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/editApiKeyWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3345 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/editAssetstoreWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/editCollectionWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/editFileWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/editFolderWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/editGroupWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/editItemWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/fileInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1229 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/fileList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/folderInfoDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/folderList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupAdminList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3129 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupInviteDialog.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupInviteList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupMemberList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupModList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/hierarchyBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/hierarchyPaginated.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3835 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/hierarchyWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      461 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/itemBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1088 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/itemList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/jsonMetadatumEditWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/jsonMetadatumView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/loadingAnimation.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/markdownWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/metadataWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/metadatumEditWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/metadatumView.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3972 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/newAssetstore.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/paginateWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/pluginConfigBreadcrumb.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/rootSelectorWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/searchField.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/searchHelp.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/searchModeSelect.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      469 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/searchResults.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/sortCollectionWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/taskProgress.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/timeline.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/uploadWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/uploadWidgetMixins.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/uploadWidgetNonModal.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      115 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/userOtpBegin.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/userOtpDisable.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/templates/widgets/userOtpEnable.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.707801 girder-5.0.0a2/girder/web/dist/src/utilities/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/utilities/EventStream.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/utilities/PluginUtils.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9489 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/utilities/S3UploadHandler.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/utilities/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.707801 girder-5.0.0a2/girder/web/dist/src/utilities/jquery/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/utilities/jquery/girderEnable.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2134 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/utilities/jquery/girderModal.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/version.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.707801 girder-5.0.0a2/girder/web/dist/src/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/App.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2561 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/View.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.711801 girder-5.0.0a2/girder/web/dist/src/views/body/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/AdminView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8160 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/AssetstoresView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6740 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/CollectionView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4353 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/CollectionsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3146 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/FilesystemImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/FolderView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/FrontPageView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11859 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/GroupView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/GroupsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6011 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/ItemView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/PluginsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/S3ImportView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5544 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/SearchResultsView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6532 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/SystemConfigurationView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6266 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/UserAccountView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5437 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/UserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/UsersView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/body/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.715801 girder-5.0.0a2/girder/web/dist/src/views/layout/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/FooterView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3163 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/GlobalNavView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/HeaderUserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/HeaderView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/LoginView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/ProgressListView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3733 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/RegisterView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2344 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/ResetPasswordView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/layout/index.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.731801 girder-5.0.0a2/girder/web/dist/src/views/widgets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    15584 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/AccessWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/ApiKeyListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14503 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/BrowserWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2441 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/CheckedMenuWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/CollectionInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/DateTimeRangeWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3368 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/DateTimeWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/EditApiKeyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5411 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/EditAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/EditCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/EditFileWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4203 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/EditFolderWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/EditGroupWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3797 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/EditItemWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/FileInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5005 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/FileListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/FolderInfoWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3360 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/FolderListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupAdminsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1838 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupInvitesWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5965 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupMembersWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2518 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupModsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    42297 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/HierarchyWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/ItemBreadcrumbWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14228 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/ItemListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/LoadingAnimation.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7648 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/MarkdownWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    17263 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/MetadataWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/NewAssetstoreWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/PaginateWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/PluginConfigBreadcrumbWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6452 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/RootSelectorWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13112 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/SearchFieldWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4508 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/SearchPaginateWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/SortCollectionWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3042 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/TaskProgressWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6664 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/TimelineWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13690 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/UploadWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3203 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/UserOtpManagementWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2673 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/views/widgets/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-04-12 16:28:02.000000 girder-5.0.0a2/girder/web/dist/src/vite-env.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/env.d.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2259 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/playwright.config.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.731801 girder-5.0.0a2/girder/web/tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2707 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/coverage.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/playwright-setup.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/playwright-teardown.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/server.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.731801 girder-5.0.0a2/girder/web/tests/spec/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/admin.spec.ts
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.731801 girder-5.0.0a2/girder/web/tests/spec/data/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/data/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/data/ten_byte_file.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1514 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_authorized_upload.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1148 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_hashsum_download.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1769 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_homepage.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1161 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_item_licenses.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      861 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_readme.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1567 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_terms.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2225 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_thumbnails.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/spec/plugin_user_quota.spec.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/web/tests/util.ts
--rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2024-04-12 16:27:17.000000 girder-5.0.0a2/girder/wsgi.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.735801 girder-5.0.0a2/girder.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2718 2024-04-12 16:28:57.000000 girder-5.0.0a2/girder.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18574 2024-04-12 16:28:57.000000 girder-5.0.0a2/girder.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:28:57.000000 girder-5.0.0a2/girder.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-04-12 16:28:57.000000 girder-5.0.0a2/girder.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:28:57.000000 girder-5.0.0a2/girder.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2024-04-12 16:28:57.000000 girder-5.0.0a2/girder.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-04-12 16:28:57.000000 girder-5.0.0a2/girder.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)   196254 2024-04-12 16:27:18.000000 girder-5.0.0a2/package-lock.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3517 2024-04-12 16:27:18.000000 girder-5.0.0a2/package.json
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.735801 girder-5.0.0a2/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/LICENSE
--rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/MANIFEST.in
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.735801 girder-5.0.0a2/pytest_girder/pytest_girder/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/pytest_girder/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/pytest_girder/assertions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6136 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/pytest_girder/fixtures.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/pytest_girder/plugin.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/pytest_girder/plugin_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/pytest_girder/utils.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/pytest_girder/web_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-04-12 16:27:18.000000 girder-5.0.0a2/pytest_girder/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      718 2024-04-12 16:27:18.000000 girder-5.0.0a2/requirements-dev.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.735801 girder-5.0.0a2/scripts/
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:28:57.735801 girder-5.0.0a2/scripts/midas/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/midas/README.rst
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11413 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/midas/migrate.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/midas/requirements.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/midas/walk_girder.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1357 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/midas/walk_midas.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4118 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/publicNames.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    35230 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/publicNames.txt
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)      604 2024-04-12 16:27:18.000000 girder-5.0.0a2/scripts/test_names.sh
--rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-04-12 16:28:57.739801 girder-5.0.0a2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-12 16:27:18.000000 girder-5.0.0a2/setup.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-04-12 16:27:18.000000 girder-5.0.0a2/tox.ini
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.518698 girder-5.0.0a2.dev10/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.410698 girder-5.0.0a2.dev10/.circleci/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1098 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/Dockerfile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      585 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/build_plugins.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13158 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/config.yml
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      316 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/generatePyEnvChecksum.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      980 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/publish_npm.sh
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      417 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.circleci/publish_pypi.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      620 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.codecov.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       75 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.dockerignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      412 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.editorconfig
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/.readthedocs.yml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20024 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/CHANGELOG.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      729 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/CMakeLists.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4925 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/CONTRIBUTING.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      866 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/Dockerfile
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      491 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2724 2024-04-12 16:12:21.518698 girder-5.0.0a2.dev10/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1513 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.402697 girder-5.0.0a2.dev10/clients/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.410698 girder-5.0.0a2.dev10/clients/python/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      309 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/README.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.410698 girder-5.0.0a2.dev10/clients/python/girder_client/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    68223 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/girder_client/__init__.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)    13535 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/girder_client/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1810 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/clients/python/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      395 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docker-compose.yml
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.414698 girder-5.0.0a2.dev10/docs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      135 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/admin-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5217 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/api-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      228 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/build-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       30 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/changelog.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2379 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/conf.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2137 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/configuration.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5131 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/dependencies.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2047 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/deployment.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      339 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/dev-installation.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22931 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/developer-cookbook.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/developer-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13030 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15086 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/favicon.ico
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.414698 girder-5.0.0a2.dev10/docs/images/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   803025 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/images/dicom-viewer.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5181 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/index.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2776 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/license.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36997 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/migration-guide.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/mount.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    38303 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/plugin-development.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21669 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/plugins.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10504 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/python-client.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       70 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/requirements-docs.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5707 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/security.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1640 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/sftp.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       92 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/user-docs.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13645 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/docs/user-guide.rst
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.418697 girder-5.0.0a2.dev10/girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      511 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.418697 girder-5.0.0a2.dev10/girder/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4349 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/access.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1341 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/api_docs.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/api_main.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    32888 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/describe.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5216 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/docs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3483 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/filter_logging.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    51167 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7285 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/sftp.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.422697 girder-5.0.0a2.dev10/girder/api/v1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12222 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/assetstore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10847 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19091 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21532 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/folder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15913 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15915 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4577 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17147 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/resource.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18817 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/system.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2065 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19063 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/api/v1/user.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.422697 girder-5.0.0a2.dev10/girder/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      358 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24760 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/mount.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2452 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/serve.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1367 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/sftpd.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1750 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/cli/shell.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7162 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5954 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/events.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2769 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.422697 girder-5.0.0a2.dev10/girder/mail_templates/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      214 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/_footer.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/_header.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      306 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/accountApproval.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      160 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/accountApproved.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/emailVerification.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/groupInvite.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      476 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/mail_templates/temporaryAccess.mako
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.426698 girder-5.0.0a2.dev10/girder/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3245 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4825 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/api_key.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6054 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/assetstore.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16104 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/collection.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20130 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/file.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    36301 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/folder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15676 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/group.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    21461 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/item.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    65727 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/model_base.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8257 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/notification.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5870 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/setting.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4697 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22202 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/upload.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24605 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6465 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14634 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/settings.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.426698 girder-5.0.0a2.dev10/girder/utility/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6482 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3111 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/_cache.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4913 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/_hash_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17371 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/abstract_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    16381 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/acl_mixin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2310 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/assetstore_utilities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1070 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/config.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/error.mako
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18688 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/filesystem_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6280 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/mail_utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2752 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/model_importer.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6735 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/path.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4435 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/progress.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    26957 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/s3_assetstore_adapter.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2440 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/search.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3589 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/server.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2946 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/setting_utilities.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6845 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/system.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2857 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/webroot.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8124 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/utility/ziputil.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.430698 girder-5.0.0a2.dev10/girder/web/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/.env.development
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      331 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/.gitignore
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      162 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/.prettierrc.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2069 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.430698 girder-5.0.0a2.dev10/girder/web/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1494 2024-04-12 16:11:18.000000 girder-5.0.0a2.dev10/girder/web/dist/Girder_Favicon.png
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7590 2024-04-12 16:11:18.000000 girder-5.0.0a2.dev10/girder/web/dist/Girder_Mark.png
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.442698 girder-5.0.0a2.dev10/girder/web/dist/assets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   127292 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-00cea317.ttf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    72868 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-13e61b43.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   183888 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-2d6e9725.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    58716 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-98c6b1f2.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   127460 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-e418b5b2.eot
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    20127 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-13634da8.eot
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   108738 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-42f60659.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23424 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-a26394f7.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    45404 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-e3950440.ttf
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18028 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-fe185d11.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   215659 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/index-269c82d1.css
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  1984729 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/index-41ef1ab1.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)  5812987 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/index-41ef1ab1.js.map
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35955 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/jsoneditor-icons-25c04e58.svg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18668 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300-6e8a28a0.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14932 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300-f677ee2d.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13860 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300italic-453e6eb2.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17668 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300italic-5bb07410.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18100 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400-81f0ec27.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14380 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400-9c50a96c.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17440 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400italic-39ec493a.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13780 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400italic-da407a15.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14880 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600-1491de1b.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18696 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600-57c79375.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13852 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600italic-10879c90.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17492 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600italic-bb878389.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15056 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700-74201a4b.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18900 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700-ea20e5db.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17452 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700italic-1e742589.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13880 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700italic-d8505544.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    19072 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800-35eb714d.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15088 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800-75db6959.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13960 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800italic-49512fd4.woff2
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17788 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800italic-49b6274b.woff
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      451 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/index.html
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.442698 girder-5.0.0a2.dev10/girder/web/dist/src/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2938 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/auth.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.446698 girder-5.0.0a2.dev10/girder/web/dist/src/collections/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      255 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/ApiKeyCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/AssetstoreCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10660 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/Collection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      278 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/CollectionCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/FileCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      275 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/FolderCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/GroupCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      263 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/ItemCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      616 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/UserCollection.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/collections/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      478 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/constants.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4733 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/dialog.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      137 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/events.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2228 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/index.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1298 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/main.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6698 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/misc.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.450698 girder-5.0.0a2.dev10/girder/web/dist/src/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2841 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/AccessControlledModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1045 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/ApiKeyModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1221 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/AssetstoreModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/CollectionCreationPolicyModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      346 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/CollectionModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10910 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/FileModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      882 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/FolderModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6427 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/GroupModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2284 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/ItemModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2964 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/MetadataMixin.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5688 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/Model.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5467 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/UserModel.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      671 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/models/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      302 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/pluginUtils.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7243 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/rest.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1604 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/router.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7074 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/routes.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.406698 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.450698 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/apidocs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      831 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/apidocs/apidocs.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.454697 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      310 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/adminConsole.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      792 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/assetstores.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      697 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/collectionList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      124 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/collectionPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      939 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/frontPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      695 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2127 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1370 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/itemPage.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1125 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/plugins.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      911 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/searchResultsList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1080 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/systemConfig.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      888 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userAccount.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1322 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userList.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      112 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userPage.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.458697 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      389 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/footer.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2843 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/global.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/globalNav.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      504 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/header.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      486 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/headerUser.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1320 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/layout.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      191 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/layoutVars.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      622 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/loading.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/progressArea.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.462698 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1788 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/accessWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/browserWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3742 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/hierarchyWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1713 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/markdownWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1662 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/metadataWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1359 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/searchFieldWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      723 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/taskProgress.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      787 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/timelineWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      811 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/uploadWidget.styl
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3818 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/userOtpManagementWidget.styl
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.406698 girder-5.0.0a2.dev10/girder/web/dist/src/templates/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.466698 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      289 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/adminConsole.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3503 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/assetstores.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1484 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1307 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1887 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/filesystemImport.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2974 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/frontPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      944 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3962 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1836 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/itemPage.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      949 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/plugins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1553 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/s3Import.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      425 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/searchResults.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      505 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/searchResultsType.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10326 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/systemConfiguration.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3634 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userAccount.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1363 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1442 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userPage.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.470697 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      179 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/alert.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      396 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layout.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      404 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutFooter.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      246 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutGlobalNav.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      234 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutHeader.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      796 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutHeaderUser.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutProgressArea.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/loginDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1719 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/registerDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1035 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/resetPasswordDialog.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.482698 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      665 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditor.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2211 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditorMixins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      188 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditorNonModal.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1711 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEntry.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1918 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/apiKeyList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1126 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/browserWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1167 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/checkedActionsMenu.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1273 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/collectionInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      565 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/confirmDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      598 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/dateTimeRangeWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      230 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/dateTimeWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1800 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editApiKeyWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3345 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editAssetstoreWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      941 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editCollectionWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFileWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      921 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFolderWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2662 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editGroupWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      907 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editItemWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      988 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1229 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1360 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderInfoDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      638 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1364 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupAdminList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3129 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupInviteDialog.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupInviteList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1421 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupMemberList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      869 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupModList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      858 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      631 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyPaginated.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3835 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      461 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/itemBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1088 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/itemList.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      513 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/jsonMetadatumEditWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      195 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/jsonMetadatumView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/loadingAnimation.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1501 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/markdownWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadataWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      667 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadatumEditWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      189 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadatumView.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3972 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/newAssetstore.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      183 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/paginateWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      250 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/pluginConfigBreadcrumb.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/rootSelectorWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      417 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchField.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      343 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchHelp.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      248 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchModeSelect.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      469 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/searchResults.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      552 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/sortCollectionWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      647 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/taskProgress.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/timeline.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      490 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidget.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1013 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidgetMixins.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      235 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidgetNonModal.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      115 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpBegin.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      212 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpDisable.pug
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1684 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpEnable.pug
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.486698 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5488 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/EventStream.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1122 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/PluginUtils.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9489 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/S3UploadHandler.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      208 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.486698 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      438 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/girderEnable.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2134 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/girderModal.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/version.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.486698 girder-5.0.0a2.dev10/girder/web/dist/src/views/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    12010 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/App.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2561 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/View.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.494698 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      815 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AdminView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8160 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AssetstoresView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6740 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4353 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3146 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FilesystemImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1679 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FolderView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1305 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FrontPageView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11859 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6011 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/ItemView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2269 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/PluginsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2907 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/S3ImportView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5544 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SearchResultsView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6532 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SystemConfigurationView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6266 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserAccountView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5437 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4185 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UsersView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1091 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/body/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      224 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.498698 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      863 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/FooterView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3163 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/GlobalNavView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1239 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderUserView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2977 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3697 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/LoginView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2190 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ProgressListView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3733 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/RegisterView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2344 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ResetPasswordView.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      515 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/index.js
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.510697 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    15584 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/AccessWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4631 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ApiKeyListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14503 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/BrowserWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2441 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CheckedMenuWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CollectionInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5988 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeRangeWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3368 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4342 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditApiKeyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5411 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3239 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1959 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFileWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4203 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFolderWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4479 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditGroupWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3797 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditItemWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      726 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5005 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1172 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderInfoWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3360 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2901 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupAdminsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1838 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupInvitesWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5965 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupMembersWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2518 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupModsWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    42297 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/HierarchyWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14228 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemListWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      446 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/LoadingAnimation.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7648 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MarkdownWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    17263 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MetadataWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2746 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/NewAssetstoreWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1061 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PaginateWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      928 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PluginConfigBreadcrumbWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6452 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/RootSelectorWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13112 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchFieldWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4508 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchPaginateWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1614 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SortCollectionWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3042 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TaskProgressWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6664 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TimelineWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13690 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UploadWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3203 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UserOtpManagementWidget.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2673 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/index.js
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      118 2024-04-12 16:11:24.000000 girder-5.0.0a2.dev10/girder/web/dist/src/vite-env.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/env.d.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2259 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/playwright.config.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.510697 girder-5.0.0a2.dev10/girder/web/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2707 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/coverage.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      351 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/playwright-setup.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1150 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/playwright-teardown.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/server.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.510697 girder-5.0.0a2.dev10/girder/web/tests/spec/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1612 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/admin.spec.ts
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/girder/web/tests/spec/data/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      272 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/data/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/data/ten_byte_file.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1514 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_authorized_upload.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1148 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_hashsum_download.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1769 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_homepage.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1161 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_item_licenses.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      861 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_readme.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1567 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_terms.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2225 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_thumbnails.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1568 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_user_quota.spec.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3551 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/web/tests/util.ts
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      239 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/girder/wsgi.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/girder.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2724 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18574 2024-04-12 16:12:21.000000 girder-5.0.0a2.dev10/girder.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      297 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      233 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2024-04-12 16:12:20.000000 girder-5.0.0a2.dev10/girder.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   196254 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/package-lock.json
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3517 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/package.json
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       43 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/MANIFEST.in
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1022 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/assertions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6136 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/fixtures.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1772 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2923 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11332 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/utils.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5970 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/pytest_girder/web_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1310 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/pytest_girder/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      718 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/requirements-dev.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/scripts/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:12:21.514698 girder-5.0.0a2.dev10/scripts/midas/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1617 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/README.rst
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11413 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/migrate.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       27 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/requirements.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1237 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/walk_girder.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1357 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/midas/walk_midas.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4118 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/publicNames.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    35230 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/publicNames.txt
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)      604 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/scripts/test_names.sh
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      520 2024-04-12 16:12:21.518698 girder-5.0.0a2.dev10/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2692 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/setup.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3535 2024-04-12 16:10:43.000000 girder-5.0.0a2.dev10/tox.ini
```

### Comparing `girder-5.0.0a2/.circleci/Dockerfile` & `girder-5.0.0a2.dev10/.circleci/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/.circleci/build_plugins.py` & `girder-5.0.0a2.dev10/.circleci/build_plugins.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/.circleci/config.yml` & `girder-5.0.0a2.dev10/.circleci/config.yml`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/.circleci/publish_npm.sh` & `girder-5.0.0a2.dev10/.circleci/publish_npm.sh`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/.codecov.yml` & `girder-5.0.0a2.dev10/.codecov.yml`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/CHANGELOG.rst` & `girder-5.0.0a2.dev10/CHANGELOG.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/CMakeLists.txt` & `girder-5.0.0a2.dev10/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/CONTRIBUTING.rst` & `girder-5.0.0a2.dev10/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/Dockerfile` & `girder-5.0.0a2.dev10/Dockerfile`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/LICENSE` & `girder-5.0.0a2.dev10/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/PKG-INFO` & `girder-5.0.0a2.dev10/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 5.0.0a2
+Version: 5.0.0a2.dev10
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-5.0.0a2/README.rst` & `girder-5.0.0a2.dev10/README.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/clients/python/girder_client/__init__.py` & `girder-5.0.0a2.dev10/clients/python/girder_client/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/clients/python/girder_client/cli.py` & `girder-5.0.0a2.dev10/clients/python/girder_client/cli.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/clients/python/setup.py` & `girder-5.0.0a2.dev10/clients/python/setup.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/api-docs.rst` & `girder-5.0.0a2.dev10/docs/api-docs.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/conf.py` & `girder-5.0.0a2.dev10/docs/conf.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/configuration.rst` & `girder-5.0.0a2.dev10/docs/configuration.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/dependencies.rst` & `girder-5.0.0a2.dev10/docs/dependencies.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/deployment.rst` & `girder-5.0.0a2.dev10/docs/deployment.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/developer-cookbook.rst` & `girder-5.0.0a2.dev10/docs/developer-cookbook.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/development.rst` & `girder-5.0.0a2.dev10/docs/development.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/favicon.ico` & `girder-5.0.0a2.dev10/docs/favicon.ico`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/images/dicom-viewer.png` & `girder-5.0.0a2.dev10/docs/images/dicom-viewer.png`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/index.rst` & `girder-5.0.0a2.dev10/docs/index.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/license.png` & `girder-5.0.0a2.dev10/docs/license.png`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/migration-guide.rst` & `girder-5.0.0a2.dev10/docs/migration-guide.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/mount.rst` & `girder-5.0.0a2.dev10/docs/mount.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/plugin-development.rst` & `girder-5.0.0a2.dev10/docs/plugin-development.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/plugins.rst` & `girder-5.0.0a2.dev10/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/python-client.rst` & `girder-5.0.0a2.dev10/docs/python-client.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/security.rst` & `girder-5.0.0a2.dev10/docs/security.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/sftp.rst` & `girder-5.0.0a2.dev10/docs/sftp.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/docs/user-guide.rst` & `girder-5.0.0a2.dev10/docs/user-guide.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/access.py` & `girder-5.0.0a2.dev10/girder/api/access.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/api_docs.mako` & `girder-5.0.0a2.dev10/girder/api/api_docs.mako`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/api_main.py` & `girder-5.0.0a2.dev10/girder/api/api_main.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/describe.py` & `girder-5.0.0a2.dev10/girder/api/describe.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/docs.py` & `girder-5.0.0a2.dev10/girder/api/docs.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/filter_logging.py` & `girder-5.0.0a2.dev10/girder/api/filter_logging.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/rest.py` & `girder-5.0.0a2.dev10/girder/api/rest.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/sftp.py` & `girder-5.0.0a2.dev10/girder/api/sftp.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/api_key.py` & `girder-5.0.0a2.dev10/girder/api/v1/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/assetstore.py` & `girder-5.0.0a2.dev10/girder/api/v1/assetstore.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/collection.py` & `girder-5.0.0a2.dev10/girder/api/v1/collection.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/file.py` & `girder-5.0.0a2.dev10/girder/api/v1/file.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/folder.py` & `girder-5.0.0a2.dev10/girder/api/v1/folder.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/group.py` & `girder-5.0.0a2.dev10/girder/api/v1/group.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/item.py` & `girder-5.0.0a2.dev10/girder/api/v1/item.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/notification.py` & `girder-5.0.0a2.dev10/girder/api/v1/notification.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/resource.py` & `girder-5.0.0a2.dev10/girder/api/v1/resource.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/system.py` & `girder-5.0.0a2.dev10/girder/api/v1/system.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/token.py` & `girder-5.0.0a2.dev10/girder/api/v1/token.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/api/v1/user.py` & `girder-5.0.0a2.dev10/girder/api/v1/user.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/cli/mount.py` & `girder-5.0.0a2.dev10/girder/cli/mount.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/cli/serve.py` & `girder-5.0.0a2.dev10/girder/cli/serve.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/cli/sftpd.py` & `girder-5.0.0a2.dev10/girder/cli/sftpd.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/cli/shell.py` & `girder-5.0.0a2.dev10/girder/cli/shell.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/constants.py` & `girder-5.0.0a2.dev10/girder/constants.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/events.py` & `girder-5.0.0a2.dev10/girder/events.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/exceptions.py` & `girder-5.0.0a2.dev10/girder/exceptions.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/__init__.py` & `girder-5.0.0a2.dev10/girder/models/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/api_key.py` & `girder-5.0.0a2.dev10/girder/models/api_key.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/assetstore.py` & `girder-5.0.0a2.dev10/girder/models/assetstore.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/collection.py` & `girder-5.0.0a2.dev10/girder/models/collection.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/file.py` & `girder-5.0.0a2.dev10/girder/models/file.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/folder.py` & `girder-5.0.0a2.dev10/girder/models/folder.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/group.py` & `girder-5.0.0a2.dev10/girder/models/group.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/item.py` & `girder-5.0.0a2.dev10/girder/models/item.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/model_base.py` & `girder-5.0.0a2.dev10/girder/models/model_base.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/notification.py` & `girder-5.0.0a2.dev10/girder/models/notification.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/setting.py` & `girder-5.0.0a2.dev10/girder/models/setting.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/token.py` & `girder-5.0.0a2.dev10/girder/models/token.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/upload.py` & `girder-5.0.0a2.dev10/girder/models/upload.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/models/user.py` & `girder-5.0.0a2.dev10/girder/models/user.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/plugin.py` & `girder-5.0.0a2.dev10/girder/plugin.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/settings.py` & `girder-5.0.0a2.dev10/girder/settings.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/__init__.py` & `girder-5.0.0a2.dev10/girder/utility/__init__.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/_cache.py` & `girder-5.0.0a2.dev10/girder/utility/_cache.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/_hash_state.py` & `girder-5.0.0a2.dev10/girder/utility/_hash_state.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/abstract_assetstore_adapter.py` & `girder-5.0.0a2.dev10/girder/utility/abstract_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/acl_mixin.py` & `girder-5.0.0a2.dev10/girder/utility/acl_mixin.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/assetstore_utilities.py` & `girder-5.0.0a2.dev10/girder/utility/assetstore_utilities.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/config.py` & `girder-5.0.0a2.dev10/girder/utility/config.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/filesystem_assetstore_adapter.py` & `girder-5.0.0a2.dev10/girder/utility/filesystem_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/mail_utils.py` & `girder-5.0.0a2.dev10/girder/utility/mail_utils.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/model_importer.py` & `girder-5.0.0a2.dev10/girder/utility/model_importer.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/path.py` & `girder-5.0.0a2.dev10/girder/utility/path.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/progress.py` & `girder-5.0.0a2.dev10/girder/utility/progress.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/s3_assetstore_adapter.py` & `girder-5.0.0a2.dev10/girder/utility/s3_assetstore_adapter.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/search.py` & `girder-5.0.0a2.dev10/girder/utility/search.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/server.py` & `girder-5.0.0a2.dev10/girder/utility/server.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/setting_utilities.py` & `girder-5.0.0a2.dev10/girder/utility/setting_utilities.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/system.py` & `girder-5.0.0a2.dev10/girder/utility/system.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/webroot.py` & `girder-5.0.0a2.dev10/girder/utility/webroot.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/utility/ziputil.py` & `girder-5.0.0a2.dev10/girder/utility/ziputil.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/README.md` & `girder-5.0.0a2.dev10/girder/web/README.md`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/Girder_Favicon.png` & `girder-5.0.0a2.dev10/girder/web/dist/Girder_Favicon.png`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/Girder_Mark.png` & `girder-5.0.0a2.dev10/girder/web/dist/Girder_Mark.png`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/fontello-00cea317.ttf` & `girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-00cea317.ttf`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/fontello-13e61b43.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-13e61b43.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/fontello-2d6e9725.svg` & `girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-2d6e9725.svg`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/fontello-98c6b1f2.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-98c6b1f2.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/fontello-e418b5b2.eot` & `girder-5.0.0a2.dev10/girder/web/dist/assets/fontello-e418b5b2.eot`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-13634da8.eot` & `girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-13634da8.eot`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-42f60659.svg` & `girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-42f60659.svg`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-a26394f7.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-a26394f7.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-e3950440.ttf` & `girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-e3950440.ttf`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/glyphicons-halflings-regular-fe185d11.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/glyphicons-halflings-regular-fe185d11.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/index-269c82d1.css` & `girder-5.0.0a2.dev10/girder/web/dist/assets/index-269c82d1.css`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/index-41ef1ab1.js` & `girder-5.0.0a2.dev10/girder/web/dist/assets/index-41ef1ab1.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/index-41ef1ab1.js.map` & `girder-5.0.0a2.dev10/girder/web/dist/assets/index-41ef1ab1.js.map`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/jsoneditor-icons-25c04e58.svg` & `girder-5.0.0a2.dev10/girder/web/dist/assets/jsoneditor-icons-25c04e58.svg`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300-6e8a28a0.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300-6e8a28a0.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300-f677ee2d.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300-f677ee2d.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300italic-453e6eb2.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300italic-453e6eb2.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-300italic-5bb07410.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-300italic-5bb07410.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400-81f0ec27.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400-81f0ec27.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400-9c50a96c.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400-9c50a96c.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400italic-39ec493a.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400italic-39ec493a.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-400italic-da407a15.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-400italic-da407a15.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600-1491de1b.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600-1491de1b.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600-57c79375.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600-57c79375.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600italic-10879c90.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600italic-10879c90.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-600italic-bb878389.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-600italic-bb878389.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700-74201a4b.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700-74201a4b.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700-ea20e5db.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700-ea20e5db.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700italic-1e742589.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700italic-1e742589.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-700italic-d8505544.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-700italic-d8505544.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800-35eb714d.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800-35eb714d.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800-75db6959.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800-75db6959.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800italic-49512fd4.woff2` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800italic-49512fd4.woff2`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/assets/open-sans-latin-800italic-49b6274b.woff` & `girder-5.0.0a2.dev10/girder/web/dist/assets/open-sans-latin-800italic-49b6274b.woff`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/auth.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/auth.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/collections/Collection.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/collections/Collection.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/collections/UserCollection.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/collections/UserCollection.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/collections/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/collections/index.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/dialog.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/dialog.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/index.ts` & `girder-5.0.0a2.dev10/girder/web/dist/src/index.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/main.ts` & `girder-5.0.0a2.dev10/girder/web/dist/src/main.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/misc.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/misc.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/AccessControlledModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/AccessControlledModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/ApiKeyModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/ApiKeyModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/AssetstoreModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/AssetstoreModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/CollectionCreationPolicyModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/CollectionCreationPolicyModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/FileModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/FileModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/FolderModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/FolderModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/GroupModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/GroupModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/ItemModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/ItemModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/MetadataMixin.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/MetadataMixin.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/Model.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/Model.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/UserModel.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/UserModel.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/models/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/models/index.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/rest.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/rest.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/router.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/router.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/routes.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/routes.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/apidocs/apidocs.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/apidocs/apidocs.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/assetstores.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/assetstores.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/collectionList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/collectionList.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/frontPage.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/frontPage.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/groupList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupList.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/groupPage.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/groupPage.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/itemPage.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/itemPage.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/plugins.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/plugins.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/searchResultsList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/searchResultsList.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/systemConfig.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/systemConfig.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/userAccount.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userAccount.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/body/userList.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/body/userList.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/global.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/global.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/globalNav.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/globalNav.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/layout.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/layout.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/layout/loading.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/layout/loading.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/accessWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/accessWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/hierarchyWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/hierarchyWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/markdownWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/markdownWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/metadataWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/metadataWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/searchFieldWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/searchFieldWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/taskProgress.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/taskProgress.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/timelineWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/timelineWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/uploadWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/uploadWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/stylesheets/widgets/userOtpManagementWidget.styl` & `girder-5.0.0a2.dev10/girder/web/dist/src/stylesheets/widgets/userOtpManagementWidget.styl`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/assetstores.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/assetstores.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/collectionList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/collectionPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/collectionPage.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/filesystemImport.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/filesystemImport.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/frontPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/frontPage.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/groupList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/groupPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/groupPage.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/itemPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/itemPage.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/plugins.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/plugins.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/s3Import.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/s3Import.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/systemConfiguration.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/systemConfiguration.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/userAccount.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userAccount.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/userList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/body/userPage.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/body/userPage.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/layout/layoutHeaderUser.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/layoutHeaderUser.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/layout/loginDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/loginDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/layout/registerDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/registerDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/layout/resetPasswordDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/layout/resetPasswordDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/accessEditor.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditor.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/accessEditorMixins.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEditorMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/accessEntry.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/accessEntry.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/apiKeyList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/apiKeyList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/browserWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/browserWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/checkedActionsMenu.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/checkedActionsMenu.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/collectionInfoDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/collectionInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/confirmDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/confirmDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/dateTimeRangeWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/dateTimeRangeWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/editApiKeyWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editApiKeyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/editAssetstoreWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editAssetstoreWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/editCollectionWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/editFileWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFileWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/editFolderWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editFolderWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/editGroupWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editGroupWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/editItemWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/editItemWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/fileInfoDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/fileList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/fileList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/folderInfoDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderInfoDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/folderList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/folderList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupAdminList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupAdminList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupInviteDialog.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupInviteDialog.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupMemberList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupMemberList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/groupModList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/groupModList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/hierarchyBreadcrumb.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyBreadcrumb.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/hierarchyPaginated.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyPaginated.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/hierarchyWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/hierarchyWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/itemList.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/itemList.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/jsonMetadatumEditWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/jsonMetadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/markdownWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/markdownWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/metadataWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadataWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/metadatumEditWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/metadatumEditWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/newAssetstore.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/newAssetstore.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/rootSelectorWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/rootSelectorWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/sortCollectionWidget.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/sortCollectionWidget.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/taskProgress.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/taskProgress.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/timeline.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/timeline.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/uploadWidgetMixins.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/uploadWidgetMixins.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/templates/widgets/userOtpEnable.pug` & `girder-5.0.0a2.dev10/girder/web/dist/src/templates/widgets/userOtpEnable.pug`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/utilities/EventStream.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/EventStream.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/utilities/PluginUtils.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/PluginUtils.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/utilities/S3UploadHandler.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/S3UploadHandler.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/utilities/jquery/girderModal.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/utilities/jquery/girderModal.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/App.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/App.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/View.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/View.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/AdminView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AdminView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/AssetstoresView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/AssetstoresView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/CollectionView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/CollectionsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/CollectionsView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/FilesystemImportView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FilesystemImportView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/FolderView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FolderView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/FrontPageView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/FrontPageView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/GroupView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/GroupsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/GroupsView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/ItemView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/ItemView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/PluginsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/PluginsView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/S3ImportView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/S3ImportView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/SearchResultsView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SearchResultsView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/SystemConfigurationView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/SystemConfigurationView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/UserAccountView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserAccountView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/UserView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UserView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/UsersView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/UsersView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/body/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/body/index.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/FooterView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/FooterView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/GlobalNavView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/GlobalNavView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/HeaderUserView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderUserView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/HeaderView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/HeaderView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/LoginView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/LoginView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/ProgressListView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ProgressListView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/RegisterView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/RegisterView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/ResetPasswordView.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/ResetPasswordView.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/layout/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/layout/index.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/AccessWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/AccessWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/ApiKeyListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ApiKeyListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/BrowserWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/BrowserWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/CheckedMenuWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CheckedMenuWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/CollectionInfoWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/CollectionInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/DateTimeRangeWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeRangeWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/DateTimeWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/DateTimeWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/EditApiKeyWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditApiKeyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/EditAssetstoreWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/EditCollectionWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/EditFileWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFileWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/EditFolderWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditFolderWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/EditGroupWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditGroupWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/EditItemWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/EditItemWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/FileInfoWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/FileListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FileListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/FolderInfoWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderInfoWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/FolderListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/FolderListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupAdminsWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupAdminsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupInvitesWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupInvitesWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupMembersWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupMembersWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/GroupModsWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/GroupModsWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/HierarchyWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/HierarchyWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/ItemBreadcrumbWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/ItemListWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/ItemListWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/MarkdownWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MarkdownWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/MetadataWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/MetadataWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/NewAssetstoreWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/NewAssetstoreWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/PaginateWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PaginateWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/PluginConfigBreadcrumbWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/PluginConfigBreadcrumbWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/RootSelectorWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/RootSelectorWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/SearchFieldWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchFieldWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/SearchPaginateWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SearchPaginateWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/SortCollectionWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/SortCollectionWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/TaskProgressWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TaskProgressWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/TimelineWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/TimelineWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/UploadWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UploadWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/UserOtpManagementWidget.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/UserOtpManagementWidget.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/dist/src/views/widgets/index.js` & `girder-5.0.0a2.dev10/girder/web/dist/src/views/widgets/index.js`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/playwright.config.ts` & `girder-5.0.0a2.dev10/girder/web/playwright.config.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/coverage.ts` & `girder-5.0.0a2.dev10/girder/web/tests/coverage.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/playwright-teardown.ts` & `girder-5.0.0a2.dev10/girder/web/tests/playwright-teardown.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/server.ts` & `girder-5.0.0a2.dev10/girder/web/tests/server.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/admin.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/admin.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_authorized_upload.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_authorized_upload.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_hashsum_download.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_hashsum_download.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_homepage.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_homepage.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_item_licenses.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_item_licenses.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_readme.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_readme.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_terms.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_terms.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_thumbnails.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_thumbnails.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/spec/plugin_user_quota.spec.ts` & `girder-5.0.0a2.dev10/girder/web/tests/spec/plugin_user_quota.spec.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder/web/tests/util.ts` & `girder-5.0.0a2.dev10/girder/web/tests/util.ts`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/girder.egg-info/PKG-INFO` & `girder-5.0.0a2.dev10/girder.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder
-Version: 5.0.0a2
+Version: 5.0.0a2.dev10
 Summary: Web-based data management platform
 Home-page: https://girder.readthedocs.org
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-5.0.0a2/girder.egg-info/SOURCES.txt` & `girder-5.0.0a2.dev10/girder.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/package-lock.json` & `girder-5.0.0a2.dev10/package-lock.json`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/package.json` & `girder-5.0.0a2.dev10/package.json`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/LICENSE` & `girder-5.0.0a2.dev10/pytest_girder/LICENSE`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/pytest_girder/assertions.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/assertions.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/pytest_girder/fixtures.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/fixtures.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/pytest_girder/plugin.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/pytest_girder/plugin_registry.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/plugin_registry.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/pytest_girder/utils.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/utils.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/pytest_girder/web_client.py` & `girder-5.0.0a2.dev10/pytest_girder/pytest_girder/web_client.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/pytest_girder/setup.py` & `girder-5.0.0a2.dev10/pytest_girder/setup.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/requirements-dev.txt` & `girder-5.0.0a2.dev10/requirements-dev.txt`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/scripts/midas/README.rst` & `girder-5.0.0a2.dev10/scripts/midas/README.rst`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/scripts/midas/migrate.py` & `girder-5.0.0a2.dev10/scripts/midas/migrate.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/scripts/midas/walk_girder.py` & `girder-5.0.0a2.dev10/scripts/midas/walk_girder.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/scripts/midas/walk_midas.py` & `girder-5.0.0a2.dev10/scripts/midas/walk_midas.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/scripts/publicNames.py` & `girder-5.0.0a2.dev10/scripts/publicNames.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/scripts/publicNames.txt` & `girder-5.0.0a2.dev10/scripts/publicNames.txt`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/scripts/test_names.sh` & `girder-5.0.0a2.dev10/scripts/test_names.sh`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/setup.cfg` & `girder-5.0.0a2.dev10/setup.cfg`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/setup.py` & `girder-5.0.0a2.dev10/setup.py`

 * *Files identical despite different names*

### Comparing `girder-5.0.0a2/tox.ini` & `girder-5.0.0a2.dev10/tox.ini`

 * *Files identical despite different names*

