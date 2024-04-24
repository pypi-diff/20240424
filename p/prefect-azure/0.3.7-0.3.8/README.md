# Comparing `tmp/prefect-azure-0.3.7.tar.gz` & `tmp/prefect_azure-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prefect-azure-0.3.7.tar", last modified: Tue Mar 19 19:31:27 2024, max compression
+gzip compressed data, was "prefect_azure-0.3.8.tar", last modified: Wed Apr 24 14:11:06 2024, max compression
```

## Comparing `prefect-azure-0.3.7.tar` & `prefect_azure-0.3.8.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:31:27.545325 prefect-azure-0.3.7/
--rw-r--r--   0 runner    (1001) docker     (127)    11356 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-03-19 19:31:27.545325 prefect-azure-0.3.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6827 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:31:27.545325 prefect-azure-0.3.7/prefect_azure/
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-19 19:31:27.545325 prefect-azure-0.3.7/prefect_azure/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    25908 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    36508 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/container_instance.py
--rw-r--r--   0 runner    (1001) docker     (127)     7920 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (127)    21662 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:31:27.541325 prefect-azure-0.3.7/prefect_azure/deployments/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/deployments/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7518 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/deployments/steps.py
--rw-r--r--   0 runner    (1001) docker     (127)     9879 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:31:27.541325 prefect-azure-0.3.7/prefect_azure/workers/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/workers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    39028 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/prefect_azure/workers/container_instance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:31:27.541325 prefect-azure-0.3.7/prefect_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-03-19 19:31:27.000000 prefect-azure-0.3.7/prefect_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-03-19 19:31:27.000000 prefect-azure-0.3.7/prefect_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-19 19:31:27.000000 prefect-azure-0.3.7/prefect_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-03-19 19:31:27.000000 prefect-azure-0.3.7/prefect_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-19 19:31:27.000000 prefect-azure-0.3.7/prefect_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-19 19:31:27.000000 prefect-azure-0.3.7/prefect_azure.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      757 2024-03-19 19:31:27.545325 prefect-azure-0.3.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1963 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-19 19:31:27.541325 prefect-azure-0.3.7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    37384 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/tests/test_aci_infrastructure.py
--rw-r--r--   0 runner    (1001) docker     (127)    39194 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/tests/test_aci_worker.py
--rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/tests/test_blob_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      672 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/tests/test_block_standards.py
--rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/tests/test_cosmos_db.py
--rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/tests/test_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/tests/test_ml_datastore.py
--rw-r--r--   0 runner    (1001) docker     (127)    80049 2024-03-19 19:30:27.000000 prefect-azure-0.3.7/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/prefect_azure/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure/_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25910 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36429 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/container_instance.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7923 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21828 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/prefect_azure/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/deployments/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7519 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/deployments/steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9880 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/prefect_azure/workers/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/workers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39029 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/prefect_azure/workers/container_instance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/prefect_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6295 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 14:11:06.000000 prefect_azure-0.3.8/prefect_azure.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.380747 prefect_azure-0.3.8/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:11:06.384748 prefect_azure-0.3.8/tests/deployments/
+-rw-r--r--   0 runner    (1001) docker     (127)    14605 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/deployments/test_steps.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37383 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_aci_infrastructure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39151 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_aci_worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10360 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_blob_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_block_standards.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1753 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_cosmos_db.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3983 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2531 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_ml_datastore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-24 14:10:54.000000 prefect_azure-0.3.8/tests/test_version.py
```

### Comparing `prefect-azure-0.3.7/PKG-INFO` & `prefect_azure-0.3.8/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,75 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.3.7
+Version: 0.3.8
 Summary: Prefect integrations with Microsoft Azure services
-Home-page: https://github.com/PrefectHQ/prefect-azure
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-azure
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
-Requires-Dist: azure_mgmt_containerinstance>=10.0
+Requires-Dist: aiohttp
 Requires-Dist: azure_identity>=1.10
+Requires-Dist: azure_mgmt_containerinstance>=10.0
 Requires-Dist: azure-mgmt-resource>=21.2
-Requires-Dist: aiohttp
+Requires-Dist: prefect>=2.14.10
 Provides-Extra: blob-storage
 Requires-Dist: azure-storage-blob; extra == "blob-storage"
 Provides-Extra: cosmos-db
 Requires-Dist: azure-cosmos; extra == "cosmos-db"
 Provides-Extra: ml-datastore
 Requires-Dist: azureml-core; extra == "ml-datastore"
 Provides-Extra: all-extras
 Requires-Dist: azure-cosmos; extra == "all-extras"
 Requires-Dist: azure-storage-blob; extra == "all-extras"
 Requires-Dist: azureml-core; extra == "all-extras"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
-Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 Requires-Dist: aiohttp; extra == "dev"
-Requires-Dist: pillow; extra == "dev"
 Requires-Dist: azure-cosmos; extra == "dev"
 Requires-Dist: azure-storage-blob; extra == "dev"
 Requires-Dist: azureml-core; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-azure
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-azure) to see additional examples and the API reference.
-
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-azure/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-azure?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-azure/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-azure?ccolor=26272B&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-azure/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-azure?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-azure/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-azure?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
 </p>
 
-## Welcome!
-
-prefect-azure is a collection of prebuilt Prefect tasks that can be used to quickly construct Prefect flows.
+`prefect-azure` is a collection of Prefect integrations for orchestration workflows with Azure.
 
 ## Getting Started
 
-### Python setup
-
-Requires an installation of Python 3.8+
-
-We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
-
-These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
-
 ### Installation
 
 Install `prefect-azure` with `pip`
 
 ```bash
 pip install prefect-azure
 ```
@@ -107,15 +85,15 @@
 ```
 
 To use ML Datastore:
 ```bash
 pip install "prefect-azure[ml_datastore]"
 ```
 
-A list of available blocks in `prefect-azure` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-azure/#blocks-catalog).
+## Examples
 
 ### Download a blob
 
 ```python
 from prefect import flow
 
 from prefect_azure import AzureBlobStorageCredentials
@@ -199,54 +177,23 @@
 Then, create the deployment either on the UI or through the CLI:
 ```bash
 prefect deployment build a_flow_module.py:log_hello_flow --name aci-dev -ib container-instance-job/aci-dev
 ```
 
 Visit [Prefect Deployments](https://docs.prefect.io/tutorials/deployments/) for more information about deployments.
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
-
 ## Azure Container Instance Worker
 The Azure Container Instance worker is an excellent way to run 
-[Prefect projects](https://docs.prefect.io/latest/concepts/projects/) on Azure. 
+your workflows on Azure. 
 
 To get started, create an Azure Container Instances typed work pool:
 ```
 prefect work-pool create -t azure-container-instance my-aci-work-pool
 ```
 
 Then, run a worker that pulls jobs from the work pool:
 ```
 prefect worker start -n my-aci-worker -p my-aci-work-pool
 ```
 
 The worker should automatically read the work pool's type and start an 
 Azure Container Instance worker.
-
-## Resources
-
-If you encounter and bugs while using `prefect-azure`, feel free to open an issue in the [prefect-azure](https://github.com/PrefectHQ/prefect-azure) repository.
-
-If you have any questions or issues while using `prefect-azure`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack)
-
-Feel free to star or watch [`prefect-azure`](https://github.com/PrefectHQ/prefect-azure) for updates too!
-
-## Contributing
-
-If you'd like to help contribute to fix an issue or add a feature to `prefect-azure`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-
-Here are the steps:
-
-1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
-2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
-3. Install the repository and its dependencies:
-```
-pip install -e ".[dev]"
-```
-4. Make desired changes
-5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-azure/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
-```
-pre-commit install
-```
-8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-azure-0.3.7/prefect_azure/__init__.py` & `prefect_azure-0.3.8/prefect_azure/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from . import _version
 from .credentials import (  # noqa
     AzureBlobStorageCredentials,
     AzureCosmosDbCredentials,
     AzureMlCredentials,
     AzureContainerInstanceCredentials,
 )
 from .workers.container_instance import AzureContainerWorker  # noqa
@@ -15,8 +14,11 @@
     "AzureMlCredentials",
     "AzureContainerInstanceCredentials",
     "AzureContainerInstanceJob",
     "AzureContainerWorker",
     "AzureBlobStorageContainer",
 ]
 
-__version__ = _version.get_versions()["version"]
+try:
+    from ._version import version as __version__
+except ImportError:
+    __version__ = "unknown"
```

### Comparing `prefect-azure-0.3.7/prefect_azure/blob_storage.py` & `prefect_azure-0.3.8/prefect_azure/blob_storage.py`

 * *Files 0% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 from typing import TYPE_CHECKING, Any, BinaryIO, Coroutine, Dict, List, Optional, Union
 
 from azure.core.exceptions import ResourceNotFoundError
 
 if TYPE_CHECKING:
     from azure.storage.blob import BlobProperties
 
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect import task
 from prefect.blocks.abstract import ObjectStorageBlock
 from prefect.filesystems import WritableDeploymentStorage, WritableFileSystem
 from prefect.logging import get_run_logger
 from prefect.utilities.asyncutils import sync_compatible
 from prefect.utilities.filesystem import filter_files
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field
 else:
     from pydantic import Field
 
 from prefect_azure.credentials import AzureBlobStorageCredentials
@@ -148,15 +149,15 @@
         blob_storage_credentials: Credentials to use for authentication with Azure.
         name_starts_with: Filters the results to return only blobs whose names
             begin with the specified prefix.
         include: Specifies one or more additional datasets to include in the response.
             Options include: 'snapshots', 'metadata', 'uncommittedblobs', 'copy',
             'deleted', 'deletedwithversions', 'tags', 'versions', 'immutabilitypolicy',
             'legalhold'.
-        **kwargs: Addtional kwargs passed to `ContainerClient.list_blobs()`
+        **kwargs: Additional kwargs passed to `ContainerClient.list_blobs()`
     Returns:
         A `list` of `dict`s containing metadata about the blob.
     Example:
         ```python
         from prefect import flow
 
         from prefect_azure import AzureBlobStorageCredentials
```

### Comparing `prefect-azure-0.3.7/prefect_azure/container_instance.py` & `prefect_azure-0.3.8/prefect_azure/container_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 """
-<span class="badge-api experimental"/>
 Integrations with the Azure Container Instances service.
 Note this module is experimental. The interfaces within may change without notice.
 
 The `AzureContainerInstanceJob` infrastructure block in this module is ideally
 configured via the Prefect UI and run via a Prefect agent, but it can be called directly
 as demonstrated in the following examples.
 
@@ -58,29 +57,29 @@
         image_registry=ACRManagedIdentity(
             registry_url="my-registry.azurecr.io",
             identity="/my/managed/identity/123abc"
         )
     )
     ```
 """
+
 import datetime
 import json
 import random
 import shlex
 import string
 import sys
 import time
 import uuid
 from copy import deepcopy
 from enum import Enum
 from typing import Dict, List, Optional, Union
 
 import anyio
 import dateutil.parser
-import prefect.infrastructure.container
 from anyio.abc import TaskStatus
 from azure.core.exceptions import HttpResponseError, ResourceNotFoundError
 from azure.core.polling import LROPoller
 from azure.mgmt.containerinstance import ContainerInstanceManagementClient
 from azure.mgmt.containerinstance.models import (
     Container,
     ContainerGroup,
@@ -93,20 +92,22 @@
     ImageRegistryCredential,
     Logs,
     OperatingSystemTypes,
     ResourceRequests,
     ResourceRequirements,
     UserAssignedIdentities,
 )
+from pydantic import VERSION as PYDANTIC_VERSION
+
+import prefect.infrastructure.container
 from prefect.blocks.core import BlockNotSavedError
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.infrastructure.base import Infrastructure, InfrastructureResult
 from prefect.utilities.asyncutils import run_sync_in_worker_thread, sync_compatible
 from prefect.utilities.dockerutils import get_prefect_image_name
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import BaseModel, Field, SecretStr
 else:
     from pydantic import BaseModel, Field, SecretStr
 
 from slugify import slugify
@@ -174,15 +175,14 @@
     """
     The result of an `AzureContainerInstanceJob` run.
     """
 
 
 class AzureContainerInstanceJob(Infrastructure):
     """
-    <span class="badge-api experimental"/>
     Run a command using a container on Azure Container Instances.
     Note this block is experimental. The interface may change without notice.
     """
 
     _block_type_name = "Azure Container Instance Job"
     _logo_url = "https://cdn.sanity.io/images/3ugk85nk/production/54e3fa7e00197a4fbd1d82ed62494cb58d08c96a-250x250.png"  # noqa
     _description = "Run tasks using Azure Container Instances. Note this block is experimental. The interface may change without notice."  # noqa
@@ -671,15 +671,15 @@
 
     @staticmethod
     def _create_image_registry_credentials(
         image_registry: Union[
             prefect.infrastructure.container.DockerRegistry,
             ACRManagedIdentity,
             None,
-        ]
+        ],
     ):
         """
         Create image registry credentials based on the type of image_registry provided.
 
         Args:
             image_registry: An instance of a DockerRegistry or
             ACRManagedIdentity object.
```

### Comparing `prefect-azure-0.3.7/prefect_azure/cosmos_db.py` & `prefect_azure-0.3.8/prefect_azure/cosmos_db.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,27 +6,26 @@
 from anyio import to_thread
 
 if TYPE_CHECKING:
     from azure.cosmos.database import ContainerProxy, DatabaseProxy
 
 from prefect import task
 from prefect.logging import get_run_logger
-
 from prefect_azure.credentials import AzureCosmosDbCredentials
 
 
 @task
 async def cosmos_db_query_items(
     query: str,
     container: Union[str, "ContainerProxy", Dict[str, Any]],
     database: Union[str, "DatabaseProxy", Dict[str, Any]],
     cosmos_db_credentials: AzureCosmosDbCredentials,
     parameters: Optional[List[Dict[str, object]]] = None,
     partition_key: Optional[Any] = None,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> List[Union[str, dict]]:
     """
     Return all results matching the given query.
 
     You can use any value for the container name in the FROM clause,
     but often the container name is used.
     In the examples below, the container name is "products,"
@@ -83,28 +82,28 @@
 
     container_client = cosmos_db_credentials.get_container_client(container, database)
     partial_query_items = partial(
         container_client.query_items,
         query,
         parameters=parameters,
         partition_key=partition_key,
-        **kwargs
+        **kwargs,
     )
     results = await to_thread.run_sync(partial_query_items)
     return results
 
 
 @task
 async def cosmos_db_read_item(
     item: Union[str, Dict[str, Any]],
     partition_key: Any,
     container: Union[str, "ContainerProxy", Dict[str, Any]],
     database: Union[str, "DatabaseProxy", Dict[str, Any]],
     cosmos_db_credentials: AzureCosmosDbCredentials,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> List[Union[str, dict]]:
     """
     Get the item identified by item.
 
     Args:
         item: The ID (name) or dict representing item to retrieve.
         partition_key: Partition key for the item to retrieve.
@@ -165,15 +164,15 @@
 
 @task
 async def cosmos_db_create_item(
     body: Dict[str, Any],
     container: Union[str, "ContainerProxy", Dict[str, Any]],
     database: Union[str, "DatabaseProxy", Dict[str, Any]],
     cosmos_db_credentials: AzureCosmosDbCredentials,
-    **kwargs: Any
+    **kwargs: Any,
 ) -> Dict[str, Any]:
     """
     Create an item in the container.
 
     To update or replace an existing item, use the upsert_item method.
 
     Args:
```

### Comparing `prefect-azure-0.3.7/prefect_azure/credentials.py` & `prefect_azure-0.3.8/prefect_azure/credentials.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,19 @@
         cls, values: Dict[str, Any]
     ) -> Dict[str, Any]:
         """
         Checks that either a connection string or account URL is provided, not both.
         """
         has_account_url = values.get("account_url") is not None
         has_conn_str = values.get("connection_string") is not None
-        if not bool(has_account_url ^ has_conn_str):
+        if not has_account_url and not has_conn_str:
+            raise ValueError(
+                "Must provide either a connection string or an account URL."
+            )
+        if has_account_url and has_conn_str:
             raise ValueError(
                 "Must provide either a connection string or account URL, but not both."
             )
         return values
 
     @_raise_help_msg("blob_storage")
     def get_client(self) -> "BlobServiceClient":
```

### Comparing `prefect-azure-0.3.7/prefect_azure/deployments/steps.py` & `prefect_azure-0.3.8/prefect_azure/deployments/steps.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,14 +34,15 @@
 For more information about using deployment steps, check out out the Prefect [docs](https://docs.prefect.io/latest/concepts/projects/#the-prefect-yaml-file).
 """  # noqa
 from pathlib import Path, PurePosixPath
 from typing import Dict, Optional
 
 from azure.identity import DefaultAzureCredential
 from azure.storage.blob import ContainerClient
+
 from prefect.utilities.filesystem import filter_files, relative_path_to_current_platform
 
 
 def push_to_azure_blob_storage(
     container: str,
     folder: str,
     credentials: Dict[str, str],
```

### Comparing `prefect-azure-0.3.7/prefect_azure/ml_datastore.py` & `prefect_azure-0.3.8/prefect_azure/ml_datastore.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import os
 from functools import partial
 from pathlib import Path
 from typing import TYPE_CHECKING, Dict, List, Union
 
 from anyio import to_thread
 from azureml.core.datastore import Datastore
+
 from prefect import get_run_logger, task
 
 if TYPE_CHECKING:
     from azureml.data.azure_storage_datastore import AzureBlobDatastore
     from azureml.data.data_reference import DataReference
 
     from prefect_azure.credentials import (
```

### Comparing `prefect-azure-0.3.7/prefect_azure/workers/container_instance.py` & `prefect_azure-0.3.8/prefect_azure/workers/container_instance.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,40 +72,41 @@
 import sys
 import time
 from enum import Enum
 from typing import Any, Dict, List, Optional, Union
 
 import anyio
 import dateutil.parser
-import prefect
 from azure.core.exceptions import HttpResponseError, ResourceNotFoundError
 from azure.core.polling import LROPoller
 from azure.mgmt.containerinstance import ContainerInstanceManagementClient
 from azure.mgmt.containerinstance.models import Container, ContainerGroup, Logs
 from azure.mgmt.resource import ResourceManagementClient
 from azure.mgmt.resource.resources.models import (
     Deployment,
     DeploymentExtended,
     DeploymentMode,
     DeploymentProperties,
 )
+from pydantic import VERSION as PYDANTIC_VERSION
+
+import prefect
 from prefect import get_client
 from prefect.client.schemas import FlowRun
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.server.schemas.core import Flow
 from prefect.server.schemas.responses import DeploymentResponse
 from prefect.utilities.asyncutils import run_sync_in_worker_thread
 from prefect.utilities.dockerutils import get_prefect_image_name
 from prefect.workers.base import (
     BaseJobConfiguration,
     BaseVariables,
     BaseWorker,
     BaseWorkerResult,
 )
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import Field, SecretStr
 else:
     from pydantic import Field, SecretStr
 
 from slugify import slugify
```

### Comparing `prefect-azure-0.3.7/prefect_azure.egg-info/PKG-INFO` & `prefect_azure-0.3.8/prefect_azure.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,97 +1,75 @@
 Metadata-Version: 2.1
 Name: prefect-azure
-Version: 0.3.7
+Version: 0.3.8
 Summary: Prefect integrations with Microsoft Azure services
-Home-page: https://github.com/PrefectHQ/prefect-azure
-Author: Prefect Technologies, Inc.
-Author-email: help@prefect.io
+Author-email: "Prefect Technologies, Inc." <help@prefect.io>
 License: Apache License 2.0
+Project-URL: Homepage, https://github.com/PrefectHQ/prefect/tree/main/src/integrations/prefect-azure
 Keywords: prefect
 Classifier: Natural Language :: English
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: prefect>=2.14.10
-Requires-Dist: azure_mgmt_containerinstance>=10.0
+Requires-Dist: aiohttp
 Requires-Dist: azure_identity>=1.10
+Requires-Dist: azure_mgmt_containerinstance>=10.0
 Requires-Dist: azure-mgmt-resource>=21.2
-Requires-Dist: aiohttp
+Requires-Dist: prefect>=2.14.10
 Provides-Extra: blob-storage
 Requires-Dist: azure-storage-blob; extra == "blob-storage"
 Provides-Extra: cosmos-db
 Requires-Dist: azure-cosmos; extra == "cosmos-db"
 Provides-Extra: ml-datastore
 Requires-Dist: azureml-core; extra == "ml-datastore"
 Provides-Extra: all-extras
 Requires-Dist: azure-cosmos; extra == "all-extras"
 Requires-Dist: azure-storage-blob; extra == "all-extras"
 Requires-Dist: azureml-core; extra == "all-extras"
 Provides-Extra: dev
-Requires-Dist: pytest; extra == "dev"
-Requires-Dist: black; extra == "dev"
-Requires-Dist: flake8; extra == "dev"
-Requires-Dist: mypy; extra == "dev"
-Requires-Dist: mkdocs; extra == "dev"
-Requires-Dist: mkdocs-material; extra == "dev"
-Requires-Dist: mkdocstrings[python]; extra == "dev"
-Requires-Dist: isort; extra == "dev"
-Requires-Dist: pre-commit; extra == "dev"
-Requires-Dist: pytest-asyncio; extra == "dev"
-Requires-Dist: mock; python_version < "3.8" and extra == "dev"
-Requires-Dist: mkdocs-gen-files; extra == "dev"
-Requires-Dist: interrogate; extra == "dev"
-Requires-Dist: coverage; extra == "dev"
 Requires-Dist: aiohttp; extra == "dev"
-Requires-Dist: pillow; extra == "dev"
 Requires-Dist: azure-cosmos; extra == "dev"
 Requires-Dist: azure-storage-blob; extra == "dev"
 Requires-Dist: azureml-core; extra == "dev"
+Requires-Dist: coverage; extra == "dev"
+Requires-Dist: interrogate; extra == "dev"
+Requires-Dist: mkdocs-gen-files; extra == "dev"
+Requires-Dist: mkdocs-material; extra == "dev"
+Requires-Dist: mkdocs; extra == "dev"
+Requires-Dist: mkdocstrings[python]; extra == "dev"
+Requires-Dist: mock; python_version < "3.8" and extra == "dev"
+Requires-Dist: mypy; extra == "dev"
+Requires-Dist: pillow; extra == "dev"
+Requires-Dist: pre-commit; extra == "dev"
+Requires-Dist: pytest-asyncio; extra == "dev"
+Requires-Dist: pytest; extra == "dev"
+Requires-Dist: pytest-xdist; extra == "dev"
 
 # prefect-azure
 
-Visit the full docs [here](https://PrefectHQ.github.io/prefect-azure) to see additional examples and the API reference.
-
 <p align="center">
     <a href="https://pypi.python.org/pypi/prefect-azure/" alt="PyPI version">
         <img alt="PyPI" src="https://img.shields.io/pypi/v/prefect-azure?color=26272B&labelColor=090422"></a>
-    <a href="https://github.com/PrefectHQ/prefect-azure/" alt="Stars">
-        <img src="https://img.shields.io/github/stars/PrefectHQ/prefect-azure?ccolor=26272B&labelColor=090422" /></a>
     <a href="https://pepy.tech/badge/prefect-azure/" alt="Downloads">
         <img src="https://img.shields.io/pypi/dm/prefect-azure?color=26272B&labelColor=090422" /></a>
-    <a href="https://github.com/PrefectHQ/prefect-azure/pulse" alt="Activity">
-        <img src="https://img.shields.io/github/commit-activity/m/PrefectHQ/prefect-azure?color=26272B&labelColor=090422" /></a>
-    <br>
-    <a href="https://prefect-community.slack.com" alt="Slack">
-        <img src="https://img.shields.io/badge/slack-join_community-red.svg?color=26272B&labelColor=090422&logo=slack" /></a>
 </p>
 
-## Welcome!
-
-prefect-azure is a collection of prebuilt Prefect tasks that can be used to quickly construct Prefect flows.
+`prefect-azure` is a collection of Prefect integrations for orchestration workflows with Azure.
 
 ## Getting Started
 
-### Python setup
-
-Requires an installation of Python 3.8+
-
-We recommend using a Python virtual environment manager such as pipenv, conda or virtualenv.
-
-These tasks are designed to work with Prefect 2. For more information about how to use Prefect, please refer to the [Prefect documentation](https://docs.prefect.io/).
-
 ### Installation
 
 Install `prefect-azure` with `pip`
 
 ```bash
 pip install prefect-azure
 ```
@@ -107,15 +85,15 @@
 ```
 
 To use ML Datastore:
 ```bash
 pip install "prefect-azure[ml_datastore]"
 ```
 
-A list of available blocks in `prefect-azure` and their setup instructions can be found [here](https://PrefectHQ.github.io/prefect-azure/#blocks-catalog).
+## Examples
 
 ### Download a blob
 
 ```python
 from prefect import flow
 
 from prefect_azure import AzureBlobStorageCredentials
@@ -199,54 +177,23 @@
 Then, create the deployment either on the UI or through the CLI:
 ```bash
 prefect deployment build a_flow_module.py:log_hello_flow --name aci-dev -ib container-instance-job/aci-dev
 ```
 
 Visit [Prefect Deployments](https://docs.prefect.io/tutorials/deployments/) for more information about deployments.
 
-For more tips on how to use tasks and flows in a Collection, check out [Using Collections](https://orion-docs.prefect.io/collections/usage/)!
-
 ## Azure Container Instance Worker
 The Azure Container Instance worker is an excellent way to run 
-[Prefect projects](https://docs.prefect.io/latest/concepts/projects/) on Azure. 
+your workflows on Azure. 
 
 To get started, create an Azure Container Instances typed work pool:
 ```
 prefect work-pool create -t azure-container-instance my-aci-work-pool
 ```
 
 Then, run a worker that pulls jobs from the work pool:
 ```
 prefect worker start -n my-aci-worker -p my-aci-work-pool
 ```
 
 The worker should automatically read the work pool's type and start an 
 Azure Container Instance worker.
-
-## Resources
-
-If you encounter and bugs while using `prefect-azure`, feel free to open an issue in the [prefect-azure](https://github.com/PrefectHQ/prefect-azure) repository.
-
-If you have any questions or issues while using `prefect-azure`, you can find help in either the [Prefect Discourse forum](https://discourse.prefect.io/) or the [Prefect Slack community](https://prefect.io/slack)
-
-Feel free to star or watch [`prefect-azure`](https://github.com/PrefectHQ/prefect-azure) for updates too!
-
-## Contributing
-
-If you'd like to help contribute to fix an issue or add a feature to `prefect-azure`, please [propose changes through a pull request from a fork of the repository](https://docs.github.com/en/pull-requests/collaborating-with-pull-requests/proposing-changes-to-your-work-with-pull-requests/creating-a-pull-request-from-a-fork).
-
-Here are the steps:
-
-1. [Fork the repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#forking-a-repository)
-2. [Clone the forked repository](https://docs.github.com/en/get-started/quickstart/fork-a-repo#cloning-your-forked-repository)
-3. Install the repository and its dependencies:
-```
-pip install -e ".[dev]"
-```
-4. Make desired changes
-5. Add tests
-6. Insert an entry to [CHANGELOG.md](https://github.com/PrefectHQ/prefect-azure/blob/main/CHANGELOG.md)
-7. Install `pre-commit` to perform quality checks prior to commit:
-```
-pre-commit install
-```
-8. `git commit`, `git push`, and create a pull request
```

### Comparing `prefect-azure-0.3.7/tests/test_aci_infrastructure.py` & `prefect_azure-0.3.8/tests/test_aci_infrastructure.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,20 +11,20 @@
 from azure.identity import ClientSecretCredential, DefaultAzureCredential
 from azure.mgmt.containerinstance.models import (
     EnvironmentVariable,
     ImageRegistryCredential,
     UserAssignedIdentities,
 )
 from azure.mgmt.resource import ResourceManagementClient
+from prefect_azure.workers.container_instance import AzureContainerWorker
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.exceptions import InfrastructureNotAvailable, InfrastructureNotFound
 from prefect.infrastructure.container import DockerRegistry
 from prefect.settings import get_current_settings
-from pydantic import VERSION as PYDANTIC_VERSION
-
-from prefect_azure.workers.container_instance import AzureContainerWorker
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import SecretStr
 else:
     from pydantic import SecretStr
 
 import prefect_azure.container_instance
@@ -780,15 +780,15 @@
 
 
 async def test_kill_raises_not_found_when_container_group_gone(
     container_instance_block, mock_aci_client
 ):
     mock_aci_client.container_groups.get.side_effect = ResourceNotFoundError()
 
-    # ResourceNotFoundError means the container group no longers exists on Azure, so
+    # ResourceNotFoundError means the container group no longer exists on Azure, so
     # it should always cause an InfrastructureNotFound exception
     with pytest.raises(InfrastructureNotFound):
         await container_instance_block.kill("test_container_group")
 
 
 async def test_kill_raises_not_available_when_container_terminated(
     container_instance_block, mock_aci_client
```

### Comparing `prefect-azure-0.3.7/tests/test_aci_worker.py` & `prefect_azure-0.3.8/tests/test_aci_worker.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,34 +5,35 @@
 
 import dateutil.parser
 import pytest
 from anyio.abc import TaskStatus
 from azure.core.exceptions import HttpResponseError, ResourceNotFoundError
 from azure.identity import ClientSecretCredential
 from azure.mgmt.resource import ResourceManagementClient
+from pydantic import VERSION as PYDANTIC_VERSION
+
 from prefect.client.schemas import FlowRun
 from prefect.exceptions import InfrastructureNotFound
 from prefect.infrastructure.container import DockerRegistry
 from prefect.server.schemas.core import Flow
 from prefect.settings import get_current_settings
 from prefect.testing.utilities import AsyncMock
 from prefect.utilities.dockerutils import get_prefect_image_name
-from pydantic import VERSION as PYDANTIC_VERSION
 
 if PYDANTIC_VERSION.startswith("2."):
     from pydantic.v1 import SecretStr
 else:
     from pydantic import SecretStr
 
 import prefect_azure.container_instance
 from prefect_azure import AzureContainerInstanceCredentials
 from prefect_azure.container_instance import ACRManagedIdentity
-from prefect_azure.workers.container_instance import AzureContainerVariables  # noqa
 from prefect_azure.workers.container_instance import (
     AzureContainerJobConfiguration,
+    AzureContainerVariables,  # noqa
     AzureContainerWorker,
     AzureContainerWorkerResult,
     ContainerGroupProvisioningState,
     ContainerRunState,
 )
 
 
@@ -951,15 +952,15 @@
     assert config.memory == 1
     assert config.env == {"TEST": "VALUE"}
     assert config.resource_group_name == "my-resource-group"
     assert config.subscription_id.get_secret_value() == "my-subscription-id"
     assert config.aci_credentials.tenant_id == "my-tenant-id"
     assert config.aci_credentials.client_id == "my-client-id"
     assert config.aci_credentials.client_secret.get_secret_value() == "my-client-secret"
-    assert type(config.arm_template) == dict
+    assert isinstance(config.arm_template, dict)
 
 
 async def test_image_populated_in_template_when_not_provided(worker_flow_run):
     config = await AzureContainerJobConfiguration.from_template_and_values(
         base_job_template=AzureContainerWorker.get_default_base_job_template(),
         values=AzureContainerVariables(
             subscription_id="my-subscription-id",
```

### Comparing `prefect-azure-0.3.7/tests/test_blob_storage.py` & `prefect_azure-0.3.8/tests/test_blob_storage.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 import uuid
 from io import BytesIO
 from pathlib import Path
 
 import pytest
 from azure.core.exceptions import ResourceExistsError
-from prefect import flow
-
 from prefect_azure.blob_storage import (
     AzureBlobStorageContainer,
     blob_storage_download,
     blob_storage_list,
     blob_storage_upload,
 )
 
+from prefect import flow
+
 
 async def test_blob_storage_download_flow(blob_storage_credentials):
     @flow
     async def blob_storage_download_flow():
         return await blob_storage_download(
             container="prefect",
             blob="prefect.txt",
```

### Comparing `prefect-azure-0.3.7/tests/test_block_standards.py` & `prefect_azure-0.3.8/tests/test_block_standards.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import pytest
+
 from prefect.blocks.core import Block
 from prefect.testing.standard_test_suites import BlockStandardTestSuite
 from prefect.utilities.dispatch import get_registry_for_type
 from prefect.utilities.importtools import to_qualified_name
 
 
 def find_module_blocks():
```

### Comparing `prefect-azure-0.3.7/tests/test_cosmos_db.py` & `prefect_azure-0.3.8/tests/test_cosmos_db.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from prefect import flow
-
 from prefect_azure.cosmos_db import (
     cosmos_db_create_item,
     cosmos_db_query_items,
     cosmos_db_read_item,
 )
 
+from prefect import flow
+
 
 async def test_cosmos_db_query_items_flow(cosmos_db_credentials):
     @flow
     async def cosmos_db_query_items_flow():
         query = "SELECT * FROM c where c.age >= @age"
         container = "Persons"
         database = "SampleDB"
```

### Comparing `prefect-azure-0.3.7/tests/test_credentials.py` & `prefect_azure-0.3.8/tests/test_credentials.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from unittest.mock import MagicMock
 
 import pytest
 from azure.storage.blob import BlobClient, BlobServiceClient, ContainerClient
 from conftest import CosmosClientMock
-from prefect import flow
-
 from prefect_azure.credentials import (
     AzureBlobStorageCredentials,
     AzureCosmosDbCredentials,
     AzureMlCredentials,
 )
 
+from prefect import flow
+
 
 def test_get_service_client(blob_connection_string):
     @flow
     def test_flow():
         client = AzureBlobStorageCredentials(
             connection_string=blob_connection_string
         ).get_client()
```

### Comparing `prefect-azure-0.3.7/tests/test_ml_datastore.py` & `prefect_azure-0.3.8/tests/test_ml_datastore.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-from prefect import flow
-
 from prefect_azure.ml_datastore import (
     ml_get_datastore,
     ml_list_datastores,
     ml_register_datastore_blob_container,
     ml_upload_datastore,
 )
 
+from prefect import flow
+
 
 def test_ml_list_datastores_flow(ml_credentials):
     @flow
     def ml_list_datastores_flow():
         results = ml_list_datastores(ml_credentials)
         return results
```

