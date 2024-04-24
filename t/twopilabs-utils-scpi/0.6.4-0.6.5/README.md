# Comparing `tmp/twopilabs-utils-scpi-0.6.4.tar.gz` & `tmp/twopilabs-utils-scpi-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/builds/devel/products/common/python/twopilabs-utils-scpi/dist/tmp4574a8uj/twopilabs-utils-scpi-0.6.4.tar", last modified: Fri Sep  1 09:00:22 2023, max compression
+gzip compressed data, was "/builds/devel/products/common/python/twopilabs-utils-scpi/dist/tmp34s4kjfy/twopilabs-utils-scpi-0.6.5.tar", last modified: Wed Apr 24 13:53:19 2024, max compression
```

## Comparing `twopilabs-utils-scpi-0.6.4.tar` & `twopilabs-utils-scpi-0.6.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/
--rw-rw-rw-   0 root         (0) root         (0)       72 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3875 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_base.py
--rw-rw-rw-   0 root         (0) root         (0)     3634 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_resource.py
--rw-rw-rw-   0 root         (0) root         (0)     2797 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_serial.py
--rw-rw-rw-   0 root         (0) root         (0)      433 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_exceptions.py
--rw-rw-rw-   0 root         (0) root         (0)      928 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_type_base.py
--rw-rw-rw-   0 root         (0) root         (0)     2769 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_device.py
--rw-rw-rw-   0 root         (0) root         (0)     2959 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_usbtmc.py
--rw-rw-rw-   0 root         (0) root         (0)     7472 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_tcpip.py
--rw-rw-rw-   0 root         (0) root         (0)    17922 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_types.py
--rw-rw-rw-   0 root         (0) root         (0)      296 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/README.md
--rw-r--r--   0 root         (0) root         (0)      806 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      962 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/
--rw-r--r--   0 root         (0) root         (0)      747 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      806 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)       15 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       55 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/requires.txt
--rw-rw-rw-   0 root         (0) root         (0)      206 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/pyproject.toml
--rw-rw-rw-   0 root         (0) root         (0)      121 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      652 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     7652 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-09-01 09:00:22.000000 twopilabs-utils-scpi-0.6.4/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      292 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-09-01 08:58:58.000000 twopilabs-utils-scpi-0.6.4/.idea/twopilabs-utils-scpi.iml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:19.000000 twopilabs-utils-scpi-0.6.5/
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-04-24 13:53:19.000000 twopilabs-utils-scpi-0.6.5/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     7652 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      206 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/pyproject.toml
+-rw-rw-rw-   0 root         (0) root         (0)       72 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/setup.py
+-rw-rw-rw-   0 root         (0) root         (0)      121 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/.gitignore
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:19.000000 twopilabs-utils-scpi-0.6.5/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      284 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/.idea/twopilabs-utils-scpi.iml
+-rw-rw-rw-   0 root         (0) root         (0)      292 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/.idea/modules.xml
+-rw-r--r--   0 root         (0) root         (0)      806 2024-04-24 13:53:19.000000 twopilabs-utils-scpi-0.6.5/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      296 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:18.000000 twopilabs-utils-scpi-0.6.5/twopilabs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:18.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:19.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/
+-rw-rw-rw-   0 root         (0) root         (0)      265 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      433 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_exceptions.py
+-rw-rw-rw-   0 root         (0) root         (0)     3875 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2959 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_usbtmc.py
+-rw-rw-rw-   0 root         (0) root         (0)     7472 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_tcpip.py
+-rw-rw-rw-   0 root         (0) root         (0)      928 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_type_base.py
+-rw-rw-rw-   0 root         (0) root         (0)     2823 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_device.py
+-rw-rw-rw-   0 root         (0) root         (0)     2797 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_serial.py
+-rw-rw-rw-   0 root         (0) root         (0)    17922 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     3634 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_resource.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-24 13:53:19.000000 twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-24 13:53:18.000000 twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)      806 2024-04-24 13:53:18.000000 twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)       15 2024-04-24 13:53:18.000000 twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-24 13:53:18.000000 twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-24 13:53:18.000000 twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/SOURCES.txt
+-rw-rw-rw-   0 root         (0) root         (0)      962 2024-04-24 13:51:49.000000 twopilabs-utils-scpi-0.6.5/.gitlab-ci.yml
```

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_base.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_base.py`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_resource.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_resource.py`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_serial.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_serial.py`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_type_base.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_type_base.py`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_device.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_device.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
                 f'exec [{type(param).__name__} -> {result.__name__}]: ' +
                 f'{str(header)[1:]} ({str(param)}) -> ({str(response)})')
         except Exception as e:
             logger.error(
                 f'exec [{type(param).__name__} -> {result.__name__}]: ' +
                 f'{str(header)[1:]} ({str(param)}) -> ({str(response)}) [{repr(e)}]')
 
+            # Re-Raise Exception
+            raise e
+
         return response
 
     def check_error(self) -> Optional[ScpiEvent]:
         """Checks if an error is available in the device's SCPI error queue and returns it. Returns None otherwise"""
         scpi_error = self.execute('SYST:ERR:NEXT?', result=ScpiEvent)
         if scpi_error.code != 0:
             return scpi_error
```

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_usbtmc.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_usbtmc.py`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_transport_tcpip.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_transport_tcpip.py`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs/utils/scpi/scpi_types.py` & `twopilabs-utils-scpi-0.6.5/twopilabs/utils/scpi/scpi_types.py`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/PKG-INFO` & `twopilabs-utils-scpi-0.6.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-utils-scpi
-Version: 0.6.4
+Version: 0.6.5
 Summary: A SCPI command/parameter abstraction layer for interfacing with measurement equipment
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `twopilabs-utils-scpi-0.6.4/.gitlab-ci.yml` & `twopilabs-utils-scpi-0.6.5/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/SOURCES.txt` & `twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/twopilabs_utils_scpi.egg-info/PKG-INFO` & `twopilabs-utils-scpi-0.6.5/twopilabs_utils_scpi.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twopilabs-utils-scpi
-Version: 0.6.4
+Version: 0.6.5
 Summary: A SCPI command/parameter abstraction layer for interfacing with measurement equipment
 Home-page: https://www.2pi-labs.com
 Author: 2pi-Labs GmbH
 Author-email: opensource@2pi-labs.com
 License: LGPLv3
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

### Comparing `twopilabs-utils-scpi-0.6.4/setup.cfg` & `twopilabs-utils-scpi-0.6.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `twopilabs-utils-scpi-0.6.4/LICENSE` & `twopilabs-utils-scpi-0.6.5/LICENSE`

 * *Files identical despite different names*

