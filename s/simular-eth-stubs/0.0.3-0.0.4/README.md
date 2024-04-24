# Comparing `tmp/simular-eth-stubs-0.0.3.tar.gz` & `tmp/simular-eth-stubs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simular-eth-stubs-0.0.3.tar", last modified: Wed Apr 24 02:31:18 2024, max compression
+gzip compressed data, was "simular-eth-stubs-0.0.4.tar", last modified: Wed Apr 24 02:35:36 2024, max compression
```

## Comparing `simular-eth-stubs-0.0.3.tar` & `simular-eth-stubs-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 02:31:18.720000 simular-eth-stubs-0.0.3/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      404 2024-04-24 02:31:18.720000 simular-eth-stubs-0.0.3/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      142 2024-04-24 02:25:41.000000 simular-eth-stubs-0.0.3/README.md
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-24 02:31:18.720000 simular-eth-stubs-0.0.3/setup.cfg
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      464 2024-04-24 02:26:30.000000 simular-eth-stubs-0.0.3/setup.py
-drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 02:31:18.720000 simular-eth-stubs-0.0.3/simular_eth_stubs.egg-info/
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      404 2024-04-24 02:31:18.000000 simular-eth-stubs-0.0.3/simular_eth_stubs.egg-info/PKG-INFO
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)      222 2024-04-24 02:31:18.000000 simular-eth-stubs-0.0.3/simular_eth_stubs.egg-info/SOURCES.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-24 02:31:18.000000 simular-eth-stubs-0.0.3/simular_eth_stubs.egg-info/dependency_links.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       12 2024-04-24 02:31:18.000000 simular-eth-stubs-0.0.3/simular_eth_stubs.egg-info/requires.txt
--rwxr-xr-x   0 cpi       (1001) cpi       (1001)       14 2024-04-24 02:31:18.000000 simular-eth-stubs-0.0.3/simular_eth_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5314 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     3980 2024-04-24 02:33:35.000000 simular-eth-stubs-0.0.4/README.md
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       38 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/setup.cfg
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      464 2024-04-24 02:34:24.000000 simular-eth-stubs-0.0.4/setup.py
+drwxr-xr-x   0 cpi       (1001) cpi       (1001)        0 2024-04-24 02:35:36.210000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)     5314 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/PKG-INFO
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)      222 2024-04-24 02:35:36.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/SOURCES.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)        1 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/dependency_links.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       12 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/requires.txt
+-rwxr-xr-x   0 cpi       (1001) cpi       (1001)       14 2024-04-24 02:35:35.000000 simular-eth-stubs-0.0.4/simular_eth_stubs.egg-info/top_level.txt
```

