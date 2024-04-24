# Comparing `tmp/simular-eth-stubs-0.0.1.tar.gz` & `tmp/simular-eth-stubs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simular-eth-stubs-0.0.1.tar", last modified: Tue Apr 23 18:07:11 2024, max compression
+gzip compressed data, was "simular-eth-stubs-0.0.2.tar", last modified: Tue Apr 23 18:31:46 2024, max compression
```

## Comparing `simular-eth-stubs-0.0.1.tar` & `simular-eth-stubs-0.0.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
-drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-04-23 18:07:11.320000 simular-eth-stubs-0.0.1/
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      227 2024-04-23 18:07:11.310000 simular-eth-stubs-0.0.1/PKG-INFO
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       28 2024-04-23 18:02:23.000000 simular-eth-stubs-0.0.1/README.md
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       38 2024-04-23 18:07:11.320000 simular-eth-stubs-0.0.1/setup.cfg
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      464 2024-04-23 18:05:16.000000 simular-eth-stubs-0.0.1/setup.py
-drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-04-23 18:07:11.310000 simular-eth-stubs-0.0.1/simular_eth_stubs.egg-info/
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      227 2024-04-23 18:07:11.000000 simular-eth-stubs-0.0.1/simular_eth_stubs.egg-info/PKG-INFO
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      182 2024-04-23 18:07:11.000000 simular-eth-stubs-0.0.1/simular_eth_stubs.egg-info/SOURCES.txt
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        1 2024-04-23 18:07:11.000000 simular-eth-stubs-0.0.1/simular_eth_stubs.egg-info/dependency_links.txt
--rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       14 2024-04-23 18:07:11.000000 simular-eth-stubs-0.0.1/simular_eth_stubs.egg-info/top_level.txt
+drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-04-23 18:31:46.160000 simular-eth-stubs-0.0.2/
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      227 2024-04-23 18:31:46.160000 simular-eth-stubs-0.0.2/PKG-INFO
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       28 2024-04-23 18:02:23.000000 simular-eth-stubs-0.0.2/README.md
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       38 2024-04-23 18:31:46.160000 simular-eth-stubs-0.0.2/setup.cfg
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      464 2024-04-23 18:25:43.000000 simular-eth-stubs-0.0.2/setup.py
+drwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        0 2024-04-23 18:31:46.160000 simular-eth-stubs-0.0.2/simular_eth_stubs.egg-info/
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      227 2024-04-23 18:31:46.000000 simular-eth-stubs-0.0.2/simular_eth_stubs.egg-info/PKG-INFO
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)      182 2024-04-23 18:31:46.000000 simular-eth-stubs-0.0.2/simular_eth_stubs.egg-info/SOURCES.txt
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)        1 2024-04-23 18:31:46.000000 simular-eth-stubs-0.0.2/simular_eth_stubs.egg-info/dependency_links.txt
+-rwxr-xr-x   0 jamesbrown  (1000) jamesbrown  (1000)       14 2024-04-23 18:31:46.000000 simular-eth-stubs-0.0.2/simular_eth_stubs.egg-info/top_level.txt
```

