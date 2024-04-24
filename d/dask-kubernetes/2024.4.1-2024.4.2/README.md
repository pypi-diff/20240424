# Comparing `tmp/dask-kubernetes-2024.4.1.tar.gz` & `tmp/dask-kubernetes-2024.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-kubernetes-2024.4.1.tar", last modified: Fri Apr 19 12:37:21 2024, max compression
+gzip compressed data, was "dask-kubernetes-2024.4.2.tar", last modified: Wed Apr 24 14:36:05 2024, max compression
```

## Comparing `dask-kubernetes-2024.4.1.tar` & `dask-kubernetes-2024.4.2.tar`

### file list

```diff
@@ -1,110 +1,110 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/
--rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/dask_kubernetes/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/classic/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/config-demo.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/fake_gcp_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    28464 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_async.py
--rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_sync.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/cli/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/cli/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes/common/
--rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/networking.py
--rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_kind.py
--rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_objects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/experimental/
--rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/experimental/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/helm/
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/helmcluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/resources/values.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/test_helm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/kubernetes.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/
--rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/_objects.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/noop/
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/noop/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/plugins/noop/noop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.285413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/
--rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)    30973 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/test_controller.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/
--rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/templates.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.277413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   283847 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   471240 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
--rw-r--r--   0 runner    (1001) docker     (127)   140704 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/kubecluster.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.289413 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
--rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/dask_kubernetes/operator/networking.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 12:37:21.281413 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-19 12:37:21.000000 dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-19 12:37:21.293413 dask-kubernetes-2024.4.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-19 12:37:14.000000 dask-kubernetes-2024.4.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1549 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.074747 dask-kubernetes-2024.4.2/dask_kubernetes/
+-rw-r--r--   0 runner    (1001) docker     (127)      694 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      500 2024-04-24 14:36:05.090747 dask-kubernetes-2024.4.2/dask_kubernetes/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/classic/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28855 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      758 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/config-demo.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/fake_gcp_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28464 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/test_async.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15181 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/test_sync.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3001 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/cli/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    16674 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8085 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/networking.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13351 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/test_kind.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2726 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/test_objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      294 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4231 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      379 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/experimental/
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/experimental/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12442 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/helmcluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)      385 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/resources/values.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6527 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/test_helm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3016 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/kubernetes.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      130 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4786 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/_objects.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30117 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.078748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/noop/
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/noop/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/plugins/noop/noop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     2213 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2327 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2567 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)    30973 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/test_controller.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/
+-rw-r--r--   0 runner    (1001) docker     (127)        3 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskautoscaler.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1059 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1828 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2096 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskworkergroup.patch.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/templates.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.070747 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.082748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/Chart.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   283847 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   471240 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)   140704 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      529 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2452 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/rolebinding.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      354 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/serviceaccount.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1453 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4177 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37802 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/kubecluster.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7698 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7940 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/dask_kubernetes/operator/networking.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 14:36:05.074747 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4189 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-24 14:36:05.000000 dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      142 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1371 2024-04-24 14:36:05.086748 dask-kubernetes-2024.4.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1033 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86677 2024-04-24 14:36:00.000000 dask-kubernetes-2024.4.2/versioneer.py
```

### Comparing `dask-kubernetes-2024.4.1/LICENSE` & `dask-kubernetes-2024.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/PKG-INFO` & `dask-kubernetes-2024.4.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2024.4.1/README.rst` & `dask-kubernetes-2024.4.2/README.rst`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/__init__.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/classic/kubecluster.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/classic/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/config-demo.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/config-demo.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_async.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/test_async.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/classic/tests/test_sync.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/classic/tests/test_sync.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/cli/cli.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/cli/cli.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/common/auth.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/common/auth.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/common/networking.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/common/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/common/objects.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/common/objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_kind.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/test_kind.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/common/tests/test_objects.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/common/tests/test_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/common/utils.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/common/utils.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/conftest.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/conftest.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/experimental/__init__.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/experimental/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/helm/helmcluster.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/helm/helmcluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/helm/tests/test_helm.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/helm/tests/test_helm.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/kubernetes.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/kubernetes.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/_objects.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/_objects.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/controller.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/controller.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/failedjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplecluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simplejob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/resources/simpleworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/controller/tests/test_controller.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/controller/tests/test_controller.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskautoscaler.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.patch.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskcluster.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.patch.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.patch.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskjob.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/daskworkergroup.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/customresources/templates.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/customresources/templates.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/chartpress.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/chartpress.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskautoscaler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskcluster.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskjob.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/crds/daskworkergroup.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrole.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/clusterrolebinding.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/deployment.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/podmonitor-workers.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/role.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/templates/servicemonitor-scheduler.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/deployment/helm/dask-kubernetes-operator/values.yaml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/kubecluster.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_discovery.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/kubecluster/tests/test_kubecluster.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes/operator/networking.py` & `dask-kubernetes-2024.4.2/dask_kubernetes/operator/networking.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/PKG-INFO` & `dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask-kubernetes
-Version: 2024.4.1
+Version: 2024.4.2
 Summary: Native Kubernetes integration for Dask
 Home-page: https://github.com/dask/dask-kubernetes
 Maintainer: Jacob Tomlinson
 License: BSD
 Keywords: dask,kubernetes,distributed
 Requires-Python: >=3.9
 License-File: LICENSE
```

### Comparing `dask-kubernetes-2024.4.1/dask_kubernetes.egg-info/SOURCES.txt` & `dask-kubernetes-2024.4.2/dask_kubernetes.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/pyproject.toml` & `dask-kubernetes-2024.4.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/setup.cfg` & `dask-kubernetes-2024.4.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/setup.py` & `dask-kubernetes-2024.4.2/setup.py`

 * *Files identical despite different names*

### Comparing `dask-kubernetes-2024.4.1/versioneer.py` & `dask-kubernetes-2024.4.2/versioneer.py`

 * *Files identical despite different names*

