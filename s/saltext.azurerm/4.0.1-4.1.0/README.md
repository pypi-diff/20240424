# Comparing `tmp/saltext.azurerm-4.0.1.tar.gz` & `tmp/saltext_azurerm-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "saltext.azurerm-4.0.1.tar", last modified: Mon Aug 14 23:54:45 2023, max compression
+gzip compressed data, was "saltext_azurerm-4.1.0.tar", last modified: Tue Apr 23 22:38:52 2024, max compression
```

## Comparing `saltext.azurerm-4.0.1.tar` & `saltext_azurerm-4.1.0.tar`

### file list

```diff
@@ -1,163 +1,175 @@
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      708 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/.coveragerc
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.719669 saltext.azurerm-4.0.1/.github/
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.719669 saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1201 2022-09-26 21:20:25.000000 saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      547 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      581 2022-09-26 21:20:25.000000 saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/docs.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      635 2022-09-26 21:20:25.000000 saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      463 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      933 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.719669 saltext.azurerm-4.0.1/.github/workflows/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    12839 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/.github/workflows/test.yml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1991 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/.gitignore
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8848 2023-02-13 15:42:34.000000 saltext.azurerm-4.0.1/.pre-commit-config.yaml
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.719669 saltext.azurerm-4.0.1/.pre-commit-hooks/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2084 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/.pre-commit-hooks/check-cli-examples.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1372 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/.pre-commit-hooks/make-autodocs.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    11890 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/.pylintrc
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      457 2022-06-22 00:54:47.000000 saltext.azurerm-4.0.1/.readthedocs.yaml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1395 2023-08-14 23:54:35.000000 saltext.azurerm-4.0.1/CHANGELOG.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5280 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/CODE-OF-CONDUCT.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      703 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/CONTRIBUTING.md
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    11352 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/LICENSE
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      481 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/NOTICE.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4407 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/PKG-INFO
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3084 2023-08-14 13:54:12.000000 saltext.azurerm-4.0.1/README.md
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.719669 saltext.azurerm-4.0.1/changelog/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       12 2022-06-22 01:31:35.000000 saltext.azurerm-4.0.1/changelog/.gitignore
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      634 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/docs/Makefile
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/_static/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/docs/_static/.gitkeep
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      238 2022-09-26 21:20:25.000000 saltext.azurerm-4.0.1/docs/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5323 2022-06-22 01:22:05.000000 saltext.azurerm-4.0.1/docs/conf.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      252 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/docs/index.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      760 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/docs/make.bat
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/ref/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/docs/ref/.gitkeep
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/ref/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      143 2022-06-22 01:16:49.000000 saltext.azurerm-4.0.1/docs/ref/clouds/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      820 2023-08-14 13:54:12.000000 saltext.azurerm-4.0.1/docs/ref/clouds/saltext.azurerm.clouds.azurerm.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/ref/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      778 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      816 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_compute.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      369 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_availability_set.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      340 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_disk.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      327 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_image.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      733 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      391 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_extension.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      399 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_image.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      497 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_dns.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      620 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_key.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      613 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_secret.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      179 2023-06-13 12:36:09.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_vault.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2189 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_network.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1092 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/modules/saltext.azurerm.modules.azurerm_resource.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/ref/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      545 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/states/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      309 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_compute.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      290 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_compute_availability_set.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      287 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_compute_virtual_machine.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      322 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_dns.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      289 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_key.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      298 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_secret.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      176 2023-06-13 12:36:09.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_vault.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      747 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_network.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      434 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/states/saltext.azurerm.states.azurerm_resource.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/ref/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      138 2022-06-22 01:16:49.000000 saltext.azurerm-4.0.1/docs/ref/utils/all.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      339 2022-06-22 00:33:58.000000 saltext.azurerm-4.0.1/docs/ref/utils/saltext.azurerm.utils.azurerm.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/docs/sitevars.rst
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/docs/topics/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5885 2022-09-26 21:20:25.000000 saltext.azurerm-4.0.1/docs/topics/authentication.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       80 2022-09-26 21:20:25.000000 saltext.azurerm-4.0.1/docs/topics/index.rst
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    17841 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/noxfile.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     1016 2023-02-13 15:42:34.000000 saltext.azurerm-4.0.1/pyproject.toml
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2591 2023-08-14 23:54:45.729669 saltext.azurerm-4.0.1/setup.cfg
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      568 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/setup.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.719669 saltext.azurerm-4.0.1/src/
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.719669 saltext.azurerm-4.0.1/src/saltext/
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/src/saltext/azurerm/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      863 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/src/saltext/azurerm/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/clouds/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    60699 2023-08-14 23:54:35.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/clouds/azurerm.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/src/saltext/azurerm/fileserver/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    14404 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/fileserver/azurefs.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      803 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/loader.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       35 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    14063 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     7448 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_availability_set.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5678 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_disk.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8509 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_image.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    59211 2023-08-14 13:54:12.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_virtual_machine.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     7027 2023-08-14 13:54:12.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_extension.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     6331 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_image.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    20227 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_dns.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    23448 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_keyvault_key.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    16546 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_keyvault_secret.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    19494 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_keyvault_vault.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    86399 2023-08-14 13:54:12.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_network.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    38085 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_resource.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/src/saltext/azurerm/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     6204 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_compute.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     9457 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_compute_availability_set.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    37184 2023-08-14 13:54:12.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_compute_virtual_machine.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    25691 2023-02-13 15:42:34.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_dns.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8639 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_keyvault_key.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    10245 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_keyvault_secret.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    18314 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_keyvault_vault.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    88144 2023-02-13 15:42:34.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_network.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    26674 2023-02-13 15:42:34.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_resource.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/src/saltext/azurerm/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       39 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/utils/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)    12926 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/utils/azurerm.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       65 2023-08-14 23:54:35.000000 saltext.azurerm-4.0.1/src/saltext/azurerm/version.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.723003 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4407 2023-08-14 23:54:45.000000 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/PKG-INFO
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5250 2023-08-14 23:54:45.000000 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/SOURCES.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        1 2023-08-14 23:54:45.000000 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/dependency_links.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)       48 2023-08-14 23:54:45.000000 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/entry_points.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        1 2022-06-22 00:15:20.000000 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/not-zip-safe
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      969 2023-08-14 23:54:45.000000 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/requires.txt
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        8 2023-08-14 23:54:45.000000 saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/top_level.txt
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)      708 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/conftest.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/integration/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/integration/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/integration/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/integration/clouds/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5587 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/tests/integration/conftest.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/integration/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/integration/modules/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/integration/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/integration/states/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     2811 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/tests/integration/states/test_compute_availability_set.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4379 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/tests/integration/states/test_compute_virtual_machine.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5633 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/integration/states/test_dns.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3566 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/tests/integration/states/test_keyvault_key.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4256 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/tests/integration/states/test_keyvault_secret.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     7796 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/tests/integration/states/test_keyvault_vault.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3392 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/integration/states/test_network_interface.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     5874 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/integration/states/test_network_route.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     6566 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/integration/states/test_network_security_group.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     4681 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/integration/states/test_public_ip_address.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     3316 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/integration/states/test_resource_group.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8846 2023-06-13 12:36:03.000000 saltext.azurerm-4.0.1/tests/integration/states/test_virtual_network.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/integration/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/integration/utils/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/unit/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/unit/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/unit/clouds/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/unit/clouds/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/unit/modules/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/unit/modules/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/unit/states/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/unit/states/__init__.py
-drwxr-xr-x   0 nmhughes  (1000) nmhughes  (1000)        0 2023-08-14 23:54:45.726336 saltext.azurerm-4.0.1/tests/unit/utils/
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)        0 2022-06-21 23:53:27.000000 saltext.azurerm-4.0.1/tests/unit/utils/__init__.py
--rw-r--r--   0 nmhughes  (1000) nmhughes  (1000)     8157 2023-07-10 10:59:30.000000 saltext.azurerm-4.0.1/tests/unit/utils/test_azurerm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.670334 saltext_azurerm-4.1.0/
+-rw-r--r--   0 root         (0) root         (0)      654 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.copier-answers.yml
+-rw-r--r--   0 root         (0) root         (0)      708 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.coveragerc
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.642334 saltext_azurerm-4.1.0/.github/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.642334 saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 root         (0) root         (0)     1284 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0 root         (0) root         (0)      554 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/docs.md
+-rw-r--r--   0 root         (0) root         (0)      631 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 root         (0) root         (0)      431 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/tech-debt.md
+-rw-r--r--   0 root         (0) root         (0)      463 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE.md
+-rw-r--r--   0 root         (0) root         (0)      933 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.642334 saltext_azurerm-4.1.0/.github/workflows/
+-rw-r--r--   0 root         (0) root         (0)      383 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/workflows/pr.yml
+-rw-r--r--   0 root         (0) root         (0)      789 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.github/workflows/tag.yml
+-rw-r--r--   0 root         (0) root         (0)     1992 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.gitignore
+-rwxr-xr-x   0 root         (0) root         (0)     4447 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.pre-commit-config.yaml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.646334 saltext_azurerm-4.1.0/.pre-commit-hooks/
+-rw-r--r--   0 root         (0) root         (0)     2083 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.pre-commit-hooks/check-cli-examples.py
+-rw-r--r--   0 root         (0) root         (0)     3626 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.pre-commit-hooks/make-autodocs.py
+-rwxr-xr-x   0 root         (0) root         (0)    22081 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.pylintrc
+-rw-r--r--   0 root         (0) root         (0)      457 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/.readthedocs.yaml
+-rw-r--r--   0 root         (0) root         (0)     1713 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/CHANGELOG.md
+-rw-r--r--   0 root         (0) root         (0)     5280 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/CODE-OF-CONDUCT.md
+-rw-r--r--   0 root         (0) root         (0)      703 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/CONTRIBUTING.md
+-rw-r--r--   0 root         (0) root         (0)    11352 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      481 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/NOTICE.txt
+-rw-r--r--   0 root         (0) root         (0)     6205 2024-04-23 22:38:52.670334 saltext_azurerm-4.1.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2980 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.646334 saltext_azurerm-4.1.0/changelog/
+-rw-r--r--   0 root         (0) root         (0)      309 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/changelog/.template.jinja
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.646334 saltext_azurerm-4.1.0/docs/
+-rw-r--r--   0 root         (0) root         (0)      634 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/Makefile
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.646334 saltext_azurerm-4.1.0/docs/_static/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/_static/.gitkeep
+-rw-r--r--   0 root         (0) root         (0)      282 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/changelog.md
+-rwxr-xr-x   0 root         (0) root         (0)     6253 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/conf.py
+-rw-r--r--   0 root         (0) root         (0)      585 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/index.rst
+-rw-r--r--   0 root         (0) root         (0)      760 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/make.bat
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.646334 saltext_azurerm-4.1.0/docs/ref/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/.gitkeep
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.646334 saltext_azurerm-4.1.0/docs/ref/clouds/
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/clouds/index.rst
+-rw-r--r--   0 root         (0) root         (0)       86 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/clouds/saltext.azurerm.clouds.azurerm.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.646334 saltext_azurerm-4.1.0/docs/ref/fileserver/
+-rw-r--r--   0 root         (0) root         (0)      185 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/fileserver/index.rst
+-rw-r--r--   0 root         (0) root         (0)       90 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/fileserver/saltext.azurerm.fileserver.azurefs.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.650334 saltext_azurerm-4.1.0/docs/ref/modules/
+-rw-r--r--   0 root         (0) root         (0)      533 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/index.rst
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute.rst
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_availability_set.rst
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_disk.rst
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_image.rst
+-rw-r--r--   0 root         (0) root         (0)      159 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine.rst
+-rw-r--r--   0 root         (0) root         (0)      189 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_extension.rst
+-rw-r--r--   0 root         (0) root         (0)      177 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_image.rst
+-rw-r--r--   0 root         (0) root         (0)       99 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_dns.rst
+-rw-r--r--   0 root         (0) root         (0)      126 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_key.rst
+-rw-r--r--   0 root         (0) root         (0)      135 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_secret.rst
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_vault.rst
+-rw-r--r--   0 root         (0) root         (0)      111 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_network.rst
+-rw-r--r--   0 root         (0) root         (0)      114 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/modules/saltext.azurerm.modules.azurerm_resource.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.650334 saltext_azurerm-4.1.0/docs/ref/states/
+-rw-r--r--   0 root         (0) root         (0)      380 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/index.rst
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_compute.rst
+-rw-r--r--   0 root         (0) root         (0)      161 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_compute_availability_set.rst
+-rw-r--r--   0 root         (0) root         (0)      158 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_compute_virtual_machine.rst
+-rw-r--r--   0 root         (0) root         (0)       98 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_dns.rst
+-rw-r--r--   0 root         (0) root         (0)      125 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_key.rst
+-rw-r--r--   0 root         (0) root         (0)      134 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_secret.rst
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_keyvault_vault.rst
+-rw-r--r--   0 root         (0) root         (0)      110 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_network.rst
+-rw-r--r--   0 root         (0) root         (0)      113 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/states/saltext.azurerm.states.azurerm_resource.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.650334 saltext_azurerm-4.1.0/docs/ref/utils/
+-rw-r--r--   0 root         (0) root         (0)      158 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/utils/index.rst
+-rw-r--r--   0 root         (0) root         (0)      121 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/utils/saltext.azurerm.utils.azurerm.rst
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/ref/utils/saltext.azurerm.utils.rst
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/sitevars.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.654334 saltext_azurerm-4.1.0/docs/topics/
+-rw-r--r--   0 root         (0) root         (0)     5854 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/topics/authentication.rst
+-rw-r--r--   0 root         (0) root         (0)       80 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/topics/index.rst
+-rw-r--r--   0 root         (0) root         (0)      878 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/docs/topics/installation.md
+-rwxr-xr-x   0 root         (0) root         (0)    17686 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/noxfile.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-23 22:38:52.670334 saltext_azurerm-4.1.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      132 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.638334 saltext_azurerm-4.1.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.638334 saltext_azurerm-4.1.0/src/saltext/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.654334 saltext_azurerm-4.1.0/src/saltext/azurerm/
+-rw-r--r--   0 root         (0) root         (0)      863 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.654334 saltext_azurerm-4.1.0/src/saltext/azurerm/clouds/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/clouds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    61524 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/clouds/azurerm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.654334 saltext_azurerm-4.1.0/src/saltext/azurerm/fileserver/
+-rw-r--r--   0 root         (0) root         (0)    14499 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/fileserver/azurefs.py
+-rw-r--r--   0 root         (0) root         (0)      803 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/loader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.658334 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/
+-rw-r--r--   0 root         (0) root         (0)       35 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14037 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute.py
+-rw-r--r--   0 root         (0) root         (0)     7432 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_availability_set.py
+-rw-r--r--   0 root         (0) root         (0)     5678 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_disk.py
+-rw-r--r--   0 root         (0) root         (0)     8485 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_image.py
+-rw-r--r--   0 root         (0) root         (0)    59121 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine.py
+-rw-r--r--   0 root         (0) root         (0)     7019 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_extension.py
+-rw-r--r--   0 root         (0) root         (0)     6331 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_image.py
+-rw-r--r--   0 root         (0) root         (0)    20196 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_dns.py
+-rw-r--r--   0 root         (0) root         (0)    23571 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_keyvault_key.py
+-rw-r--r--   0 root         (0) root         (0)    16683 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_keyvault_secret.py
+-rw-r--r--   0 root         (0) root         (0)    19428 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_keyvault_vault.py
+-rw-r--r--   0 root         (0) root         (0)    86213 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_network.py
+-rw-r--r--   0 root         (0) root         (0)    38004 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.662334 saltext_azurerm-4.1.0/src/saltext/azurerm/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6202 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_compute.py
+-rw-r--r--   0 root         (0) root         (0)     9466 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_compute_availability_set.py
+-rw-r--r--   0 root         (0) root         (0)    37173 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_compute_virtual_machine.py
+-rw-r--r--   0 root         (0) root         (0)    26095 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_dns.py
+-rw-r--r--   0 root         (0) root         (0)     8640 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_keyvault_key.py
+-rw-r--r--   0 root         (0) root         (0)    10292 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_keyvault_secret.py
+-rw-r--r--   0 root         (0) root         (0)    18329 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_keyvault_vault.py
+-rw-r--r--   0 root         (0) root         (0)    89365 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_network.py
+-rw-r--r--   0 root         (0) root         (0)    26884 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.662334 saltext_azurerm-4.1.0/src/saltext/azurerm/utils/
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13291 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/utils/azurerm.py
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext/azurerm/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6205 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5577 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       48 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-23 22:38:52.000000 saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.662334 saltext_azurerm-4.1.0/tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.662334 saltext_azurerm-4.1.0/tests/functional/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/functional/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3500 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/functional/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.662334 saltext_azurerm-4.1.0/tests/integration/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.662334 saltext_azurerm-4.1.0/tests/integration/clouds/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/clouds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5471 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.662334 saltext_azurerm-4.1.0/tests/integration/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/tests/integration/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2863 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_compute_availability_set.py
+-rw-r--r--   0 root         (0) root         (0)     4431 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_compute_virtual_machine.py
+-rw-r--r--   0 root         (0) root         (0)     5685 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_dns.py
+-rw-r--r--   0 root         (0) root         (0)     3618 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_keyvault_key.py
+-rw-r--r--   0 root         (0) root         (0)     4308 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_keyvault_secret.py
+-rw-r--r--   0 root         (0) root         (0)     7848 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_keyvault_vault.py
+-rw-r--r--   0 root         (0) root         (0)     3444 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_network_interface.py
+-rw-r--r--   0 root         (0) root         (0)     5926 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_network_route.py
+-rw-r--r--   0 root         (0) root         (0)     6618 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_network_security_group.py
+-rw-r--r--   0 root         (0) root         (0)     5613 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_public_ip_address.py
+-rw-r--r--   0 root         (0) root         (0)     2285 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_resource_group.py
+-rw-r--r--   0 root         (0) root         (0)     8898 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/states/test_virtual_network.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/tests/integration/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/integration/utils/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/tests/unit/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/unit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/tests/unit/clouds/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/unit/clouds/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1683 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/unit/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/tests/unit/modules/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/unit/modules/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/tests/unit/states/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/unit/states/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-23 22:38:52.666334 saltext_azurerm-4.1.0/tests/unit/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/unit/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8157 2024-04-23 22:38:47.000000 saltext_azurerm-4.1.0/tests/unit/utils/test_azurerm.py
```

### Comparing `saltext.azurerm-4.0.1/.coveragerc` & `saltext_azurerm-4.1.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/bug_report.md` & `saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 name: Bug report
 about: Create a report to help us improve
 title: "[BUG]"
-labels: bug, needs triage
+labels: bug, needs-triage
 assignees: ''
 
 ---
 
 **Description**
 A clear and concise description of what the bug is.
 
@@ -17,14 +17,17 @@
 
 - [ ] on-prem machine
 - [ ] VM (Virtualbox, KVM, etc. please specify)
 - [ ] VM running on a cloud service, please be explicit and add details
 - [ ] container (Kubernetes, Docker, containerd, etc. please specify)
 - [ ] or a combination, please be explicit
 - [ ] jails if it is FreeBSD
+- [ ] classic packaging
+- [ ] onedir packaging
+- [ ] used bootstrap to install
 
 
 **Steps to Reproduce the behavior**
 (Include debug logs if possible and relevant)
 
 **Expected behavior**
 A clear and concise description of what you expected to happen.
@@ -32,14 +35,14 @@
 **Screenshots**
 If applicable, add screenshots to help explain your problem.
 
 **Versions Report**
 <details><summary>salt --versions-report</summary>
 (Provided by running salt --versions-report. Please also mention any differences in master/minion versions.)
 
-```
+```yaml
 PASTE HERE
 ```
 </details>
 
 **Additional context**
 Add any other context about the problem here.
```

### Comparing `saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/config.yml` & `saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/config.yml`

 * *Files 26% similar despite different names*

```diff
@@ -6,9 +6,9 @@
   - name: Salt-Users Forum
     url: https://groups.google.com/forum/#!forum/salt-users
     about: Please ask and answer questions here.
   - name: Salt on LiberaChat
     url: https://web.libera.chat/#salt
     about: Please ask and answer questions here.
   - name: Security vulnerabilities
-    email: security@saltstack.com
+    email: saltproject-security.pdl@broadcom.com
     about: Please report security vulnerabilities here.
```

### Comparing `saltext.azurerm-4.0.1/.github/ISSUE_TEMPLATE/feature_request.md` & `saltext_azurerm-4.1.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 ---
 name: Feature request
 about: Suggest an idea for this project
 title: "[FEATURE REQUEST]"
-labels: enhancement, needs triage
+labels: feature, needs-triage
 assignees: ''
 
 ---
 
 **Is your feature request related to a problem? Please describe.**
 A clear and concise description of what the problem is. Ex. I'm always frustrated when [...]
```

### Comparing `saltext.azurerm-4.0.1/.github/PULL_REQUEST_TEMPLATE.md` & `saltext_azurerm-4.1.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/.gitignore` & `saltext_azurerm-4.1.0/.gitignore`

 * *Files 8% similar despite different names*

```diff
@@ -106,20 +106,14 @@
 .venv
 env/
 venv/
 ENV/
 env.bak/
 venv.bak/
 
-# vscode
-.vscode/
-
-#salt env
-Saltfile
-
 # Spyder project settings
 .spyderproject
 .spyproject
 
 # Rope project settings
 .ropeproject
 
@@ -130,19 +124,21 @@
 .mypy_cache/
 .dmypy.json
 dmypy.json
 
 # Pyre type checker
 .pyre/
 
+# Ignore the setuptools_scm auto-generated version module
+src/saltext/azurerm/version.py
+
 # Ignore CI generated artifacts
 artifacts/
 
-# Just a dir for local whatever
-local/
-
+# IDE
+.vscode/
 .DS_Store
 .idea/
-src/.DS_Store
-src/saltext/.DS_Store
-.vscode/
 *.swp
+
+#salt env
+Saltfile
```

### Comparing `saltext.azurerm-4.0.1/.pre-commit-hooks/check-cli-examples.py` & `saltext_azurerm-4.1.0/.pre-commit-hooks/check-cli-examples.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import ast
 import pathlib
 import re
 import sys
 
 CODE_ROOT = pathlib.Path(__file__).resolve().parent.parent
-EXECUTION_MODULES_PATH = CODE_ROOT / "src" / "saltext" / " azurerm" / "modules"
+EXECUTION_MODULES_PATH = CODE_ROOT / "src" / "saltext" / "azurerm" / "modules"
 
 
 def check_cli_examples(files):
     """
     Check that every function on every execution module provides a CLI example
     """
     errors = 0
```

### Comparing `saltext.azurerm-4.0.1/CHANGELOG.md` & `saltext_azurerm-4.1.0/CHANGELOG.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,26 @@
 The changelog format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/).
 
 This project uses [Semantic Versioning](https://semver.org/) - MAJOR.MINOR.PATCH
 
 # Changelog
 
+## 4.1.0 (2024-04-22)
+
+
+### Fixed
+
+- Fixed TypeError for ManagedIdentityCredential when using service principal credentials. [#46](https://github.com/salt-extensions/saltext-azurerm/issues/46)
+
+
+### Added
+
+- Set Virtual Machine Tags via Salt Cloud [#47](https://github.com/salt-extensions/saltext-azurerm/issues/47)
+
+
 # Saltext.Azurerm 4.0.1 (2023-08-14)
 
 ### Fixed
 
 - Fix NameError for __salt__ access and a public IP KeyError (#40)
```

### Comparing `saltext.azurerm-4.0.1/CODE-OF-CONDUCT.md` & `saltext_azurerm-4.1.0/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/CONTRIBUTING.md` & `saltext_azurerm-4.1.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/LICENSE` & `saltext_azurerm-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/README.md` & `saltext_azurerm-4.1.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # Salt Extension Modules for Azure Resource Manager
 
 [![Documentation Status](https://readthedocs.org/projects/saltext-azurerm/badge/?version=latest)](https://saltext-azurerm.readthedocs.io/en/latest/?badge=latest)
 
-This is a collection of Salt extension modules for use with  Microsoft Azure Resource Manager
+Salt Extension for interacting with Microsoft Azure
 
 ## Security
 
 If you think you've found a security vulnerability, see
 [Salt's security guide][security].
 
 ## User Documentation
@@ -18,57 +18,58 @@
 
 The saltext-azurerm project team welcomes contributions from the community.
 
 The [Salt Contributing guide][salt-contributing] has a lot of relevant
 information, but if you'd like to jump right in here's how to get started:
 
 
-    # Clone the repo
-    git clone --origin salt git@github.com:salt-extensions/saltext-azurerm.git
+```bash
+# Clone the repo
+git clone --origin salt git@github.com:salt-extensions/saltext-azurerm.git
 
-    # Change to the repo dir
-    cd saltext-azurerm
+# Change to the repo dir
+cd saltext-azurerm
 
-    # Create a new venv
-    python3 -m venv env --prompt azurerm
-    source env/bin/activate
+# Create a new venv
+python3 -m venv env --prompt saltext-azurerm
+source env/bin/activate
 
-    # On mac, you may need to upgrade pip
-    python -m pip install --upgrade pip
+# On mac, you may need to upgrade pip
+python -m pip install --upgrade pip
 
-    # On WSL or some flavors of linux you may need to install the `enchant`
-    # library in order to build the docs
-    sudo apt-get install -y enchant
+# On WSL or some flavors of linux you may need to install the `enchant`
+# library in order to build the docs
+sudo apt-get install -y enchant
 
-    # Install extension + test/dev/doc dependencies into your environment
-    python -m pip install -e .[tests,dev,docs]
+# Install extension + test/dev/doc dependencies into your environment
+python -m pip install -e '.[tests,dev,docs]'
 
-    # Run tests!
-    python -m nox -e tests-3
+# Run tests!
+python -m nox -e tests-3
 
-    # skip requirements install for next time
-    export SKIP_REQUIREMENTS_INSTALL=1
-
-    # Build the docs, serve, and view in your web browser:
-    python -m nox -e docs && (cd docs/_build/html; python -m webbrowser localhost:8000; python -m http.server; cd -)
+# skip requirements install for next time
+export SKIP_REQUIREMENTS_INSTALL=1
 
+# Build the docs, serve, and view in your web browser:
+python -m nox -e docs && (cd docs/_build/html; python -m webbrowser localhost:8000; python -m http.server; cd -)
+```
 
 Writing code isn't the only way to contribute! We value contributions in any of
 these areas:
 
 * Documentation - especially examples of how to use this module to solve
   specific problems.
 * Triaging [issues][issues] and participating in [discussions][discussions]
 * Reviewing [Pull Requests][PRs] (we really like
   [Conventional Comments][comments]!)
 
 You could also contribute in other ways:
 
 * Writing blog posts
-* Posting on social media about how you used Salt+Prometheus to solve your
+* Posting on social media about how you used Salt+Azurerm to solve your
   problems, including videos
 * Giving talks at conferences
 * Publishing videos
 * Asking/answering questions in IRC, Slack, or email groups
 
 Any of these things are super valuable to our community, and we sincerely
 appreciate every contribution!
```

### Comparing `saltext.azurerm-4.0.1/docs/Makefile` & `saltext_azurerm-4.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/docs/conf.py` & `saltext_azurerm-4.1.0/docs/conf.py`

 * *Files 16% similar despite different names*

```diff
@@ -5,30 +5,34 @@
 # https://www.sphinx-doc.org/en/master/usage/configuration.html
 # -- Path setup --------------------------------------------------------------
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
 #
 import datetime
+import email.policy
 import os
 import sys
+from pathlib import Path
 
 try:
     from importlib_metadata import distribution
 except ImportError:
     from importlib.metadata import distribution
 
 
 try:
     docs_basepath = os.path.abspath(os.path.dirname(__file__))
 except NameError:
     # sphinx-intl and six execute some code which will raise this NameError
     # assume we're in the doc/ directory
     docs_basepath = os.path.abspath(os.path.dirname("."))
 
+PROJECT_ROOT_DIR = Path(docs_basepath).parent
+
 addtl_paths = (
     os.path.join(os.pardir, "src"),  # saltext.azurerm itself (for autodoc)
     "_ext",  # custom Sphinx extensions
 )
 
 for addtl_path in addtl_paths:
     sys.path.insert(0, os.path.abspath(os.path.join(docs_basepath, addtl_path)))
@@ -40,14 +44,27 @@
 this_year = datetime.datetime.today().year
 if this_year == 2021:
     copyright_year = 2021
 else:
     copyright_year = f"2021 - {this_year}"
 project = dist.metadata["Summary"]
 author = dist.metadata["Author"]
+
+if author is None:
+    # Core metadata is serialized differently with pyproject.toml:
+    # https://packaging.python.org/en/latest/specifications/pyproject-toml/#authors-maintainers
+    author_email = dist.metadata["Author-email"]
+    em = email.message_from_string(
+        f"To: {author_email}",
+        policy=email.policy.default,
+    )
+    if em["To"].addresses and em["To"].addresses[0]:
+        author = em["To"].addresses[0].display_name
+    author = author or ""
+
 copyright = f"{copyright_year}, {author}"
 
 # The full version, including alpha/beta/rc tags
 release = dist.version
 
 
 # Variables to pass into the docs from sitevars.rst for rst substitution
@@ -71,14 +88,23 @@
     "sphinx.ext.napoleon",
     "sphinx.ext.intersphinx",
     "sphinx.ext.viewcode",
     "sphinx.ext.todo",
     "sphinx.ext.coverage",
     "sphinx_copybutton",
     "sphinxcontrib.spelling",
+    "sphinxcontrib.towncrier.ext",
+    "myst_parser",
+    "sphinx_inline_tabs",
+]
+
+myst_enable_extensions = [
+    "colon_fence",
+    "deflist",
+    "tasklist",
 ]
 
 # Add any paths that contain templates here, relative to this directory.
 templates_path = ["_templates"]
 
 # List of patterns, relative to source directory, that match files and
 # directories to ignore when looking for source files.
@@ -93,14 +119,16 @@
     ".gitlab-ci",
     ".gitignore",
     "sitevars.rst",
 ]
 
 autosummary_generate = False
 
+suppress_warnings = ["myst.header"]
+
 # -- Options for HTML output -------------------------------------------------
 
 # The theme to use for HTML and HTML Help pages.  See the documentation for
 # a list of builtin themes.
 #
 html_theme = "furo"
 html_title = project
@@ -132,24 +160,29 @@
 napoleon_use_ivar = False
 napoleon_use_param = True
 napoleon_use_rtype = True
 
 # ----- Intersphinx Config ---------------------------------------------------------------------------------------->
 intersphinx_mapping = {
     "python": ("https://docs.python.org/3", None),
-    "pytest": ("https://pytest.readthedocs.io/en/stable", None),
+    "pytest": ("https://docs.pytest.org/en/stable", None),
     "salt": ("https://docs.saltproject.io/en/latest", None),
 }
 # <---- Intersphinx Config -----------------------------------------------------------------------------------------
 
 # ----- Autodoc Config ---------------------------------------------------------------------------------------------->
 autodoc_default_options = {"member-order": "bysource"}
 autodoc_mock_imports = ["salt"]
 # <---- Autodoc Config -----------------------------------------------------------------------------------------------
 
+# Towncrier draft config
+towncrier_draft_autoversion_mode = "sphinx-release"
+towncrier_draft_include_empty = True
+towncrier_draft_working_directory = str(PROJECT_ROOT_DIR)
+
 
 def setup(app):
     app.add_crossref_type(
         directivename="fixture",
         rolename="fixture",
         indextemplate="pair: %s; fixture",
     )
```

### Comparing `saltext.azurerm-4.0.1/docs/make.bat` & `saltext_azurerm-4.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/docs/topics/authentication.rst` & `saltext_azurerm-4.1.0/docs/topics/authentication.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,34 +1,34 @@
 ======================
 Authentication Systems
 ======================
 
-This system has migrated from the older version management library (``msrestazure``) to 
+This system has migrated from the older version management library (``msrestazure``) to
 using the systems supported through ``azure-identity``.
 
 Azure Identity Authentication
 =============================
 The `azure identity library <https://docs.microsoft.com/en-us/python/api/azure-
-identity/azure.identity?view=azure-python>`_ offers many different credentials to 
-generate for Azure SDK Clients. The different login mechanisms that are supported by this 
-code include ``ClientSecretCredential``, ``UsernamePasswordCredential``, and 
-``DefaultAzureCredential``, respectively. Based on the different parameters provided in 
-either the function call or the testing (``.sls``) file, the user can decide which 
+identity/azure.identity?view=azure-python>`_ offers many different credentials to
+generate for Azure SDK Clients. The different login mechanisms that are supported by this
+code include ``ClientSecretCredential``, ``UsernamePasswordCredential``, and
+``DefaultAzureCredential``, respectively. Based on the different parameters provided in
+either the function call or the testing (``.sls``) file, the user can decide which
 authentication mechanisms to activate.
 
 ClientSecretCredential
 ======================
-The ``ClientSecretCredential`` authenticates a service principal using a client secret. 
-This credential was updated from msrestazure's ``ServicePrincipalCredentials``, 
-maintaining the same functionality but allowing the code to be more adaptable to updated 
-dependencies. It is the first authentication option in the code, requiring the ``client 
-ID``, ``client secret``, ``tenant ID``, and ``subscription ID``. This type of 
-authentication is ideal for controlling which resources can be accessed and level of 
+The ``ClientSecretCredential`` authenticates a service principal using a client secret.
+This credential was updated from msrestazure's ``ServicePrincipalCredentials``,
+maintaining the same functionality but allowing the code to be more adaptable to updated
+dependencies. It is the first authentication option in the code, requiring the ``client
+ID``, ``client secret``, ``tenant ID``, and ``subscription ID``. This type of
+authentication is ideal for controlling which resources can be accessed and level of
 access. The ``client secret`` is `generated <https://docs.microsoft.com/en-us/azure/active-
-directory/develop/quickstart-register-app#add-credentials>`_ for App Registration. 
+directory/develop/quickstart-register-app#add-credentials>`_ for App Registration.
 This information is provided to salt through pillar in the ``test.sls`` file:
 
 .. code-block:: yaml
 
         azurerm:
             mysubscription:
                 subscription_id: 3287abc8-f98a-c678-3bde-326766fd3617
@@ -49,23 +49,23 @@
                 - tags:
                     how_awesome: very
                     contact_name: Elmer Fudd Gantry
                 - connection_auth: {{ profile }}
 
 UsernamePasswordCredential
 ==========================
-The ``UsernamePasswordCredential`` authenticates a user using work and school accounts' 
-usernames and passwords (Microsoft accounts are not supported). This credential was 
-updated from msrestazure's ``UserPassCredentials``, also maintaining functionality while 
-being compatible with updated dependencies. This is the second authentication option in 
-the code and requires a ``username``, ``password``, and ``subscription ID``. This type of authentication 
-is not as recommended as the other types because it is not as secure or compatible with 
-other functionalities (such as multi-factor authentication and consent prompting). This 
-information can be provided to Salt through the testing file, similar to the example 
-above, but with changed variables. This information is also passed through Salt by pillar 
+The ``UsernamePasswordCredential`` authenticates a user using work and school accounts'
+usernames and passwords (Microsoft accounts are not supported). This credential was
+updated from msrestazure's ``UserPassCredentials``, also maintaining functionality while
+being compatible with updated dependencies. This is the second authentication option in
+the code and requires a ``username``, ``password``, and ``subscription ID``. This type of authentication
+is not as recommended as the other types because it is not as secure or compatible with
+other functionalities (such as multi-factor authentication and consent prompting). This
+information can be provided to Salt through the testing file, similar to the example
+above, but with changed variables. This information is also passed through Salt by pillar
 in the ``test.sls`` file:
 
 .. code-block:: yaml
 
         azurerm:
             user_pass_auth:
                 subscription_id: 3287abc8-f98a-c678-3bde-326766fd3617
@@ -86,30 +86,30 @@
                     contact_name: Elmer Fudd Gantry
                 - connection_auth: {{ profile }}
 
 
 
 DefaultAzureCredential
 ======================
-The ``DefaultAzureCredential`` authenticates  when no other specifications are provided. 
-This credential was updated from msrestazure's ``MSIAuthentication``, so it now allows 
-the user to get the access tokens rather than just setting them. This type of 
-authentication is the last and default authentication option. Based on different 
-situations, DefaultAzureCredential automatically goes through multiple different 
+The ``DefaultAzureCredential`` authenticates  when no other specifications are provided.
+This credential was updated from msrestazure's ``MSIAuthentication``, so it now allows
+the user to get the access tokens rather than just setting them. This type of
+authentication is the last and default authentication option. Based on different
+situations, DefaultAzureCredential automatically goes through multiple different
 mechanisms and detects the best fit authentication method:
 
 #. Environment: Authenticates using `environment variables <https://docs.microsoft.com/en-us/python/api/azure-
    identity/azure.identity.environmentcredential?view=azure-python>`_.
 #. Managed Identity: Authenticates with managed identity if the application is deployed to an Azure host.
 #. VS Code: Authenticates as the VS Code Azure Account Extension user if signed in.
 #. Azure CLI: Authenticates as the Azure CLI user if signed in (via ``az login`` command)
 #. Azure PowerShell: Authenticates as the Azure PowerShell user if signed in (via ``Connect-AzAccount`` command)
 #. Interactive Browser: Authenticates a user via default browser
 
-To implement, no pillar is needed, as it authenticates without those extra parameters and 
+To implement, no pillar is needed, as it authenticates without those extra parameters and
 only the subscription id in the ``test.sls`` file:
 
 .. code-block:: jinja
 
         {% set profile = {"subscription_id" : "3287abc8-f98a-c678-3bde-326766fd3617"} %}
         Ensure resource group exists:
             azurerm_resource.resource_group_present:
@@ -117,10 +117,9 @@
                 - location: westus
                 - tags:
                     how_awesome: very
                     contact_name: Elmer Fudd Gantry
                 - connection_auth: {{ profile }}
 
 
-Because of its flexibility, ``DefaultAzureCredential`` is the preferred method of 
-authentication. 
-
+Because of its flexibility, ``DefaultAzureCredential`` is the preferred method of
+authentication.
```

### Comparing `saltext.azurerm-4.0.1/noxfile.py` & `saltext_azurerm-4.1.0/noxfile.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,68 +15,68 @@
 # Nox options
 #  Reuse existing virtualenvs
 nox.options.reuse_existing_virtualenvs = True
 #  Don't fail on missing interpreters
 nox.options.error_on_missing_interpreters = False
 
 # Python versions to test against
-PYTHON_VERSIONS = ("3", "3.5", "3.6", "3.7", "3.8", "3.9", "3.10")
+PYTHON_VERSIONS = ("3", "3.8", "3.9", "3.10")
 # Be verbose when running under a CI context
 CI_RUN = (
     os.environ.get("JENKINS_URL") or os.environ.get("CI") or os.environ.get("DRONE") is not None
 )
 PIP_INSTALL_SILENT = CI_RUN is False
 SKIP_REQUIREMENTS_INSTALL = "SKIP_REQUIREMENTS_INSTALL" in os.environ
 EXTRA_REQUIREMENTS_INSTALL = os.environ.get("EXTRA_REQUIREMENTS_INSTALL")
 
 COVERAGE_VERSION_REQUIREMENT = "coverage==5.2"
-SALT_REQUIREMENT = os.environ.get("SALT_REQUIREMENT") or "salt>=3006.1"
+SALT_REQUIREMENT = os.environ.get("SALT_REQUIREMENT") or "salt>=3005"
 if SALT_REQUIREMENT == "salt==master":
     SALT_REQUIREMENT = "git+https://github.com/saltstack/salt.git@master"
 
 # Prevent Python from writing bytecode
 os.environ["PYTHONDONTWRITEBYTECODE"] = "1"
 
 # Global Path Definitions
 REPO_ROOT = pathlib.Path(__file__).resolve().parent
 # Change current directory to REPO_ROOT
 os.chdir(str(REPO_ROOT))
 
 ARTIFACTS_DIR = REPO_ROOT / "artifacts"
 # Make sure the artifacts directory exists
 ARTIFACTS_DIR.mkdir(parents=True, exist_ok=True)
-RUNTESTS_LOGFILE = ARTIFACTS_DIR / "runtests-{}.log".format(
-    datetime.datetime.now().strftime("%Y%m%d%H%M%S.%f")
-)
+CUR_TIME = datetime.datetime.now().strftime("%Y%m%d%H%M%S.%f")
+RUNTESTS_LOGFILE = ARTIFACTS_DIR / f"runtests-{CUR_TIME}.log"
 COVERAGE_REPORT_DB = REPO_ROOT / ".coverage"
 COVERAGE_REPORT_PROJECT = ARTIFACTS_DIR.relative_to(REPO_ROOT) / "coverage-project.xml"
 COVERAGE_REPORT_TESTS = ARTIFACTS_DIR.relative_to(REPO_ROOT) / "coverage-tests.xml"
 JUNIT_REPORT = ARTIFACTS_DIR.relative_to(REPO_ROOT) / "junit-report.xml"
 
 
 def _get_session_python_version_info(session):
     try:
         version_info = session._runner._real_python_version_info
     except AttributeError:
         session_py_version = session.run_always(
             "python",
-            "-c" 'import sys; sys.stdout.write("{}.{}.{}".format(*sys.version_info))',
+            "-c",
+            'import sys; sys.stdout.write("{}.{}.{}".format(*sys.version_info))',
             silent=True,
             log=False,
         )
         version_info = tuple(int(part) for part in session_py_version.split(".") if part.isdigit())
         session._runner._real_python_version_info = version_info
     return version_info
 
 
 def _get_pydir(session):
     version_info = _get_session_python_version_info(session)
-    if version_info < (3, 5):
-        session.error("Only Python >= 3.5 is supported")
-    return "py{}.{}".format(*version_info)
+    if version_info < (3, 8):
+        session.error("Only Python >= 3.8 is supported")
+    return f"py{version_info[0]}.{version_info[1]}"
 
 
 def _install_requirements(
     session,
     *passed_requirements,  # pylint: disable=unused-argument
     install_coverage_requirements=True,
     install_test_requirements=True,
@@ -286,34 +286,30 @@
             contents = stdout.read()
             if contents:
                 contents = contents.decode("utf-8")
                 sys.stdout.write(contents)
                 sys.stdout.flush()
                 if pylint_report_path:
                     # Write report
-                    with open(  # pylint: disable=unspecified-encoding
-                        pylint_report_path, "w"
-                    ) as wfh:
+                    with open(pylint_report_path, "w", encoding="utf-8") as wfh:
                         wfh.write(contents)
                     session.log("Report file written to %r", pylint_report_path)
             stdout.close()
 
 
 def _lint_pre_commit(session, rcfile, flags, paths):
     if "VIRTUAL_ENV" not in os.environ:
         session.error(
             "This should be running from within a virtualenv and "
             "'VIRTUAL_ENV' was not found as an environment variable."
         )
     if "pre-commit" not in os.environ["VIRTUAL_ENV"]:
         session.error(
             "This should be running from within a pre-commit virtualenv and "
-            "'VIRTUAL_ENV'({}) does not appear to be a pre-commit virtualenv.".format(
-                os.environ["VIRTUAL_ENV"]
-            )
+            f"'VIRTUAL_ENV'({os.environ['VIRTUAL_ENV']}) does not appear to be a pre-commit virtualenv."
         )
 
     # Let's patch nox to make it run inside the pre-commit virtualenv
     session._runner.venv = VirtualEnv(
         os.environ["VIRTUAL_ENV"],
         interpreter=session._runner.func.python,
         reuse_existing=True,
@@ -485,28 +481,23 @@
             "python",
             "-c",
             "import json; import conf; print(json.dumps(conf.intersphinx_mapping))",
             silent=True,
             log=False,
         )
     )
+    intersphinx_mapping_list = ", ".join(list(intersphinx_mapping))
     try:
         mapping_entry = intersphinx_mapping[session.posargs[0]]
     except IndexError:
         session.error(
-            "You need to pass at least one argument whose value must be one of: {}".format(
-                ", ".join(list(intersphinx_mapping))
-            )
+            f"You need to pass at least one argument whose value must be one of: {intersphinx_mapping_list}"
         )
     except KeyError:
-        session.error(
-            "Only acceptable values for first argument are: {}".format(
-                ", ".join(list(intersphinx_mapping))
-            )
-        )
+        session.error(f"Only acceptable values for first argument are: {intersphinx_mapping_list}")
     session.run(
         "python", "-m", "sphinx.ext.intersphinx", mapping_entry[0].rstrip("/") + "/objects.inv"
     )
     os.chdir(str(REPO_ROOT))
 
 
 @nox.session(name="gen-api-docs", python="3")
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/__init__.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/__init__.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/clouds/azurerm.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/clouds/azurerm.py`

 * *Files 5% similar despite different names*

```diff
@@ -695,15 +695,17 @@
 
     if kwargs.get("network_resource_group") is None:
         kwargs["network_resource_group"] = config.get_cloud_config_value(
             "resource_group", vm_, __opts__, search_global=False
         )
 
     if kwargs.get("iface_name") is None:
-        kwargs["iface_name"] = "{}-iface0".format(vm_["name"])
+        kwargs["iface_name"] = "{}-iface0".format(  # pylint: disable=consider-using-f-string
+            vm_["name"]
+        )
 
     # Handle IP configuration based on provided parameters
     ip_kwargs = {}
     ip_configurations = None
 
     if "load_balancer_backend_address_pools" in kwargs:
         ip_kwargs["load_balancer_backend_address_pools"] = kwargs[
@@ -712,36 +714,40 @@
     if "private_ip_address" in kwargs.keys():
         ip_kwargs["private_ip_address"] = kwargs["private_ip_address"]
         ip_kwargs["private_ip_allocation_method"] = IPAllocationMethod.static
     else:
         ip_kwargs["private_ip_allocation_method"] = IPAllocationMethod.dynamic
 
     if kwargs.get("allocate_public_ip") is True:
-        pub_ip_name = "{}-ip".format(kwargs["iface_name"])
+        pub_ip_name = "{}-ip".format(  # pylint: disable=consider-using-f-string
+            kwargs["iface_name"]
+        )
         pub_ip_data = __salt__["azurerm_network.public_ip_address_create_or_update"](
             name=pub_ip_name, resource_group=kwargs["resource_group"], **conn_kwargs
         )
 
         ip_kwargs["public_ip_address"] = PublicIPAddress(
             id=str(pub_ip_data["id"]),
         )
         ip_kwargs["name"] = pub_ip_name
         ip_configurations = [ip_kwargs]
     else:
-        priv_ip_name = "{}-ip".format(kwargs["iface_name"])
+        priv_ip_name = "{}-ip".format(  # pylint: disable=consider-using-f-string
+            kwargs["iface_name"]
+        )
         ip_kwargs["name"] = priv_ip_name
         ip_configurations = [ip_kwargs]
     # pylint: disable=unused-variable
     netiface = __salt__["azurerm_network.network_interface_create_or_update"](
         name=kwargs["iface_name"],
         ip_configurations=ip_configurations,
         subnet=kwargs["subnet"],
         virtual_network=kwargs["network"],
         resource_group=kwargs["resource_group"],
-        **conn_kwargs
+        **conn_kwargs,
     )
 
     return _get_network_interface(kwargs["iface_name"], kwargs["resource_group"])
 
 
 def request_instance(vm_, kwargs=None):
     """
@@ -800,15 +806,15 @@
     if vm_.get("name") is None:
         vm_["name"] = config.get_cloud_config_value("name", vm_, __opts__, search_global=True)
 
     # pylint: disable=unused-variable
     iface_data, public_ips, private_ips = create_network_interface(call="action", kwargs=vm_)
     vm_["iface_id"] = iface_data["id"]
 
-    disk_name = "{}-vol0".format(vm_["name"])
+    disk_name = "{}-vol0".format(vm_["name"])  # pylint: disable=consider-using-f-string
 
     vm_username = config.get_cloud_config_value(
         "ssh_username",
         vm_,
         __opts__,
         search_global=True,
         default=config.get_cloud_config_value("win_username", vm_, __opts__, search_global=True),
@@ -820,15 +826,15 @@
     )
     if ssh_publickeyfile is not None:
         try:
             with salt.utils.files.fopen(ssh_publickeyfile, "r") as spkc_:
                 ssh_publickeyfile_contents = spkc_.read()
         except Exception as exc:  # pylint: disable=broad-except
             raise SaltCloudConfigError(  # pylint: disable=raise-missing-from
-                "Failed to read ssh publickey file '{}': {}".format(ssh_publickeyfile, exc.args[-1])
+                f"Failed to read ssh publickey file '{ssh_publickeyfile}': {exc.args[-1]}"
             )
 
     disable_password_authentication = config.get_cloud_config_value(
         "disable_password_authentication",
         vm_,
         __opts__,
         search_global=False,
@@ -838,15 +844,15 @@
     os_kwargs = {}
     win_installer = config.get_cloud_config_value(
         "win_installer", vm_, __opts__, search_global=True
     )
     if not win_installer and ssh_publickeyfile_contents is not None:
         sshpublickey = SshPublicKey(
             key_data=ssh_publickeyfile_contents,
-            path="/home/{}/.ssh/authorized_keys".format(vm_username),
+            path=f"/home/{vm_username}/.ssh/authorized_keys",
         )
         sshconfiguration = SshConfiguration(
             public_keys=[sshpublickey],
         )
         linuxconfiguration = LinuxConfiguration(
             disable_password_authentication=disable_password_authentication,
             ssh=sshconfiguration,
@@ -888,15 +894,15 @@
         os_kwargs["admin_password"] = vm_password
 
     availability_set = config.get_cloud_config_value(
         "availability_set", vm_, __opts__, search_global=False, default=None
     )
     if availability_set is not None and isinstance(availability_set, str):
         availability_set = {
-            "id": "/subscriptions/{}/resourceGroups/{}/providers/Microsoft.Compute/availabilitySets/{}".format(
+            "id": "/subscriptions/{}/resourceGroups/{}/providers/Microsoft.Compute/availabilitySets/{}".format(  # pylint: disable=consider-using-f-string
                 subscription_id, vm_["resource_group"], availability_set
             )
         }
     else:
         availability_set = None
 
     cloud_env = _get_cloud_environment()
@@ -920,15 +926,20 @@
         if isinstance(volume, str):
             volume = {"name": volume}
 
         volume.setdefault(
             "name",
             volume.get(
                 "name",
-                volume.get("name", "{}-datadisk{}".format(vm_["name"], str(lun))),
+                volume.get(
+                    "name",
+                    "{}-datadisk{}".format(  # pylint: disable=consider-using-f-string
+                        vm_["name"], str(lun)
+                    ),
+                ),
             ),
         )
 
         volume.setdefault(
             "disk_size_gb",
             volume.get("logical_disk_size_in_gb", volume.get("size", 100)),
         )
@@ -943,15 +954,15 @@
         lun += 1
         # The default vhd is {vm_name}-datadisk{lun}.vhd
         if "media_link" in volume:
             volume["vhd"] = VirtualHardDisk(uri=volume["media_link"])
             del volume["media_link"]
         elif volume.get("vhd") == "unmanaged":
             volume["vhd"] = VirtualHardDisk(
-                uri="https://{}.blob.{}/vhds/{}-datadisk{}.vhd".format(
+                uri="https://{}.blob.{}/vhds/{}-datadisk{}.vhd".format(  # pylint: disable=consider-using-f-string
                     vm_["storage_account"],
                     storage_endpoint_suffix,
                     vm_["name"],
                     volume["lun"],
                 ),
             )
         elif "vhd" in volume:
@@ -986,15 +997,15 @@
         else:
             os_type = "Linux"
         os_disk = OSDisk(
             caching=CachingTypes.none,
             create_option=DiskCreateOptionTypes.from_image,
             name=disk_name,
             vhd=VirtualHardDisk(
-                uri="https://{}.blob.{}/vhds/{}.vhd".format(
+                uri="https://{}.blob.{}/vhds/{}.vhd".format(  # pylint: disable=consider-using-f-string
                     vm_["storage_account"],
                     storage_endpoint_suffix,
                     disk_name,
                 ),
             ),
             os_type=os_type,
             image=source_image,
@@ -1103,20 +1114,23 @@
             image_reference=img_ref,
         ),
         os_profile=OSProfile(admin_username=vm_username, computer_name=vm_["name"], **os_kwargs),
         network_profile=NetworkProfile(
             network_interfaces=[NetworkInterfaceReference(id=vm_["iface_id"])],
         ),
         availability_set=availability_set,
+        tags=config.get_cloud_config_value(
+            "tags", vm_, __opts__, search_global=False, default=None
+        ),
     )
 
     salt.utils.cloud.fire_event(
         "event",
         "requesting instance",
-        "salt/cloud/{}/requesting".format(vm_["name"]),
+        "salt/cloud/{}/requesting".format(vm_["name"]),  # pylint: disable=consider-using-f-string
         args=__utils__["cloud.filter_event"](
             "requesting", vm_, ["name", "profile", "provider", "driver"]
         ),
         sock_dir=__opts__["sock_dir"],
         transport=__opts__["transport"],
     )
 
@@ -1160,15 +1174,15 @@
 
     if vm_.get("bootstrap_interface") is None:
         vm_["bootstrap_interface"] = "public"
 
     salt.utils.cloud.fire_event(
         "event",
         "starting create",
-        "salt/cloud/{}/creating".format(vm_["name"]),
+        "salt/cloud/{}/creating".format(vm_["name"]),  # pylint: disable=consider-using-f-string
         args=__utils__["cloud.filter_event"](
             "creating", vm_, ["name", "profile", "provider", "driver"]
         ),
         sock_dir=__opts__["sock_dir"],
         transport=__opts__["transport"],
     )
     __utils__["cloud.cachedir_index_add"](vm_["name"], vm_["profile"], "azurerm", vm_["driver"])
@@ -1176,15 +1190,19 @@
         vm_["location"] = get_location(kwargs=vm_)
 
     log.info("Creating Cloud VM %s in %s", vm_["name"], vm_["location"])
 
     vm_request = request_instance(vm_=vm_)
 
     if not vm_request or "error" in vm_request:
-        err_message = "Error creating VM {}! ({})".format(vm_["name"], str(vm_request))
+        err_message = (
+            "Error creating VM {}! ({})".format(  # pylint: disable=consider-using-f-string
+                vm_["name"], str(vm_request)
+            )
+        )
         log.error(err_message)
         raise SaltCloudSystemExit(err_message)
 
     def _query_node_data(name, bootstrap_interface):
         """
         Query node data.
         """
@@ -1238,15 +1256,15 @@
     log.debug("'%s' VM creation details:\n%s", vm_["name"], pprint.pformat(data))
 
     ret.update(data)
 
     salt.utils.cloud.fire_event(
         "event",
         "created instance",
-        "salt/cloud/{}/created".format(vm_["name"]),
+        "salt/cloud/{}/created".format(vm_["name"]),  # pylint: disable=consider-using-f-string
         args=__utils__["cloud.filter_event"](
             "created", vm_, ["name", "profile", "provider", "driver"]
         ),
         sock_dir=__opts__["sock_dir"],
         transport=__opts__["transport"],
     )
 
@@ -1447,15 +1465,15 @@
         "cloud_environment", get_configured_provider(), __opts__, search_global=False
     )
     try:
         cloud_env_module = importlib.import_module("msrestazure.azure_cloud")
         cloud_env = getattr(cloud_env_module, cloud_environment or "AZURE_PUBLIC_CLOUD")
     except (AttributeError, ImportError):
         raise SaltCloudSystemExit(  # pylint: disable=raise-missing-from
-            "The azure {} cloud environment is not available.".format(cloud_environment)
+            f"The azure {cloud_environment} cloud environment is not available."
         )
 
     return cloud_env
 
 
 def _get_block_blob_service(kwargs=None):
     """
@@ -1704,15 +1722,15 @@
         location=location,
         publisher=publisher,
         extension_type=virtual_machine_extension_type,
         version=type_handler_version,
         settings=settings,
         auto_upgrade_minor_version=auto_upgrade_minor_version,
         protected_settings=protected_settings,
-        **conn_kwargs
+        **conn_kwargs,
     )
 
     return ret
 
 
 def stop(name, call=None):
     """
@@ -1744,15 +1762,15 @@
             )
             if ret:
                 break
             if "error" in ret and "was not found" in ret["error"]:
                 continue
 
         if not ret or "error" in ret:
-            ret = {"error": "Unable to find virtual machine with name: {}".format(name)}
+            ret = {"error": f"Unable to find virtual machine with name: {name}"}
     else:
         ret = __salt__["azurerm_compute_virtual_machine.deallocate"](
             name=name, resource_group=resource_group, **conn_kwargs
         )
 
     return ret
 
@@ -1787,14 +1805,14 @@
             )
             if ret:
                 break
             if "error" in ret and "was not found" in ret["error"]:
                 continue
 
         if not ret or "error" in ret:
-            ret = {"error": "Unable to find virtual machine with name: {}".format(name)}
+            ret = {"error": f"Unable to find virtual machine with name: {name}"}
     else:
         ret = __salt__["azurerm_compute_virtual_machine.start"](
             name=name, resource_group=resource_group, **conn_kwargs
         )
 
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/fileserver/azurefs.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/fileserver/azurefs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
 The backend for serving files from the Azure blob storage service.
 
 .. versionadded:: 2015.8.0
 
-To enable, add ``azurefs`` to the :conf_master:`fileserver_backend` option in
-the Master config file.
+To enable, add ``azurefs`` to the `fileserver_backend` option in the
+Master config file.
 
 .. code-block:: yaml
 
     fileserver_backend:
       - azurefs
 
 Starting in Salt 2018.3.0, this fileserver requires the standalone Azure
@@ -268,15 +268,17 @@
     ret = {"hash_type": __opts__["hash_type"]}
     relpath = fnd["rel"]
     path = fnd["path"]
     hash_cachedir = os.path.join(__opts__["cachedir"], "azurefs", "hashes")
     hashdest = salt.utils.path.join(
         hash_cachedir,
         load["saltenv"],
-        "{}.hash.{}".format(relpath, __opts__["hash_type"]),
+        "{}.hash.{}".format(  # pylint: disable=consider-using-f-string
+            relpath, __opts__["hash_type"]
+        ),
     )
     if not os.path.isfile(hashdest):
         if not os.path.exists(os.path.dirname(hashdest)):
             os.makedirs(os.path.dirname(hashdest))
         ret["hsum"] = salt.utils.hashutils.get_hash(path, __opts__["hash_type"])
         with salt.utils.files.fopen(hashdest, "w+") as fp_:
             fp_.write(salt.utils.stringutils.to_str(ret["hsum"]))
@@ -332,15 +334,15 @@
     """
     Get the cache path for the container in question
 
     Cache paths are generate by combining the account name, container name,
     and saltenv, separated by underscores
     """
     root = os.path.join(__opts__["cachedir"], "azurefs")
-    container_dir = "{}_{}_{}".format(
+    container_dir = "{}_{}_{}".format(  # pylint: disable=consider-using-f-string
         container.get("account_name", ""),
         container.get("container_name", ""),
         container.get("saltenv", "base"),
     )
     return os.path.join(root, container_dir)
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/loader.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/loader.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
 def availability_set_create_or_update(
     name, resource_group, **kwargs
 ):  # pylint: disable=invalid-name
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_availability_set.py)
-     and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Create or update an availability set.
 
     :param name: The availability set to create.
 
     :param resource_group: The resource group name assigned to the
         availability set.
@@ -92,15 +92,15 @@
 
 
 def availability_set_delete(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_availability_set.py)
-     and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Delete an availability set.
 
     :param name: The availability set to delete.
 
     :param resource_group: The resource group name assigned to the
         availability set.
@@ -118,15 +118,15 @@
 
 
 def availability_set_get(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_availability_set.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Get a dictionary representing an availability set's properties.
 
     :param name: The availability set to get.
 
     :param resource_group: The resource group name assigned to the
         availability set.
@@ -144,15 +144,15 @@
 
 
 def availability_sets_list(resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_availability_set.py)
-     and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     List all availability sets within a resource group.
 
     :param resource_group: The resource group name to list availability
         sets within.
 
     CLI Example:
@@ -168,15 +168,15 @@
 
 
 def availability_sets_list_available_sizes(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_availability_set.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     List all available virtual machine sizes that can be used to
     to create a new virtual machine in an existing availability set.
 
     :param name: The availability set name to list available
         virtual machine sizes within.
 
@@ -198,15 +198,15 @@
 def virtual_machine_capture(
     name, destination_name, resource_group, prefix="capture-", overwrite=False, **kwargs
 ):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Captures the VM by copying virtual hard disks of the VM and outputs
     a template that can be used to create similar VMs.
 
     :param name: The name of the virtual machine.
 
     :param destination_name: The destination container name.
@@ -236,15 +236,15 @@
 
 
 def virtual_machine_get(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Retrieves information about the model view or the instance view of a
     virtual machine.
 
     :param name: The name of the virtual machine.
 
     :param resource_group: The resource group name assigned to the
@@ -263,15 +263,15 @@
 
 
 def virtual_machine_convert_to_managed_disks(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Converts virtual machine disks from blob-based to managed disks. Virtual
     machine must be stop-deallocated before invoking this operation.
 
     :param name: The name of the virtual machine to convert.
 
     :param resource_group: The resource group name assigned to the
@@ -290,15 +290,15 @@
 
 
 def virtual_machine_deallocate(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Power off a virtual machine and deallocate compute resources.
 
     :param name: The name of the virtual machine to deallocate.
 
     :param resource_group: The resource group name assigned to the
         virtual machine.
@@ -316,15 +316,15 @@
 
 
 def virtual_machine_generalize(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Set the state of a virtual machine to 'generalized'.
 
     :param name: The name of the virtual machine.
 
     :param resource_group: The resource group name assigned to the
         virtual machine.
@@ -342,15 +342,15 @@
 
 
 def virtual_machines_list(resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     List all virtual machines within a resource group.
 
     :param resource_group: The resource group name to list virtual
         machines within.
 
     CLI Example:
@@ -364,15 +364,15 @@
 
 
 def virtual_machines_list_all(**kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     List all virtual machines within a subscription.
 
     CLI Example:
 
     .. code-block:: bash
 
@@ -385,15 +385,15 @@
 def virtual_machines_list_available_sizes(
     name, resource_group, **kwargs
 ):  # pylint: disable=invalid-name
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Lists all available virtual machine sizes to which the specified virtual
     machine can be resized.
 
     :param name: The name of the virtual machine.
 
     :param resource_group: The resource group name assigned to the
@@ -412,15 +412,15 @@
 
 
 def virtual_machine_power_off(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-      and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Power off (stop) a virtual machine.
 
     :param name: The name of the virtual machine to stop.
 
     :param resource_group: The resource group name assigned to the
         virtual machine.
@@ -490,15 +490,15 @@
 
 
 def virtual_machine_redeploy(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_virtual_machine.py)
-     and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Redeploy a virtual machine.
 
     :param name: The name of the virtual machine to redeploy.
 
     :param resource_group: The resource group name assigned to the
         virtual machine.
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_availability_set.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_availability_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,30 +97,30 @@
         kwargs["virtual_machines"] = vm_list
 
     try:
         setmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "compute", "AvailabilitySet", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         av_set = compconn.availability_sets.create_or_update(
             resource_group_name=resource_group,
             availability_set_name=name,
             parameters=setmodel,
         )
         result = av_set.as_dict()
 
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("compute", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def delete(name, resource_group, **kwargs):
     """
     .. versionadded:: 2.1.0
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_disk.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_disk.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_image.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_image.py`

 * *Files 2% similar despite different names*

```diff
@@ -156,42 +156,42 @@
                 "ImageStorageProfile",
                 os_disk=os_disk,
                 data_disks=data_disks,
                 zone_resilient=zone_resilient,
                 **kwargs,
             )
         except TypeError as exc:
-            result = {"error": "The object model could not be built. ({})".format(str(exc))}
+            result = {"error": f"The object model could not be built. ({str(exc)})"}
             return result
 
     try:
         imagemodel = saltext.azurerm.utils.azurerm.create_object_model(
             "compute",
             "Image",
             source_virtual_machine=source_vm,
             storage_profile=spmodel,
             hyper_vgeneration=hyper_vgeneration,
             **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         image = compconn.images.begin_create_or_update(
             resource_group_name=resource_group, image_name=name, parameters=imagemodel
         )
 
         image.wait()
         result = image.result().as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("compute", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def delete(name, resource_group, **kwargs):
     """
     .. versionadded:: 2.1.0
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_virtual_machine.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine.py`

 * *Files 1% similar despite different names*

```diff
@@ -246,15 +246,15 @@
         licensed on-premises. This element is only used for images that contain the Windows Server operating system.
 
     :param zones: A list of the virtual machine zones.
 
     :param availability_set: The resource ID of the availability set that the virtual machine should be assigned to.
         Virtual machines specified in the same availability set are allocated to different nodes to maximize
         availability. For more information about availability sets, see `Manage the availability of virtual
-        machines <https://docs.microsoft.com/azure/virtual-machines/virtual-machines-windows-manage-availability>`_.
+        machines <https://learn.microsoft.com/en-us/azure/virtual-machines/availability-set-overview>`_.
         Currently, a VM can only be added to availability set at creation time. An existing VM cannot be added to an
         availability set. This parameter cannot be specified if the ``virtual_machine_scale_set`` parameter is also
         specified.
 
     :param virtual_machine_scale_set: The resource ID of the virtual machine scale set that the virtual machine should
         be assigned to. Virtual machines specified in the same virtual machine scale set are allocated to different
         nodes to maximize availability. Currently, a VM can only be added to virtual machine scale set at creation time.
@@ -369,32 +369,30 @@
             pubip = __salt__["azurerm_network.public_ip_address_create_or_update"](
                 f"{name}-pip0", resource_group, **kwargs
             )
 
             try:
                 ipc.update({"public_ip_address": {"id": pubip["id"]}})
             except KeyError as exc:
-                result = {
-                    "error": "The public IP address could not be created. ({})".format(str(exc))
-                }
+                result = {"error": f"The public IP address could not be created. ({str(exc)})"}
                 return result
 
         iface = __salt__["azurerm_network.network_interface_create_or_update"](
             f"{name}-nic0",
             [ipc],
             subnet,
             virtual_network,
             network_resource_group or resource_group,
             **kwargs,
         )
 
         try:
             nic = {"id": iface["id"]}
         except KeyError as exc:
-            result = {"error": "The network interface could not be created. ({})".format(str(exc))}
+            result = {"error": f"The network interface could not be created. ({str(exc)})"}
             return result
 
         network_interfaces.append(nic)
 
     # default os disk name
     if not os_disk_name and os_disk_simplename:
         os_disk_name = f"{name}-osdisk0"
@@ -636,15 +634,15 @@
         params["additional_capabilities"] = {"ultra_ssd_enabled": ultra_ssd_enabled}
 
     try:
         vmmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "compute", "VirtualMachine", **params
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         # pylint: disable=invalid-name
         vm = compconn.virtual_machines.begin_create_or_update(
             resource_group_name=resource_group, vm_name=name, parameters=vmmodel
         )
@@ -704,15 +702,15 @@
                 )
                 log.debug("Return from userdata extension: %s", userdata_ret)
 
         # attach disk encryption extension
         if enable_disk_enc and provision_vm_agent and disk_enc_keyvault and disk_enc_volume_type:
             try:
                 disk_enc_keyvault_name = (parse_resource_id(disk_enc_keyvault))["name"]
-                disk_enc_keyvault_url = "https://{}.vault.azure.net/".format(disk_enc_keyvault_name)
+                disk_enc_keyvault_url = f"https://{disk_enc_keyvault_name}.vault.azure.net/"
 
                 extension_info = {
                     "publisher": "Microsoft.Azure.Security",
                     "settings": {
                         "VolumeType": disk_enc_volume_type,
                         "EncryptionOperation": "EnableEncryption",
                         "KeyVaultResourceId": disk_enc_keyvault,
@@ -765,15 +763,15 @@
             network_interfaces.append(iface_details)
 
         result["network_profile"]["network_interfaces"] = network_interfaces
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("compute", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def delete(
     name,
     resource_group,
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_extension.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_extension.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,15 +115,15 @@
             publisher=publisher,
             type_properties_type=extension_type,
             type_handler_version=version,
             auto_upgrade_minor_version=auto_upgrade_minor_version,
             **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         extension = compconn.virtual_machine_extensions.begin_create_or_update(
             vm_extension_name=name,
             vm_name=vm_name,
             resource_group_name=resource_group,
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_image.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_compute_virtual_machine_image.py`

 * *Files identical despite different names*

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_dns.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_dns.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
     dnsconn = saltext.azurerm.utils.azurerm.get_client(client, **kwargs)
 
     try:
         record_set_model = saltext.azurerm.utils.azurerm.create_object_model(
             "dns", "RecordSet", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         if zone_type.lower() == "private":
             record_set = dnsconn.record_sets.create_or_update(
                 relative_record_set_name=name,
                 private_zone_name=zone_name,
@@ -136,15 +136,15 @@
                 if_none_match=kwargs.get("if_none_match"),
             )
         result = record_set.as_dict()
     except (HttpResponseError, ResourceNotFoundError) as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def record_set_delete(name, zone_name, resource_group, record_type, zone_type="Public", **kwargs):
     """
     .. versionadded:: 3000
@@ -259,15 +259,15 @@
 def record_sets_list_by_type(
     zone_name,
     resource_group,
     record_type,
     top=None,
     recordsetnamesuffix=None,
     zone_type="Public",
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 3000
 
     Lists the record sets of a specified type in a DNS zone.
 
     :param zone_name: The name of the DNS zone (without a terminating dot).
@@ -437,15 +437,15 @@
         kwargs["resolution_virtual_networks"] = [
             {"id": vnet} for vnet in kwargs["resolution_virtual_networks"]
         ]
 
     try:
         zone_model = saltext.azurerm.utils.azurerm.create_object_model(client, obj, **kwargs)
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         if zone_type.lower() == "private":
             zone = dnsconn.private_zones.begin_create_or_update(
                 private_zone_name=name,
                 resource_group_name=resource_group,
@@ -466,15 +466,15 @@
                 if_none_match=kwargs.get("if_none_match"),
             )
             result = zone.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("dns", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def zone_delete(name, resource_group, zone_type="Public", **kwargs):
     """
     .. versionadded:: 3000
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_keyvault_key.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_keyvault_key.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,14 +64,19 @@
     """
     .. versionadded:: 2.1.0
 
     Load the key client and return a KeyClient object.
 
     :param vault_url: The URL of the vault that the client will access.
 
+    CLI Example:
+
+    .. code-block:: bash
+
+        salt-call azurerm_keyvault_key.get_key_client https://myvault.vault.azure.net/
     """
     credential = saltext.azurerm.utils.azurerm.get_identity_credentials(**kwargs)
     key_client = KeyClient(vault_url=vault_url, credential=credential)
 
     return key_client
 
 
@@ -577,15 +582,15 @@
         kwargs["key_type"] = kwargs.get("key_type").upper().replace("_", "-")
 
     try:
         keymodel = saltext.azurerm.utils.azurerm.create_object_model(
             "keyvault-keys", "JsonWebKey", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         key = kconn.import_key(
             name=name,
             hardware_protected=hardware_protected,
             enabled=enabled,
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_keyvault_secret.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_keyvault_secret.py`

 * *Files 0% similar despite different names*

```diff
@@ -70,14 +70,19 @@
     """
     .. versionadded:: 2.1.0
 
     Load the secret client and return a SecretClient object.
 
     :param vault_url: The URL of the vault that the client will access.
 
+    CLI Example:
+
+    .. code-block:: bash
+
+        salt-call azurerm_keyvault_secret.get_secret_client https://myvault.vault.azure.net/
     """
     credential = saltext.azurerm.utils.azurerm.get_identity_credentials(**kwargs)
 
     secret_client = SecretClient(vault_url=vault_url, credential=credential)
 
     return secret_client
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_keyvault_vault.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_keyvault_vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,25 +130,26 @@
         - ``tenant_id``: (Required) The Azure Active Directory tenant ID that should be used for authenticating
           requests to the key vault.
         - ``object_id``: (Required) The object ID of a user, service principal, or security group in the Azure Active
           Directory tenant for the vault. The object ID must be unique for the list of access policies.
         - ``application_id``: (Optional) Application ID of the client making request on behalf of a principal.
         - ``permissions``: (Required) A dictionary representing permissions the identity has for keys, secrets, and
           certifications. Valid parameters include:
-            - ``keys``: A list that represents permissions to keys. Possible values include: 'backup', 'create',
-              'decrypt', 'delete', 'encrypt', 'get', 'import_enum', 'list', 'purge', 'recover', 'restore', 'sign',
-              'unwrap_key', 'update', 'verify', and 'wrap_key'.
-            - ``secrets``: A list that represents permissions to secrets. Possible values include: 'backup', 'delete',
-              'get', 'list', 'purge', 'recover', 'restore', and 'set'.
-            - ``certificates``: A list that represents permissions to certificates. Possible values include: 'create',
-              'delete', 'deleteissuers', 'get', 'getissuers', 'import_enum', 'list', 'listissuers', 'managecontacts',
-              'manageissuers', 'purge', 'recover', 'setissuers', and 'update'.
-            - ``storage``: A list that represents permissions to storage accounts. Possible values include: 'backup',
-              'delete', 'deletesas', 'get', 'getsas', 'list', 'listsas', 'purge', 'recover', 'regeneratekey',
-              'restore', 'set', 'setsas', and 'update'.
+
+          - ``keys``: A list that represents permissions to keys. Possible values include: 'backup', 'create',
+            'decrypt', 'delete', 'encrypt', 'get', 'import_enum', 'list', 'purge', 'recover', 'restore', 'sign',
+            'unwrap_key', 'update', 'verify', and 'wrap_key'.
+          - ``secrets``: A list that represents permissions to secrets. Possible values include: 'backup', 'delete',
+            'get', 'list', 'purge', 'recover', 'restore', and 'set'.
+          - ``certificates``: A list that represents permissions to certificates. Possible values include: 'create',
+            'delete', 'deleteissuers', 'get', 'getissuers', 'import_enum', 'list', 'listissuers', 'managecontacts',
+            'manageissuers', 'purge', 'recover', 'setissuers', and 'update'.
+          - ``storage``: A list that represents permissions to storage accounts. Possible values include: 'backup',
+            'delete', 'deletesas', 'get', 'getsas', 'list', 'listsas', 'purge', 'recover', 'regeneratekey',
+            'restore', 'set', 'setsas', and 'update'.
 
     :param vault_uri: The URI of the vault for performing operations on keys and secrets.
 
     :param create_mode: The vault's create mode to indicate whether the vault needs to be recovered or not.
         Possible values include: 'recover' and 'default'.
 
     :param enabled_for_deployment: A boolean value specifying whether Azure Virtual Machines are permitted to
@@ -220,28 +221,28 @@
             enabled_for_template_deployment=enabled_for_template_deployment,
             soft_delete_retention_in_days=soft_delete_retention,
             enable_rbac_authorization=enable_rbac_authorization,
             network_acls=network_acls,
             **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     # Create the VaultCreateOrUpdateParameters object
     try:
         paramsmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "keyvault",
             "VaultCreateOrUpdateParameters",
             location=location,
             properties=propsmodel,
             tags=tags,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         vault = vconn.vaults.begin_create_or_update(
             vault_name=name, resource_group_name=resource_group, parameters=paramsmodel
         )
 
@@ -494,25 +495,26 @@
         - ``tenant_id``: (Required) The Azure Active Directory tenant ID that should be used for authenticating
           requests to the key vault.
         - ``object_id``: (Required) The object ID of a user, service principal, or security group in the Azure Active
           Directory tenant for the vault. The object ID must be unique for the list of access policies.
         - ``application_id``: (Optional) Application ID of the client making request on behalf of a principal.
         - ``permissions``: (Required) A dictionary representing permissions the identity has for keys, secrets, and
           certifications. Valid parameters include:
-            - ``keys``: A list that represents permissions to keys. Possible values include: 'backup', 'create',
-              'decrypt', 'delete', 'encrypt', 'get', 'import_enum', 'list', 'purge', 'recover', 'restore', 'sign',
-              'unwrap_key', 'update', 'verify', and 'wrap_key'.
-            - ``secrets``: A list that represents permissions to secrets. Possible values include: 'backup', 'delete',
-              'get', 'list', 'purge', 'recover', 'restore', and 'set'.
-            - ``certificates``: A list that represents permissions to certificates. Possible values include: 'create',
-              'delete', 'deleteissuers', 'get', 'getissuers', 'import_enum', 'list', 'listissuers', 'managecontacts',
-              'manageissuers', 'purge', 'recover', 'setissuers', and 'update'.
-            - ``storage``: A list that represents permissions to storage accounts. Possible values include: 'backup',
-              'delete', 'deletesas', 'get', 'getsas', 'list', 'listsas', 'purge', 'recover', 'regeneratekey',
-              'restore', 'set', 'setsas', and 'update'.
+
+          - ``keys``: A list that represents permissions to keys. Possible values include: 'backup', 'create',
+            'decrypt', 'delete', 'encrypt', 'get', 'import_enum', 'list', 'purge', 'recover', 'restore', 'sign',
+            'unwrap_key', 'update', 'verify', and 'wrap_key'.
+          - ``secrets``: A list that represents permissions to secrets. Possible values include: 'backup', 'delete',
+            'get', 'list', 'purge', 'recover', 'restore', and 'set'.
+          - ``certificates``: A list that represents permissions to certificates. Possible values include: 'create',
+            'delete', 'deleteissuers', 'get', 'getissuers', 'import_enum', 'list', 'listissuers', 'managecontacts',
+            'manageissuers', 'purge', 'recover', 'setissuers', and 'update'.
+          - ``storage``: A list that represents permissions to storage accounts. Possible values include: 'backup',
+            'delete', 'deletesas', 'get', 'getsas', 'list', 'listsas', 'purge', 'recover', 'regeneratekey',
+            'restore', 'set', 'setsas', and 'update'.
 
     CLI Example:
 
     .. code-block:: bash
 
         salt-call azurerm_keyvault_vault.update_access_policy test_name test_rg test_kind test_policies
 
@@ -525,15 +527,15 @@
         propsmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "keyvault",
             "VaultAccessPolicyProperties",
             access_policies=access_policies,
             **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         vault = vconn.vaults.update_access_policy(
             vault_name=name,
             resource_group_name=resource_group,
             operation_kind=operation_kind,
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_network.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_network.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         return default_rules
 
     try:
         for default_rule in default_rules:
             if default_rule["name"] == name:
                 result = default_rule
         if not result:
-            result = {"error": "Unable to find {} in {}!".format(name, security_group)}
+            result = {"error": f"Unable to find {name} in {security_group}!"}
     except KeyError as exc:
         log.error("Unable to find %s in %s!", name, security_group)
         result = {"error": str(exc)}
 
     return result
 
 
@@ -258,15 +258,15 @@
     destination_address_prefix=None,
     source_port_range=None,
     destination_port_range=None,
     source_address_prefixes=None,
     destination_address_prefixes=None,
     source_port_ranges=None,
     destination_port_ranges=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Create or update a security rule within a specified network security group.
 
     :param name: The name of the security rule to create.
@@ -343,15 +343,15 @@
         # pylint: disable=eval-used
         if not eval(params[0]) and not eval(params[1]):
             log.error("Either the %s or %s parameter must be provided!", params[0], params[1])
             return False
         # pylint: disable=eval-used
         if eval(params[0]):
             # pylint: disable=exec-used
-            exec("{} = None".format(params[1]))
+            exec(f"{params[1]} = None")
 
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         rulemodel = saltext.azurerm.utils.azurerm.create_object_model(
             "network",
             "SecurityRule",
@@ -364,18 +364,18 @@
             source_port_range=source_port_range,
             source_address_prefixes=source_address_prefixes,
             source_address_prefix=source_address_prefix,
             destination_port_ranges=destination_port_ranges,
             destination_port_range=destination_port_range,
             destination_address_prefixes=destination_address_prefixes,
             destination_address_prefix=destination_address_prefix,
-            **kwargs
+            **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         secrule = netconn.security_rules.begin_create_or_update(
             resource_group_name=resource_group,
             network_security_group_name=security_group,
             security_rule_name=name,
@@ -384,15 +384,15 @@
         secrule.wait()
         secrule_result = secrule.result()
         result = secrule_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def security_rule_delete(security_rule, security_group, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -498,15 +498,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         secgroupmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "network", "NetworkSecurityGroup", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         secgroup = netconn.network_security_groups.begin_create_or_update(
             resource_group_name=resource_group,
             network_security_group_name=name,
             parameters=secgroupmodel,
@@ -515,15 +515,15 @@
         secgroup.wait()
         secgroup_result = secgroup.result()
         result = secgroup_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def network_security_group_delete(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -763,18 +763,18 @@
 
     try:
         snetmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "network",
             "Subnet",
             address_prefix=address_prefix,
             resource_group=resource_group,
-            **kwargs
+            **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         subnet = netconn.subnets.begin_create_or_update(
             resource_group_name=resource_group,
             virtual_network_name=virtual_network,
             subnet_name=name,
@@ -784,15 +784,15 @@
         subnet.wait()
         sn_result = subnet.result()
         result = sn_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def subnet_delete(name, virtual_network, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -935,18 +935,18 @@
 
     try:
         vnetmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "network",
             "VirtualNetwork",
             address_space=address_space,
             dhcp_options=dhcp_options,
-            **kwargs
+            **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         vnet = netconn.virtual_networks.begin_create_or_update(
             virtual_network_name=name,
             resource_group_name=resource_group,
             parameters=vnetmodel,
@@ -955,15 +955,15 @@
         vnet.wait()
         vnet_result = vnet.result()
         result = vnet_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def virtual_network_delete(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -1150,15 +1150,15 @@
     if isinstance(kwargs.get("frontend_ip_configurations"), list):
         for idx in range(0, len(kwargs["frontend_ip_configurations"])):
             # Use Public IP Address name to link to the ID of an existing Public IP
             if "public_ip_address" in kwargs["frontend_ip_configurations"][idx]:
                 pub_ip = public_ip_address_get(
                     name=kwargs["frontend_ip_configurations"][idx]["public_ip_address"],
                     resource_group=resource_group,
-                    **kwargs
+                    **kwargs,
                 )
                 if "error" not in pub_ip:
                     kwargs["frontend_ip_configurations"][idx]["public_ip_address"] = {
                         "id": str(pub_ip["id"])
                     }
             # Use Subnet name to link to the ID of an existing Subnet
             elif "subnet" in kwargs["frontend_ip_configurations"][idx]:
@@ -1267,15 +1267,15 @@
                 }
 
     try:
         lbmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "network", "LoadBalancer", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         load_balancer = netconn.load_balancers.begin_create_or_update(
             resource_group_name=resource_group,
             load_balancer_name=name,
             parameters=lbmodel,
@@ -1284,15 +1284,15 @@
         load_balancer.wait()
         lb_result = load_balancer.result()
         result = lb_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def load_balancer_delete(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -1534,26 +1534,26 @@
                     if isinstance(ipconfig.get("load_balancer_inbound_nat_rules"), list):
                         # TODO: Add ID lookup for referenced object names
                         pass
                     if ipconfig.get("public_ip_address"):
                         pub_ip = public_ip_address_get(
                             name=ipconfig["public_ip_address"],
                             resource_group=resource_group,
-                            **kwargs
+                            **kwargs,
                         )
                         if "error" not in pub_ip:
                             ipconfig["public_ip_address"] = {"id": str(pub_ip["id"])}
 
     # Make the Network Interface
     try:
         nicmodel = saltext.azurerm.utils.azurerm.create_object_model(
             "network", "NetworkInterface", ip_configurations=ip_configurations, **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         interface = netconn.network_interfaces.begin_create_or_update(
             resource_group_name=resource_group,
             network_interface_name=name,
             parameters=nicmodel,
@@ -1562,15 +1562,15 @@
         interface.wait()
         nic_result = interface.result()
         result = nic_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def network_interfaces_list_all(**kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -1925,15 +1925,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         pub_ip_model = saltext.azurerm.utils.azurerm.create_object_model(
             "network", "PublicIPAddress", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         ip = netconn.public_ip_addresses.begin_create_or_update(
             resource_group_name=resource_group,
             public_ip_address_name=name,
             parameters=pub_ip_model,
@@ -1942,15 +1942,15 @@
         ip.wait()
         ip_result = ip.result()
         result = ip_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def public_ip_addresses_list_all(**kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -2127,15 +2127,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         rule_model = saltext.azurerm.utils.azurerm.create_object_model(
             "network", "RouteFilterRule", access=access, communities=communities, **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         rule = netconn.route_filter_rules.create_or_update(
             resource_group_name=resource_group,
             route_filter_name=route_filter,
             rule_name=name,
@@ -2147,15 +2147,15 @@
     except HttpResponseError as exc:
         message = str(exc)
         if kwargs.get("subscription_id") == str(message).strip():
             message = "Subscription not authorized for this operation!"
         saltext.azurerm.utils.azurerm.log_cloud_error("network", message, **kwargs)
         result = {"error": message}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def route_filter_rules_list(route_filter, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -2287,15 +2287,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         rt_filter_model = saltext.azurerm.utils.azurerm.create_object_model(
             "network", "RouteFilter", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         rt_filter = netconn.route_filters.create_or_update(
             resource_group_name=resource_group,
             route_filter_name=name,
             route_filter_parameters=rt_filter_model,
@@ -2303,15 +2303,15 @@
         rt_filter.wait()
         rt_result = rt_filter.result()
         result = rt_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def route_filters_list(resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -2448,15 +2448,15 @@
 def route_create_or_update(
     name,
     address_prefix,
     next_hop_type,
     route_table,
     resource_group,
     next_hop_ip_address=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Create or update a route within a specified route table.
 
     :param name: The name of the route to create.
@@ -2486,18 +2486,18 @@
     try:
         rt_model = saltext.azurerm.utils.azurerm.create_object_model(
             "network",
             "Route",
             address_prefix=address_prefix,
             next_hop_type=next_hop_type,
             next_hop_ip_address=next_hop_ip_address,
-            **kwargs
+            **kwargs,
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         route = netconn.routes.begin_create_or_update(
             resource_group_name=resource_group,
             route_table_name=route_table,
             route_name=name,
@@ -2506,15 +2506,15 @@
         route.wait()
         rt_result = route.result()
         result = rt_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def routes_list(route_table, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -2644,15 +2644,15 @@
     netconn = saltext.azurerm.utils.azurerm.get_client("network", **kwargs)
 
     try:
         rt_tbl_model = saltext.azurerm.utils.azurerm.create_object_model(
             "network", "RouteTable", **kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         table = netconn.route_tables.begin_create_or_update(
             resource_group_name=resource_group,
             route_table_name=name,
             parameters=rt_tbl_model,
@@ -2661,15 +2661,15 @@
         table.wait()
         tbl_result = table.result()
         result = tbl_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("network", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def route_tables_list(resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/modules/azurerm_resource.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/modules/azurerm_resource.py`

 * *Files 2% similar despite different names*

```diff
@@ -355,15 +355,15 @@
     resource_group,
     deploy_mode="incremental",
     debug_setting="none",
     deploy_params=None,
     parameters_link=None,
     deploy_template=None,
     template_link=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Deploys resources to a resource group.
 
     :param name: The name of the deployment to create or update.
@@ -480,28 +480,28 @@
     deploy_kwargs.update(prop_kwargs)
 
     try:
         deploy_model = saltext.azurerm.utils.azurerm.create_object_model(
             "resource.resources", "DeploymentProperties", **deploy_kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         validate = deployment_validate(
             name=name,
             resource_group=resource_group,
             deploy_mode=deploy_kwargs.get("mode"),
             debug_setting=deploy_kwargs.get("debug_setting"),
             deploy_params=deploy_kwargs.get("parameters"),
             parameters_link=deploy_kwargs.get("parameters_link"),
             deploy_template=deploy_kwargs.get("template"),
             template_link=deploy_kwargs.get("template_link"),
-            **kwargs
+            **kwargs,
         )
         if "error" in validate:
             result = validate
         else:
             deploy = resconn.deployments.begin_create_or_update(
                 deployment_name=name,
                 resource_group_name=resource_group,
@@ -510,15 +510,15 @@
             deploy.wait()
             deploy_result = deploy.result()
             result = deploy_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def deployment_get(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -582,15 +582,15 @@
     resource_group,
     deploy_mode=None,
     debug_setting=None,
     deploy_params=None,
     parameters_link=None,
     deploy_template=None,
     template_link=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Validates whether the specified template is syntactically correct
     and will be accepted by Azure Resource Manager.
 
@@ -661,15 +661,15 @@
     deploy_kwargs.update(prop_kwargs)
 
     try:
         deploy_model = saltext.azurerm.utils.azurerm.create_object_model(
             "resource.resources", "DeploymentProperties", **deploy_kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         local_validation = deploy_model.validate()
         if local_validation:
             raise local_validation[0]
 
@@ -681,15 +681,15 @@
         deploy.wait()
         deploy_result = deploy.result()
         result = deploy_result.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def deployment_export_template(name, resource_group, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -939,15 +939,15 @@
     # Delete this section when the ticket above is resolved.
     #  BEGIN
     definition_list = policy_definitions_list(**kwargs)
     if definition_name in definition_list:
         definition = definition_list[definition_name]
     else:
         definition = {
-            "error": 'The policy definition named "{}" could not be found.'.format(definition_name)
+            "error": f'The policy definition named "{definition_name}" could not be found.'
         }
     #  END
 
     if "error" not in definition:
         definition_id = str(definition["id"])
 
         prop_kwargs = {"policy_definition_id": definition_id}
@@ -956,31 +956,29 @@
         policy_kwargs.update(prop_kwargs)
 
         try:
             policy_model = saltext.azurerm.utils.azurerm.create_object_model(
                 "resource.policy", "PolicyAssignment", **policy_kwargs
             )
         except TypeError as exc:
-            result = {"error": "The object model could not be built. ({})".format(str(exc))}
+            result = {"error": f"The object model could not be built. ({str(exc)})"}
             return result
 
         try:
             policy = polconn.policy_assignments.create(
                 scope=scope, policy_assignment_name=name, parameters=policy_model
             )
             result = policy.as_dict()
         except HttpResponseError as exc:
             saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
             result = {"error": str(exc)}
         except SerializationError as exc:
-            result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+            result = {"error": f"The object model could not be parsed. ({str(exc)})"}
     else:
-        result = {
-            "error": 'The policy definition named "{}" could not be found.'.format(definition_name)
-        }
+        result = {"error": f'The policy definition named "{definition_name}" could not be found.'}
 
     return result
 
 
 def policy_assignment_get(name, scope, **kwargs):
     """
     .. versionadded:: 2019.2.0
@@ -1079,15 +1077,15 @@
     .. versionadded:: 2019.2.0
 
     Create or update a policy definition.
 
     :param name: The name of the policy definition to create or update.
 
     :param policy_rule: A dictionary defining the
-        `policy rule <https://docs.microsoft.com/en-us/azure/azure-policy/policy-definition#policy-rule>`_.
+        `policy rule <https://learn.microsoft.com/en-us/azure/governance/policy/concepts/definition-structure-policy-rule>`_.
 
     CLI Example:
 
     .. code-block:: bash
 
         salt-call azurerm_resource.policy_definition_create_or_update testpolicy '{...rule definition..}'
 
@@ -1105,27 +1103,27 @@
     policy_kwargs.update(prop_kwargs)
 
     try:
         policy_model = saltext.azurerm.utils.azurerm.create_object_model(
             "resource.policy", "PolicyDefinition", **policy_kwargs
         )
     except TypeError as exc:
-        result = {"error": "The object model could not be built. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be built. ({str(exc)})"}
         return result
 
     try:
         policy = polconn.policy_definitions.create_or_update(
             policy_definition_name=name, parameters=policy_model
         )
         result = policy.as_dict()
     except HttpResponseError as exc:
         saltext.azurerm.utils.azurerm.log_cloud_error("resource", str(exc), **kwargs)
         result = {"error": str(exc)}
     except SerializationError as exc:
-        result = {"error": "The object model could not be parsed. ({})".format(str(exc))}
+        result = {"error": f"The object model could not be parsed. ({str(exc)})"}
 
     return result
 
 
 def policy_definition_delete(name, **kwargs):
     """
     .. versionadded:: 2019.2.0
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_compute.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_compute.py`

 * *Files 0% similar despite different names*

```diff
@@ -101,15 +101,15 @@
     connection_auth=None,
     **kwargs
 ):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_availability_set.py)
-     and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Ensure an availability set exists.
 
     :param name:
         Name of the availability set.
 
     :param resource_group:
@@ -169,15 +169,15 @@
 
 
 def availability_set_absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
     **WARNING: This function has been moved to another file (azurerm_compute_availability_set.py)
-     and will be deprecated in the future.**
+    and will be deprecated in the future.**
 
     Ensure an availability set does not exist in a resource group.
 
     :param name:
         Name of the availability set.
 
     :param resource_group:
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_compute_availability_set.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_compute_availability_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -77,15 +77,15 @@
     resource_group,
     tags=None,
     platform_update_domain_count=None,
     platform_fault_domain_count=None,
     virtual_machines=None,
     sku=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2.1.0
 
     Ensure an availability set exists.
 
     :param name:
@@ -184,20 +184,20 @@
                 ret["changes"]["virtual_machines"] = {
                     "old": aset_vms,
                     "new": virtual_machines,
                 }
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Availability set {} is already present.".format(name)
+            ret["comment"] = f"Availability set {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Availability set {} would be updated.".format(name)
+            ret["comment"] = f"Availability set {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -206,38 +206,42 @@
                 "platform_fault_domain_count": platform_fault_domain_count,
                 "sku": sku,
                 "tags": tags,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Availability set {} would be created.".format(name)
+        ret["comment"] = f"Availability set {name} would be created."
         ret["result"] = None
         return ret
 
     aset_kwargs = kwargs.copy()
     aset_kwargs.update(connection_auth)
 
     aset = __salt__["azurerm_compute_availability_set.create_or_update"](
         name=name,
         resource_group=resource_group,
         virtual_machines=virtual_machines,
         platform_update_domain_count=platform_update_domain_count,
         platform_fault_domain_count=platform_fault_domain_count,
         sku=sku,
         tags=tags,
-        **aset_kwargs
+        **aset_kwargs,
     )
 
     if "error" not in aset:
         ret["result"] = True
-        ret["comment"] = "Availability set {} has been created.".format(name)
+        ret["comment"] = f"Availability set {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create availability set {}! ({})".format(name, aset.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create availability set {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, aset.get("error")
+    )
     return ret
 
 
 def absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -261,31 +265,31 @@
 
     aset = __salt__["azurerm_compute_availability_set.get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in aset:
         ret["result"] = True
-        ret["comment"] = "Availability set {} was not found.".format(name)
+        ret["comment"] = f"Availability set {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Availability set {} would be deleted.".format(name)
+        ret["comment"] = f"Availability set {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": aset,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_compute_availability_set.delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Availability set {} has been deleted.".format(name)
+        ret["comment"] = f"Availability set {name} has been deleted."
         ret["changes"] = {"old": aset, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete availability set {}!".format(name)
+    ret["comment"] = f"Failed to delete availability set {name}!"
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_compute_virtual_machine.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_compute_virtual_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -253,15 +253,15 @@
         licensed on-premises. This element is only used for images that contain the Windows Server operating system.
 
     :param zones: A list of the virtual machine zones.
 
     :param availability_set: The resource ID of the availability set that the virtual machine should be assigned to.
         Virtual machines specified in the same availability set are allocated to different nodes to maximize
         availability. For more information about availability sets, see `Manage the availability of virtual
-        machines <https://docs.microsoft.com/azure/virtual-machines/virtual-machines-windows-manage-availability>`_.
+        machines <https://learn.microsoft.com/en-us/azure/virtual-machines/availability-set-overview>`_.
         Currently, a VM can only be added to availability set at creation time. An existing VM cannot be added to an
         availability set. This parameter cannot be specified if the ``virtual_machine_scale_set`` parameter is also
         specified.
 
     :param virtual_machine_scale_set: The resource ID of the virtual machine scale set that the virtual machine should
         be assigned to. Virtual machines specified in the same virtual machine scale set are allocated to different
         nodes to maximize availability. Currently, a VM can only be added to virtual machine scale set at creation time.
@@ -543,25 +543,25 @@
         if admin_password and force_admin_password:
             ret["changes"]["admin_password"] = {"new": "REDACTED"}
         elif ret["changes"]:
             ret["changes"]["admin_password"] = {"new": "REDACTED"}
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Virtual machine {} is already present.".format(name)
+            ret["comment"] = f"Virtual machine {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Virtual machine {} would be updated.".format(name)
+            ret["comment"] = f"Virtual machine {name} would be updated."
             return ret
 
     if __opts__["test"]:
         ret["result"] = None
-        ret["comment"] = "Virtual machine {} would be created.".format(name)
+        ret["comment"] = f"Virtual machine {name} would be created."
         return ret
 
     vm_kwargs = kwargs.copy()
     vm_kwargs.update(connection_auth)
 
     virt_mach = __salt__["azurerm_compute_virtual_machine.create_or_update"](
         name=name,
@@ -618,15 +618,17 @@
         ret["changes"] = {"old": {}, "new": virt_mach}
 
     if "error" not in virt_mach:
         ret["result"] = True
         ret["comment"] = f"Virtual machine {name} has been {action}d."
         return ret
 
-    ret["comment"] = "Failed to {} virtual machine {}! ({})".format(
+    ret[
+        "comment"
+    ] = "Failed to {} virtual machine {}! ({})".format(  # pylint: disable=consider-using-f-string
         action, name, virt_mach.get("error")
     )
     if not ret["result"]:
         ret["changes"] = {}
     return ret
 
 
@@ -684,19 +686,19 @@
 
     virt_mach = __salt__["azurerm_compute_virtual_machine.get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in virt_mach:
         ret["result"] = True
-        ret["comment"] = "Virtual machine {} was not found.".format(name)
+        ret["comment"] = f"Virtual machine {name} was not found."
         return ret
 
     if __opts__["test"]:
-        ret["comment"] = "Virtual machine {} would be deleted.".format(name)
+        ret["comment"] = f"Virtual machine {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": virt_mach,
             "new": {},
         }
         return ret
 
@@ -798,13 +800,13 @@
                             pip_name,
                             pip_group,
                             azurerm_log_level="info",
                             **connection_auth,
                         )
 
         ret["result"] = True
-        ret["comment"] = "Virtual machine {} has been deleted.".format(name)
+        ret["comment"] = f"Virtual machine {name} has been deleted."
         ret["changes"] = {"old": virt_mach, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete virtual machine {}!".format(name)
+    ret["comment"] = f"Failed to delete virtual machine {name}!"
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_dns.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_dns.py`

 * *Files 5% similar despite different names*

```diff
@@ -120,15 +120,15 @@
     if_match=None,
     if_none_match=None,
     registration_virtual_networks=None,
     resolution_virtual_networks=None,
     tags=None,
     zone_type="Public",
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 3000
 
     Ensure a DNS zone exists.
 
     :param name:
@@ -159,15 +159,15 @@
 
     :param tags:
         A dictionary of strings can be passed as tag metadata to the DNS zone object.
 
     :param zone_type:
         The type of this DNS zone (Public or Private). Possible values include: 'Public', 'Private'.
         Default value: 'Public'
-         (requires `azure-mgmt-dns <https://pypi.python.org/pypi/azure-mgmt-dns>`_ >= 2.0.0rc1)
+        (requires `azure-mgmt-dns <https://pypi.python.org/pypi/azure-mgmt-dns>`_ >= 2.0.0rc1)
 
     :param connection_auth:
         A dict with subscription and authentication parameters to be used in connecting to the
         Azure Resource Manager API.
 
     Example usage:
 
@@ -246,20 +246,20 @@
                     ret["changes"]["resolution_virtual_networks"] = {
                         "old": remote_res_vnets,
                         "new": local_res_vnets,
                     }
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "DNS zone {} is already present.".format(name)
+            ret["comment"] = f"DNS zone {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "DNS zone {} would be updated.".format(name)
+            ret["comment"] = f"DNS zone {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -269,15 +269,15 @@
                 "resolution_virtual_networks": resolution_virtual_networks,
                 "tags": tags,
                 "zone_type": zone_type,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "DNS zone {} would be created.".format(name)
+        ret["comment"] = f"DNS zone {name} would be created."
         ret["result"] = None
         return ret
 
     zone_kwargs = kwargs.copy()
     zone_kwargs.update(connection_auth)
 
     zone = __salt__["azurerm_dns.zone_create_or_update"](
@@ -286,23 +286,27 @@
         etag=etag,
         if_match=if_match,
         if_none_match=if_none_match,
         registration_virtual_networks=registration_virtual_networks,
         resolution_virtual_networks=resolution_virtual_networks,
         tags=tags,
         zone_type=zone_type,
-        **zone_kwargs
+        **zone_kwargs,
     )
 
     if "error" not in zone:
         ret["result"] = True
-        ret["comment"] = "DNS zone {} has been created.".format(name)
+        ret["comment"] = f"DNS zone {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create DNS zone {}! ({})".format(name, zone.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create DNS zone {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, zone.get("error")
+    )
     return ret
 
 
 def zone_absent(name, resource_group, zone_type="Public", connection_auth=None):
     """
     .. versionadded:: 3000
 
@@ -317,52 +321,52 @@
     :param connection_auth:
         A dict with subscription and authentication parameters to be used in connecting to the
         Azure Resource Manager API.
 
     :param zone_type:
         The type of this DNS zone (Public or Private). Possible values include: 'Public', 'Private'.
         Default value: 'Public'
-         (requires `azure-mgmt-dns <https://pypi.python.org/pypi/azure-mgmt-dns>`_ >= 2.0.0rc1)
+        (requires `azure-mgmt-dns <https://pypi.python.org/pypi/azure-mgmt-dns>`_ >= 2.0.0rc1)
 
     """
     ret = {"name": name, "result": False, "comment": "", "changes": {}}
 
     if not isinstance(connection_auth, dict):
         ret["comment"] = "Connection information must be specified via connection_auth dictionary!"
         return ret
 
     zone = __salt__["azurerm_dns.zone_get"](
         name, resource_group, azurerm_log_level="info", zone_type=zone_type, **connection_auth
     )
 
     if "error" in zone:
         ret["result"] = True
-        ret["comment"] = "DNS zone {} was not found.".format(name)
+        ret["comment"] = f"DNS zone {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "DNS zone {} would be deleted.".format(name)
+        ret["comment"] = f"DNS zone {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": zone,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_dns.zone_delete"](
         name, resource_group, zone_type=zone_type, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "DNS zone {} has been deleted.".format(name)
+        ret["comment"] = f"DNS zone {name} has been deleted."
         ret["changes"] = {"old": zone, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete DNS zone {}!".format(name)
+    ret["comment"] = f"Failed to delete DNS zone {name}!"
     return ret
 
 
 def record_set_present(
     name,
     zone_name,
     resource_group,
@@ -380,15 +384,15 @@
     ptr_records=None,
     srv_records=None,
     txt_records=None,
     cname_record=None,
     soa_record=None,
     caa_records=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 3000
 
     Ensure a record set exists in a DNS zone.
 
     :param name:
@@ -426,69 +430,69 @@
 
     :param ttl:
         The TTL (time-to-live) of the records in the record set. Required when specifying record information.
 
     :param arecords:
         The list of A records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.arecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.arecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param aaaa_records:
         The list of AAAA records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.aaaarecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.aaaarecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param mx_records:
         The list of MX records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.mxrecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.mxrecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param ns_records:
         The list of NS records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.nsrecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.nsrecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param ptr_records:
         The list of PTR records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.ptrrecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.ptrrecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param srv_records:
         The list of SRV records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.srvrecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.srvrecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param txt_records:
         The list of TXT records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.txtrecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.txtrecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param cname_record:
         The CNAME record in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.cnamerecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.cnamerecord?view=azure-python>`__
         to create a dictionary representing the record object.
 
     :param soa_record:
         The SOA record in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.soarecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.soarecord?view=azure-python>`__
         to create a dictionary representing the record object.
 
     :param caa_records:
         The list of CAA records in the record set. View the
         `Azure SDK documentation
-        <https://docs.microsoft.com/en-us/python/api/azure.mgmt.dns.models.caarecord?view=azure-python>`__
+        <https://learn.microsoft.com/en-us/python/api/azure-mgmt-dns/azure.mgmt.dns.v2018_05_01.models.caarecord?view=azure-python>`__
         to create a list of dictionaries representing the record objects.
 
     :param connection_auth:
         A dict with subscription and authentication parameters to be used in connecting to the
         Azure Resource Manager API.
 
     Example usage:
@@ -532,15 +536,15 @@
     rec_set = __salt__["azurerm_dns.record_set_get"](
         name,
         zone_name,
         resource_group,
         record_type,
         zone_type,
         azurerm_log_level="info",
-        **connection_auth
+        **connection_auth,
     )
 
     if "error" not in rec_set:
         metadata_changes = salt.utils.dictdiffer.deep_diff(
             rec_set.get("metadata", {}), metadata or {}
         )
         if metadata_changes:
@@ -556,26 +560,27 @@
                 if not rec_set.get(record_str):
                     ret["changes"] = {"new": {record_str: record}}
                     continue
                 if record_str[-1] != "s":
                     if not isinstance(record, dict):
                         ret[
                             "comment"
-                        ] = "{} record information must be specified as a dictionary!".format(
+                        ] = "{} record information must be specified as a dictionary!".format(  # pylint: disable=consider-using-f-string
                             record_str
                         )
                         return ret
                     for key, val in record.items():
                         if val != rec_set[record_str].get(key):
                             ret["changes"] = {"new": {record_str: record}}
                 elif record_str[-1] == "s":
                     if not isinstance(record, list):
-                        ret["comment"] = (
-                            "{} record information must be specified as a list of"
-                            " dictionaries!".format(record_str)
+                        ret[
+                            "comment"
+                        ] = "{} record information must be specified as a list of dictionaries!".format(  # pylint: disable=consider-using-f-string
+                            record_str
                         )
                         return ret
                     local, remote = (sorted(config) for config in (record, rec_set[record_str]))
                     for val in local:
                         for key in val:
                             local_val = val[key]
                             remote_val = remote.get(key)
@@ -584,20 +589,20 @@
                             if isinstance(remote_val, str):
                                 remote_val = remote_val.lower()
                             if local_val != remote_val:
                                 ret["changes"] = {"new": {record_str: record}}
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Record set {} is already present.".format(name)
+            ret["comment"] = f"Record set {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Record set {} would be updated.".format(name)
+            ret["comment"] = f"Record set {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -612,15 +617,15 @@
         for record in record_vars:
             # pylint: disable=eval-used
             if eval(record):
                 # pylint: disable=eval-used
                 ret["changes"]["new"][record] = eval(record)
 
     if __opts__["test"]:
-        ret["comment"] = "Record set {} would be created.".format(name)
+        ret["comment"] = f"Record set {name} would be created."
         ret["result"] = None
         return ret
 
     rec_set_kwargs = kwargs.copy()
     rec_set_kwargs.update(connection_auth)
 
     rec_set = __salt__["azurerm_dns.record_set_create_or_update"](
@@ -640,23 +645,27 @@
         ns_records=ns_records,
         ptr_records=ptr_records,
         srv_records=srv_records,
         txt_records=txt_records,
         cname_record=cname_record,
         soa_record=soa_record,
         caa_records=caa_records,
-        **rec_set_kwargs
+        **rec_set_kwargs,
     )
 
     if "error" not in rec_set:
         ret["result"] = True
-        ret["comment"] = "Record set {} has been created.".format(name)
+        ret["comment"] = f"Record set {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create record set {}! ({})".format(name, rec_set.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create record set {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, rec_set.get("error")
+    )
     return ret
 
 
 def record_set_absent(
     name, zone_name, resource_group, record_type, zone_type="Public", connection_auth=None
 ):
     """
@@ -693,41 +702,41 @@
     rec_set = __salt__["azurerm_dns.record_set_get"](
         name,
         zone_name,
         resource_group,
         record_type=record_type,
         azurerm_log_level="info",
         zone_type=zone_type,
-        **connection_auth
+        **connection_auth,
     )
 
     if "error" in rec_set:
         ret["result"] = True
-        ret["comment"] = "Record set {} was not found in zone {}.".format(name, zone_name)
+        ret["comment"] = f"Record set {name} was not found in zone {zone_name}."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Record set {} would be deleted.".format(name)
+        ret["comment"] = f"Record set {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": rec_set,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_dns.record_set_delete"](
         name,
         zone_name,
         resource_group,
         record_type=record_type,
         zone_type=zone_type,
-        **connection_auth
+        **connection_auth,
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Record set {} has been deleted.".format(name)
+        ret["comment"] = f"Record set {name} has been deleted."
         ret["changes"] = {"old": rec_set, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete record set {}!".format(name)
+    ret["comment"] = f"Failed to delete record set {name}!"
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_keyvault_key.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_keyvault_key.py`

 * *Files 4% similar despite different names*

```diff
@@ -165,24 +165,24 @@
                 ret["changes"]["not_before"] = {
                     "old": key.get("properties", {}).get("not_before"),
                     "new": not_before,
                 }
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Key {} is already present.".format(name)
+            ret["comment"] = f"Key {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Key {} would be updated.".format(name)
+            ret["comment"] = f"Key {name} would be updated."
             return ret
 
     if __opts__["test"]:
-        ret["comment"] = "Key {} would be created.".format(name)
+        ret["comment"] = f"Key {name} would be created."
         ret["result"] = None
         return ret
 
     key_kwargs = kwargs.copy()
     key_kwargs.update(connection_auth)
 
     key = __salt__["azurerm_keyvault_key.create_key"](
@@ -204,15 +204,17 @@
         ret["changes"] = {"old": {}, "new": key}
 
     if "error" not in key:
         ret["result"] = True
         ret["comment"] = f"Key {name} has been {action}d."
         return ret
 
-    ret["comment"] = "Failed to {} Key {}! ({})".format(action, name, key.get("error"))
+    ret["comment"] = "Failed to {} Key {}! ({})".format(  # pylint: disable=consider-using-f-string
+        action, name, key.get("error")
+    )
     if not ret["result"]:
         ret["changes"] = {}
     return ret
 
 
 def absent(name, vault_url, connection_auth=None):
     """
@@ -250,31 +252,31 @@
         vault_url=vault_url,
         azurerm_log_level="info",
         **connection_auth,
     )
 
     if "error" in key:
         ret["result"] = True
-        ret["comment"] = "Key {} was not found.".format(name)
+        ret["comment"] = f"Key {name} was not found."
         return ret
 
     if __opts__["test"]:
-        ret["comment"] = "Key {} would be deleted.".format(name)
+        ret["comment"] = f"Key {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": key,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_keyvault_key.begin_delete_key"](
         name=name, vault_url=vault_url, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Key {} has been deleted.".format(name)
+        ret["comment"] = f"Key {name} has been deleted."
         ret["changes"] = {"old": key, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete Key {}!".format(name)
+    ret["comment"] = f"Failed to delete Key {name}!"
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_keyvault_secret.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_keyvault_secret.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,24 +161,24 @@
                 ret["changes"]["not_before"] = {
                     "old": secret.get("properties", {}).get("not_before"),
                     "new": not_before,
                 }
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Secret {} is already present.".format(name)
+            ret["comment"] = f"Secret {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Secret {} would be updated.".format(name)
+            ret["comment"] = f"Secret {name} would be updated."
             return ret
 
     if __opts__["test"]:
-        ret["comment"] = "Secret {} would be created.".format(name)
+        ret["comment"] = f"Secret {name} would be created."
         ret["result"] = None
         return ret
 
     secret_kwargs = kwargs.copy()
     secret_kwargs.update(connection_auth)
 
     if action == "create" or (action == "update" and ret["changes"].get("value")):
@@ -212,15 +212,19 @@
             ret["changes"]["new"]["value"] = "REDACTED"
 
     if "error" not in secret:
         ret["result"] = True
         ret["comment"] = f"Secret {name} has been {action}d."
         return ret
 
-    ret["comment"] = "Failed to {} Secret {}! ({})".format(action, name, secret.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to {} Secret {}! ({})".format(  # pylint: disable=consider-using-f-string
+        action, name, secret.get("error")
+    )
     if not ret["result"]:
         ret["changes"] = {}
     return ret
 
 
 def absent(name, vault_url, purge=False, wait=False, connection_auth=None):
     """
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_keyvault_vault.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_keyvault_vault.py`

 * *Files 5% similar despite different names*

```diff
@@ -328,24 +328,24 @@
                 ret["changes"]["properties"]["network_acls"] = acls_changes
 
         if not ret["changes"]["properties"]:
             del ret["changes"]["properties"]
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Key Vault {} is already present.".format(name)
+            ret["comment"] = f"Key Vault {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Key Vault {} would be updated.".format(name)
+            ret["comment"] = f"Key Vault {name} would be updated."
             return ret
 
     if __opts__["test"]:
-        ret["comment"] = "Key vault {} would be created.".format(name)
+        ret["comment"] = f"Key vault {name} would be created."
         ret["result"] = None
         return ret
 
     vault_kwargs = kwargs.copy()
     vault_kwargs.update(connection_auth)
 
     vault = __salt__["azurerm_keyvault_vault.create_or_update"](
@@ -373,15 +373,19 @@
         ret["changes"] = {"old": {}, "new": vault}
 
     if "error" not in vault:
         ret["result"] = True
         ret["comment"] = f"Key Vault {name} has been {action}d."
         return ret
 
-    ret["comment"] = "Failed to {} Key Vault {}! ({})".format(action, name, vault.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to {} Key Vault {}! ({})".format(  # pylint: disable=consider-using-f-string
+        action, name, vault.get("error")
+    )
     if not ret["result"]:
         ret["changes"] = {}
     return ret
 
 
 def absent(name, resource_group, connection_auth=None):
     """
@@ -414,29 +418,29 @@
 
     vault = __salt__["azurerm_keyvault_vault.get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in vault:
         ret["result"] = True
-        ret["comment"] = "Key Vault {} was not found.".format(name)
+        ret["comment"] = f"Key Vault {name} was not found."
         return ret
 
     if __opts__["test"]:
-        ret["comment"] = "Key Vault {} would be deleted.".format(name)
+        ret["comment"] = f"Key Vault {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": vault,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_keyvault_vault.delete"](name, resource_group, **connection_auth)
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Key Vault {} has been deleted.".format(name)
+        ret["comment"] = f"Key Vault {name} has been deleted."
         ret["changes"] = {"old": vault, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete Key Vault {}!".format(name)
+    ret["comment"] = f"Failed to delete Key Vault {name}!"
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_network.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_network.py`

 * *Files 8% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 def virtual_network_present(
     name,
     address_prefixes,
     resource_group,
     dns_servers=None,
     tags=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a virtual network exists.
 
     :param name:
@@ -192,20 +192,20 @@
             ret["changes"]["enable_vm_protection"] = {
                 "old": vnet.get("enable_vm_protection"),
                 "new": kwargs.get("enable_vm_protection"),
             }
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Virtual network {} is already present.".format(name)
+            ret["comment"] = f"Virtual network {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Virtual network {} would be updated.".format(name)
+            ret["comment"] = f"Virtual network {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -215,36 +215,40 @@
                 "enable_ddos_protection": kwargs.get("enable_ddos_protection", False),
                 "enable_vm_protection": kwargs.get("enable_vm_protection", False),
                 "tags": tags,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Virtual network {} would be created.".format(name)
+        ret["comment"] = f"Virtual network {name} would be created."
         ret["result"] = None
         return ret
 
     vnet_kwargs = kwargs.copy()
     vnet_kwargs.update(connection_auth)
 
     vnet = __salt__["azurerm_network.virtual_network_create_or_update"](
         name=name,
         resource_group=resource_group,
         address_prefixes=address_prefixes,
         dns_servers=dns_servers,
         tags=tags,
-        **vnet_kwargs
+        **vnet_kwargs,
     )
 
     if "error" not in vnet:
         ret["result"] = True
-        ret["comment"] = "Virtual network {} has been created.".format(name)
+        ret["comment"] = f"Virtual network {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create virtual network {}! ({})".format(name, vnet.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create virtual network {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, vnet.get("error")
+    )
     return ret
 
 
 def virtual_network_absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -268,49 +272,49 @@
 
     vnet = __salt__["azurerm_network.virtual_network_get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in vnet:
         ret["result"] = True
-        ret["comment"] = "Virtual network {} was not found.".format(name)
+        ret["comment"] = f"Virtual network {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Virtual network {} would be deleted.".format(name)
+        ret["comment"] = f"Virtual network {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": vnet,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.virtual_network_delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Virtual network {} has been deleted.".format(name)
+        ret["comment"] = f"Virtual network {name} has been deleted."
         ret["changes"] = {"old": vnet, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete virtual network {}!".format(name)
+    ret["comment"] = f"Failed to delete virtual network {name}!"
     return ret
 
 
 def subnet_present(
     name,
     address_prefix,
     virtual_network,
     resource_group,
     security_group=None,
     route_table=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a subnet exists.
 
     :param name:
@@ -386,57 +390,61 @@
             rttbl_name = snet["route_table"]["id"].split("/")[-1]
 
         if route_table and (route_table != rttbl_name):
             ret["changes"]["route_table"] = {"old": rttbl_name, "new": route_table}
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Subnet {} is already present.".format(name)
+            ret["comment"] = f"Subnet {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Subnet {} would be updated.".format(name)
+            ret["comment"] = f"Subnet {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
                 "address_prefix": address_prefix,
                 "network_security_group": security_group,
                 "route_table": route_table,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Subnet {} would be created.".format(name)
+        ret["comment"] = f"Subnet {name} would be created."
         ret["result"] = None
         return ret
 
     snet_kwargs = kwargs.copy()
     snet_kwargs.update(connection_auth)
 
     snet = __salt__["azurerm_network.subnet_create_or_update"](
         name=name,
         virtual_network=virtual_network,
         resource_group=resource_group,
         address_prefix=address_prefix,
         network_security_group=security_group,
         route_table=route_table,
-        **snet_kwargs
+        **snet_kwargs,
     )
 
     if "error" not in snet:
         ret["result"] = True
-        ret["comment"] = "Subnet {} has been created.".format(name)
+        ret["comment"] = f"Subnet {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create subnet {}! ({})".format(name, snet.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create subnet {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, snet.get("error")
+    )
     return ret
 
 
 def subnet_absent(name, virtual_network, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -463,37 +471,37 @@
 
     snet = __salt__["azurerm_network.subnet_get"](
         name, virtual_network, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in snet:
         ret["result"] = True
-        ret["comment"] = "Subnet {} was not found.".format(name)
+        ret["comment"] = f"Subnet {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Subnet {} would be deleted.".format(name)
+        ret["comment"] = f"Subnet {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": snet,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.subnet_delete"](
         name, virtual_network, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Subnet {} has been deleted.".format(name)
+        ret["comment"] = f"Subnet {name} has been deleted."
         ret["changes"] = {"old": snet, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete subnet {}!".format(name)
+    ret["comment"] = f"Failed to delete subnet {name}!"
     return ret
 
 
 def network_security_group_present(
     name, resource_group, tags=None, security_rules=None, connection_auth=None, **kwargs
 ):
     """
@@ -573,63 +581,69 @@
 
         if security_rules:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 nsg.get("security_rules", []), security_rules
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"security_rules" {}'.format(comp_ret["comment"])
+                ret[
+                    "comment"
+                ] = '"security_rules" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["security_rules"] = comp_ret["changes"]
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Network security group {} is already present.".format(name)
+            ret["comment"] = f"Network security group {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Network security group {} would be updated.".format(name)
+            ret["comment"] = f"Network security group {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
                 "resource_group": resource_group,
                 "tags": tags,
                 "security_rules": security_rules,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Network security group {} would be created.".format(name)
+        ret["comment"] = f"Network security group {name} would be created."
         ret["result"] = None
         return ret
 
     nsg_kwargs = kwargs.copy()
     nsg_kwargs.update(connection_auth)
 
     nsg = __salt__["azurerm_network.network_security_group_create_or_update"](
         name=name,
         resource_group=resource_group,
         tags=tags,
         security_rules=security_rules,
-        **nsg_kwargs
+        **nsg_kwargs,
     )
 
     if "error" not in nsg:
         ret["result"] = True
-        ret["comment"] = "Network security group {} has been created.".format(name)
+        ret["comment"] = f"Network security group {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create network security group {}! ({})".format(
+    ret[
+        "comment"
+    ] = "Failed to create network security group {}! ({})".format(  # pylint: disable=consider-using-f-string
         name, nsg.get("error")
     )
     return ret
 
 
 def network_security_group_absent(name, resource_group, connection_auth=None):
     """
@@ -655,37 +669,37 @@
 
     nsg = __salt__["azurerm_network.network_security_group_get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in nsg:
         ret["result"] = True
-        ret["comment"] = "Network security group {} was not found.".format(name)
+        ret["comment"] = f"Network security group {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Network security group {} would be deleted.".format(name)
+        ret["comment"] = f"Network security group {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": nsg,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.network_security_group_delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Network security group {} has been deleted.".format(name)
+        ret["comment"] = f"Network security group {name} has been deleted."
         ret["changes"] = {"old": nsg, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete network security group {}!".format(name)
+    ret["comment"] = f"Failed to delete network security group {name}!"
     return ret
 
 
 def security_rule_present(
     name,
     access,
     direction,
@@ -699,15 +713,15 @@
     source_port_range=None,
     description=None,
     destination_address_prefixes=None,
     destination_port_ranges=None,
     source_address_prefixes=None,
     source_port_ranges=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a security rule exists.
 
     :param name:
@@ -808,26 +822,28 @@
         ("destination_port_ranges", "destination_port_range"),
         ("destination_address_prefixes", "destination_address_prefix"),
     ]
 
     for params in exclusive_params:
         # pylint: disable=eval-used
         if not eval(params[0]) and not eval(params[1]):
-            ret["comment"] = "Either the {} or {} parameter must be provided!".format(
+            ret[
+                "comment"
+            ] = "Either the {} or {} parameter must be provided!".format(  # pylint: disable=consider-using-f-string
                 params[0], params[1]
             )
             return ret
         # pylint: disable=eval-used
         if eval(params[0]):
             # pylint: disable=eval-used
             if not isinstance(eval(params[0]), list):
-                ret["comment"] = "The {} parameter must be a list!".format(params[0])
+                ret["comment"] = f"The {params[0]} parameter must be a list!"
                 return ret
             # pylint: disable=exec-used
-            exec("{} = None".format(params[1]))
+            exec(f"{params[1]} = None")
 
     rule = __salt__["azurerm_network.security_rule_get"](
         name, security_group, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" not in rule:
         # access changes
@@ -942,20 +958,20 @@
                             "old": rule.get("source_address_prefixes"),
                             "new": source_address_prefixes,
                         }
                         break
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Security rule {} is already present.".format(name)
+            ret["comment"] = f"Security rule {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Security rule {} would be updated.".format(name)
+            ret["comment"] = f"Security rule {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -972,15 +988,15 @@
                 "source_address_prefixes": source_address_prefixes,
                 "source_port_range": source_port_range,
                 "source_port_ranges": source_port_ranges,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Security rule {} would be created.".format(name)
+        ret["comment"] = f"Security rule {name} would be created."
         ret["result"] = None
         return ret
 
     rule_kwargs = kwargs.copy()
     rule_kwargs.update(connection_auth)
 
     rule = __salt__["azurerm_network.security_rule_create_or_update"](
@@ -996,23 +1012,27 @@
         destination_address_prefixes=destination_address_prefixes,
         destination_port_range=destination_port_range,
         destination_port_ranges=destination_port_ranges,
         source_address_prefix=source_address_prefix,
         source_address_prefixes=source_address_prefixes,
         source_port_range=source_port_range,
         source_port_ranges=source_port_ranges,
-        **rule_kwargs
+        **rule_kwargs,
     )
 
     if "error" not in rule:
         ret["result"] = True
-        ret["comment"] = "Security rule {} has been created.".format(name)
+        ret["comment"] = f"Security rule {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create security rule {}! ({})".format(name, rule.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create security rule {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, rule.get("error")
+    )
     return ret
 
 
 def security_rule_absent(name, security_group, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -1039,37 +1059,37 @@
 
     rule = __salt__["azurerm_network.security_rule_get"](
         name, security_group, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in rule:
         ret["result"] = True
-        ret["comment"] = "Security rule {} was not found.".format(name)
+        ret["comment"] = f"Security rule {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Security rule {} would be deleted.".format(name)
+        ret["comment"] = f"Security rule {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": rule,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.security_rule_delete"](
         name, security_group, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Security rule {} has been deleted.".format(name)
+        ret["comment"] = f"Security rule {name} has been deleted."
         ret["changes"] = {"old": rule, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete security rule {}!".format(name)
+    ret["comment"] = f"Failed to delete security rule {name}!"
     return ret
 
 
 def load_balancer_present(
     name,
     resource_group,
     sku=None,
@@ -1078,15 +1098,15 @@
     load_balancing_rules=None,
     probes=None,
     inbound_nat_rules=None,
     inbound_nat_pools=None,
     outbound_nat_rules=None,
     tags=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a load balancer exists.
 
     :param name:
@@ -1278,114 +1298,140 @@
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 load_bal.get("frontend_ip_configurations", []),
                 frontend_ip_configurations,
                 ["public_ip_address", "subnet"],
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"frontend_ip_configurations" {}'.format(comp_ret["comment"])
+                ret[
+                    "comment"
+                ] = '"frontend_ip_configurations" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["frontend_ip_configurations"] = comp_ret["changes"]
 
         # backend_address_pools changes
         if backend_address_pools:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 load_bal.get("backend_address_pools", []), backend_address_pools
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"backend_address_pools" {}'.format(comp_ret["comment"])
+                ret[
+                    "comment"
+                ] = '"backend_address_pools" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["backend_address_pools"] = comp_ret["changes"]
 
         # probes changes
         if probes:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 load_bal.get("probes", []), probes
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"probes" {}'.format(comp_ret["comment"])
+                ret["comment"] = '"probes" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["probes"] = comp_ret["changes"]
 
         # load_balancing_rules changes
         if load_balancing_rules:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 load_bal.get("load_balancing_rules", []),
                 load_balancing_rules,
                 ["frontend_ip_configuration", "backend_address_pool", "probe"],
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"load_balancing_rules" {}'.format(comp_ret["comment"])
+                ret[
+                    "comment"
+                ] = '"load_balancing_rules" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["load_balancing_rules"] = comp_ret["changes"]
 
         # inbound_nat_rules changes
         if inbound_nat_rules:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 load_bal.get("inbound_nat_rules", []),
                 inbound_nat_rules,
                 ["frontend_ip_configuration"],
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"inbound_nat_rules" {}'.format(comp_ret["comment"])
+                ret[
+                    "comment"
+                ] = '"inbound_nat_rules" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["inbound_nat_rules"] = comp_ret["changes"]
 
         # inbound_nat_pools changes
         if inbound_nat_pools:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 load_bal.get("inbound_nat_pools", []),
                 inbound_nat_pools,
                 ["frontend_ip_configuration"],
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"inbound_nat_pools" {}'.format(comp_ret["comment"])
+                ret[
+                    "comment"
+                ] = '"inbound_nat_pools" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["inbound_nat_pools"] = comp_ret["changes"]
 
         # outbound_nat_rules changes
         if outbound_nat_rules:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 load_bal.get("outbound_nat_rules", []),
                 outbound_nat_rules,
                 ["frontend_ip_configuration"],
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"outbound_nat_rules" {}'.format(comp_ret["comment"])
+                ret[
+                    "comment"
+                ] = '"outbound_nat_rules" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["outbound_nat_rules"] = comp_ret["changes"]
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Load balancer {} is already present.".format(name)
+            ret["comment"] = f"Load balancer {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Load balancer {} would be updated.".format(name)
+            ret["comment"] = f"Load balancer {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -1398,15 +1444,15 @@
                 "inbound_nat_rules": inbound_nat_rules,
                 "inbound_nat_pools": inbound_nat_pools,
                 "outbound_nat_rules": outbound_nat_rules,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Load balancer {} would be created.".format(name)
+        ret["comment"] = f"Load balancer {name} would be created."
         ret["result"] = None
         return ret
 
     lb_kwargs = kwargs.copy()
     lb_kwargs.update(connection_auth)
 
     load_bal = __salt__["azurerm_network.load_balancer_create_or_update"](
@@ -1417,23 +1463,27 @@
         frontend_ip_configurations=frontend_ip_configurations,
         backend_address_pools=backend_address_pools,
         load_balancing_rules=load_balancing_rules,
         probes=probes,
         inbound_nat_rules=inbound_nat_rules,
         inbound_nat_pools=inbound_nat_pools,
         outbound_nat_rules=outbound_nat_rules,
-        **lb_kwargs
+        **lb_kwargs,
     )
 
     if "error" not in load_bal:
         ret["result"] = True
-        ret["comment"] = "Load balancer {} has been created.".format(name)
+        ret["comment"] = f"Load balancer {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create load balancer {}! ({})".format(name, load_bal.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create load balancer {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, load_bal.get("error")
+    )
     return ret
 
 
 def load_balancer_absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -1457,51 +1507,51 @@
 
     load_bal = __salt__["azurerm_network.load_balancer_get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in load_bal:
         ret["result"] = True
-        ret["comment"] = "Load balancer {} was not found.".format(name)
+        ret["comment"] = f"Load balancer {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Load balancer {} would be deleted.".format(name)
+        ret["comment"] = f"Load balancer {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": load_bal,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.load_balancer_delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Load balancer {} has been deleted.".format(name)
+        ret["comment"] = f"Load balancer {name} has been deleted."
         ret["changes"] = {"old": load_bal, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete load balancer {}!".format(name)
+    ret["comment"] = f"Failed to delete load balancer {name}!"
     return ret
 
 
 def public_ip_address_present(
     name,
     resource_group,
     tags=None,
     sku=None,
     public_ip_allocation_method=None,
     public_ip_address_version=None,
     dns_settings=None,
     idle_timeout_in_minutes=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a public IP address exists.
 
     :param name:
@@ -1626,20 +1676,20 @@
             ret["changes"]["idle_timeout_in_minutes"] = {
                 "old": pub_ip.get("idle_timeout_in_minutes"),
                 "new": idle_timeout_in_minutes,
             }
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Public IP address {} is already present.".format(name)
+            ret["comment"] = f"Public IP address {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Public IP address {} would be updated.".format(name)
+            ret["comment"] = f"Public IP address {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -1649,15 +1699,15 @@
                 "public_ip_allocation_method": public_ip_allocation_method,
                 "public_ip_address_version": public_ip_address_version,
                 "idle_timeout_in_minutes": idle_timeout_in_minutes,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Public IP address {} would be created.".format(name)
+        ret["comment"] = f"Public IP address {name} would be created."
         ret["result"] = None
         return ret
 
     pub_ip_kwargs = kwargs.copy()
     pub_ip_kwargs.update(connection_auth)
 
     pub_ip = __salt__["azurerm_network.public_ip_address_create_or_update"](
@@ -1665,23 +1715,27 @@
         resource_group=resource_group,
         sku=sku,
         tags=tags,
         dns_settings=dns_settings,
         public_ip_allocation_method=public_ip_allocation_method,
         public_ip_address_version=public_ip_address_version,
         idle_timeout_in_minutes=idle_timeout_in_minutes,
-        **pub_ip_kwargs
+        **pub_ip_kwargs,
     )
 
     if "error" not in pub_ip:
         ret["result"] = True
-        ret["comment"] = "Public IP address {} has been created.".format(name)
+        ret["comment"] = f"Public IP address {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create public IP address {}! ({})".format(name, pub_ip.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create public IP address {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, pub_ip.get("error")
+    )
     return ret
 
 
 def public_ip_address_absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -1705,37 +1759,37 @@
 
     pub_ip = __salt__["azurerm_network.public_ip_address_get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in pub_ip:
         ret["result"] = True
-        ret["comment"] = "Public IP address {} was not found.".format(name)
+        ret["comment"] = f"Public IP address {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Public IP address {} would be deleted.".format(name)
+        ret["comment"] = f"Public IP address {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": pub_ip,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.public_ip_address_delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Public IP address {} has been deleted.".format(name)
+        ret["comment"] = f"Public IP address {name} has been deleted."
         ret["changes"] = {"old": pub_ip, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete public IP address {}!".format(name)
+    ret["comment"] = f"Failed to delete public IP address {name}!"
     return ret
 
 
 def network_interface_present(
     name,
     ip_configurations,
     subnet,
@@ -1746,15 +1800,15 @@
     network_security_group=None,
     dns_settings=None,
     mac_address=None,
     primary=None,
     enable_accelerated_networking=None,
     enable_ip_forwarding=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a network interface exists.
 
     :param name:
@@ -1923,28 +1977,32 @@
         comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
             iface.get("ip_configurations", []),
             ip_configurations,
             ["public_ip_address", "subnet"],
         )
 
         if comp_ret.get("comment"):
-            ret["comment"] = '"ip_configurations" {}'.format(comp_ret["comment"])
+            ret[
+                "comment"
+            ] = '"ip_configurations" {}'.format(  # pylint: disable=consider-using-f-string
+                comp_ret["comment"]
+            )
             return ret
 
         if comp_ret.get("changes"):
             ret["changes"]["ip_configurations"] = comp_ret["changes"]
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Network interface {} is already present.".format(name)
+            ret["comment"] = f"Network interface {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Network interface {} would be updated.".format(name)
+            ret["comment"] = f"Network interface {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
@@ -1957,15 +2015,15 @@
                 "mac_address": mac_address,
                 "primary": primary,
                 "tags": tags,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Network interface {} would be created.".format(name)
+        ret["comment"] = f"Network interface {name} would be created."
         ret["result"] = None
         return ret
 
     iface_kwargs = kwargs.copy()
     iface_kwargs.update(connection_auth)
 
     iface = __salt__["azurerm_network.network_interface_create_or_update"](
@@ -1978,23 +2036,27 @@
         enable_accelerated_networking=enable_accelerated_networking,
         enable_ip_forwarding=enable_ip_forwarding,
         mac_address=mac_address,
         primary=primary,
         network_security_group=network_security_group,
         virtual_machine=virtual_machine,
         tags=tags,
-        **iface_kwargs
+        **iface_kwargs,
     )
 
     if "error" not in iface:
         ret["result"] = True
-        ret["comment"] = "Network interface {} has been created.".format(name)
+        ret["comment"] = f"Network interface {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create network interface {}! ({})".format(name, iface.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create network interface {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, iface.get("error")
+    )
     return ret
 
 
 def network_interface_absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -2018,48 +2080,48 @@
 
     iface = __salt__["azurerm_network.network_interface_get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in iface:
         ret["result"] = True
-        ret["comment"] = "Network interface {} was not found.".format(name)
+        ret["comment"] = f"Network interface {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Network interface {} would be deleted.".format(name)
+        ret["comment"] = f"Network interface {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": iface,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.network_interface_delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Network interface {} has been deleted.".format(name)
+        ret["comment"] = f"Network interface {name} has been deleted."
         ret["changes"] = {"old": iface, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete network interface {}!)".format(name)
+    ret["comment"] = f"Failed to delete network interface {name}!)"
     return ret
 
 
 def route_table_present(
     name,
     resource_group,
     tags=None,
     routes=None,
     disable_bgp_route_propagation=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a route table exists.
 
     :param name:
@@ -2135,64 +2197,70 @@
         # routes changes
         if routes:
             comp_ret = saltext.azurerm.utils.azurerm.compare_list_of_dicts(
                 rt_tbl.get("routes", []), routes
             )
 
             if comp_ret.get("comment"):
-                ret["comment"] = '"routes" {}'.format(comp_ret["comment"])
+                ret["comment"] = '"routes" {}'.format(  # pylint: disable=consider-using-f-string
+                    comp_ret["comment"]
+                )
                 return ret
 
             if comp_ret.get("changes"):
                 ret["changes"]["routes"] = comp_ret["changes"]
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Route table {} is already present.".format(name)
+            ret["comment"] = f"Route table {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Route table {} would be updated.".format(name)
+            ret["comment"] = f"Route table {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
                 "tags": tags,
                 "routes": routes,
                 "disable_bgp_route_propagation": disable_bgp_route_propagation,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Route table {} would be created.".format(name)
+        ret["comment"] = f"Route table {name} would be created."
         ret["result"] = None
         return ret
 
     rt_tbl_kwargs = kwargs.copy()
     rt_tbl_kwargs.update(connection_auth)
 
     rt_tbl = __salt__["azurerm_network.route_table_create_or_update"](
         name=name,
         resource_group=resource_group,
         disable_bgp_route_propagation=disable_bgp_route_propagation,
         routes=routes,
         tags=tags,
-        **rt_tbl_kwargs
+        **rt_tbl_kwargs,
     )
 
     if "error" not in rt_tbl:
         ret["result"] = True
-        ret["comment"] = "Route table {} has been created.".format(name)
+        ret["comment"] = f"Route table {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create route table {}! ({})".format(name, rt_tbl.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create route table {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, rt_tbl.get("error")
+    )
     return ret
 
 
 def route_table_absent(name, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -2216,49 +2284,49 @@
 
     rt_tbl = __salt__["azurerm_network.route_table_get"](
         name, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in rt_tbl:
         ret["result"] = True
-        ret["comment"] = "Route table {} was not found.".format(name)
+        ret["comment"] = f"Route table {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Route table {} would be deleted.".format(name)
+        ret["comment"] = f"Route table {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": rt_tbl,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.route_table_delete"](
         name, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Route table {} has been deleted.".format(name)
+        ret["comment"] = f"Route table {name} has been deleted."
         ret["changes"] = {"old": rt_tbl, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete route table {}!".format(name)
+    ret["comment"] = f"Failed to delete route table {name}!"
     return ret
 
 
 def route_present(
     name,
     address_prefix,
     next_hop_type,
     route_table,
     resource_group,
     next_hop_ip_address=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a route exists within a route table.
 
     :param name:
@@ -2330,57 +2398,61 @@
             ret["changes"]["next_hop_ip_address"] = {
                 "old": route.get("next_hop_ip_address"),
                 "new": next_hop_ip_address,
             }
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Route {} is already present.".format(name)
+            ret["comment"] = f"Route {name} is already present."
             return ret
 
         if __opts__["test"]:
             ret["result"] = None
-            ret["comment"] = "Route {} would be updated.".format(name)
+            ret["comment"] = f"Route {name} would be updated."
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
                 "address_prefix": address_prefix,
                 "next_hop_type": next_hop_type,
                 "next_hop_ip_address": next_hop_ip_address,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Route {} would be created.".format(name)
+        ret["comment"] = f"Route {name} would be created."
         ret["result"] = None
         return ret
 
     route_kwargs = kwargs.copy()
     route_kwargs.update(connection_auth)
 
     route = __salt__["azurerm_network.route_create_or_update"](
         name=name,
         route_table=route_table,
         resource_group=resource_group,
         address_prefix=address_prefix,
         next_hop_type=next_hop_type,
         next_hop_ip_address=next_hop_ip_address,
-        **route_kwargs
+        **route_kwargs,
     )
 
     if "error" not in route:
         ret["result"] = True
-        ret["comment"] = "Route {} has been created.".format(name)
+        ret["comment"] = f"Route {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create route {}! ({})".format(name, route.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create route {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, route.get("error")
+    )
     return ret
 
 
 def route_absent(name, route_table, resource_group, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -2407,31 +2479,31 @@
 
     route = __salt__["azurerm_network.route_get"](
         name, route_table, resource_group, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in route:
         ret["result"] = True
-        ret["comment"] = "Route {} was not found.".format(name)
+        ret["comment"] = f"Route {name} was not found."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Route {} would be deleted.".format(name)
+        ret["comment"] = f"Route {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": route,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_network.route_delete"](
         name, route_table, resource_group, **connection_auth
     )
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Route {} has been deleted.".format(name)
+        ret["comment"] = f"Route {name} has been deleted."
         ret["changes"] = {"old": route, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete route {}!".format(name)
+    ret["comment"] = f"Failed to delete route {name}!"
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/states/azurerm_resource.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/states/azurerm_resource.py`

 * *Files 7% similar despite different names*

```diff
@@ -140,25 +140,25 @@
 
     if present:
         group = __salt__["azurerm_resource.resource_group_get"](name, **connection_auth)
         ret["changes"] = salt.utils.dictdiffer.deep_diff(group.get("tags", {}), tags or {})
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Resource group {} is already present.".format(name)
+            ret["comment"] = f"Resource group {name} is already present."
             return ret
 
         if __opts__["test"]:
-            ret["comment"] = "Resource group {} tags would be updated.".format(name)
+            ret["comment"] = f"Resource group {name} tags would be updated."
             ret["result"] = None
             ret["changes"] = {"old": group.get("tags", {}), "new": tags}
             return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Resource group {} would be created.".format(name)
+        ret["comment"] = f"Resource group {name} would be created."
         ret["result"] = None
         ret["changes"] = {
             "old": {},
             "new": {
                 "name": name,
                 "location": location,
                 "managed_by": managed_by,
@@ -173,19 +173,23 @@
     group = __salt__["azurerm_resource.resource_group_create_or_update"](
         name, location, managed_by=managed_by, tags=tags, **group_kwargs
     )
     present = __salt__["azurerm_resource.resource_group_check_existence"](name, **connection_auth)
 
     if present:
         ret["result"] = True
-        ret["comment"] = "Resource group {} has been created.".format(name)
+        ret["comment"] = f"Resource group {name} has been created."
         ret["changes"] = {"old": {}, "new": group}
         return ret
 
-    ret["comment"] = "Failed to create resource group {}! ({})".format(name, group.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create resource group {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, group.get("error")
+    )
     return ret
 
 
 def resource_group_absent(name, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -206,21 +210,21 @@
 
     group = {}
 
     present = __salt__["azurerm_resource.resource_group_check_existence"](name, **connection_auth)
 
     if not present:
         ret["result"] = True
-        ret["comment"] = "Resource group {} is already absent.".format(name)
+        ret["comment"] = f"Resource group {name} is already absent."
         return ret
 
     elif __opts__["test"]:
         group = __salt__["azurerm_resource.resource_group_get"](name, **connection_auth)
 
-        ret["comment"] = "Resource group {} would be deleted.".format(name)
+        ret["comment"] = f"Resource group {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": group,
             "new": {},
         }
         return ret
 
@@ -232,19 +236,19 @@
     else:
         present = __salt__["azurerm_resource.resource_group_check_existence"](
             name, **connection_auth
         )
 
     if not present:
         ret["result"] = True
-        ret["comment"] = "Resource group {} has been deleted.".format(name)
+        ret["comment"] = f"Resource group {name} has been deleted."
         ret["changes"] = {"old": group, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete resource group {}!".format(name)
+    ret["comment"] = f"Failed to delete resource group {name}!"
     return ret
 
 
 def policy_definition_present(
     name,
     policy_rule=None,
     policy_type=None,
@@ -256,40 +260,40 @@
     policy_rule_json=None,
     policy_rule_file=None,
     template="jinja",
     source_hash=None,
     source_hash_name=None,
     skip_verify=False,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a security policy definition exists.
 
     :param name:
         Name of the policy definition.
 
     :param policy_rule:
         A YAML dictionary defining the policy rule. See `Azure Policy Definition documentation
-        <https://docs.microsoft.com/en-us/azure/azure-policy/policy-definition#policy-rule>`_ for details on the
+        <https://learn.microsoft.com/en-us/azure/governance/policy/concepts/definition-structure-policy-rule>`_ for details on the
         structure. One of ``policy_rule``, ``policy_rule_json``, or ``policy_rule_file`` is required, in that order of
         precedence for use if multiple parameters are used.
 
     :param policy_rule_json:
         A text field defining the entirety of a policy definition in JSON. See `Azure Policy Definition documentation
-        <https://docs.microsoft.com/en-us/azure/azure-policy/policy-definition#policy-rule>`_ for details on the
+        <https://learn.microsoft.com/en-us/azure/governance/policy/concepts/definition-structure-policy-rule>`_ for details on the
         structure. One of ``policy_rule``, ``policy_rule_json``, or ``policy_rule_file`` is required, in that order of
         precedence for use if multiple parameters are used. Note that the `name` field in the JSON will override the
         ``name`` parameter in the state.
 
     :param policy_rule_file:
         The source of a JSON file defining the entirety of a policy definition. See `Azure Policy Definition
-        documentation <https://docs.microsoft.com/en-us/azure/azure-policy/policy-definition#policy-rule>`_ for
+        documentation <https://learn.microsoft.com/en-us/azure/governance/policy/concepts/definition-structure-policy-rule>`_ for
         details on the structure. One of ``policy_rule``, ``policy_rule_json``, or ``policy_rule_file`` is required,
         in that order of precedence for use if multiple parameters are used. Note that the `name` field in the JSON
         will override the ``name`` parameter in the state.
 
     :param skip_verify:
         Used for the ``policy_rule_file`` parameter. If ``True``, hash verification of remote file sources
         (``http://``, ``https://``, ``ftp://``) will be skipped, and the ``source_hash`` argument will be ignored.
@@ -377,15 +381,15 @@
         return ret
 
     temp_rule = {}
     if policy_rule_json:
         try:
             temp_rule = json.loads(policy_rule_json)
         except Exception as exc:  # pylint: disable=broad-except
-            ret["comment"] = "Unable to load policy rule json! ({})".format(exc)
+            ret["comment"] = f"Unable to load policy rule json! ({exc})"
             return ret
     elif policy_rule_file:
         try:
             # pylint: disable=unused-variable
             sfn, source_sum, comment_ = __salt__["file.get_managed"](
                 None,
                 template,
@@ -395,31 +399,35 @@
                 None,
                 None,
                 None,
                 __env__,
                 None,
                 None,
                 skip_verify=skip_verify,
-                **kwargs
+                **kwargs,
             )
         except Exception as exc:  # pylint: disable=broad-except
-            ret["comment"] = 'Unable to locate policy rule file "{}"! ({})'.format(
+            ret[
+                "comment"
+            ] = 'Unable to locate policy rule file "{}"! ({})'.format(  # pylint: disable=consider-using-f-string
                 policy_rule_file, exc
             )
             return ret
 
         if not sfn:
-            ret["comment"] = 'Unable to locate policy rule file "{}"!)'.format(policy_rule_file)
+            ret["comment"] = f'Unable to locate policy rule file "{policy_rule_file}"!)'
             return ret
 
         try:
             with salt.utils.files.fopen(sfn, "r") as prf:
                 temp_rule = json.load(prf)
         except Exception as exc:  # pylint: disable=broad-except
-            ret["comment"] = 'Unable to load policy rule file "{}"! ({})'.format(
+            ret[
+                "comment"
+            ] = 'Unable to load policy rule file "{}"! ({})'.format(  # pylint: disable=consider-using-f-string
                 policy_rule_file, exc
             )
             return ret
 
         if sfn:
             salt.utils.files.remove(sfn)
 
@@ -475,19 +483,19 @@
             policy.get("parameters", {}), parameters or {}
         )
         if param_changes:
             ret["changes"]["parameters"] = param_changes
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Policy definition {} is already present.".format(name)
+            ret["comment"] = f"Policy definition {name} is already present."
             return ret
 
         if __opts__["test"]:
-            ret["comment"] = "Policy definition {} would be updated.".format(name)
+            ret["comment"] = f"Policy definition {name} would be updated."
             ret["result"] = None
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
@@ -499,15 +507,15 @@
                 "metadata": metadata,
                 "parameters": parameters,
                 "policy_rule": policy_rule,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Policy definition {} would be created.".format(name)
+        ret["comment"] = f"Policy definition {name} would be created."
         ret["result"] = None
         return ret
 
     # Convert OrderedDict to dict
     if isinstance(metadata, dict):
         metadata = json.loads(json.dumps(metadata))
     if isinstance(parameters, dict):
@@ -521,23 +529,27 @@
         policy_rule=policy_rule,
         policy_type=policy_type,
         mode=mode,
         display_name=display_name,
         description=description,
         metadata=metadata,
         parameters=parameters,
-        **policy_kwargs
+        **policy_kwargs,
     )
 
     if "error" not in policy:
         ret["result"] = True
-        ret["comment"] = "Policy definition {} has been created.".format(name)
+        ret["comment"] = f"Policy definition {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create policy definition {}! ({})".format(name, policy.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create policy definition {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, policy.get("error")
+    )
     return ret
 
 
 def policy_definition_absent(name, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -558,48 +570,48 @@
 
     policy = __salt__["azurerm_resource.policy_definition_get"](
         name, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in policy:
         ret["result"] = True
-        ret["comment"] = "Policy definition {} is already absent.".format(name)
+        ret["comment"] = f"Policy definition {name} is already absent."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Policy definition {} would be deleted.".format(name)
+        ret["comment"] = f"Policy definition {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": policy,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_resource.policy_definition_delete"](name, **connection_auth)
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Policy definition {} has been deleted.".format(name)
+        ret["comment"] = f"Policy definition {name} has been deleted."
         ret["changes"] = {"old": policy, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete policy definition {}!".format(name)
+    ret["comment"] = f"Failed to delete policy definition {name}!"
     return ret
 
 
 def policy_assignment_present(
     name,
     scope,
     definition_name,
     display_name=None,
     description=None,
     assignment_type=None,
     parameters=None,
     connection_auth=None,
-    **kwargs
+    **kwargs,
 ):
     """
     .. versionadded:: 2019.2.0
 
     Ensure a security policy assignment exists.
 
     :param name:
@@ -678,19 +690,19 @@
             policy.get("parameters", {}), parameters or {}
         )
         if param_changes:
             ret["changes"]["parameters"] = param_changes
 
         if not ret["changes"]:
             ret["result"] = True
-            ret["comment"] = "Policy assignment {} is already present.".format(name)
+            ret["comment"] = f"Policy assignment {name} is already present."
             return ret
 
         if __opts__["test"]:
-            ret["comment"] = "Policy assignment {} would be updated.".format(name)
+            ret["comment"] = f"Policy assignment {name} would be updated."
             ret["result"] = None
             return ret
 
     else:
         ret["changes"] = {
             "old": {},
             "new": {
@@ -701,15 +713,15 @@
                 "display_name": display_name,
                 "description": description,
                 "parameters": parameters,
             },
         }
 
     if __opts__["test"]:
-        ret["comment"] = "Policy assignment {} would be created.".format(name)
+        ret["comment"] = f"Policy assignment {name} would be created."
         ret["result"] = None
         return ret
 
     if isinstance(parameters, dict):
         parameters = json.loads(json.dumps(parameters))
 
     policy_kwargs = kwargs.copy()
@@ -718,23 +730,27 @@
         name=name,
         scope=scope,
         definition_name=definition_name,
         type=assignment_type,
         display_name=display_name,
         description=description,
         parameters=parameters,
-        **policy_kwargs
+        **policy_kwargs,
     )
 
     if "error" not in policy:
         ret["result"] = True
-        ret["comment"] = "Policy assignment {} has been created.".format(name)
+        ret["comment"] = f"Policy assignment {name} has been created."
         return ret
 
-    ret["comment"] = "Failed to create policy assignment {}! ({})".format(name, policy.get("error"))
+    ret[
+        "comment"
+    ] = "Failed to create policy assignment {}! ({})".format(  # pylint: disable=consider-using-f-string
+        name, policy.get("error")
+    )
     return ret
 
 
 def policy_assignment_absent(name, scope, connection_auth=None):
     """
     .. versionadded:: 2019.2.0
 
@@ -758,29 +774,29 @@
 
     policy = __salt__["azurerm_resource.policy_assignment_get"](
         name, scope, azurerm_log_level="info", **connection_auth
     )
 
     if "error" in policy:
         ret["result"] = True
-        ret["comment"] = "Policy assignment {} is already absent.".format(name)
+        ret["comment"] = f"Policy assignment {name} is already absent."
         return ret
 
     elif __opts__["test"]:
-        ret["comment"] = "Policy assignment {} would be deleted.".format(name)
+        ret["comment"] = f"Policy assignment {name} would be deleted."
         ret["result"] = None
         ret["changes"] = {
             "old": policy,
             "new": {},
         }
         return ret
 
     deleted = __salt__["azurerm_resource.policy_assignment_delete"](name, scope, **connection_auth)
 
     if deleted:
         ret["result"] = True
-        ret["comment"] = "Policy assignment {} has been deleted.".format(name)
+        ret["comment"] = f"Policy assignment {name} has been deleted."
         ret["changes"] = {"old": policy, "new": {}}
         return ret
 
-    ret["comment"] = "Failed to delete policy assignment {}!".format(name)
+    ret["comment"] = f"Failed to delete policy assignment {name}!"
     return ret
```

### Comparing `saltext.azurerm-4.0.1/src/saltext/azurerm/utils/azurerm.py` & `saltext_azurerm-4.1.0/src/saltext/azurerm/utils/azurerm.py`

 * *Files 4% similar despite different names*

```diff
@@ -95,22 +95,27 @@
             )
     except (AttributeError, ImportError, MetadataEndpointError):
         raise SaltSystemExit(  # pylint: disable=raise-missing-from
             f"The Azure cloud environment {kwargs['cloud_environment']} is not available."
         )
 
     try:
-        credentials = DefaultAzureCredential(authority=authority, **kwargs)
+        if "client_id" in kwargs and "tenant" in kwargs and "secret" in kwargs:
+            credentials = get_identity_credentials(**kwargs)
+        else:
+            kwargs.pop("client_id", None)
+            credentials = DefaultAzureCredential(authority=authority, **kwargs)
     except ClientAuthenticationError:
         raise SaltInvocationError(  # pylint: disable=raise-missing-from
             "Unable to determine credentials. "
             "A subscription_id with username and password, "
             "or client_id, secret, and tenant or a profile with the "
             "required parameters populated"
         )
+
     try:
         subscription_id = salt.utils.stringutils.to_str(kwargs["subscription_id"])
     except KeyError:
         raise SaltInvocationError(  # pylint: disable=raise-missing-from
             "A subscription_id must be specified"
         )
 
@@ -170,15 +175,14 @@
     else:
         client = Client(
             credential=credentials,
             subscription_id=subscription_id,
             base_url=cloud_env.endpoints.resource_manager,
             user_agent_policy=user_agent,
         )
-
     return client
 
 
 def log_cloud_error(client, message, **kwargs):
     """
     Log an azurerm cloud error exception
     """
@@ -214,20 +218,20 @@
 def create_object_model(module_name, object_name, **kwargs):
     """
     Assemble an object from incoming parameters.
     """
     object_kwargs = {}
 
     try:
-        model_module = importlib.import_module("azure.mgmt.{}.models".format(module_name))
+        model_module = importlib.import_module(f"azure.mgmt.{module_name}.models")
         # pylint: disable=invalid-name
         Model = getattr(model_module, object_name)
     except ImportError:
         raise sys.exit(  # pylint: disable=raise-missing-from
-            "The {} model in the {} Azure module is not available.".format(object_name, module_name)
+            f"The {object_name} model in the {module_name} Azure module is not available."
         )
 
     if "_attribute_map" in dir(Model):
         for attr, items in Model._attribute_map.items():  # pylint: disable=protected-access
             param = kwargs.get(attr)
             if param is not None:
                 if items["type"][0].isupper() and isinstance(param, dict):
@@ -328,23 +332,28 @@
         "client_certificate_path": "AZURE_CLIENT_CERTIFICATE_PATH",
         "username": "AZURE_USERNAME",
         "password": "AZURE_PASSWORD",
     }
     for keyword, value in kwarg_map.items():
         if kwargs.get(keyword):
             os.environ[value] = kwargs[keyword]
-
     try:
         if kwargs.get("cloud_environment") and kwargs.get("cloud_environment").startswith("http"):
             authority = kwargs["cloud_environment"]
         else:
             authority = getattr(
                 KnownAuthorities, kwargs.get("cloud_environment", "AZURE_PUBLIC_CLOUD")
             )
         log.debug("AUTHORITY: %s", authority)
+
     except AttributeError as exc:
         log.error('Unknown authority presented for "cloud_environment": %s', exc)
         authority = KnownAuthorities.AZURE_PUBLIC_CLOUD
 
-    credential = DefaultAzureCredential(authority=authority)
+    try:
+        credential = DefaultAzureCredential(authority=authority)
+    except ClientAuthenticationError:
+        raise SaltInvocationError(  # pylint: disable=raise-missing-from
+            "Unable to determine credentials. "
+        )
 
     return credential
```

### Comparing `saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/SOURCES.txt` & `saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -1,70 +1,76 @@
+.copier-answers.yml
 .coveragerc
 .gitignore
 .pre-commit-config.yaml
 .pylintrc
 .readthedocs.yaml
 CHANGELOG.md
 CODE-OF-CONDUCT.md
 CONTRIBUTING.md
 LICENSE
 NOTICE.txt
 README.md
 noxfile.py
 pyproject.toml
-setup.cfg
 setup.py
 .github/ISSUE_TEMPLATE.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/config.yml
 .github/ISSUE_TEMPLATE/docs.md
 .github/ISSUE_TEMPLATE/feature_request.md
-.github/workflows/test.yml
+.github/ISSUE_TEMPLATE/tech-debt.md
+.github/workflows/pr.yml
+.github/workflows/tag.yml
 .pre-commit-hooks/check-cli-examples.py
 .pre-commit-hooks/make-autodocs.py
-changelog/.gitignore
+changelog/.template.jinja
 docs/Makefile
-docs/all.rst
+docs/changelog.md
 docs/conf.py
 docs/index.rst
 docs/make.bat
 docs/sitevars.rst
 docs/_static/.gitkeep
 docs/ref/.gitkeep
-docs/ref/clouds/all.rst
+docs/ref/clouds/index.rst
 docs/ref/clouds/saltext.azurerm.clouds.azurerm.rst
-docs/ref/modules/all.rst
+docs/ref/fileserver/index.rst
+docs/ref/fileserver/saltext.azurerm.fileserver.azurefs.rst
+docs/ref/modules/index.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_compute.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_compute_availability_set.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_compute_disk.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_compute_image.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_extension.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_compute_virtual_machine_image.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_dns.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_key.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_secret.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_keyvault_vault.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_network.rst
 docs/ref/modules/saltext.azurerm.modules.azurerm_resource.rst
-docs/ref/states/all.rst
+docs/ref/states/index.rst
 docs/ref/states/saltext.azurerm.states.azurerm_compute.rst
 docs/ref/states/saltext.azurerm.states.azurerm_compute_availability_set.rst
 docs/ref/states/saltext.azurerm.states.azurerm_compute_virtual_machine.rst
 docs/ref/states/saltext.azurerm.states.azurerm_dns.rst
 docs/ref/states/saltext.azurerm.states.azurerm_keyvault_key.rst
 docs/ref/states/saltext.azurerm.states.azurerm_keyvault_secret.rst
 docs/ref/states/saltext.azurerm.states.azurerm_keyvault_vault.rst
 docs/ref/states/saltext.azurerm.states.azurerm_network.rst
 docs/ref/states/saltext.azurerm.states.azurerm_resource.rst
-docs/ref/utils/all.rst
+docs/ref/utils/index.rst
 docs/ref/utils/saltext.azurerm.utils.azurerm.rst
+docs/ref/utils/saltext.azurerm.utils.rst
 docs/topics/authentication.rst
 docs/topics/index.rst
+docs/topics/installation.md
 src/saltext.azurerm.egg-info/PKG-INFO
 src/saltext.azurerm.egg-info/SOURCES.txt
 src/saltext.azurerm.egg-info/dependency_links.txt
 src/saltext.azurerm.egg-info/entry_points.txt
 src/saltext.azurerm.egg-info/not-zip-safe
 src/saltext.azurerm.egg-info/requires.txt
 src/saltext.azurerm.egg-info/top_level.txt
@@ -98,14 +104,16 @@
 src/saltext/azurerm/states/azurerm_keyvault_vault.py
 src/saltext/azurerm/states/azurerm_network.py
 src/saltext/azurerm/states/azurerm_resource.py
 src/saltext/azurerm/utils/__init__.py
 src/saltext/azurerm/utils/azurerm.py
 tests/__init__.py
 tests/conftest.py
+tests/functional/__init__.py
+tests/functional/conftest.py
 tests/integration/__init__.py
 tests/integration/conftest.py
 tests/integration/clouds/__init__.py
 tests/integration/modules/__init__.py
 tests/integration/states/__init__.py
 tests/integration/states/test_compute_availability_set.py
 tests/integration/states/test_compute_virtual_machine.py
@@ -117,12 +125,13 @@
 tests/integration/states/test_network_route.py
 tests/integration/states/test_network_security_group.py
 tests/integration/states/test_public_ip_address.py
 tests/integration/states/test_resource_group.py
 tests/integration/states/test_virtual_network.py
 tests/integration/utils/__init__.py
 tests/unit/__init__.py
+tests/unit/conftest.py
 tests/unit/clouds/__init__.py
 tests/unit/modules/__init__.py
 tests/unit/states/__init__.py
 tests/unit/utils/__init__.py
 tests/unit/utils/test_azurerm.py
```

### Comparing `saltext.azurerm-4.0.1/src/saltext.azurerm.egg-info/requires.txt` & `saltext_azurerm-4.1.0/src/saltext.azurerm.egg-info/requires.txt`

 * *Files 18% similar despite different names*

```diff
@@ -20,36 +20,40 @@
 azure-storage-blob==12.12.0
 azure-storage-common==2.1.0
 azure-storage-file==2.1.0
 azure-storage-nspkg==3.1.0
 azure-storage-queue==12.3.0
 msrest==0.7.1
 msrestazure==0.6.4
+salt>=3005
+
+[changelog]
+towncrier==22.12.0
 
 [dev]
-nox==2022.1.7
-pre-commit==2.13.0
-pylint<2.14.0
-SaltPyLint
+nox
+pre-commit>=2.4.0
+pylint
+saltpylint
 
 [docs]
-sphinx>=3.5.1
-Jinja2
-furo
-sphinx-copybutton
+sphinx
 sphinx-prompt
 sphinxcontrib-spelling
-importlib_metadata<=4.13.0
+sphinx-copybutton
+towncrier==22.12.0
+sphinxcontrib-towncrier
+myst_parser
+furo
+sphinx-inline-tabs
 
 [docsauto]
 sphinx-autobuild
 
-[release]
-twine
-wheel
+[lint]
+pylint
+saltpylint
 
 [tests]
-mock>=3.0.5
-pytest>=7.2.0
-pytest-salt-factories>=1.0.0rc23
-pytest-ordering
-Jinja2
+pytest>=6.1.0
+pytest-ordering>=0.6
+pytest-salt-factories>=1.0.0rc19
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/conftest.py` & `saltext_azurerm-4.1.0/tests/integration/conftest.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,20 @@
 def minion(minion):
     with minion.started():
         yield minion
 
 
 @pytest.fixture
 def salt_run_cli(master):
-    return master.get_salt_run_cli()
+    return master.salt_run_cli()
 
 
 @pytest.fixture
 def salt_cli(master):
-    return master.get_salt_cli()
+    return master.salt_cli()
 
 
 @pytest.fixture
 def salt_call_cli(minion):
     return minion.salt_call_cli()
 
 
@@ -45,17 +45,15 @@
         "Organization": "Everest",
         "Owner": "Elmer Fudd Gantry",
     }
 
 
 @pytest.fixture(scope="session")
 def resource_group():
-    yield "rg-salt-inttest-" + "".join(
-        random.choice(string.ascii_lowercase + string.digits) for _ in range(20)
-    )
+    yield "github"
 
 
 @pytest.fixture(scope="session")
 def virt_mach():
     yield "vm-salt-" + "".join(
         random.choice(string.ascii_lowercase + string.digits) for _ in range(5)
     )
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_compute_availability_set.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_compute_availability_set.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.mark.run(order=4)
 def test_present(salt_call_cli, availability_set, resource_group, connection_auth):
     expected = {
         "__id__": availability_set,
         "__run_num__": 0,
         "__sls__": None,
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_compute_virtual_machine.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_compute_virtual_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import random
 import string
 
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.fixture(scope="session")
 def password():
     yield "#PASS" + "".join(
         random.choice(string.ascii_lowercase + string.digits) for _ in range(16)
     ) + "!"
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_dns.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_dns.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.mark.run(order=3)
 def test_zone_present(salt_call_cli, zone, resource_group, connection_auth):
     expected = {
         "__id__": zone,
         "__run_num__": 0,
         "__sls__": None,
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_keyvault_key.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_keyvault_key.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import random
 import string
 
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.fixture(scope="session")
 def key():
     yield "key-salt-" + "".join(
         random.choice(string.ascii_lowercase + string.digits) for _ in range(8)
     )
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_keyvault_secret.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_keyvault_secret.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import random
 import string
 
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.fixture(scope="session")
 def secret():
     yield "secret-salt-" + "".join(
         random.choice(string.ascii_lowercase + string.digits) for _ in range(8)
     )
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_keyvault_vault.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_keyvault_vault.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import time
 
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.mark.run(order=3)
 def test_present(
     salt_call_cli,
     resource_group,
     location,
     keyvault,
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_network_interface.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_network_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.mark.run(order=4)
 def test_present(
     salt_call_cli, network_interface, subnet, vnet, resource_group, ip_config, connection_auth
 ):
     expected = {
         "__id__": network_interface,
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_network_route.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_network_route.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.mark.run(order=3)
 def test_table_present(salt_call_cli, route_table, resource_group, connection_auth):
     expected = {
         "__id__": route_table,
         "__run_num__": 0,
         "__sls__": None,
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_network_security_group.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_network_security_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,16 @@
 import random
 import string
 
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.fixture(scope="session")
 def nsg():
     yield "nsg-salt-" + "".join(
         random.choice(string.ascii_lowercase + string.digits) for _ in range(8)
     )
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_public_ip_address.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_public_ip_address.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.mark.run(order=3)
 # Creates a public IP address with a "Standard" SKU for Bastion Host tests and another one with a "Basic" SKU
 # for the virtual network gateway tests
 def test_present(salt_call_cli, public_ip_addr, public_ip_addr2, resource_group, connection_auth):
     idle_timeout = 10
     standard_expected = {
@@ -141,7 +145,34 @@
         resource_group=resource_group,
         connection_auth=connection_auth,
     )
     data = list(ret.data.values())[0]
     assert data["changes"]["new"] == expected["changes"]["new"]
     assert data["changes"]["old"]["name"] == expected["changes"]["old"]["name"]
     assert data["result"] == expected["result"]
+
+
+@pytest.mark.run(order=-3)
+def test_absent_second_ip(salt_call_cli, public_ip_addr2, resource_group, connection_auth):
+    expected = {
+        "changes": {
+            "new": {},
+            "old": {
+                "name": public_ip_addr2,
+            },
+        },
+        "comment": f"Public IP address {public_ip_addr2} has been deleted.",
+        "name": public_ip_addr2,
+        "result": True,
+    }
+    ret = salt_call_cli.run(
+        "--local",
+        "state.single",
+        "azurerm_network.public_ip_address_absent",
+        name=public_ip_addr2,
+        resource_group=resource_group,
+        connection_auth=connection_auth,
+    )
+    data = list(ret.data.values())[0]
+    assert data["changes"]["new"] == expected["changes"]["new"]
+    assert data["changes"]["old"]["name"] == expected["changes"]["old"]["name"]
+    assert data["result"] == expected["result"]
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_resource_group.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_resource_group.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,62 @@
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
 
-@pytest.mark.run(order=1)
-def test_present(salt_call_cli, resource_group, location, connection_auth):
+
+@pytest.mark.run(order=1, before="test_changes_remove_tag")
+def test_changes_add_tag(salt_call_cli, resource_group, location, tags, connection_auth):
     expected = {
         "__id__": resource_group,
         "__run_num__": 0,
         "__sls__": None,
         "changes": {
             "new": {
                 "location": location,
                 "name": resource_group,
-                "type": "Microsoft.Resources/resourceGroups",
                 "properties": {"provisioning_state": "Succeeded"},
+                "tags": tags,
+                "type": "Microsoft.Resources/resourceGroups",
             },
             "old": {},
         },
         "comment": f"Resource group {resource_group} has been created.",
         "name": resource_group,
         "result": True,
     }
-    # ret = resource.resource_group_present(resource_group, location, connection_auth=connection_auth)
+
     ret = salt_call_cli.run(
         "--local",
         "state.single",
         "azurerm_resource.resource_group_present",
         name=resource_group,
         location=location,
         connection_auth=connection_auth,
+        tags=tags,
     )
     data = list(ret.data.values())[0]
     data["changes"]["new"].pop("id")
     data.pop("duration")
     data.pop("start_time")
     assert data == expected
 
 
-@pytest.mark.run(order=1, after="test_present", before="test_absent")
-def test_changes(salt_call_cli, resource_group, location, tags, connection_auth):
+@pytest.mark.run(order=1, after="test_changes_add_tag")
+def test_changes_remove_tag(salt_call_cli, resource_group, location, connection_auth):
     expected = {
         "__id__": resource_group,
         "__run_num__": 0,
         "__sls__": None,
         "changes": {
             "new": {
                 "location": location,
                 "name": resource_group,
                 "properties": {"provisioning_state": "Succeeded"},
-                "tags": tags,
                 "type": "Microsoft.Resources/resourceGroups",
             },
             "old": {},
         },
         "comment": f"Resource group {resource_group} has been created.",
         "name": resource_group,
         "result": True,
@@ -60,48 +65,14 @@
     ret = salt_call_cli.run(
         "--local",
         "state.single",
         "azurerm_resource.resource_group_present",
         name=resource_group,
         location=location,
         connection_auth=connection_auth,
-        tags=tags,
+        tags=None,  # Set tags to None
     )
     data = list(ret.data.values())[0]
     data["changes"]["new"].pop("id")
     data.pop("duration")
     data.pop("start_time")
     assert data == expected
-
-
-@pytest.mark.run(order=-1)
-def test_absent(salt_call_cli, resource_group, location, tags, connection_auth):
-    expected = {
-        "__id__": resource_group,
-        "__run_num__": 0,
-        "__sls__": None,
-        "changes": {
-            "new": {},
-            "old": {
-                "location": location,
-                "name": resource_group,
-                "properties": {"provisioning_state": "Succeeded"},
-                "tags": tags,
-                "type": "Microsoft.Resources/resourceGroups",
-            },
-        },
-        "comment": f"Resource group {resource_group} has been deleted.",
-        "name": resource_group,
-        "result": True,
-    }
-    ret = salt_call_cli.run(
-        "--local",
-        "state.single",
-        "azurerm_resource.resource_group_absent",
-        name=resource_group,
-        connection_auth=connection_auth,
-    )
-    data = list(ret.data.values())[0]
-    data.pop("duration")
-    data.pop("start_time")
-    expected["changes"]["old"]["id"] = data["changes"]["old"]["id"]
-    assert data == expected
```

### Comparing `saltext.azurerm-4.0.1/tests/integration/states/test_virtual_network.py` & `saltext_azurerm-4.1.0/tests/integration/states/test_virtual_network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 import pytest
 
+pytestmark = [
+    pytest.mark.destructive_test,
+]
+
 
 @pytest.mark.run(order=3)
 def test_present(salt_call_cli, vnet, resource_group, location, connection_auth):
     vnet_addr_prefixes = ["10.0.0.0/16"]
     expected = {
         "__id__": vnet,
         "__run_num__": 0,
```

### Comparing `saltext.azurerm-4.0.1/tests/unit/utils/test_azurerm.py` & `saltext_azurerm-4.1.0/tests/unit/utils/test_azurerm.py`

 * *Files identical despite different names*

