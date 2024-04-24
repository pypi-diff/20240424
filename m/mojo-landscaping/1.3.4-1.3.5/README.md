# Comparing `tmp/mojo_landscaping-1.3.4.tar.gz` & `tmp/mojo_landscaping-1.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mojo_landscaping-1.3.4.tar", max compression
+gzip compressed data, was "mojo_landscaping-1.3.5.tar", max compression
```

## Comparing `mojo_landscaping-1.3.4.tar` & `mojo_landscaping-1.3.5.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0        0        0     1083 2024-01-26 02:56:23.556649 mojo_landscaping-1.3.4/LICENSE.txt
--rw-r--r--   0        0        0     1980 2024-01-26 02:56:23.556797 mojo_landscaping-1.3.4/README.rst
--rw-r--r--   0        0        0      860 2024-03-29 20:45:56.856999 mojo_landscaping-1.3.4/pyproject.toml
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558283 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/__init__.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558375 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/__init__.py
--rw-r--r--   0        0        0    10616 2024-01-26 02:56:23.558500 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/localcommandagent.py
--rw-r--r--   0        0        0     2023 2024-01-26 02:56:23.558582 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/poweragentbase.py
--rw-r--r--   0        0        0      888 2024-01-26 02:56:23.558668 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/serialagentbase.py
--rw-r--r--   0        0        0      863 2024-01-26 02:56:23.558750 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/systemagentbase.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558826 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/client/__init__.py
--rw-r--r--   0        0        0     1655 2024-01-26 02:56:23.558936 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/client/clientbase.py
--rw-r--r--   0        0        0     9168 2024-01-26 02:56:23.559060 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/client/clientcoordinatorbase.py
--rw-r--r--   0        0        0     7291 2024-01-26 02:56:23.559207 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559287 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/cluster/__init__.py
--rw-r--r--   0        0        0     1747 2024-01-26 02:56:23.559382 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/cluster/nodebase.py
--rw-r--r--   0        0        0    10817 2024-01-26 02:56:23.559462 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py
--rw-r--r--   0        0        0     7396 2024-01-26 02:56:23.559533 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py
--rw-r--r--   0        0        0     2402 2024-01-26 02:56:23.559631 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/configurationextractor.py
--rw-r--r--   0        0        0      769 2024-01-26 02:56:23.559704 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/constants.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559778 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/coordinators/__init__.py
--rw-r--r--   0        0        0     6949 2024-01-26 02:56:23.559916 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/coordinators/coordinatorbase.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.560009 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/coupling/__init__.py
--rw-r--r--   0        0        0     1496 2024-01-26 02:56:23.560104 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py
--rw-r--r--   0        0        0     3346 2024-01-26 02:56:23.560189 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/friendlyidentifier.py
--rw-r--r--   0        0        0     5876 2024-01-26 02:56:23.560280 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/includefilters.py
--rw-r--r--   0        0        0    19639 2024-02-16 22:32:11.631790 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscape.py
--rw-r--r--   0        0        0    15428 2024-01-26 02:56:23.560725 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapedevice.py
--rw-r--r--   0        0        0     1800 2024-03-29 20:38:14.167319 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapedevicecluster.py
--rw-r--r--   0        0        0     1300 2024-01-26 02:56:23.560909 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapedevicegroup.py
--rw-r--r--   0        0        0      846 2024-01-26 02:56:23.560993 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapeparameters.py
--rw-r--r--   0        0        0    13782 2024-01-26 02:56:23.561075 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapeservice.py
--rw-r--r--   0        0        0     1164 2024-01-26 02:56:23.561163 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapingextensionprotocol.py
--rw-r--r--   0        0        0    17195 2024-03-08 02:21:32.965401 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py
--rw-r--r--   0        0        0     2163 2024-01-26 02:56:23.561530 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py
--rw-r--r--   0        0        0    17352 2024-01-26 02:56:23.561610 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py
--rw-r--r--   0        0        0    14061 2024-03-29 20:46:40.802157 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py
--rw-r--r--   0        0        0      998 2024-01-26 02:56:23.561816 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapinglayerbase.py
--rw-r--r--   0        0        0      972 2024-01-26 02:56:23.561888 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py
--rw-r--r--   0        0        0     3812 2024-01-26 02:56:23.561978 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/protocolextension.py
--rw-r--r--   0        0        0        0 2024-01-26 02:56:23.562051 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/service/__init__.py
--rw-r--r--   0        0        0     1670 2024-01-26 02:56:23.562154 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/service/servicebase.py
--rw-r--r--   0        0        0     9042 2024-01-26 02:56:23.562249 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/service/servicecoordinatorbase.py
--rw-r--r--   0        0        0     7346 2024-01-26 02:56:23.562352 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py
--rw-r--r--   0        0        0     1695 2024-01-26 02:56:23.562437 mojo_landscaping-1.3.4/source/packages/mojo/landscaping/wellknown.py
--rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.4/setup.py
--rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1083 2024-01-26 02:56:23.556649 mojo_landscaping-1.3.5/LICENSE.txt
+-rw-r--r--   0        0        0     1980 2024-01-26 02:56:23.556797 mojo_landscaping-1.3.5/README.rst
+-rw-r--r--   0        0        0      860 2024-04-24 04:07:26.555302 mojo_landscaping-1.3.5/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558283 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/__init__.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558375 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/__init__.py
+-rw-r--r--   0        0        0    10616 2024-01-26 02:56:23.558500 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/localcommandagent.py
+-rw-r--r--   0        0        0     2023 2024-01-26 02:56:23.558582 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/poweragentbase.py
+-rw-r--r--   0        0        0      888 2024-01-26 02:56:23.558668 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/serialagentbase.py
+-rw-r--r--   0        0        0      863 2024-01-26 02:56:23.558750 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/systemagentbase.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.558826 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/__init__.py
+-rw-r--r--   0        0        0     1655 2024-01-26 02:56:23.558936 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientbase.py
+-rw-r--r--   0        0        0     9168 2024-01-26 02:56:23.559060 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorbase.py
+-rw-r--r--   0        0        0     7291 2024-01-26 02:56:23.559207 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559287 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/__init__.py
+-rw-r--r--   0        0        0     1747 2024-01-26 02:56:23.559382 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodebase.py
+-rw-r--r--   0        0        0    10817 2024-01-26 02:56:23.559462 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py
+-rw-r--r--   0        0        0     7396 2024-01-26 02:56:23.559533 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py
+-rw-r--r--   0        0        0     2402 2024-01-26 02:56:23.559631 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/configurationextractor.py
+-rw-r--r--   0        0        0      769 2024-01-26 02:56:23.559704 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/constants.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.559778 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coordinators/__init__.py
+-rw-r--r--   0        0        0     6949 2024-01-26 02:56:23.559916 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coordinators/coordinatorbase.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.560009 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coupling/__init__.py
+-rw-r--r--   0        0        0     1496 2024-01-26 02:56:23.560104 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py
+-rw-r--r--   0        0        0     3346 2024-01-26 02:56:23.560189 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/friendlyidentifier.py
+-rw-r--r--   0        0        0     5876 2024-01-26 02:56:23.560280 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/includefilters.py
+-rw-r--r--   0        0        0    19639 2024-02-16 22:32:11.631790 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscape.py
+-rw-r--r--   0        0        0    15428 2024-01-26 02:56:23.560725 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevice.py
+-rw-r--r--   0        0        0     1800 2024-03-29 20:38:14.167319 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevicecluster.py
+-rw-r--r--   0        0        0     1300 2024-01-26 02:56:23.560909 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevicegroup.py
+-rw-r--r--   0        0        0      846 2024-01-26 02:56:23.560993 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeparameters.py
+-rw-r--r--   0        0        0    13782 2024-01-26 02:56:23.561075 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeservice.py
+-rw-r--r--   0        0        0     1164 2024-01-26 02:56:23.561163 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapingextensionprotocol.py
+-rw-r--r--   0        0        0    17195 2024-03-08 02:21:32.965401 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py
+-rw-r--r--   0        0        0     2163 2024-01-26 02:56:23.561530 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py
+-rw-r--r--   0        0        0    17352 2024-01-26 02:56:23.561610 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py
+-rw-r--r--   0        0        0    14061 2024-03-29 20:46:40.802157 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py
+-rw-r--r--   0        0        0      998 2024-01-26 02:56:23.561816 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapinglayerbase.py
+-rw-r--r--   0        0        0      972 2024-01-26 02:56:23.561888 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py
+-rw-r--r--   0        0        0     3812 2024-01-26 02:56:23.561978 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/protocolextension.py
+-rw-r--r--   0        0        0        0 2024-01-26 02:56:23.562051 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/__init__.py
+-rw-r--r--   0        0        0     1670 2024-01-26 02:56:23.562154 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicebase.py
+-rw-r--r--   0        0        0     9042 2024-01-26 02:56:23.562249 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorbase.py
+-rw-r--r--   0        0        0     7346 2024-01-26 02:56:23.562352 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py
+-rw-r--r--   0        0        0     1695 2024-01-26 02:56:23.562437 mojo_landscaping-1.3.5/source/packages/mojo/landscaping/wellknown.py
+-rw-r--r--   0        0        0     3109 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.5/setup.py
+-rw-r--r--   0        0        0     2884 1970-01-01 00:00:00.000000 mojo_landscaping-1.3.5/PKG-INFO
```

### Comparing `mojo_landscaping-1.3.4/LICENSE.txt` & `mojo_landscaping-1.3.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/README.rst` & `mojo_landscaping-1.3.5/README.rst`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/pyproject.toml` & `mojo_landscaping-1.3.5/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [tool.poetry]
 name = "mojo-landscaping"
 description = "Automation Mojo Landscaping Package"
-version = "1.3.4"
+version = "1.3.5"
 authors = ["Myron W Walker"]
 readme = "README.rst"
 license = "LICENSE.txt"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: POSIX"
```

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/localcommandagent.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/localcommandagent.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/poweragentbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/poweragentbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/serialagentbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/serialagentbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/agents/systemagentbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/agents/systemagentbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/client/clientbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/client/clientcoordinatorbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/client/clientcoordinatorcouplingbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/cluster/nodebase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodebase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/cluster/nodecoordinatorcouplingbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/configurationextractor.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/configurationextractor.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/constants.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/constants.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/coordinators/coordinatorbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coordinators/coordinatorbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/coupling/coordinatorcoupling.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/friendlyidentifier.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/friendlyidentifier.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/includefilters.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/includefilters.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscape.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscape.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapedevice.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevice.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapedevicecluster.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevicecluster.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapedevicegroup.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapedevicegroup.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapeparameters.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeparameters.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapeservice.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapeservice.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/landscapingextensionprotocol.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/landscapingextensionprotocol.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeconfigurationlayer.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeinstallationlayer.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeintegrationlayer.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapeoperationallayer.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/landscapinglayerbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/landscapinglayerbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/layers/topologyintegrationlayer.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/protocolextension.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/protocolextension.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/service/servicebase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicebase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/service/servicecoordinatorbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/service/servicecoordinatorcouplingbase.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/source/packages/mojo/landscaping/wellknown.py` & `mojo_landscaping-1.3.5/source/packages/mojo/landscaping/wellknown.py`

 * *Files identical despite different names*

### Comparing `mojo_landscaping-1.3.4/setup.py` & `mojo_landscaping-1.3.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
  'mojo-credentials>=1.3.1,<1.4.0',
  'mojo-extension>=1.3.8,<1.4.0',
  'mojo-interfaces>=1.3.1,<1.4.0',
  'mojo-xmodules>=1.3.16,<1.4.0']
 
 setup_kwargs = {
     'name': 'mojo-landscaping',
-    'version': '1.3.4',
+    'version': '1.3.5',
     'description': 'Automation Mojo Landscaping Package',
     'long_description': '=======================\npython-package-template\n=======================\nThis is a template repository that can be used to quickly create a python package project.\n\n=========================\nFeatures of this Template\n=========================\n* Machine Setup\n* Virtual Environment Setup (Poetry)\n* PyPi Publishing\n* Sphinx Documentation\n\n========================\nHow to Use This Template\n========================\n- Click the \'Use this template\' button\n- Fill in the information to create your repository\n- Checkout your new repository\n- Change the following in \'repository-config.ini\'\n\n  #. \'PROJECT NAME\'\n  #. \'REPOSITORY_NAME\'\n\n- If you have machine dependencies to add, put them in \'setup-ubuntu-machine\'\n- Modify the pyproject.toml file with the correct package-name, author, publishing information, etc.\n- Rename the VSCODE workspace file \'mv workspaces/default-workspace.template workspaces/(project name).template\'\n- Replace the README.rst file with your own README\n- Update the LICENSE.txt file with your copyright information and license.\n- Add your dependencies with python poetry \'poetry add (dependency name)\'\n- Drop your package code in \'source/packages\'\n- Modify the name of your package root in \'pyproject.toml\'\n\n  #. \'packages = [{include="(root folder name)", from="source/packages"}]\'\n\n=================\nCode Organization\n=================\n* .vscode - Common tasks\n* development - This is where the runtime environment scripts are located\n* repository-setup - Scripts for homing your repository and to your checkout and machine setup\n* userguide - Where you put your user guide\n* source/packages - Put your root folder here \'source/packages/(root-module-folder)\'\n* source/sphinx - This is the Sphinx documentation folder\n* workspaces - This is where you add VSCode workspaces templates and where workspaces show up when homed.\n\n==========\nReferences\n==========\n\n- `User Guide <userguide/userguide.rst>`\n- `Coding Standards <userguide/10-00-coding-standards.rst>`\n',
     'author': 'Myron W Walker',
     'author_email': 'None',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `mojo_landscaping-1.3.4/PKG-INFO` & `mojo_landscaping-1.3.5/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mojo-landscaping
-Version: 1.3.4
+Version: 1.3.5
 Summary: Automation Mojo Landscaping Package
 License: LICENSE.txt
 Keywords: python
 Author: Myron W Walker
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: License :: Other/Proprietary License
```

