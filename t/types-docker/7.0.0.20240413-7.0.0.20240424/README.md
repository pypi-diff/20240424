# Comparing `tmp/types-docker-7.0.0.20240413.tar.gz` & `tmp/types-docker-7.0.0.20240424.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "types-docker-7.0.0.20240413.tar", last modified: Sat Apr 13 02:07:04 2024, max compression
+gzip compressed data, was "types-docker-7.0.0.20240424.tar", last modified: Wed Apr 24 02:17:53 2024, max compression
```

## Comparing `types-docker-7.0.0.20240413.tar` & `types-docker-7.0.0.20240424.tar`

### file list

```diff
@@ -1,88 +1,88 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.526066 types-docker-7.0.0.20240413/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-13 02:07:03.000000 types-docker-7.0.0.20240413/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-13 02:07:03.000000 types-docker-7.0.0.20240413/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-13 02:07:04.526066 types-docker-7.0.0.20240413/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.518066 types-docker-7.0.0.20240413/docker-stubs/
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-13 02:07:03.000000 types-docker-7.0.0.20240413/docker-stubs/METADATA.toml
--rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/__init__.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.522066 types-docker-7.0.0.20240413/docker-stubs/api/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/container.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/exec_api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/image.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/network.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/plugin.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/secret.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/service.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/api/volume.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/auth.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/constants.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.522066 types-docker-7.0.0.20240413/docker-stubs/context/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/context/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/context/api.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/context/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/context/context.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.522066 types-docker-7.0.0.20240413/docker-stubs/credentials/
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/credentials/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/credentials/constants.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/credentials/errors.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/credentials/store.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/credentials/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/errors.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.522066 types-docker-7.0.0.20240413/docker-stubs/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/configs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/images.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/nodes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/plugins.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/resource.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/secrets.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/swarm.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/models/volumes.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:03.000000 types-docker-7.0.0.20240413/docker-stubs/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/tls.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.526066 types-docker-7.0.0.20240413/docker-stubs/transport/
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/transport/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/transport/basehttpadapter.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/transport/npipeconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/transport/npipesocket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/transport/sshconn.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/transport/unixconn.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.526066 types-docker-7.0.0.20240413/docker-stubs/types/
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/base.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/containers.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/daemon.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/healthcheck.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/networks.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/services.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/types/swarm.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.526066 types-docker-7.0.0.20240413/docker-stubs/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/build.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/config.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/decorators.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/fnmatch.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/json_stream.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/ports.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/proxy.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/socket.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/utils/utils.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-13 02:06:51.000000 types-docker-7.0.0.20240413/docker-stubs/version.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-13 02:07:04.526066 types-docker-7.0.0.20240413/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-13 02:07:03.000000 types-docker-7.0.0.20240413/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-13 02:07:04.526066 types-docker-7.0.0.20240413/types_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-13 02:07:04.000000 types-docker-7.0.0.20240413/types_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-13 02:07:04.000000 types-docker-7.0.0.20240413/types_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-13 02:07:04.000000 types-docker-7.0.0.20240413/types_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-13 02:07:04.000000 types-docker-7.0.0.20240413/types_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-13 02:07:04.000000 types-docker-7.0.0.20240413/types_docker.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.338317 types-docker-7.0.0.20240424/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-24 02:17:52.000000 types-docker-7.0.0.20240424/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-24 02:17:52.000000 types-docker-7.0.0.20240424/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-24 02:17:53.338317 types-docker-7.0.0.20240424/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.330317 types-docker-7.0.0.20240424/docker-stubs/
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-24 02:17:52.000000 types-docker-7.0.0.20240424/docker-stubs/METADATA.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      281 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/__init__.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.330317 types-docker-7.0.0.20240424/docker-stubs/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1794 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1607 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      310 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4660 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/container.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/exec_api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2359 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/image.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1422 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/network.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      651 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/plugin.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/secret.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/service.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1431 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      513 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/api/volume.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1444 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/auth.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      760 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/constants.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.334317 types-docker-7.0.0.20240424/docker-stubs/context/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/context/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/context/api.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/context/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/context/context.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.334317 types-docker-7.0.0.20240424/docker-stubs/credentials/
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/credentials/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/credentials/constants.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/credentials/errors.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/credentials/store.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/credentials/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2206 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/errors.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.334317 types-docker-7.0.0.20240424/docker-stubs/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/configs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/images.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      337 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/nodes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/plugins.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/resource.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/secrets.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/swarm.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/models/volumes.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:52.000000 types-docker-7.0.0.20240424/docker-stubs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/tls.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.334317 types-docker-7.0.0.20240424/docker-stubs/transport/
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/transport/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      113 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/transport/basehttpadapter.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/transport/npipeconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1757 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/transport/npipesocket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1678 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/transport/sshconn.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/transport/unixconn.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.338317 types-docker-7.0.0.20240424/docker-stubs/types/
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      177 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/base.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5853 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/containers.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      188 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/daemon.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/healthcheck.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/networks.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     5699 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/services.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/types/swarm.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.338317 types-docker-7.0.0.20240424/docker-stubs/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/build.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/config.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/decorators.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/fnmatch.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      403 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/json_stream.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/ports.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1036 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/proxy.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/socket.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/utils/utils.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 02:17:28.000000 types-docker-7.0.0.20240424/docker-stubs/version.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 02:17:53.338317 types-docker-7.0.0.20240424/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3354 2024-04-24 02:17:52.000000 types-docker-7.0.0.20240424/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 02:17:53.338317 types-docker-7.0.0.20240424/types_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-24 02:17:53.000000 types-docker-7.0.0.20240424/types_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-24 02:17:53.000000 types-docker-7.0.0.20240424/types_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 02:17:53.000000 types-docker-7.0.0.20240424/types_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-24 02:17:53.000000 types-docker-7.0.0.20240424/types_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-24 02:17:53.000000 types-docker-7.0.0.20240424/types_docker.egg-info/top_level.txt
```

### Comparing `types-docker-7.0.0.20240413/PKG-INFO` & `types-docker-7.0.0.20240424/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240413
+Version: 7.0.0.20240424
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b61d90c6f5dc4600055916f98c0e63deec0546e9` and was tested
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/build.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/service.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,47 @@
 from _typeshed import Incomplete
 
-log: Incomplete
-
-class BuildApiMixin:
-    def build(
+class ServiceApiMixin:
+    def create_service(
         self,
-        path: Incomplete | None = None,
-        tag: str | None = None,
-        quiet: bool = False,
-        fileobj: Incomplete | None = None,
-        nocache: bool = False,
-        rm: bool = False,
-        timeout: Incomplete | None = None,
-        custom_context: bool = False,
-        encoding: Incomplete | None = None,
-        pull: bool = False,
-        forcerm: bool = False,
-        dockerfile: Incomplete | None = None,
-        container_limits: Incomplete | None = None,
-        decode: bool = False,
-        buildargs: Incomplete | None = None,
-        gzip: bool = False,
-        shmsize: Incomplete | None = None,
+        task_template,
+        name: Incomplete | None = None,
         labels: Incomplete | None = None,
-        cache_from: Incomplete | None = None,
-        target: Incomplete | None = None,
-        network_mode: Incomplete | None = None,
-        squash: Incomplete | None = None,
-        extra_hosts: Incomplete | None = None,
-        platform: Incomplete | None = None,
-        isolation: Incomplete | None = None,
-        use_config_proxy: bool = True,
+        mode: Incomplete | None = None,
+        update_config: Incomplete | None = None,
+        networks: Incomplete | None = None,
+        endpoint_config: Incomplete | None = None,
+        endpoint_spec: Incomplete | None = None,
+        rollback_config: Incomplete | None = None,
     ): ...
-    def prune_builds(
-        self, filters: Incomplete | None = None, keep_storage: Incomplete | None = None, all: Incomplete | None = None
+    def inspect_service(self, service, insert_defaults: Incomplete | None = None): ...
+    def inspect_task(self, task): ...
+    def remove_service(self, service): ...
+    def services(self, filters: Incomplete | None = None, status: Incomplete | None = None): ...
+    def service_logs(
+        self,
+        service,
+        details: bool = False,
+        follow: bool = False,
+        stdout: bool = False,
+        stderr: bool = False,
+        since: int = 0,
+        timestamps: bool = False,
+        tail: str = "all",
+        is_tty: Incomplete | None = None,
+    ): ...
+    def tasks(self, filters: Incomplete | None = None): ...
+    def update_service(
+        self,
+        service,
+        version,
+        task_template: Incomplete | None = None,
+        name: Incomplete | None = None,
+        labels: Incomplete | None = None,
+        mode: Incomplete | None = None,
+        update_config: Incomplete | None = None,
+        networks: Incomplete | None = None,
+        endpoint_config: Incomplete | None = None,
+        endpoint_spec: Incomplete | None = None,
+        fetch_current_spec: bool = False,
+        rollback_config: Incomplete | None = None,
     ): ...
-
-def process_dockerfile(dockerfile, path): ...
```

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/client.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/container.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/container.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/daemon.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/daemon.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/exec_api.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/exec_api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/image.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/image.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/network.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/network.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/plugin.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/plugin.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/service.pyi` & `types-docker-7.0.0.20240424/docker-stubs/types/networks.pyi`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,31 @@
 from _typeshed import Incomplete
 
-class ServiceApiMixin:
-    def create_service(
+class EndpointConfig(dict[str, Incomplete]):
+    def __init__(
         self,
-        task_template,
-        name: Incomplete | None = None,
-        labels: Incomplete | None = None,
-        mode: Incomplete | None = None,
-        update_config: Incomplete | None = None,
-        networks: Incomplete | None = None,
-        endpoint_config: Incomplete | None = None,
-        endpoint_spec: Incomplete | None = None,
-        rollback_config: Incomplete | None = None,
-    ): ...
-    def inspect_service(self, service, insert_defaults: Incomplete | None = None): ...
-    def inspect_task(self, task): ...
-    def remove_service(self, service): ...
-    def services(self, filters: Incomplete | None = None, status: Incomplete | None = None): ...
-    def service_logs(
-        self,
-        service,
-        details: bool = False,
-        follow: bool = False,
-        stdout: bool = False,
-        stderr: bool = False,
-        since: int = 0,
-        timestamps: bool = False,
-        tail: str = "all",
-        is_tty: Incomplete | None = None,
-    ): ...
-    def tasks(self, filters: Incomplete | None = None): ...
-    def update_service(
-        self,
-        service,
         version,
-        task_template: Incomplete | None = None,
-        name: Incomplete | None = None,
-        labels: Incomplete | None = None,
-        mode: Incomplete | None = None,
-        update_config: Incomplete | None = None,
-        networks: Incomplete | None = None,
-        endpoint_config: Incomplete | None = None,
-        endpoint_spec: Incomplete | None = None,
-        fetch_current_spec: bool = False,
-        rollback_config: Incomplete | None = None,
-    ): ...
+        aliases: Incomplete | None = None,
+        links: Incomplete | None = None,
+        ipv4_address: Incomplete | None = None,
+        ipv6_address: Incomplete | None = None,
+        link_local_ips: Incomplete | None = None,
+        driver_opt: Incomplete | None = None,
+        mac_address: Incomplete | None = None,
+    ) -> None: ...
+
+class NetworkingConfig(dict[str, Incomplete]):
+    def __init__(self, endpoints_config: Incomplete | None = None) -> None: ...
+
+class IPAMConfig(dict[str, Incomplete]):
+    def __init__(
+        self, driver: str = "default", pool_configs: Incomplete | None = None, options: Incomplete | None = None
+    ) -> None: ...
+
+class IPAMPool(dict[str, Incomplete]):
+    def __init__(
+        self,
+        subnet: Incomplete | None = None,
+        iprange: Incomplete | None = None,
+        gateway: Incomplete | None = None,
+        aux_addresses: Incomplete | None = None,
+    ) -> None: ...
```

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/swarm.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/api/volume.pyi` & `types-docker-7.0.0.20240424/docker-stubs/api/volume.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/auth.pyi` & `types-docker-7.0.0.20240424/docker-stubs/auth.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/client.pyi` & `types-docker-7.0.0.20240424/docker-stubs/client.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/constants.pyi` & `types-docker-7.0.0.20240424/docker-stubs/constants.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/context/api.pyi` & `types-docker-7.0.0.20240424/docker-stubs/context/api.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/context/context.pyi` & `types-docker-7.0.0.20240424/docker-stubs/context/context.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/errors.pyi` & `types-docker-7.0.0.20240424/docker-stubs/errors.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/models/containers.pyi` & `types-docker-7.0.0.20240424/docker-stubs/models/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/models/images.pyi` & `types-docker-7.0.0.20240424/docker-stubs/models/images.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/models/networks.pyi` & `types-docker-7.0.0.20240424/docker-stubs/models/networks.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/models/plugins.pyi` & `types-docker-7.0.0.20240424/docker-stubs/models/plugins.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/models/resource.pyi` & `types-docker-7.0.0.20240424/docker-stubs/models/resource.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/models/services.pyi` & `types-docker-7.0.0.20240424/docker-stubs/models/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/models/swarm.pyi` & `types-docker-7.0.0.20240424/docker-stubs/models/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/transport/npipeconn.pyi` & `types-docker-7.0.0.20240424/docker-stubs/transport/npipeconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/transport/npipesocket.pyi` & `types-docker-7.0.0.20240424/docker-stubs/transport/npipesocket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/transport/sshconn.pyi` & `types-docker-7.0.0.20240424/docker-stubs/transport/sshconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/transport/unixconn.pyi` & `types-docker-7.0.0.20240424/docker-stubs/transport/unixconn.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/types/__init__.pyi` & `types-docker-7.0.0.20240424/docker-stubs/types/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/types/containers.pyi` & `types-docker-7.0.0.20240424/docker-stubs/types/containers.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/types/healthcheck.pyi` & `types-docker-7.0.0.20240424/docker-stubs/types/healthcheck.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/types/services.pyi` & `types-docker-7.0.0.20240424/docker-stubs/types/services.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/types/swarm.pyi` & `types-docker-7.0.0.20240424/docker-stubs/types/swarm.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/utils/__init__.pyi` & `types-docker-7.0.0.20240424/docker-stubs/utils/__init__.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/utils/build.pyi` & `types-docker-7.0.0.20240424/docker-stubs/utils/build.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/utils/proxy.pyi` & `types-docker-7.0.0.20240424/docker-stubs/utils/proxy.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/utils/socket.pyi` & `types-docker-7.0.0.20240424/docker-stubs/utils/socket.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/docker-stubs/utils/utils.pyi` & `types-docker-7.0.0.20240424/docker-stubs/utils/utils.pyi`

 * *Files identical despite different names*

### Comparing `types-docker-7.0.0.20240413/setup.py` & `types-docker-7.0.0.20240424/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,21 +17,21 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b61d90c6f5dc4600055916f98c0e63deec0546e9` and was tested
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
 '''.lstrip()
 
 setup(name=name,
-      version="7.0.0.20240413",
+      version="7.0.0.20240424",
       description=description,
       long_description=long_description,
       long_description_content_type="text/markdown",
       url="https://github.com/python/typeshed",
       project_urls={
           "GitHub": "https://github.com/python/typeshed",
           "Changes": "https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md",
```

### Comparing `types-docker-7.0.0.20240413/types_docker.egg-info/PKG-INFO` & `types-docker-7.0.0.20240424/types_docker.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: types-docker
-Version: 7.0.0.20240413
+Version: 7.0.0.20240424
 Summary: Typing stubs for docker
 Home-page: https://github.com/python/typeshed
 License: Apache-2.0 license
 Project-URL: GitHub, https://github.com/python/typeshed
 Project-URL: Changes, https://github.com/typeshed-internal/stub_uploader/blob/main/data/changelogs/docker.md
 Project-URL: Issue tracker, https://github.com/python/typeshed/issues
 Project-URL: Chat, https://gitter.im/python/typing
@@ -28,10 +28,10 @@
 This version of `types-docker` aims to provide accurate annotations
 for `docker==7.0.*`.
 The source for this package can be found at
 https://github.com/python/typeshed/tree/main/stubs/docker. All fixes for
 types and metadata should be contributed there.
 
 See https://github.com/python/typeshed/blob/main/README.md for more details.
-This package was generated from typeshed commit `b61d90c6f5dc4600055916f98c0e63deec0546e9` and was tested
+This package was generated from typeshed commit `7ed91bc2e77ec18d28307dc6086a778ecc9c7bb3` and was tested
 with mypy 1.9.0, pyright 1.1.358, and
 pytype 2024.4.11.
```

### Comparing `types-docker-7.0.0.20240413/types_docker.egg-info/SOURCES.txt` & `types-docker-7.0.0.20240424/types_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

