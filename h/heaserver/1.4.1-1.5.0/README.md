# Comparing `tmp/heaserver-1.4.1.tar.gz` & `tmp/heaserver-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "heaserver-1.4.1.tar", last modified: Thu Apr 18 02:11:33 2024, max compression
+gzip compressed data, was "heaserver-1.5.0.tar", last modified: Wed Apr 24 17:42:46 2024, max compression
```

## Comparing `heaserver-1.4.1.tar` & `heaserver-1.5.0.tar`

### file list

```diff
@@ -1,298 +1,298 @@
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.365593 heaserver-1.4.1/
--rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.4.1/.editorconfig
--rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.4.1/.gitignore
--rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.4.1/LICENSE
--rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.4.1/MANIFEST.in
--rw-rw-rw-   0        0        0     7124 2024-04-18 02:11:33.364593 heaserver-1.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5129 2024-04-18 02:10:17.000000 heaserver-1.4.1/README.md
--rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.4.1/RELEASING.md
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.907437 heaserver-1.4.1/awss3integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.907437 heaserver-1.4.1/awss3integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.941143 heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/__init__.py
--rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
--rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/service.py
--rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.943141 heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/wstl/
--rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/wstl/all.json
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.909434 heaserver-1.4.1/awss3tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.909434 heaserver-1.4.1/awss3tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.945141 heaserver-1.4.1/awss3tests/heaserver/awss3tests/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.4.1/awss3tests/heaserver/awss3tests/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.955146 heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.4.1/awss3tests/heaserver/awss3tests/test_all.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.911435 heaserver-1.4.1/integrationtests/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.911435 heaserver-1.4.1/integrationtests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.982141 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.021146 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
--rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
--rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
--rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
--rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
--rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0     5992 2024-04-09 21:13:46.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
--rw-rw-rw-   0        0        0     5553 2024-04-05 18:40:52.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5322 2024-04-09 21:13:46.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
--rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/service.py
--rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
--rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
--rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
--rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     4749 2024-04-09 21:13:46.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
--rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
--rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
--rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.023142 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/wstl/
--rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
--rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.4.1/pytest.ini
--rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.4.1/requirements_dev.txt
--rw-rw-rw-   0        0        0       42 2024-04-18 02:11:33.365593 heaserver-1.4.1/setup.cfg
--rw-rw-rw-   0        0        0     2870 2024-04-18 02:10:47.000000 heaserver-1.4.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.914435 heaserver-1.4.1/src/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.914435 heaserver-1.4.1/src/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.076203 heaserver-1.4.1/src/heaserver/service/
--rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/__init__.py
--rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.4.1/src/heaserver/service/activity.py
--rw-rw-rw-   0        0        0    14193 2024-02-07 00:24:57.000000 heaserver-1.4.1/src/heaserver/service/aiohttp.py
--rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/appfactory.py
--rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/appproperty.py
--rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/backgroundtasks.py
--rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/caching.py
--rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/caching_strategy.py
--rw-rw-rw-   0        0        0    23214 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/client.py
--rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/config.py
--rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/customhdrs.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.088206 heaserver-1.4.1/src/heaserver/service/db/
--rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.4.1/src/heaserver/service/db/__init__.py
--rw-rw-rw-   0        0        0    26582 2024-04-17 04:08:55.000000 heaserver-1.4.1/src/heaserver/service/db/aws.py
--rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.4.1/src/heaserver/service/db/awsservicelib.py
--rw-rw-rw-   0        0        0    31583 2024-04-16 21:19:24.000000 heaserver-1.4.1/src/heaserver/service/db/database.py
--rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.4.1/src/heaserver/service/db/dbapi2.py
--rw-rw-rw-   0        0        0    31960 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/db/mongo.py
--rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.4.1/src/heaserver/service/db/mongoexpr.py
--rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.4.1/src/heaserver/service/db/mongoservicelib.py
--rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/defaults.py
--rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/error.py
--rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/expression.py
--rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/functional.py
--rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.4.1/src/heaserver/service/heaobjectsupport.py
--rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/jsonschema.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.097203 heaserver-1.4.1/src/heaserver/service/jsonschemafiles/
--rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/jsonschemafiles/__init__.py
--rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/jsonschemafiles/cjtemplate.json
--rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/jsonschemafiles/nvpjson.json
--rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/jsonschemafiles/wstl.json
--rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/jsonschemafiles/wstlaction.json
--rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/jsonschemavalidator.py
--rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/messagebroker.py
--rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/mimetypes.py
--rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.4.1/src/heaserver/service/oidcclaimhdrs.py
--rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/openapi.py
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.4.1/src/heaserver/service/py.typed
--rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/registryproperty.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.108203 heaserver-1.4.1/src/heaserver/service/representor/
--rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/representor/__init__.py
--rw-rw-rw-   0        0        0    25695 2024-04-01 23:40:09.000000 heaserver-1.4.1/src/heaserver/service/representor/cj.py
--rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/representor/error.py
--rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/representor/factory.py
--rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/representor/nvpjson.py
--rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/representor/representor.py
--rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/representor/wstljson.py
--rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.4.1/src/heaserver/service/representor/xwwwformurlencoded.py
--rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.4.1/src/heaserver/service/requestproperty.py
--rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.4.1/src/heaserver/service/response.py
--rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/runner.py
--rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.4.1/src/heaserver/service/sources.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.131203 heaserver-1.4.1/src/heaserver/service/testcase/
--rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/__init__.py
--rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/aiohttptestcase.py
--rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/awsdockermongo.py
--rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/awss3microservicetestcase.py
--rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/collection.py
--rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/docker.py
--rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/dockermongo.py
--rw-rw-rw-   0        0        0    40278 2024-04-01 23:40:09.000000 heaserver-1.4.1/src/heaserver/service/testcase/expectedvalues.py
--rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.4.1/src/heaserver/service/testcase/microservicetestcase.py
--rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.4.1/src/heaserver/service/testcase/mixin.py
--rw-rw-rw-   0        0        0    18431 2024-04-05 18:40:52.000000 heaserver-1.4.1/src/heaserver/service/testcase/mockaws.py
--rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/mockdatabase.py
--rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/mockmongo.py
--rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/simpleaiohttptestcase.py
--rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/swaggerui.py
--rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/testenv.py
--rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/testcase/util.py
--rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.4.1/src/heaserver/service/uritemplate.py
--rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.4.1/src/heaserver/service/util.py
--rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.4.1/src/heaserver/service/wstl.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.362594 heaserver-1.4.1/src/heaserver.egg-info/
--rw-rw-rw-   0        0        0     7124 2024-04-18 02:11:32.000000 heaserver-1.4.1/src/heaserver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    17591 2024-04-18 02:11:32.000000 heaserver-1.4.1/src/heaserver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-18 02:11:32.000000 heaserver-1.4.1/src/heaserver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      455 2024-04-18 02:11:32.000000 heaserver-1.4.1/src/heaserver.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-18 02:11:32.000000 heaserver-1.4.1/src/heaserver.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.917435 heaserver-1.4.1/tests/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:32.917435 heaserver-1.4.1/tests/heaserver/
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.196824 heaserver-1.4.1/tests/heaserver/servicetest/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.245689 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.247254 heaserver-1.4.1/tests/heaserver/servicetest/aiohttpdata/
--rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
--rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/componentpermissionstestcase.py
--rw-rw-rw-   0        0        0    17429 2024-04-09 21:13:46.000000 heaserver-1.4.1/tests/heaserver/servicetest/componenttestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.251939 heaserver-1.4.1/tests/heaserver/servicetest/db/
--rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.266544 heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/test_mongo.py
--rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/db/test_mongoexpr.py
--rw-rw-rw-   0        0        0     5351 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/organizationpermissionstestcase.py
--rw-rw-rw-   0        0        0     5775 2024-04-09 21:13:46.000000 heaserver-1.4.1/tests/heaserver/servicetest/organizationtestcase.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.291539 heaserver-1.4.1/tests/heaserver/servicetest/representor/
--rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.359594 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
--rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
--rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
--rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
--rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
--rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
--rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
--rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
--rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/all.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_item_href.json
--rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_item_link.json
--rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_queries.json
--rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_template.json
--rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
--rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
--rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/test_cj.py
--rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/test_factory.py
--rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/test_nvpjson.py
--rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/test_supports_links.py
--rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/test_wstljson.py
--rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.4.1/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
--rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/service.py
--rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_activity.py
--rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_aiohttp.py
--rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_backgroundtasks.py
--rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_caching.py
--rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_client.py
--rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_component_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_configuration.py
--rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_database_classes.py
--rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_delete_component.py
--rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_expression.py
--rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_functional.py
--rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_get_all_components.py
--rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_get_component.py
--rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_get_organization_permissions.py
--rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_heaobjectsupport.py
--rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_jsonschemavalidator.py
--rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_mimetypes.py
--rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_not_imported.py
--rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
--rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_post_component.py
--rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_put_component.py
--rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_put_organization_permissions.py
--rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_response.py
--rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_testenv.py
--rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_uritemplate.py
--rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_util.py
--rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/test_wstl.py
-drwxrwxrwx   0        0        0        0 2024-04-18 02:11:33.361595 heaserver-1.4.1/tests/heaserver/servicetest/wstl/
--rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl/all.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_1.json
--rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_10a.json
--rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_10b.json
--rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_11.json
--rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_2.json
--rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_3.json
--rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_4.json
--rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_5.json
--rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_6.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_7.json
--rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_8.json
--rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.4.1/tests/heaserver/servicetest/wstl_9.json
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.595402 heaserver-1.5.0/
+-rw-rw-rw-   0        0        0      261 2022-03-11 01:28:19.000000 heaserver-1.5.0/.editorconfig
+-rw-rw-rw-   0        0        0      303 2023-12-16 23:04:09.000000 heaserver-1.5.0/.gitignore
+-rw-rw-rw-   0        0        0    11625 2022-03-11 01:28:19.000000 heaserver-1.5.0/LICENSE
+-rw-rw-rw-   0        0        0      243 2023-12-16 23:04:09.000000 heaserver-1.5.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     7410 2024-04-24 17:42:46.593402 heaserver-1.5.0/PKG-INFO
+-rw-rw-rw-   0        0        0     5415 2024-04-24 17:41:47.000000 heaserver-1.5.0/README.md
+-rw-rw-rw-   0        0        0     1612 2023-12-16 23:04:09.000000 heaserver-1.5.0/RELEASING.md
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.099751 heaserver-1.5.0/awss3integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.100753 heaserver-1.5.0/awss3integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.130874 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/__init__.py
+-rw-rw-rw-   0        0        0    34976 2024-04-01 23:40:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py
+-rw-rw-rw-   0        0        0     1416 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/service.py
+-rw-rw-rw-   0        0        0    19401 2024-04-08 18:06:35.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.132874 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/wstl/
+-rw-rw-rw-   0        0        0    16955 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.101753 heaserver-1.5.0/awss3tests/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.102753 heaserver-1.5.0/awss3tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.134874 heaserver-1.5.0/awss3tests/heaserver/awss3tests/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.143993 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5872 2024-03-19 23:09:56.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     3169 2023-12-16 23:04:09.000000 heaserver-1.5.0/awss3tests/heaserver/awss3tests/test_all.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.103752 heaserver-1.5.0/integrationtests/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.104751 heaserver-1.5.0/integrationtests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.171990 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.204244 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1722 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0      612 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     1465 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      630 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0     3839 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     6100 2024-04-16 21:05:42.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1290 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160
+-rw-rw-rw-   0        0        0     1236 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     1723 2024-03-19 23:29:00.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520
+-rw-rw-rw-   0        0        0     1043 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624
+-rw-rw-rw-   0        0        0      627 2023-12-20 00:04:02.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056
+-rw-rw-rw-   0        0        0     5996 2023-12-16 23:04:09.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py
+-rw-rw-rw-   0        0        0     6620 2023-12-16 23:04:09.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5992 2024-04-09 21:13:46.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py
+-rw-rw-rw-   0        0        0     5775 2024-04-22 16:37:36.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5544 2024-04-22 17:09:51.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py
+-rw-rw-rw-   0        0        0    12856 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/service.py
+-rw-rw-rw-   0        0        0     1024 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      198 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_delete_component.py
+-rw-rw-rw-   0        0        0      194 2022-03-11 01:28:19.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_all_components.py
+-rw-rw-rw-   0        0        0      888 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py
+-rw-rw-rw-   0        0        0      207 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     4749 2024-04-09 21:13:46.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py
+-rw-rw-rw-   0        0        0     1011 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0      521 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py
+-rw-rw-rw-   0        0        0      404 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_put_component.py
+-rw-rw-rw-   0        0        0      203 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_put_organization_permissions.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.206799 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/wstl/
+-rw-rw-rw-   0        0        0    16440 2023-12-16 23:04:10.000000 heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json
+-rw-rw-rw-   0        0        0      132 2023-12-16 23:04:10.000000 heaserver-1.5.0/pytest.ini
+-rw-rw-rw-   0        0        0      237 2023-12-16 23:04:10.000000 heaserver-1.5.0/requirements_dev.txt
+-rw-rw-rw-   0        0        0       42 2024-04-24 17:42:46.595402 heaserver-1.5.0/setup.cfg
+-rw-rw-rw-   0        0        0     2870 2024-04-24 17:42:09.000000 heaserver-1.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.106753 heaserver-1.5.0/src/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.106753 heaserver-1.5.0/src/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.290086 heaserver-1.5.0/src/heaserver/service/
+-rw-rw-rw-   0        0        0     1176 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/__init__.py
+-rw-rw-rw-   0        0        0     7213 2024-01-04 00:01:31.000000 heaserver-1.5.0/src/heaserver/service/activity.py
+-rw-rw-rw-   0        0        0    14193 2024-02-07 00:24:57.000000 heaserver-1.5.0/src/heaserver/service/aiohttp.py
+-rw-rw-rw-   0        0        0     1688 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/appfactory.py
+-rw-rw-rw-   0        0        0      758 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/appproperty.py
+-rw-rw-rw-   0        0        0     8521 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/backgroundtasks.py
+-rw-rw-rw-   0        0        0     1497 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/caching.py
+-rw-rw-rw-   0        0        0       64 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/caching_strategy.py
+-rw-rw-rw-   0        0        0    23443 2024-04-22 20:13:28.000000 heaserver-1.5.0/src/heaserver/service/client.py
+-rw-rw-rw-   0        0        0     2460 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/config.py
+-rw-rw-rw-   0        0        0      256 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/customhdrs.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.312079 heaserver-1.5.0/src/heaserver/service/db/
+-rw-rw-rw-   0        0        0      392 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/db/__init__.py
+-rw-rw-rw-   0        0        0    27286 2024-04-22 15:45:21.000000 heaserver-1.5.0/src/heaserver/service/db/aws.py
+-rw-rw-rw-   0        0        0    58921 2024-03-27 00:01:36.000000 heaserver-1.5.0/src/heaserver/service/db/awsservicelib.py
+-rw-rw-rw-   0        0        0    31583 2024-04-18 02:12:50.000000 heaserver-1.5.0/src/heaserver/service/db/database.py
+-rw-rw-rw-   0        0        0     6599 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/db/dbapi2.py
+-rw-rw-rw-   0        0        0    31960 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/db/mongo.py
+-rw-rw-rw-   0        0        0     4515 2024-04-05 18:40:52.000000 heaserver-1.5.0/src/heaserver/service/db/mongoexpr.py
+-rw-rw-rw-   0        0        0    26453 2024-04-03 23:37:27.000000 heaserver-1.5.0/src/heaserver/service/db/mongoservicelib.py
+-rw-rw-rw-   0        0        0      252 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/defaults.py
+-rw-rw-rw-   0        0        0      150 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/error.py
+-rw-rw-rw-   0        0        0     4709 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/expression.py
+-rw-rw-rw-   0        0        0      773 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/functional.py
+-rw-rw-rw-   0        0        0    19840 2024-03-21 03:54:08.000000 heaserver-1.5.0/src/heaserver/service/heaobjectsupport.py
+-rw-rw-rw-   0        0        0      683 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschema.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.321078 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/
+-rw-rw-rw-   0        0        0      606 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/__init__.py
+-rw-rw-rw-   0        0        0      787 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/cjtemplate.json
+-rw-rw-rw-   0        0        0       87 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/nvpjson.json
+-rw-rw-rw-   0        0        0     2214 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstl.json
+-rw-rw-rw-   0        0        0     4970 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstlaction.json
+-rw-rw-rw-   0        0        0      987 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/jsonschemavalidator.py
+-rw-rw-rw-   0        0        0    21655 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/messagebroker.py
+-rw-rw-rw-   0        0        0      539 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/mimetypes.py
+-rw-rw-rw-   0        0        0      639 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/oidcclaimhdrs.py
+-rw-rw-rw-   0        0        0     1558 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/openapi.py
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/py.typed
+-rw-rw-rw-   0        0        0      103 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/registryproperty.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.340081 heaserver-1.5.0/src/heaserver/service/representor/
+-rw-rw-rw-   0        0        0     1426 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/__init__.py
+-rw-rw-rw-   0        0        0    26065 2024-04-22 23:13:47.000000 heaserver-1.5.0/src/heaserver/service/representor/cj.py
+-rw-rw-rw-   0        0        0      170 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/error.py
+-rw-rw-rw-   0        0        0     7259 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/factory.py
+-rw-rw-rw-   0        0        0     2231 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/nvpjson.py
+-rw-rw-rw-   0        0        0     3244 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/representor.py
+-rw-rw-rw-   0        0        0     1551 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/representor/wstljson.py
+-rw-rw-rw-   0        0        0     1742 2024-03-19 23:15:41.000000 heaserver-1.5.0/src/heaserver/service/representor/xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0      114 2022-03-11 01:28:19.000000 heaserver-1.5.0/src/heaserver/service/requestproperty.py
+-rw-rw-rw-   0        0        0    29114 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/response.py
+-rw-rw-rw-   0        0        0    15617 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/runner.py
+-rw-rw-rw-   0        0        0       32 2024-03-26 22:51:02.000000 heaserver-1.5.0/src/heaserver/service/sources.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.371271 heaserver-1.5.0/src/heaserver/service/testcase/
+-rw-rw-rw-   0        0        0      167 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/__init__.py
+-rw-rw-rw-   0        0        0     2123 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/aiohttptestcase.py
+-rw-rw-rw-   0        0        0     1508 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/awsdockermongo.py
+-rw-rw-rw-   0        0        0     3944 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/awss3microservicetestcase.py
+-rw-rw-rw-   0        0        0    15471 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/collection.py
+-rw-rw-rw-   0        0        0     6655 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/docker.py
+-rw-rw-rw-   0        0        0     8062 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/dockermongo.py
+-rw-rw-rw-   0        0        0    40481 2024-04-22 17:03:29.000000 heaserver-1.5.0/src/heaserver/service/testcase/expectedvalues.py
+-rw-rw-rw-   0        0        0    17534 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/testcase/microservicetestcase.py
+-rw-rw-rw-   0        0        0   130477 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/testcase/mixin.py
+-rw-rw-rw-   0        0        0    18431 2024-04-05 18:40:52.000000 heaserver-1.5.0/src/heaserver/service/testcase/mockaws.py
+-rw-rw-rw-   0        0        0      662 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/mockdatabase.py
+-rw-rw-rw-   0        0        0    21242 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/mockmongo.py
+-rw-rw-rw-   0        0        0      555 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/simpleaiohttptestcase.py
+-rw-rw-rw-   0        0        0     7531 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/swaggerui.py
+-rw-rw-rw-   0        0        0    29140 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/testenv.py
+-rw-rw-rw-   0        0        0     2132 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/testcase/util.py
+-rw-rw-rw-   0        0        0     2877 2023-12-16 23:04:10.000000 heaserver-1.5.0/src/heaserver/service/uritemplate.py
+-rw-rw-rw-   0        0        0    11636 2024-01-04 00:01:31.000000 heaserver-1.5.0/src/heaserver/service/util.py
+-rw-rw-rw-   0        0        0    36804 2024-04-01 23:40:09.000000 heaserver-1.5.0/src/heaserver/service/wstl.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.592402 heaserver-1.5.0/src/heaserver.egg-info/
+-rw-rw-rw-   0        0        0     7410 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    17591 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      455 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-24 17:42:46.000000 heaserver-1.5.0/src/heaserver.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.109751 heaserver-1.5.0/tests/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.110752 heaserver-1.5.0/tests/heaserver/
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.448098 heaserver-1.5.0/tests/heaserver/servicetest/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.493402 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0    11044 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     5139 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0    13515 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     2266 2024-03-19 23:09:55.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1937 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     2605 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     2586 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0      826 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0    21674 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1870 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     3356 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0    18112 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0    12001 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.495403 heaserver-1.5.0/tests/heaserver/servicetest/aiohttpdata/
+-rw-rw-rw-   0        0        0      258 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/aiohttpdata/requirements_dev.txt
+-rw-rw-rw-   0        0        0     6442 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/componentpermissionstestcase.py
+-rw-rw-rw-   0        0        0    17429 2024-04-09 21:13:46.000000 heaserver-1.5.0/tests/heaserver/servicetest/componenttestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.498402 heaserver-1.5.0/tests/heaserver/servicetest/db/
+-rw-rw-rw-   0        0        0        0 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.506403 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0     1344 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7924 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0      551 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongo.py
+-rw-rw-rw-   0        0        0     7303 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongoexpr.py
+-rw-rw-rw-   0        0        0     5571 2024-04-22 17:04:47.000000 heaserver-1.5.0/tests/heaserver/servicetest/organizationpermissionstestcase.py
+-rw-rw-rw-   0        0        0     5997 2024-04-22 17:06:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/organizationtestcase.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.527403 heaserver-1.5.0/tests/heaserver/servicetest/representor/
+-rw-rw-rw-   0        0        0        0 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.589403 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0    54596 2024-03-29 23:13:01.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444
+-rw-rw-rw-   0        0        0    62667 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0    54545 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312
+-rw-rw-rw-   0        0        0     6469 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7286 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     1327 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852
+-rw-rw-rw-   0        0        0     6209 2024-03-29 23:04:43.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280
+-rw-rw-rw-   0        0        0     7761 2024-04-03 18:03:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360
+-rw-rw-rw-   0        0        0     6190 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128
+-rw-rw-rw-   0        0        0     5067 2024-03-19 23:09:56.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836
+-rw-rw-rw-   0        0        0     4471 2024-03-22 18:51:04.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904
+-rw-rw-rw-   0        0        0      192 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_item_href.json
+-rw-rw-rw-   0        0        0      268 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_item_link.json
+-rw-rw-rw-   0        0        0      642 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_queries.json
+-rw-rw-rw-   0        0        0     2670 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_template.json
+-rw-rw-rw-   0        0        0      267 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_item.json
+-rw-rw-rw-   0        0        0      263 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_toplevel_link_for_list.json
+-rw-rw-rw-   0        0        0    62769 2024-04-01 23:40:09.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_cj.py
+-rw-rw-rw-   0        0        0     2671 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_factory.py
+-rw-rw-rw-   0        0        0     4181 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_nvpjson.py
+-rw-rw-rw-   0        0        0      281 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_supports_links.py
+-rw-rw-rw-   0        0        0     5676 2024-04-01 23:40:09.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_wstljson.py
+-rw-rw-rw-   0        0        0     2396 2024-03-21 03:54:08.000000 heaserver-1.5.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py
+-rw-rw-rw-   0        0        0    13067 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/service.py
+-rw-rw-rw-   0        0        0     9455 2024-01-04 00:01:31.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_activity.py
+-rw-rw-rw-   0        0        0     3976 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_aiohttp.py
+-rw-rw-rw-   0        0        0     5894 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_backgroundtasks.py
+-rw-rw-rw-   0        0        0     2506 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_caching.py
+-rw-rw-rw-   0        0        0     7131 2024-04-09 21:13:46.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_client.py
+-rw-rw-rw-   0        0        0     1193 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1127 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_configuration.py
+-rw-rw-rw-   0        0        0      819 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_database_classes.py
+-rw-rw-rw-   0        0        0      204 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_delete_component.py
+-rw-rw-rw-   0        0        0     6181 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_expression.py
+-rw-rw-rw-   0        0        0      405 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_functional.py
+-rw-rw-rw-   0        0        0      422 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_get_all_components.py
+-rw-rw-rw-   0        0        0     3070 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_get_component.py
+-rw-rw-rw-   0        0        0      209 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_get_organization_permissions.py
+-rw-rw-rw-   0        0        0     5366 2024-04-09 21:13:46.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_heaobjectsupport.py
+-rw-rw-rw-   0        0        0     5746 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_jsonschemavalidator.py
+-rw-rw-rw-   0        0        0      909 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_mimetypes.py
+-rw-rw-rw-   0        0        0      331 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_not_imported.py
+-rw-rw-rw-   0        0        0     1005 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py
+-rw-rw-rw-   0        0        0     1274 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_post_component.py
+-rw-rw-rw-   0        0        0     1265 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_put_component.py
+-rw-rw-rw-   0        0        0      253 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_put_organization_permissions.py
+-rw-rw-rw-   0        0        0     2488 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_response.py
+-rw-rw-rw-   0        0        0      570 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_testenv.py
+-rw-rw-rw-   0        0        0     1929 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_uritemplate.py
+-rw-rw-rw-   0        0        0     8782 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_util.py
+-rw-rw-rw-   0        0        0     6255 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/test_wstl.py
+drwxrwxrwx   0        0        0        0 2024-04-24 17:42:46.591403 heaserver-1.5.0/tests/heaserver/servicetest/wstl/
+-rw-rw-rw-   0        0        0    16436 2023-12-16 23:04:10.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl/all.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_1.json
+-rw-rw-rw-   0        0        0     1214 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_10a.json
+-rw-rw-rw-   0        0        0     1240 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_10b.json
+-rw-rw-rw-   0        0        0     2355 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_11.json
+-rw-rw-rw-   0        0        0     1187 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_2.json
+-rw-rw-rw-   0        0        0     1190 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_3.json
+-rw-rw-rw-   0        0        0     1158 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_4.json
+-rw-rw-rw-   0        0        0      269 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_5.json
+-rw-rw-rw-   0        0        0      531 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_6.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_7.json
+-rw-rw-rw-   0        0        0     1185 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_8.json
+-rw-rw-rw-   0        0        0      204 2022-03-11 01:28:19.000000 heaserver-1.5.0/tests/heaserver/servicetest/wstl_9.json
```

### Comparing `heaserver-1.4.1/LICENSE` & `heaserver-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/PKG-INFO` & `heaserver-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.4.1
+Version: 1.5.0
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.4.0
+Requires-Dist: heaobject~=1.5.0
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,14 +47,22 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.0
+* Added attribute-level permissions.
+* Temporarily restored the role check that was removed in version 1.4.1 in case an AWS credentials object with overly
+permissive permissions is altered.
+
+## Version 1.4.2
+* Synchronize around getting temporary credentials.
+
 ## Version 1.4.1
 * Increased the boto3 max connection pool size from the default value (10) to 25.
 * Fixed a connection leak in DatabaseContextManager, and fixed the documentation for the connection() method.
 * Updated heaobject dependency.
 * Removed an unnecessary role check.
 
 ## Version 1.4.0
```

### Comparing `heaserver-1.4.1/README.md` & `heaserver-1.5.0/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,12 +1,20 @@
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.0
+* Added attribute-level permissions.
+* Temporarily restored the role check that was removed in version 1.4.1 in case an AWS credentials object with overly
+permissive permissions is altered.
+
+## Version 1.4.2
+* Synchronize around getting temporary credentials.
+
 ## Version 1.4.1
 * Increased the boto3 max connection pool size from the default value (10) to 25.
 * Fixed a connection leak in DatabaseContextManager, and fixed the documentation for the connection() method.
 * Updated heaobject dependency.
 * Removed an unnecessary role check.
 
 ## Version 1.4.0
```

### Comparing `heaserver-1.4.1/RELEASING.md` & `heaserver-1.5.0/RELEASING.md`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py` & `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/awss3foldertestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/service.py` & `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/test_all.py` & `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3integrationtests/heaserver/awss3tests/wstl/all.json` & `heaserver-1.5.0/awss3integrationtests/heaserver/awss3tests/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.0/awss3tests/heaserver/awss3tests/__pycache__/test_all.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/awss3tests/heaserver/awss3tests/test_all.py` & `heaserver-1.5.0/awss3tests/heaserver/awss3tests/test_all.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_component_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_delete_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_get_organization_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_mongoservicelib.cpython-311-pytest-7.4.4.pyc.40780`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_organization_with_bad_permissions.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.35160`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.24968`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.28520`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_component.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.15624`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/__pycache__/test_put_organization_permissions.cpython-310-pytest-7.4.0.pyc.41056`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/clienttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py` & `heaserver-1.5.0/tests/heaserver/servicetest/organizationpermissionstestcase.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 Creates a test case class for use with the unittest library that is built into Python.
 """
 from heaobject.root import Permission
 
 from . import service
-from heaserver.service.testcase.dockermongo import MockDockerMongoManager
 from heaserver.service.testcase.microservicetestcase import get_test_case_cls_default
 from heaobject.user import NONE_USER, TEST_USER, ALL_USERS
 from heaserver.service.testcase.expectedvalues import Action, Link
 from datetime import datetime
 
 db_store = {
     service.MONGODB_ORGANIZATION_COLLECTION: [
@@ -33,15 +32,17 @@
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'admin_ids': [],
-            'accounts': []
+            'admin_group_ids': [],
+            'manager_group_ids': [],
+            'member_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
@@ -68,30 +69,31 @@
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
             'admin_ids': [],
-            'accounts': []
+            'admin_group_ids': [],
+            'manager_group_ids': [],
+            'member_group_ids': []
         }
     ]}
 
 content = {
     service.MONGODB_ORGANIZATION_COLLECTION: {
         '666f6f2d6261722d71757578': b'The quick brown fox jumps over the lazy dog',
         '0123456789ab0123456789ab': b''
     }
 }
 
 OrganizationPermissionsTestCase = \
     get_test_case_cls_default(coll=service.MONGODB_ORGANIZATION_COLLECTION,
-                              db_manager_cls=MockDockerMongoManager,
                               wstl_package=service.__package__,
-                              href='http://localhost:8080/organizations/',
+                              href='http://localhost:8080/organizations',
                               fixtures=db_store,
                               content=content,
                               get_actions=[Action(
                                   name='heaserver-organizations-organization-get-properties',
                                   rel=['properties']),
                                   Action(
                                       name='heaserver-organizations-organization-get-open-choices',
```

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/organizationtestcase.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/organizationpermissionstestcase.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,107 +2,125 @@
 Creates a test case class for use with the unittest library that is built into Python.
 """
 from heaobject.root import Permission
 
 from . import service
 from heaserver.service.testcase.dockermongo import MockDockerMongoManager
 from heaserver.service.testcase.microservicetestcase import get_test_case_cls_default
-from heaserver.service.testcase.expectedvalues import Action, Link
 from heaobject.user import NONE_USER, TEST_USER, ALL_USERS
+from heaserver.service.testcase.expectedvalues import Action, Link
+from datetime import datetime
 
 db_store = {
     service.MONGODB_ORGANIZATION_COLLECTION: [
         {
             "id": "666f6f2d6261722d71757578",
             "source": None,
             "source_detail": None,
             "name": "Bob",
             "display_name": "Bob",
             "description": "Description of Bob",
             "owner": NONE_USER,
+            "created": datetime(2021, 12, 2, 17, 31, 15, 630000),
+            "modified": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "invites": [],
             "shares": [{
                 'type': 'heaobject.root.ShareImpl',
                 'invite': None,
                 'user': ALL_USERS,
                 'permissions': [Permission.CHECK_DYNAMIC.name]
             }],
             "derived_by": None,
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
-            "member_ids": [TEST_USER],
+            "member_ids": [],
             'type': 'heaobject.organization.Organization',
-            'mime_type': 'application/x.organization',
-            'created': None,
-            'modified': None,
             'admin_ids': [],
             'accounts': [],
-            'type_display_name': 'Organization'
+            'admin_group_ids': [],
+            'manager_group_ids': [],
+            'member_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
             "description": "Description of Reximus",
             "owner": NONE_USER,
+            "created": datetime(2021, 12, 2, 17, 31, 15, 630000),
+            "modified": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "invites": [],
-            "shares": [{
-                'type': 'heaobject.root.ShareImpl',
-                'invite': None,
-                'user': ALL_USERS,
-                'permissions': [Permission.CHECK_DYNAMIC.name]
-            }],
+            "shares": [
+                {
+                    'type': 'heaobject.root.ShareImpl',
+                    'invite': None,
+                    'user': ALL_USERS,
+                    'permissions': [Permission.CHECK_DYNAMIC.name]
+                },
+                {
+                    'type': 'heaobject.root.ShareImpl',
+                    'invite': None,
+                    'user': TEST_USER,
+                    'permissions': [Permission.VIEWER.name]
+                }
+            ],
             "derived_by": None,
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
-            "manager_ids": [TEST_USER],
+            "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
-            'mime_type': 'application/x.organization',
-            'created': None,
-            'modified': None,
             'admin_ids': [],
             'accounts': [],
-            'type_display_name': 'Organization'
+            'admin_group_ids': [],
+            'manager_group_ids': [],
+            'member_group_ids': []
         }
     ]}
 
 content = {
     service.MONGODB_ORGANIZATION_COLLECTION: {
-        '666f6f2d6261722d71757578': b'The quick brown fox jumps over the lazy dog'
+        '666f6f2d6261722d71757578': b'The quick brown fox jumps over the lazy dog',
+        '0123456789ab0123456789ab': b''
     }
 }
 
-OrganizationTestCase = \
+OrganizationPermissionsTestCase = \
     get_test_case_cls_default(coll=service.MONGODB_ORGANIZATION_COLLECTION,
                               db_manager_cls=MockDockerMongoManager,
                               wstl_package=service.__package__,
                               href='http://localhost:8080/organizations/',
                               fixtures=db_store,
                               content=content,
-                              get_actions=[Action(name='heaserver-organizations-organization-get-properties',
-                                                  rel=['properties']),
-                                           Action(name='heaserver-organizations-organization-get-open-choices',
-                                                  url='http://localhost:8080/organizations/{id}/opener',
-                                                  rel=['hea-opener-choices']),
-                                           Action(name='heaserver-organizations-organization-duplicate',
-                                                  url='http://localhost:8080/organizations/{id}/duplicator',
-                                                  rel=['duplicator'])
-                                           ],
-                              get_all_actions=[Action(name='heaserver-organizations-organization-get-properties',
-                                                      rel=['properties']),
-                                               Action(name='heaserver-organizations-organization-get-open-choices',
-                                                      url='http://localhost:8080/organizations/{id}/opener',
-                                                      rel=['hea-opener-choices']),
-                                               Action(name='heaserver-organizations-organization-duplicate',
-                                                      url='http://localhost:8080/organizations/{id}/duplicator',
-                                                      rel=['duplicator'])],
+                              get_actions=[Action(
+                                  name='heaserver-organizations-organization-get-properties',
+                                  rel=['properties']),
+                                  Action(
+                                      name='heaserver-organizations-organization-get-open-choices',
+                                      url='/organizations/{id}/opener',
+                                      rel=['hea-opener-choices']),
+                                  Action(
+                                      name='heaserver-organizations-organization-duplicate',
+                                      url='/organizations/{id}/duplicator',
+                                      rel=['duplicator'])
+                              ],
+                              get_all_actions=[Action(
+                                  name='heaserver-organizations-organization-get-properties',
+                                  rel=['properties']),
+                                  Action(
+                                      name='heaserver-organizations-organization-get-open-choices',
+                                      url='/organizations/{id}/opener',
+                                      rel=['hea-opener-choices']),
+                                  Action(
+                                      name='heaserver-organizations-organization-duplicate',
+                                      url='/organizations/{id}/duplicator',
+                                      rel=['duplicator'])],
                               expected_opener=Link(
                                   url=f'http://localhost:8080/organizations/{db_store[service.MONGODB_ORGANIZATION_COLLECTION][0]["id"]}/content',
                                   rel=['hea-default', 'hea-opener', 'text/plain']),
                               duplicate_action_name='heaserver-organizations-organization-duplicate-form',
                               put_content_status=204, sub=TEST_USER)
```

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/service.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_client.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_get_component.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/test_post_component.py` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/integrationtests/heaserver/serviceintegrationtest/wstl/all.json` & `heaserver-1.5.0/integrationtests/heaserver/serviceintegrationtest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/setup.py` & `heaserver-1.5.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,27 +8,27 @@
 from os import path
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name='heaserver',
-      version='1.4.1',
+      version='1.5.0',
       description='The server side of HEA.',
       long_description=long_description,
       long_description_content_type='text/markdown',
       url='https://risr.hci.utah.edu',
       author='Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT',
       author_email='Andrew.Post@hci.utah.edu',
       python_requires='>=3.10',
       package_dir={'': 'src'},
       packages=find_namespace_packages(where='src'),
       package_data={'heaserver.service': ['py.typed', 'jsonschemafiles/*']},
       install_requires=[
-          'heaobject~=1.4.0',
+          'heaobject~=1.5.0',
           'aiohttp[speedups]~=3.8.6',
           'hea-aiohttp-remotes~=1.2.1',  # replace with aiohttp-remotes if they incorporate our patch.
           'motor~=3.2.0',
           'motor-types~=1.0.0b2',
           'accept-types~=0.4.1',
           'mongoquery~=1.4.2',
           'jsonschema~=4.17.3',
```

### Comparing `heaserver-1.4.1/src/heaserver/service/__init__.py` & `heaserver-1.5.0/src/heaserver/service/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/activity.py` & `heaserver-1.5.0/src/heaserver/service/activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/aiohttp.py` & `heaserver-1.5.0/src/heaserver/service/aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/appfactory.py` & `heaserver-1.5.0/src/heaserver/service/appfactory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/appproperty.py` & `heaserver-1.5.0/src/heaserver/service/appproperty.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/backgroundtasks.py` & `heaserver-1.5.0/src/heaserver/service/backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/caching.py` & `heaserver-1.5.0/src/heaserver/service/caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/client.py` & `heaserver-1.5.0/src/heaserver/service/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -281,15 +281,17 @@
     """
     Coroutine that deletes a HEAObject.
 
     :param app: the aiohttp application context (required).
     :param url: the URL (str or URL) of the resource (required).
     :param headers: optional dict of headers.
     :param client_session: a client session. If None, the default session will be used.
-    :returns if successful it returns None else if it fails it will raise HttpError
+    :returns if successful it returns None else if it fails it will raise an exception.
+    :raises aiohttp.client_exceptions.ClientResponseError: if the response's status code was unexpected.
+    :raises aiohttp.client_exceptions.ClientConnectionError: if a connection to the service could not be established.
     """
     _logger = logging.getLogger(__name__)
     session = client_session if client_session is not None else app[appproperty.HEA_CLIENT_SESSION]
     _logger.debug('Deleting %s', str(url))
     async with session.delete(url, headers=headers, raise_for_status=False) as response_:
         if response_.status != 204:
             await _raise_client_response_error(response_)
```

### Comparing `heaserver-1.4.1/src/heaserver/service/config.py` & `heaserver-1.5.0/src/heaserver/service/config.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/db/aws.py` & `heaserver-1.5.0/src/heaserver/service/db/aws.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,14 +26,15 @@
 from .. import client
 from yarl import URL
 from typing import Optional, Any, TypeVar, cast, overload, Literal
 from configparser import ConfigParser
 import asyncio
 from threading import Lock
 from contextlib import closing
+from collections import defaultdict
 from collections.abc import Callable, Sequence, AsyncGenerator
 import logging
 
 _boto3_client_lock = Lock()
 _boto3_resource_lock = Lock()
 _boto3_client_config = botocore.config.Config(max_pool_connections=25)
 
@@ -51,14 +52,18 @@
     """
     # this is the buffer we give to refresh credentials in minutes on our end before they expire on aws
     EXPIRATION_LIMIT = 540
     MAX_DURATION_SECONDS = 43200
 
     _S3Service = TypeVar('_S3Service')
 
+    def __init__(self, *args, **kwargs):
+        super().__init__(*args, **kwargs)
+        self.__locks = defaultdict(asyncio.Lock)
+
     @property
     def file_system_type(self) -> type[AWSFileSystem]:
         return AWSFileSystem
 
     async def update_credentials(self, request: Request, credentials: AWSCredentials) -> None:
         """
         This is a wrapper function to be extended by tests
@@ -325,33 +330,34 @@
             :return: the boto3 client provided with credentials
             :raise ValueError if no previously saved credentials it raises ValueError
         """
         logger = logging.getLogger(__name__)
         assert credentials.role_arn is not None, 'credentials must have a non-None role_arn attribute'
         loop = asyncio.get_running_loop()
 
-        if credentials.has_expired(S3.EXPIRATION_LIMIT):
-            logger.debug("credentials need to be refreshed")
-            cloud_creds = await self.generate_cloud_credentials(request, credentials.role_arn)
-            if not cloud_creds:
-                raise ValueError(f'Could not generate cloud credentials with these params {credentials.role_arn}')
-            if logger.getEffectiveLevel() == logging.DEBUG:
-                logger.debug("credentials successfully obtained from cloud: %s" % cloud_creds.to_dict())
-            credentials.account = cloud_creds.account
-            credentials.password = cloud_creds.password
-            credentials.session_token = cloud_creds.session_token
-            credentials.expiration = cloud_creds.expiration
-            await self.update_credentials(request=request, credentials=credentials)
-            logger.debug("credentials updated in the database")
-        return await loop.run_in_executor(None, partial(creator,
-                                                        service_name,
-                                                        region_name=credentials.where,
-                                                        aws_access_key_id=credentials.account,
-                                                        aws_secret_access_key=credentials.password,
-                                                        aws_session_token=credentials.session_token))
+        async with self.__locks[credentials.id]:
+            if credentials.has_expired(S3.EXPIRATION_LIMIT):
+                logger.debug("credentials need to be refreshed")
+                cloud_creds = await self.generate_cloud_credentials(request, credentials.role_arn)
+                if not cloud_creds:
+                    raise ValueError(f'Could not generate cloud credentials with these params {credentials.role_arn}')
+                if logger.getEffectiveLevel() == logging.DEBUG:
+                    logger.debug("credentials successfully obtained from cloud: %s", cloud_creds.to_dict())
+                credentials.account = cloud_creds.account
+                credentials.password = cloud_creds.password
+                credentials.session_token = cloud_creds.session_token
+                credentials.expiration = cloud_creds.expiration
+                await self.update_credentials(request=request, credentials=credentials)
+                logger.debug("credentials updated in the database")
+            return await loop.run_in_executor(None, partial(creator,
+                                                            service_name,
+                                                            region_name=credentials.where,
+                                                            aws_access_key_id=credentials.account,
+                                                            aws_secret_access_key=credentials.password,
+                                                            aws_session_token=credentials.session_token))
 
 
 class S3WithMongo(S3, Mongo):
     def __init__(self, config: Optional[ConfigParser], **kwargs):
         super().__init__(config, **kwargs)
 
 
@@ -511,24 +517,30 @@
         raise ValueError('Cannot get credentials arn which is required')
     auth = request.headers.get(hdrs.AUTHORIZATION, '')
     auth_token = auth.split(' ')
 
     if len(auth_token) != 2:
         raise ValueError("Bearer Token is required in header")
     logger.debug('Getting credentials for user %s with role %s...', sub, arn)
+    roles_url = await type_to_resource_url(request, Role)
     try:
-        logger.debug('User %s has role %s', sub, arn)
-        loop = asyncio.get_running_loop()
-        sts_client_call = partial(boto3.client, 'sts', config=_boto3_client_config)
-        with closing(await loop.run_in_executor(None, sts_client_call)) as sts_client:
-            assumed_role_object = await loop.run_in_executor(None, partial(sts_client.assume_role_with_web_identity,
-                                                                            WebIdentityToken=auth_token[1],
-                                                                            RoleArn=arn,
-                                                                            RoleSessionName=sub,
-                                                                            DurationSeconds=S3.MAX_DURATION_SECONDS))
+        if await client.has(request.app, URL(roles_url) / 'byname' / encode_role(arn),
+                        headers={hdrs.AUTHORIZATION: auth, SUB: sub}):
+            logger.debug('User %s has role %s', sub, arn)
+            loop = asyncio.get_running_loop()
+            sts_client_call = partial(boto3.client, 'sts', config=_boto3_client_config)
+            with closing(await loop.run_in_executor(None, sts_client_call)) as sts_client:
+                assumed_role_object = await loop.run_in_executor(None, partial(sts_client.assume_role_with_web_identity,
+                                                                                WebIdentityToken=auth_token[1],
+                                                                                RoleArn=arn,
+                                                                                RoleSessionName=sub,
+                                                                                DurationSeconds=S3.MAX_DURATION_SECONDS))
+        else:
+            logger.debug('User does not have role %s, so temporary credentials could not be generated', arn)
+            return None
     except ClientError:
         logger.exception('User %s does not have role %s', sub, arn)
         return None
     creds_dict = assumed_role_object.get('Credentials')
     if not creds_dict:
         return None
     creds = AWSCredentials()
```

### Comparing `heaserver-1.4.1/src/heaserver/service/db/awsservicelib.py` & `heaserver-1.5.0/src/heaserver/service/db/awsservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/db/database.py` & `heaserver-1.5.0/src/heaserver/service/db/database.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/db/dbapi2.py` & `heaserver-1.5.0/src/heaserver/service/db/dbapi2.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/db/mongo.py` & `heaserver-1.5.0/src/heaserver/service/db/mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/db/mongoexpr.py` & `heaserver-1.5.0/src/heaserver/service/db/mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/db/mongoservicelib.py` & `heaserver-1.5.0/src/heaserver/service/db/mongoservicelib.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/expression.py` & `heaserver-1.5.0/src/heaserver/service/expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/functional.py` & `heaserver-1.5.0/src/heaserver/service/functional.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/heaobjectsupport.py` & `heaserver-1.5.0/src/heaserver/service/heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/jsonschema.py` & `heaserver-1.5.0/src/heaserver/service/jsonschema.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/jsonschemafiles/__init__.py` & `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/jsonschemafiles/cjtemplate.json` & `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/cjtemplate.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/jsonschemafiles/wstl.json` & `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstl.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/jsonschemafiles/wstlaction.json` & `heaserver-1.5.0/src/heaserver/service/jsonschemafiles/wstlaction.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/jsonschemavalidator.py` & `heaserver-1.5.0/src/heaserver/service/jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/messagebroker.py` & `heaserver-1.5.0/src/heaserver/service/messagebroker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/mimetypes.py` & `heaserver-1.5.0/src/heaserver/service/mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/oidcclaimhdrs.py` & `heaserver-1.5.0/src/heaserver/service/oidcclaimhdrs.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/openapi.py` & `heaserver-1.5.0/src/heaserver/service/openapi.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/representor/__init__.py` & `heaserver-1.5.0/src/heaserver/service/representor/__init__.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/representor/cj.py` & `heaserver-1.5.0/src/heaserver/service/representor/cj.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,18 +9,20 @@
 """
 
 import uritemplate
 import logging
 import operator
 from itertools import groupby
 from heaobject import root
-from heaobject.root import is_heaobject_dict, is_heaobject_dict_list, is_primitive_list, is_primitive, DesktopObjectDict
+from heaobject.user import NONE_USER
+from heaobject.root import is_heaobject_dict, is_heaobject_dict_list, is_primitive_list, is_primitive, DesktopObjectDict, desktop_object_from_dict, Permission
 from json.decoder import JSONDecodeError
 from .error import ParseException, FormatException
 from .. import jsonschemavalidator
+from ..oidcclaimhdrs import SUB
 from aiohttp.web import Request
 from typing import Any, Union, Optional, Type
 from collections.abc import Generator, Callable, Mapping, Sequence, Iterable, Mapping
 from .representor import Representor, Link
 from ..wstl import get_section, has_section, get_extended_property_value, has_extended_property_value
 from heaserver.service.expression import get_eval_for
 from copy import deepcopy
@@ -95,14 +97,15 @@
         :param wstl_obj: dict with run-time WeSTL JSON.
         :param coll_url: the URL of the collection.
         :param link_callback: a callable that will be called whenever a link is created. The first
         parameter contains the index of the item, or None if the link is global. The second parameter
         contains the link as a heaserver.service.representor.Link object.
         :return: a Collection+JSON dict.
         """
+        sub = request.headers.get(SUB, NONE_USER)
         wstl = wstl_obj['wstl']
         collection: dict[str, Any] = {}
         collection['version'] = '1.0'
         wstl_hea = wstl.get('hea', {})
         collection['href'] = wstl_hea.get('href', '#')
         collection['permissions'] = wstl_hea.get('permissions', [[]] * len(wstl.get('data', [])))
 
@@ -113,15 +116,15 @@
         items = tuple(item for item in _get_items(request, wstl, link_callback=link_callback, tvars=tvars))
         if items:
             collection['items'] = items
         links = tuple(link for link in _get_links(wstl.get('actions', []), tvars, link_callback=link_callback))
         if links:
             collection['links'] = links
         if 'template' not in collection:
-            template = _get_template(wstl.get('actions', []), tvars if len(wstl.get('data', [])) <= 1 else {}, wstl.get('data', []))
+            template = _get_template(sub, wstl.get('actions', []), tvars if len(wstl.get('data', [])) <= 1 else {}, wstl.get('data', []))
             if template:
                 collection['template'] = template
         queries = tuple(query for query in _get_queries(wstl.get('actions', [])))
         if queries:
             collection['queries'] = queries
         if 'error' in wstl:
             collection['error'] = _get_error(wstl['error'])
@@ -315,15 +318,15 @@
                     'pattern': d.get('pattern')
                 }
                 q['data'].append(data_)
                 add_extended_property_values(d, data_)
             yield q
 
 
-def _get_template(wstl_actions: list[dict[str, Any]], tvars: dict[str, Any], data: Sequence[DesktopObjectDict] | None = None) -> dict:
+def _get_template(sub: str, wstl_actions: list[dict[str, Any]], tvars: dict[str, Any], data: Sequence[DesktopObjectDict] | None = None) -> dict:
     """
     Generates a template from the first action with a cj-template target, skipping such actions when there are multiple
     desktop objects in the data. Additionally, for any action with a cj-template target and when there is one desktop
     object in the data, the action will be skipped if its itemif expression evaluates to False.
     """
     cj_template = {}
     for wstl_action in wstl_actions:
@@ -332,73 +335,75 @@
                 continue
             is_add = _is_in_target('add', wstl_action)
 
             cj_template['prompt'] = wstl_action.get('prompt', wstl_action['name'])
             cj_template['rel'] = ' '.join(wstl_action['rel'])
 
             cj_template['data'] = []
+            obj = desktop_object_from_dict(data[0]) if len(data) > 0 else None
             for input_ in wstl_action['inputs']:
                 nm = input_['name']
+                read_only = obj.is_attribute_read_only(sub, nm) if obj is not None else False
                 if is_add:
                     value_ = input_.get('value', None)
                 elif has_section(input_):
                     value_ = tvars.get(f'{get_section(input_)}')
                 else:
                     value_ = tvars.get(nm, None)
                 if is_heaobject_dict_list(value_) and len(value_) > 0:
                     if not has_section(input_):
                         data_ = {
                             'name': input_['name'],
                             'value': value_,
                             'prompt': input_.get('prompt', nm),
                             'required': input_.get('required', False),
-                            'readOnly': input_.get('readOnly', False),
+                            'readOnly': input_.get('readOnly', read_only),
                             'pattern': input_.get('pattern')
                         }
                         add_extended_property_values(input_, data_)
                         cj_template['data'].append(data_)
                     else:
                         template_val = {
                             'section': get_section(input_),
                             'index': -1,
                             'name': nm,
                             'value': input_.get('value') if has_section(input_) else (
                                 value_ if value_ is not None else input_.get('value')),
                             'prompt': input_.get('prompt', nm),
                             'required': input_.get('required', False),
-                            'readOnly': input_.get('readOnly', False),
+                            'readOnly': input_.get('readOnly', read_only),
                             'pattern': input_.get('pattern')
                         }
                         if has_extended_property_value('sectionPrompt', input_):
                             template_val['sectionPrompt'] = get_extended_property_value('sectionPrompt', input_)
                         add_extended_property_values(input_, template_val)
                         cj_template['data'].append(template_val)
                         for i, v in enumerate(value_):
                             data_ = {
                                 'section': get_section(input_),
                                 'index': i,
                                 'name': input_['name'],
                                 'value': v.get(input_['name']),
                                 'prompt': input_.get('prompt', nm),
                                 'required': input_.get('required', False),
-                                'readOnly': input_.get('readOnly', False),
+                                'readOnly': input_.get('readOnly', read_only),
                                 'pattern': input_.get('pattern')
                             }
                             if has_extended_property_value('sectionPrompt', input_):
                                 data_['sectionPrompt'] = get_extended_property_value('sectionPrompt', input_)
                             add_extended_property_values(input_, data_)
                             cj_template['data'].append(data_)
                 elif is_heaobject_dict(value_) and len(value_) > 0:
                     data_ = {
                         'section': get_section(input_),
                         'name': input_['name'],
                         'value': value_[input_['name']],
                         'prompt': input_.get('prompt', nm),
                         'required': input_.get('required', False),
-                        'readOnly': input_.get('readOnly', False),
+                        'readOnly': input_.get('readOnly', read_only),
                         'pattern': input_.get('pattern')
                     }
                     if has_extended_property_value('sectionPrompt', input_):
                         input_['sectionPrompt'] = get_extended_property_value('sectionPrompt', input_)
                     add_extended_property_values(input_, data_)
                     cj_template['data'].append(data_)
                 elif is_primitive(value_) or is_primitive_list(value_):
@@ -409,15 +414,15 @@
                     if has_extended_property_value('sectionPrompt', input_):
                         data_['sectionPrompt'] = get_extended_property_value('sectionPrompt', input_)
                     data_ = data_ | {
                         'name': nm,
                         'value': input_.get('value') if has_section(input_) else (value_ if value_ is not None else input_.get('value')),  # this is the line
                         'prompt': input_.get('prompt', nm),
                         'required': input_.get('required', False),
-                        'readOnly': input_.get('readOnly', False),
+                        'readOnly': input_.get('readOnly', read_only),
                         'pattern': input_.get('pattern')
                     }
                     add_extended_property_values(input_, data_)
                     cj_template['data'].append(data_)
                 else:
                     raise ValueError(value_)
             resorted = []
```

### Comparing `heaserver-1.4.1/src/heaserver/service/representor/factory.py` & `heaserver-1.5.0/src/heaserver/service/representor/factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/representor/nvpjson.py` & `heaserver-1.5.0/src/heaserver/service/representor/nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/representor/representor.py` & `heaserver-1.5.0/src/heaserver/service/representor/representor.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/representor/wstljson.py` & `heaserver-1.5.0/src/heaserver/service/representor/wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/representor/xwwwformurlencoded.py` & `heaserver-1.5.0/src/heaserver/service/representor/xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/response.py` & `heaserver-1.5.0/src/heaserver/service/response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/runner.py` & `heaserver-1.5.0/src/heaserver/service/runner.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/aiohttptestcase.py` & `heaserver-1.5.0/src/heaserver/service/testcase/aiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/awsdockermongo.py` & `heaserver-1.5.0/src/heaserver/service/testcase/awsdockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/awss3microservicetestcase.py` & `heaserver-1.5.0/src/heaserver/service/testcase/awss3microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/collection.py` & `heaserver-1.5.0/src/heaserver/service/testcase/collection.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/docker.py` & `heaserver-1.5.0/src/heaserver/service/testcase/docker.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/dockermongo.py` & `heaserver-1.5.0/src/heaserver/service/testcase/dockermongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/expectedvalues.py` & `heaserver-1.5.0/src/heaserver/service/testcase/expectedvalues.py`

 * *Files 2% similar despite different names*

```diff
@@ -311,15 +311,15 @@
     queries_ = queries()
     if queries_:
         collection['collection']['queries'] = queries_
     for action, action_name, rel, itemif in ((wstl_builder.find_action(a.name), a.name, a.rel, a.itemif) for a in get_actions_):
         if action is None:
             raise ValueError(f'Invalid action name in get_all_actions {action_name}')
         if itemif is None or get_eval_for(obj).eval(itemif):
-            _set_collection_template(action, collection, obj, 1, rel)
+            _set_collection_template(action, collection, obj, 1, rel, sub)
     return [collection]
 
 
 def expected_opener_body(
     fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
     coll: str | CollectionKey,
     wstl_builder: wstl.RuntimeWeSTLDocumentBuilder,
@@ -529,15 +529,15 @@
                                      'permissions': [[p.name for p in perm] for perm in perms],
                                      'items': items,
                                      'version': '1.0'}}
     for action, action_name, rel, itemif in ((wstl_builder.find_action(a.name), a.name, a.rel, a.itemif) for a in get_all_actions_):
         if action is None:
             raise ValueError(f'Invalid action name in get_all_actions {action_name}')
         if len(set(i['type'] for i in collection)) < 2 and (itemif is None or get_eval_for(f).eval(itemif)):
-            _set_collection_template(action, collection_doc, f, len(collection), rel)
+            _set_collection_template(action, collection_doc, f, len(collection), rel, sub)
     top_level_links_ = top_level_links()
     if top_level_links_:
         collection_doc['collection']['links'] = top_level_links_
     return [collection_doc]
 
 
 def expected_values(fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
@@ -602,91 +602,91 @@
 
 
 def _create_template(d: DesktopObjectDict, exclude=('id',)) -> Dict[str, Dict[str, List[Dict[str, Any]]]]:
     return {'template': {'data': [z for x, y in d.items() if (not exclude or x not in exclude) for z in
                                   _nvpjson_property_to_cj_part_generator(x, y)]}}
 
 
-def _template_data_generator(action: dict[str, Any], desktop_object_dict: DesktopObjectDict, len_fixtures=1):
+def _template_data_generator(sub: str, action: dict[str, Any], desktop_object_dict: DesktopObjectDict, len_fixtures=1):
     targets = action['target'].split()
     for input in action.get('inputs', []):
         section = wstl.get_section(input)
         if optionsFromUrl := wstl.get_extended_property_value('optionsFromUrl', input):
             if 'href' not in optionsFromUrl:
                 optionsFromUrlPath = optionsFromUrl['path']
                 optionsFromUrl['href'] = 'http://localhost:8080' + ('/' if optionsFromUrlPath else '') + optionsFromUrlPath
         if 'add' in targets:
-            yield _new_template_data_item(input, input['value'])
+            yield _new_template_data_item(input, input['value'], sub)
 
         elif len_fixtures == 1:
             nm = input['name']
             if nm in ('meta'):
                 continue
             val = desktop_object_dict.get(section, []) if wstl.has_section(input) else desktop_object_dict.get(nm)
             if isinstance(val, list):
                 if wstl.has_section(input):
                     if val:
-                        yield _new_template_data_item(input, input.get('value')) | {
+                        yield _new_template_data_item(input, input.get('value'), sub) | {
                             'index': -1,
                             'section': section
                         } | _section_prompt_key_value(input)
                         for i_, v in enumerate(val):
-                            yield _new_template_data_item(input, v.get(nm, input.get('value'))) | {
+                            yield _new_template_data_item(input, v.get(nm, input.get('value')), sub) | {
                                 'index': i_,
                                 'section': section
                             } | _section_prompt_key_value(input)
                     else:
-                        yield _new_template_data_item(input, input.get('value')) | {
+                        yield _new_template_data_item(input, input.get('value'), sub) | {
                             'index': -1,
                             'section': section
                         } | _section_prompt_key_value(input)
                 else:
-                    yield _new_template_data_item(input, val)
+                    yield _new_template_data_item(input, val, sub)
             elif isinstance(val, dict):
-                yield _new_template_data_item(input, val.get(nm, input.get('value'))) | {
+                yield _new_template_data_item(input, val.get(nm, input.get('value')), sub) | {
                     'section': section
                 } | _section_prompt_key_value(input)
             else:
-                yield _new_template_data_item(input, val if val is not None else input.get('value'))
+                yield _new_template_data_item(input, val if val is not None else input.get('value'), sub)
         elif not section:
-            yield _new_template_data_item(input, input.get('value'))
+            yield _new_template_data_item(input, input.get('value'), sub)
         else:
-            yield _new_template_data_item(input, input.get('value')) | {'section': section,
+            yield _new_template_data_item(input, input.get('value'), sub) | {'section': section,
                                                                         'index': -1} | _section_prompt_key_value(input)
 
 
 def _section_prompt_key_value(i):
     epv = wstl.get_extended_property_value('sectionPrompt', i)
     return {'sectionPrompt': epv} if epv is not None else {}
 
 
-def _new_template_data_item(i: dict[str, Any], value: Any) -> dict[str, Any]:
+def _new_template_data_item(i: dict[str, Any], value: Any, sub: str) -> dict[str, Any]:
     rtn = {'name': i['name'],
            'value': _value_append(value),
            'prompt': i.get('prompt', i['name']),
            'required': i.get('required', False),
            'pattern': i.get('pattern'),
-           'readOnly': i.get('readOnly', False)}
+           'readOnly': i.get('readOnly', True if i['name'] in ('modified', 'created') or (i['name'] == 'owner' and i.get('value', NONE_USER) != sub) else False)}
     add_extended_property_values(i, rtn)
     return rtn
 
 
-def _set_collection_template(action, collection_doc, fixture, len_fixtures, rel):
+def _set_collection_template(action, collection_doc, fixture, len_fixtures, rel, sub):
     """
     Adds a template object to the provided Collection+JSON document.
 
     :param action:
     :param collection_doc:
     :param fixture:
     :param len_fixtures:
     :param rel:
     """
     targets = action['target'].split()
     if 'cj-template' in targets:
-        template = {'data': [d for d in _template_data_generator(action, fixture, len_fixtures)],
+        template = {'data': [d for d in _template_data_generator(sub, action, fixture, len_fixtures)],
                     'prompt': action.get('prompt', action['name']),
                     'rel': ' '.join(rel) if rel is not None else ''}
         collection_doc['collection']['template'] = template
 
 
 def _expected_one_form(
     fixtures: Mapping[str, List[DesktopObjectDict]] | Mapping[CollectionKey, List[DesktopObjectDict]],
@@ -738,15 +738,15 @@
                               None)
             if field_name:
                 for d in template_data:
                     if d['name'] == field_name:
                         d['value'] = link['href']
 
     links_ = [get_link(a) for a in actions or []]
-    template_data = [d for d in _template_data_generator(action, obj_dict)]
+    template_data = [d for d in _template_data_generator(sub, action, obj_dict)]
     set_default_values_from_headata_links()
     obj = desktop_object_from_dict(obj_dict)
     return [{
         'collection': {
             'version': '1.0',
             'href': str(href),
             'permissions': [[perm.name for perm in obj.get_permissions(sub)]],
```

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/microservicetestcase.py` & `heaserver-1.5.0/src/heaserver/service/testcase/microservicetestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/mixin.py` & `heaserver-1.5.0/src/heaserver/service/testcase/mixin.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/mockaws.py` & `heaserver-1.5.0/src/heaserver/service/testcase/mockaws.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/mockdatabase.py` & `heaserver-1.5.0/src/heaserver/service/testcase/mockdatabase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/mockmongo.py` & `heaserver-1.5.0/src/heaserver/service/testcase/mockmongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/simpleaiohttptestcase.py` & `heaserver-1.5.0/src/heaserver/service/testcase/simpleaiohttptestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/swaggerui.py` & `heaserver-1.5.0/src/heaserver/service/testcase/swaggerui.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/testenv.py` & `heaserver-1.5.0/src/heaserver/service/testcase/testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/testcase/util.py` & `heaserver-1.5.0/src/heaserver/service/testcase/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/uritemplate.py` & `heaserver-1.5.0/src/heaserver/service/uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/util.py` & `heaserver-1.5.0/src/heaserver/service/util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver/service/wstl.py` & `heaserver-1.5.0/src/heaserver/service/wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/src/heaserver.egg-info/PKG-INFO` & `heaserver-1.5.0/src/heaserver.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: heaserver
-Version: 1.4.1
+Version: 1.5.0
 Summary: The server side of HEA.
 Home-page: https://risr.hci.utah.edu
 Author: Research Informatics Shared Resource, Huntsman Cancer Institute, Salt Lake City, UT
 Author-email: Andrew.Post@hci.utah.edu
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -20,15 +20,15 @@
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: heaobject~=1.4.0
+Requires-Dist: heaobject~=1.5.0
 Requires-Dist: aiohttp[speedups]~=3.8.6
 Requires-Dist: hea-aiohttp-remotes~=1.2.1
 Requires-Dist: motor~=3.2.0
 Requires-Dist: motor-types~=1.0.0b2
 Requires-Dist: accept-types~=0.4.1
 Requires-Dist: mongoquery~=1.4.2
 Requires-Dist: jsonschema~=4.17.3
@@ -47,14 +47,22 @@
 Requires-Dist: types-cachetools~=5.3.0
 
 # HEA Server Framework
 [Research Informatics Shared Resource](https://risr.hci.utah.edu), [Huntsman Cancer Institute](https://healthcare.utah.edu/huntsmancancerinstitute/), Salt Lake City, UT
 
 The HEA Server Framework contains shared code for creating HEA microservices.
 
+## Version 1.5.0
+* Added attribute-level permissions.
+* Temporarily restored the role check that was removed in version 1.4.1 in case an AWS credentials object with overly
+permissive permissions is altered.
+
+## Version 1.4.2
+* Synchronize around getting temporary credentials.
+
 ## Version 1.4.1
 * Increased the boto3 max connection pool size from the default value (10) to 25.
 * Fixed a connection leak in DatabaseContextManager, and fixed the documentation for the connection() method.
 * Updated heaobject dependency.
 * Removed an unnecessary role check.
 
 ## Version 1.4.0
```

### Comparing `heaserver-1.4.1/src/heaserver.egg-info/SOURCES.txt` & `heaserver-1.5.0/src/heaserver.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_aiohttp.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_caching.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_client.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_component_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_organization_with_bad_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_post_component.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_component.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_put_organization_permissions.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_response.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_testenv.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_uritemplate.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_util.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.0/tests/heaserver/servicetest/__pycache__/test_wstl.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/componentpermissionstestcase.py` & `heaserver-1.5.0/tests/heaserver/servicetest/componentpermissionstestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/componenttestcase.py` & `heaserver-1.5.0/tests/heaserver/servicetest/componenttestcase.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongo.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088` & `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.33088`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.0/tests/heaserver/servicetest/db/__pycache__/test_mongoexpr.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/db/test_mongo.py` & `heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongo.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/db/test_mongoexpr.py` & `heaserver-1.5.0/tests/heaserver/servicetest/db/test_mongoexpr.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/organizationpermissionstestcase.py` & `heaserver-1.5.0/tests/heaserver/servicetest/organizationtestcase.py`

 * *Files 12% similar despite different names*

```diff
@@ -31,86 +31,81 @@
             "derived_by": None,
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "23423DAFSDF12adfasdf3",
             "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
-            'admin_ids': []
+            'mime_type': 'application/x.organization',
+            'admin_ids': [TEST_USER],
+            'accounts': [],
+            'type_display_name': 'Organization',
+            'admin_group_ids': [],
+            'manager_group_ids': [],
+            'member_group_ids': []
         },
         {
             "id": "0123456789ab0123456789ab",
             "source": None,
             "source_detail": None,
             "name": "Reximus",
             "display_name": "Reximus",
             "description": "Description of Reximus",
             "owner": NONE_USER,
             "created": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "modified": datetime(2021, 12, 2, 17, 31, 15, 630000),
             "invites": [],
-            "shares": [
-                {
-                    'type': 'heaobject.root.ShareImpl',
-                    'invite': None,
-                    'user': ALL_USERS,
-                    'permissions': [Permission.CHECK_DYNAMIC.name]
-                },
-                {
-                    'type': 'heaobject.root.ShareImpl',
-                    'invite': None,
-                    'user': TEST_USER,
-                    'permissions': [Permission.VIEWER.name]
-                }
-            ],
+            "shares": [{
+                'type': 'heaobject.root.ShareImpl',
+                'invite': None,
+                'user': ALL_USERS,
+                'permissions': [Permission.CHECK_DYNAMIC.name]
+            }],
             "derived_by": None,
             "derived_from": [],
             "aws_account_ids": [],
             "principal_investigator_id": "11234867890b0123a56789ab",
-            "manager_ids": [''],
+            "manager_ids": [],
             "member_ids": [],
             'type': 'heaobject.organization.Organization',
-            'admin_ids': []
+            'mime_type': 'application/x.organization',
+            'admin_ids': [TEST_USER],
+            'accounts': [],
+            'type_display_name': 'Organization',
+            'admin_group_ids': [],
+            'manager_group_ids': [],
+            'member_group_ids': []
         }
     ]}
 
 content = {
     service.MONGODB_ORGANIZATION_COLLECTION: {
-        '666f6f2d6261722d71757578': b'The quick brown fox jumps over the lazy dog',
-        '0123456789ab0123456789ab': b''
+        '666f6f2d6261722d71757578': b'The quick brown fox jumps over the lazy dog'
     }
 }
 
-OrganizationPermissionsTestCase = \
-    get_test_case_cls_default(coll=service.MONGODB_ORGANIZATION_COLLECTION,
-                              wstl_package=service.__package__,
-                              href='http://localhost:8080/organizations',
-                              fixtures=db_store,
-                              content=content,
-                              get_actions=[Action(
-                                  name='heaserver-organizations-organization-get-properties',
-                                  rel=['properties']),
-                                  Action(
-                                      name='heaserver-organizations-organization-get-open-choices',
-                                      url='/organizations/{id}/opener',
-                                      rel=['hea-opener-choices']),
-                                  Action(
-                                      name='heaserver-organizations-organization-duplicate',
-                                      url='/organizations/{id}/duplicator',
-                                      rel=['duplicator'])
-                              ],
-                              get_all_actions=[Action(
-                                  name='heaserver-organizations-organization-get-properties',
-                                  rel=['properties']),
-                                  Action(
-                                      name='heaserver-organizations-organization-get-open-choices',
-                                      url='/organizations/{id}/opener',
-                                      rel=['hea-opener-choices']),
-                                  Action(
-                                      name='heaserver-organizations-organization-duplicate',
-                                      url='/organizations/{id}/duplicator',
-                                      rel=['duplicator'])],
-                              expected_opener=Link(
-                                  url=f'http://localhost:8080/organizations/{db_store[service.MONGODB_ORGANIZATION_COLLECTION][0]["id"]}/content',
-                                  rel=['hea-default', 'hea-opener', 'text/plain']),
-                              duplicate_action_name='heaserver-organizations-organization-duplicate-form',
-                              put_content_status=204, sub=TEST_USER)
+
+OrganizationTestCase = get_test_case_cls_default(coll=service.MONGODB_ORGANIZATION_COLLECTION,
+                                                 wstl_package=service.__package__,
+                                                 href='http://localhost:8080/organizations',
+                                                 fixtures=db_store,
+                                                 content=content,
+                                                 get_actions=[Action(name='heaserver-organizations-organization-get-properties',
+                                                                         rel=['properties']),
+                                                              Action(name='heaserver-organizations-organization-get-open-choices',
+                                                                         url='http://localhost:8080/organizations/{id}/opener',
+                                                                         rel=['hea-opener-choices']),
+                                                              Action(name='heaserver-organizations-organization-duplicate',
+                                                                         url='http://localhost:8080/organizations/{id}/duplicator',
+                                                                         rel=['duplicator'])
+                                                              ],
+                                                 get_all_actions=[Action(name='heaserver-organizations-organization-get-properties',
+                                                                             rel=['properties']),
+                                                                  Action(name='heaserver-organizations-organization-get-open-choices',
+                                                                             url='http://localhost:8080/organizations/{id}/opener',
+                                                                             rel=['hea-opener-choices']),
+                                                                  Action(name='heaserver-organizations-organization-duplicate',
+                                                                             url='http://localhost:8080/organizations/{id}/duplicator',
+                                                                             rel=['duplicator'])],
+                                                 expected_opener=Link(url=f'http://localhost:8080/organizations/{db_store[service.MONGODB_ORGANIZATION_COLLECTION][0]["id"]}/content', rel=['hea-default', 'hea-opener', 'text/plain']),
+                                                 duplicate_action_name='heaserver-organizations-organization-duplicate-form',
+                                                 put_content_status=204, sub=TEST_USER)
```

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.27996`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35228`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.35444`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_cj.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.35312`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_factory.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_nvpjson.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.29420`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_supports_links.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11224`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.11864`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13080`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.13852`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.15488`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.1816`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.19788`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.28016`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.30312`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.34620`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.35280`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.37360`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_wstljson.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.16864`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.19712`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.23624`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.29888`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.33128`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.3836`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/__pycache__/test_xwwwformurlencoded.cpython-311-pytest-7.4.4.pyc.4904`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_queries.json` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_queries.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/all_cj_template.json` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/all_cj_template.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/test_cj.py` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_cj.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/test_factory.py` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_factory.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/test_nvpjson.py` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_nvpjson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/test_wstljson.py` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_wstljson.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py` & `heaserver-1.5.0/tests/heaserver/servicetest/representor/test_xwwwformurlencoded.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/service.py` & `heaserver-1.5.0/tests/heaserver/servicetest/service.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_activity.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_activity.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_aiohttp.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_aiohttp.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_backgroundtasks.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_backgroundtasks.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_caching.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_caching.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_client.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_client.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_component_with_bad_permissions.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_component_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_configuration.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_configuration.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_database_classes.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_database_classes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_expression.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_expression.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_get_component.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_get_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_heaobjectsupport.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_heaobjectsupport.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_jsonschemavalidator.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_jsonschemavalidator.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_mimetypes.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_mimetypes.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_organization_with_bad_permissions.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_organization_with_bad_permissions.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_post_component.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_post_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_put_component.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_put_component.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_response.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_response.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_testenv.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_testenv.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_uritemplate.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_uritemplate.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_util.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_util.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/test_wstl.py` & `heaserver-1.5.0/tests/heaserver/servicetest/test_wstl.py`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl/all.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl/all.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_1.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_1.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_10a.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_10a.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_10b.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_10b.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_11.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_11.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_2.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_2.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_3.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_3.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_4.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_4.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_6.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_6.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_7.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_7.json`

 * *Files identical despite different names*

### Comparing `heaserver-1.4.1/tests/heaserver/servicetest/wstl_8.json` & `heaserver-1.5.0/tests/heaserver/servicetest/wstl_8.json`

 * *Files identical despite different names*

