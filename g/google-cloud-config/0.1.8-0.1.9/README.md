# Comparing `tmp/google-cloud-config-0.1.8.tar.gz` & `tmp/google-cloud-config-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "google-cloud-config-0.1.8.tar", last modified: Fri Mar 22 12:19:01 2024, max compression
+gzip compressed data, was "google-cloud-config-0.1.9.tar", last modified: Wed Apr 24 19:17:16 2024, max compression
```

## Comparing `google-cloud-config-0.1.8.tar` & `google-cloud-config-0.1.9.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/
--rw-rw-r--   0 root         (0)     1003    11358 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/LICENSE
--rw-rw-r--   0 root         (0)     1003      860 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0)     1003     5273 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/PKG-INFO
--rw-rw-r--   0 root         (0)     1003     3860 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/README.rst
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.554672 google-cloud-config-0.1.8/google/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.554672 google-cloud-config-0.1.8/google/cloud/
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.558672 google-cloud-config-0.1.8/google/cloud/config/
--rw-rw-r--   0 root         (0)     1003     3583 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config/__init__.py
--rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.558672 google-cloud-config-0.1.8/google/cloud/config_v1/
--rw-rw-r--   0 root         (0)     1003     3472 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003     9382 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/gapic_metadata.json
--rw-rw-r--   0 root         (0)     1003      652 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/gapic_version.py
--rw-rw-r--   0 root         (0)     1003       80 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/py.typed
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.558672 google-cloud-config-0.1.8/google/cloud/config_v1/services/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.562672 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/
--rw-rw-r--   0 root         (0)     1003      737 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/__init__.py
--rw-rw-r--   0 root         (0)     1003   140924 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/async_client.py
--rw-rw-r--   0 root         (0)     1003   163769 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/client.py
--rw-rw-r--   0 root         (0)     1003    25568 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/pagers.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.562672 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/
--rw-rw-r--   0 root         (0)     1003     1288 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/__init__.py
--rw-rw-r--   0 root         (0)     1003    18252 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/base.py
--rw-rw-r--   0 root         (0)     1003    46270 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/grpc.py
--rw-rw-r--   0 root         (0)     1003    47185 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/grpc_asyncio.py
--rw-rw-r--   0 root         (0)     1003   155063 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/rest.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.562672 google-cloud-config-0.1.8/google/cloud/config_v1/types/
--rw-rw-r--   0 root         (0)     1003     3247 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/types/__init__.py
--rw-rw-r--   0 root         (0)     1003    88266 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/google/cloud/config_v1/types/config.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/google_cloud_config.egg-info/
--rw-r--r--   0 root         (0)     1003     5273 2024-03-22 12:19:01.000000 google-cloud-config-0.1.8/google_cloud_config.egg-info/PKG-INFO
--rw-r--r--   0 root         (0)     1003     1324 2024-03-22 12:19:01.000000 google-cloud-config-0.1.8/google_cloud_config.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:19:01.000000 google-cloud-config-0.1.8/google_cloud_config.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0)     1003        1 2024-03-22 12:19:01.000000 google-cloud-config-0.1.8/google_cloud_config.egg-info/not-zip-safe
--rw-r--r--   0 root         (0)     1003      342 2024-03-22 12:19:01.000000 google-cloud-config-0.1.8/google_cloud_config.egg-info/requires.txt
--rw-r--r--   0 root         (0)     1003        7 2024-03-22 12:19:01.000000 google-cloud-config-0.1.8/google_cloud_config.egg-info/top_level.txt
--rw-r--r--   0 root         (0)     1003       38 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/setup.cfg
--rw-rw-r--   0 root         (0)     1003     3206 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/setup.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/tests/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/tests/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/tests/unit/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/tests/unit/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/tests/unit/gapic/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/tests/unit/gapic/__init__.py
-drwxr-sr-x   0 root         (0)     1003        0 2024-03-22 12:19:01.566672 google-cloud-config-0.1.8/tests/unit/gapic/config_v1/
--rw-rw-r--   0 root         (0)     1003      600 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/tests/unit/gapic/config_v1/__init__.py
--rw-rw-r--   0 root         (0)     1003   617989 2024-03-22 12:15:14.000000 google-cloud-config-0.1.8/tests/unit/gapic/config_v1/test_config.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/
+-rw-rw-r--   0 root         (0)     1003    11358 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/LICENSE
+-rw-rw-r--   0 root         (0)     1003      860 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0)     1003     5273 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/PKG-INFO
+-rw-rw-r--   0 root         (0)     1003     3860 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/README.rst
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.037931 google-cloud-config-0.1.9/google/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.037931 google-cloud-config-0.1.9/google/cloud/
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.041931 google-cloud-config-0.1.9/google/cloud/config/
+-rw-rw-r--   0 root         (0)     1003     3583 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config/__init__.py
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.041931 google-cloud-config-0.1.9/google/cloud/config_v1/
+-rw-rw-r--   0 root         (0)     1003     3472 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003     9382 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/gapic_metadata.json
+-rw-rw-r--   0 root         (0)     1003      652 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/gapic_version.py
+-rw-rw-r--   0 root         (0)     1003       80 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/py.typed
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.041931 google-cloud-config-0.1.9/google/cloud/config_v1/services/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.045930 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/
+-rw-rw-r--   0 root         (0)     1003      737 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/__init__.py
+-rw-rw-r--   0 root         (0)     1003   140924 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/async_client.py
+-rw-rw-r--   0 root         (0)     1003   163769 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/client.py
+-rw-rw-r--   0 root         (0)     1003    25568 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/pagers.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.045930 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/
+-rw-rw-r--   0 root         (0)     1003     1288 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/__init__.py
+-rw-rw-r--   0 root         (0)     1003    18252 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/base.py
+-rw-rw-r--   0 root         (0)     1003    46270 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/grpc.py
+-rw-rw-r--   0 root         (0)     1003    47185 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/grpc_asyncio.py
+-rw-rw-r--   0 root         (0)     1003   155063 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/rest.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.045930 google-cloud-config-0.1.9/google/cloud/config_v1/types/
+-rw-rw-r--   0 root         (0)     1003     3247 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/types/__init__.py
+-rw-rw-r--   0 root         (0)     1003    89309 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/google/cloud/config_v1/types/config.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/google_cloud_config.egg-info/
+-rw-r--r--   0 root         (0)     1003     5273 2024-04-24 19:17:15.000000 google-cloud-config-0.1.9/google_cloud_config.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0)     1003     1324 2024-04-24 19:17:16.000000 google-cloud-config-0.1.9/google_cloud_config.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-24 19:17:15.000000 google-cloud-config-0.1.9/google_cloud_config.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0)     1003        1 2024-04-24 19:17:15.000000 google-cloud-config-0.1.9/google_cloud_config.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0)     1003      342 2024-04-24 19:17:15.000000 google-cloud-config-0.1.9/google_cloud_config.egg-info/requires.txt
+-rw-r--r--   0 root         (0)     1003        7 2024-04-24 19:17:15.000000 google-cloud-config-0.1.9/google_cloud_config.egg-info/top_level.txt
+-rw-r--r--   0 root         (0)     1003       38 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/setup.cfg
+-rw-rw-r--   0 root         (0)     1003     3206 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/setup.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/tests/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/tests/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/tests/unit/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/tests/unit/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/tests/unit/gapic/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/tests/unit/gapic/__init__.py
+drwxr-sr-x   0 root         (0)     1003        0 2024-04-24 19:17:16.049930 google-cloud-config-0.1.9/tests/unit/gapic/config_v1/
+-rw-rw-r--   0 root         (0)     1003      600 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/tests/unit/gapic/config_v1/__init__.py
+-rw-rw-r--   0 root         (0)     1003   668346 2024-04-24 19:14:04.000000 google-cloud-config-0.1.9/tests/unit/gapic/config_v1/test_config.py
```

### Comparing `google-cloud-config-0.1.8/LICENSE` & `google-cloud-config-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/MANIFEST.in` & `google-cloud-config-0.1.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/PKG-INFO` & `google-cloud-config-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-config
-Version: 0.1.8
+Version: 0.1.9
 Summary: Google Cloud Config API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-config
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-config-0.1.8/README.rst` & `google-cloud-config-0.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config/__init__.py` & `google-cloud-config-0.1.9/google/cloud/config/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config/gapic_version.py` & `google-cloud-config-0.1.9/google/cloud/config/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
+__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/__init__.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/gapic_metadata.json` & `google-cloud-config-0.1.9/google/cloud/config_v1/gapic_metadata.json`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/gapic_version.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/gapic_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,8 +9,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
-__version__ = "0.1.8"  # {x-release-please-version}
+__version__ = "0.1.9"  # {x-release-please-version}
```

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/__init__.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/__init__.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/async_client.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/async_client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/client.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/client.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/pagers.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/pagers.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/__init__.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/base.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/base.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/grpc.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/grpc.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/grpc_asyncio.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/grpc_asyncio.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/services/config/transports/rest.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/services/config/transports/rest.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/types/__init__.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/types/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/google/cloud/config_v1/types/config.py` & `google-cloud-config-0.1.9/google/cloud/config_v1/types/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,14 +215,20 @@
             set on the deployment. It is in the format of
             "Major.Minor.Patch", for example, "1.3.10".
         quota_validation (google.cloud.config_v1.types.QuotaValidation):
             Optional. Input to control quota checks for
             resources in terraform configuration files.
             There are limited resources on which quota
             validation applies.
+        annotations (MutableMapping[str, str]):
+            Optional. Arbitrary key-value metadata
+            storage e.g. to help client tools identify
+            deployments during automation. See
+            https://google.aip.dev/148#annotations for
+            details on format and size limitations.
     """
 
     class State(proto.Enum):
         r"""Possible states of a deployment.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -415,14 +421,19 @@
         number=22,
     )
     quota_validation: "QuotaValidation" = proto.Field(
         proto.ENUM,
         number=23,
         enum="QuotaValidation",
     )
+    annotations: MutableMapping[str, str] = proto.MapField(
+        proto.STRING,
+        proto.STRING,
+        number=24,
+    )
 
 
 class TerraformBlueprint(proto.Message):
     r"""TerraformBlueprint describes the source of a Terraform root
     module which describes the resources and configs to be deployed.
 
     This message has `oneof`_ fields (mutually exclusive fields).
@@ -2009,14 +2020,23 @@
             the full list of the errors encountered during a Terraform
             preview. Format: ``gs://{bucket}/{object}``.
         preview_artifacts (google.cloud.config_v1.types.PreviewArtifacts):
             Output only. Artifacts from preview.
         logs (str):
             Output only. Location of preview logs in
             ``gs://{bucket}/{object}`` format.
+        tf_version (str):
+            Output only. The current Terraform version
+            set on the preview. It is in the format of
+            "Major.Minor.Patch", for example, "1.3.10".
+        tf_version_constraint (str):
+            Optional. The user-specified Terraform
+            version constraint. Example: "=1.3.10".
+
+            This field is a member of `oneof`_ ``_tf_version_constraint``.
     """
 
     class State(proto.Enum):
         r"""Possible states of a preview.
 
         Values:
             STATE_UNSPECIFIED (0):
@@ -2178,14 +2198,23 @@
         number=16,
         message="PreviewArtifacts",
     )
     logs: str = proto.Field(
         proto.STRING,
         number=17,
     )
+    tf_version: str = proto.Field(
+        proto.STRING,
+        number=18,
+    )
+    tf_version_constraint: str = proto.Field(
+        proto.STRING,
+        number=19,
+        optional=True,
+    )
 
 
 class PreviewOperationMetadata(proto.Message):
     r"""Ephemeral metadata content describing the state of a preview
     operation.
 
     Attributes:
```

### Comparing `google-cloud-config-0.1.8/google_cloud_config.egg-info/PKG-INFO` & `google-cloud-config-0.1.9/google_cloud_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: google-cloud-config
-Version: 0.1.8
+Version: 0.1.9
 Summary: Google Cloud Config API client library
 Home-page: https://github.com/googleapis/google-cloud-python/tree/main/packages/google-cloud-config
 Author: Google LLC
 Author-email: googleapis-packages@google.com
 License: Apache 2.0
 Platform: Posix; MacOS X; Windows
 Classifier: Development Status :: 4 - Beta
```

### Comparing `google-cloud-config-0.1.8/google_cloud_config.egg-info/SOURCES.txt` & `google-cloud-config-0.1.9/google_cloud_config.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/setup.py` & `google-cloud-config-0.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/tests/__init__.py` & `google-cloud-config-0.1.9/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/tests/unit/__init__.py` & `google-cloud-config-0.1.9/tests/unit/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/tests/unit/gapic/__init__.py` & `google-cloud-config-0.1.9/tests/unit/gapic/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/tests/unit/gapic/config_v1/__init__.py` & `google-cloud-config-0.1.9/tests/unit/gapic/config_v1/__init__.py`

 * *Files identical despite different names*

### Comparing `google-cloud-config-0.1.8/tests/unit/gapic/config_v1/test_config.py` & `google-cloud-config-0.1.9/tests/unit/gapic/config_v1/test_config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1092,15 +1092,16 @@
             unreachable=["unreachable_value"],
         )
         response = client.list_deployments(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListDeploymentsRequest()
+        request = config.ListDeploymentsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDeploymentsPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -1116,14 +1117,69 @@
     with mock.patch.object(type(client.transport.list_deployments), "__call__") as call:
         client.list_deployments()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ListDeploymentsRequest()
 
 
+def test_list_deployments_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ListDeploymentsRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+        order_by="order_by_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_deployments), "__call__") as call:
+        client.list_deployments(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListDeploymentsRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+            order_by="order_by_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_deployments_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_deployments), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.ListDeploymentsResponse(
+                next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
+            )
+        )
+        response = await client.list_deployments()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListDeploymentsRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_deployments_async(
     transport: str = "grpc_asyncio", request_type=config.ListDeploymentsRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1143,15 +1199,16 @@
             )
         )
         response = await client.list_deployments(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListDeploymentsRequest()
+        request = config.ListDeploymentsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListDeploymentsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -1532,15 +1589,16 @@
             quota_validation=config.QuotaValidation.ENABLED,
         )
         response = client.get_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetDeploymentRequest()
+        request = config.GetDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Deployment)
     assert response.name == "name_value"
     assert response.state == config.Deployment.State.CREATING
     assert response.latest_revision == "latest_revision_value"
     assert response.state_detail == "state_detail_value"
@@ -1570,14 +1628,77 @@
     with mock.patch.object(type(client.transport.get_deployment), "__call__") as call:
         client.get_deployment()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.GetDeploymentRequest()
 
 
+def test_get_deployment_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.GetDeploymentRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_deployment), "__call__") as call:
+        client.get_deployment(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetDeploymentRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_deployment_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_deployment), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.Deployment(
+                name="name_value",
+                state=config.Deployment.State.CREATING,
+                latest_revision="latest_revision_value",
+                state_detail="state_detail_value",
+                error_code=config.Deployment.ErrorCode.REVISION_FAILED,
+                delete_build="delete_build_value",
+                delete_logs="delete_logs_value",
+                error_logs="error_logs_value",
+                artifacts_gcs_bucket="artifacts_gcs_bucket_value",
+                service_account="service_account_value",
+                import_existing_resources=True,
+                worker_pool="worker_pool_value",
+                lock_state=config.Deployment.LockState.LOCKED,
+                tf_version_constraint="tf_version_constraint_value",
+                tf_version="tf_version_value",
+                quota_validation=config.QuotaValidation.ENABLED,
+            )
+        )
+        response = await client.get_deployment()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetDeploymentRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_deployment_async(
     transport: str = "grpc_asyncio", request_type=config.GetDeploymentRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1611,15 +1732,16 @@
             )
         )
         response = await client.get_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetDeploymentRequest()
+        request = config.GetDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Deployment)
     assert response.name == "name_value"
     assert response.state == config.Deployment.State.CREATING
     assert response.latest_revision == "latest_revision_value"
     assert response.state_detail == "state_detail_value"
@@ -1805,15 +1927,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.create_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.CreateDeploymentRequest()
+        request = config.CreateDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_create_deployment_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -1829,14 +1952,68 @@
     ) as call:
         client.create_deployment()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.CreateDeploymentRequest()
 
 
+def test_create_deployment_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.CreateDeploymentRequest(
+        parent="parent_value",
+        deployment_id="deployment_id_value",
+        request_id="request_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_deployment), "__call__"
+    ) as call:
+        client.create_deployment(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.CreateDeploymentRequest(
+            parent="parent_value",
+            deployment_id="deployment_id_value",
+            request_id="request_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_deployment_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.create_deployment), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.create_deployment()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.CreateDeploymentRequest()
+
+
 @pytest.mark.asyncio
 async def test_create_deployment_async(
     transport: str = "grpc_asyncio", request_type=config.CreateDeploymentRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -1855,15 +2032,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.create_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.CreateDeploymentRequest()
+        request = config.CreateDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_create_deployment_async_from_dict():
@@ -2085,15 +2263,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.update_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.UpdateDeploymentRequest()
+        request = config.UpdateDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_update_deployment_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -2109,14 +2288,64 @@
     ) as call:
         client.update_deployment()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.UpdateDeploymentRequest()
 
 
+def test_update_deployment_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.UpdateDeploymentRequest(
+        request_id="request_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_deployment), "__call__"
+    ) as call:
+        client.update_deployment(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.UpdateDeploymentRequest(
+            request_id="request_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_update_deployment_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.update_deployment), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.update_deployment()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.UpdateDeploymentRequest()
+
+
 @pytest.mark.asyncio
 async def test_update_deployment_async(
     transport: str = "grpc_asyncio", request_type=config.UpdateDeploymentRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2135,15 +2364,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.update_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.UpdateDeploymentRequest()
+        request = config.UpdateDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_update_deployment_async_from_dict():
@@ -2355,15 +2585,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.delete_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.DeleteDeploymentRequest()
+        request = config.DeleteDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_delete_deployment_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -2379,14 +2610,66 @@
     ) as call:
         client.delete_deployment()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.DeleteDeploymentRequest()
 
 
+def test_delete_deployment_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.DeleteDeploymentRequest(
+        name="name_value",
+        request_id="request_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_deployment), "__call__"
+    ) as call:
+        client.delete_deployment(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.DeleteDeploymentRequest(
+            name="name_value",
+            request_id="request_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_deployment_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.delete_deployment), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.delete_deployment()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.DeleteDeploymentRequest()
+
+
 @pytest.mark.asyncio
 async def test_delete_deployment_async(
     transport: str = "grpc_asyncio", request_type=config.DeleteDeploymentRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2405,15 +2688,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.delete_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.DeleteDeploymentRequest()
+        request = config.DeleteDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_delete_deployment_async_from_dict():
@@ -2596,15 +2880,16 @@
             unreachable=["unreachable_value"],
         )
         response = client.list_revisions(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListRevisionsRequest()
+        request = config.ListRevisionsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListRevisionsPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -2620,14 +2905,69 @@
     with mock.patch.object(type(client.transport.list_revisions), "__call__") as call:
         client.list_revisions()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ListRevisionsRequest()
 
 
+def test_list_revisions_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ListRevisionsRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+        order_by="order_by_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_revisions), "__call__") as call:
+        client.list_revisions(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListRevisionsRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+            order_by="order_by_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_revisions_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_revisions), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.ListRevisionsResponse(
+                next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
+            )
+        )
+        response = await client.list_revisions()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListRevisionsRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_revisions_async(
     transport: str = "grpc_asyncio", request_type=config.ListRevisionsRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -2647,15 +2987,16 @@
             )
         )
         response = await client.list_revisions(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListRevisionsRequest()
+        request = config.ListRevisionsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListRevisionsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -3035,15 +3376,16 @@
             quota_validation=config.QuotaValidation.ENABLED,
         )
         response = client.get_revision(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetRevisionRequest()
+        request = config.GetRevisionRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Revision)
     assert response.name == "name_value"
     assert response.action == config.Revision.Action.CREATE
     assert response.state == config.Revision.State.APPLYING
     assert response.state_detail == "state_detail_value"
@@ -3074,14 +3416,76 @@
     with mock.patch.object(type(client.transport.get_revision), "__call__") as call:
         client.get_revision()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.GetRevisionRequest()
 
 
+def test_get_revision_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.GetRevisionRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_revision), "__call__") as call:
+        client.get_revision(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetRevisionRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_revision_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_revision), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.Revision(
+                name="name_value",
+                action=config.Revision.Action.CREATE,
+                state=config.Revision.State.APPLYING,
+                state_detail="state_detail_value",
+                error_code=config.Revision.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED,
+                build="build_value",
+                logs="logs_value",
+                error_logs="error_logs_value",
+                service_account="service_account_value",
+                import_existing_resources=True,
+                worker_pool="worker_pool_value",
+                tf_version_constraint="tf_version_constraint_value",
+                tf_version="tf_version_value",
+                quota_validation_results="quota_validation_results_value",
+                quota_validation=config.QuotaValidation.ENABLED,
+            )
+        )
+        response = await client.get_revision()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetRevisionRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_revision_async(
     transport: str = "grpc_asyncio", request_type=config.GetRevisionRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3114,15 +3518,16 @@
             )
         )
         response = await client.get_revision(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetRevisionRequest()
+        request = config.GetRevisionRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Revision)
     assert response.name == "name_value"
     assert response.action == config.Revision.Action.CREATE
     assert response.state == config.Revision.State.APPLYING
     assert response.state_detail == "state_detail_value"
@@ -3311,15 +3716,16 @@
             state=config.Resource.State.PLANNED,
         )
         response = client.get_resource(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetResourceRequest()
+        request = config.GetResourceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Resource)
     assert response.name == "name_value"
     assert response.intent == config.Resource.Intent.CREATE
     assert response.state == config.Resource.State.PLANNED
 
@@ -3336,14 +3742,64 @@
     with mock.patch.object(type(client.transport.get_resource), "__call__") as call:
         client.get_resource()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.GetResourceRequest()
 
 
+def test_get_resource_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.GetResourceRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_resource), "__call__") as call:
+        client.get_resource(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetResourceRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_resource_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_resource), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.Resource(
+                name="name_value",
+                intent=config.Resource.Intent.CREATE,
+                state=config.Resource.State.PLANNED,
+            )
+        )
+        response = await client.get_resource()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetResourceRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_resource_async(
     transport: str = "grpc_asyncio", request_type=config.GetResourceRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3364,15 +3820,16 @@
             )
         )
         response = await client.get_resource(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetResourceRequest()
+        request = config.GetResourceRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Resource)
     assert response.name == "name_value"
     assert response.intent == config.Resource.Intent.CREATE
     assert response.state == config.Resource.State.PLANNED
 
@@ -3546,15 +4003,16 @@
             unreachable=["unreachable_value"],
         )
         response = client.list_resources(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListResourcesRequest()
+        request = config.ListResourcesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListResourcesPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -3570,14 +4028,69 @@
     with mock.patch.object(type(client.transport.list_resources), "__call__") as call:
         client.list_resources()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ListResourcesRequest()
 
 
+def test_list_resources_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ListResourcesRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+        order_by="order_by_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_resources), "__call__") as call:
+        client.list_resources(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListResourcesRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+            order_by="order_by_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_resources_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_resources), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.ListResourcesResponse(
+                next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
+            )
+        )
+        response = await client.list_resources()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListResourcesRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_resources_async(
     transport: str = "grpc_asyncio", request_type=config.ListResourcesRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -3597,15 +4110,16 @@
             )
         )
         response = await client.list_resources(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListResourcesRequest()
+        request = config.ListResourcesRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListResourcesAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -3973,15 +4487,16 @@
             signed_uri="signed_uri_value",
         )
         response = client.export_deployment_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportDeploymentStatefileRequest()
+        request = config.ExportDeploymentStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Statefile)
     assert response.signed_uri == "signed_uri_value"
 
 
 def test_export_deployment_statefile_empty_call():
@@ -3998,14 +4513,66 @@
     ) as call:
         client.export_deployment_statefile()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ExportDeploymentStatefileRequest()
 
 
+def test_export_deployment_statefile_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ExportDeploymentStatefileRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.export_deployment_statefile), "__call__"
+    ) as call:
+        client.export_deployment_statefile(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportDeploymentStatefileRequest(
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_export_deployment_statefile_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.export_deployment_statefile), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.Statefile(
+                signed_uri="signed_uri_value",
+            )
+        )
+        response = await client.export_deployment_statefile()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportDeploymentStatefileRequest()
+
+
 @pytest.mark.asyncio
 async def test_export_deployment_statefile_async(
     transport: str = "grpc_asyncio",
     request_type=config.ExportDeploymentStatefileRequest,
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -4027,15 +4594,16 @@
             )
         )
         response = await client.export_deployment_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportDeploymentStatefileRequest()
+        request = config.ExportDeploymentStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Statefile)
     assert response.signed_uri == "signed_uri_value"
 
 
 @pytest.mark.asyncio
@@ -4132,15 +4700,16 @@
             signed_uri="signed_uri_value",
         )
         response = client.export_revision_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportRevisionStatefileRequest()
+        request = config.ExportRevisionStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Statefile)
     assert response.signed_uri == "signed_uri_value"
 
 
 def test_export_revision_statefile_empty_call():
@@ -4157,14 +4726,66 @@
     ) as call:
         client.export_revision_statefile()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ExportRevisionStatefileRequest()
 
 
+def test_export_revision_statefile_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ExportRevisionStatefileRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.export_revision_statefile), "__call__"
+    ) as call:
+        client.export_revision_statefile(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportRevisionStatefileRequest(
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_export_revision_statefile_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.export_revision_statefile), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.Statefile(
+                signed_uri="signed_uri_value",
+            )
+        )
+        response = await client.export_revision_statefile()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportRevisionStatefileRequest()
+
+
 @pytest.mark.asyncio
 async def test_export_revision_statefile_async(
     transport: str = "grpc_asyncio", request_type=config.ExportRevisionStatefileRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -4185,15 +4806,16 @@
             )
         )
         response = await client.export_revision_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportRevisionStatefileRequest()
+        request = config.ExportRevisionStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Statefile)
     assert response.signed_uri == "signed_uri_value"
 
 
 @pytest.mark.asyncio
@@ -4288,15 +4910,16 @@
             signed_uri="signed_uri_value",
         )
         response = client.import_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ImportStatefileRequest()
+        request = config.ImportStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Statefile)
     assert response.signed_uri == "signed_uri_value"
 
 
 def test_import_statefile_empty_call():
@@ -4311,14 +4934,62 @@
     with mock.patch.object(type(client.transport.import_statefile), "__call__") as call:
         client.import_statefile()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ImportStatefileRequest()
 
 
+def test_import_statefile_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ImportStatefileRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_statefile), "__call__") as call:
+        client.import_statefile(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ImportStatefileRequest(
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_import_statefile_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.import_statefile), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.Statefile(
+                signed_uri="signed_uri_value",
+            )
+        )
+        response = await client.import_statefile()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ImportStatefileRequest()
+
+
 @pytest.mark.asyncio
 async def test_import_statefile_async(
     transport: str = "grpc_asyncio", request_type=config.ImportStatefileRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -4337,15 +5008,16 @@
             )
         )
         response = await client.import_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ImportStatefileRequest()
+        request = config.ImportStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Statefile)
     assert response.signed_uri == "signed_uri_value"
 
 
 @pytest.mark.asyncio
@@ -4524,15 +5196,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = None
         response = client.delete_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.DeleteStatefileRequest()
+        request = config.DeleteStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 def test_delete_statefile_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -4546,14 +5219,58 @@
     with mock.patch.object(type(client.transport.delete_statefile), "__call__") as call:
         client.delete_statefile()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.DeleteStatefileRequest()
 
 
+def test_delete_statefile_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.DeleteStatefileRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_statefile), "__call__") as call:
+        client.delete_statefile(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.DeleteStatefileRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_statefile_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_statefile), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
+        response = await client.delete_statefile()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.DeleteStatefileRequest()
+
+
 @pytest.mark.asyncio
 async def test_delete_statefile_async(
     transport: str = "grpc_asyncio", request_type=config.DeleteStatefileRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -4568,15 +5285,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(None)
         response = await client.delete_statefile(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.DeleteStatefileRequest()
+        request = config.DeleteStatefileRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert response is None
 
 
 @pytest.mark.asyncio
 async def test_delete_statefile_async_from_dict():
@@ -4744,15 +5462,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.lock_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.LockDeploymentRequest()
+        request = config.LockDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_lock_deployment_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -4766,14 +5485,60 @@
     with mock.patch.object(type(client.transport.lock_deployment), "__call__") as call:
         client.lock_deployment()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.LockDeploymentRequest()
 
 
+def test_lock_deployment_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.LockDeploymentRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.lock_deployment), "__call__") as call:
+        client.lock_deployment(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.LockDeploymentRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_lock_deployment_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.lock_deployment), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.lock_deployment()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.LockDeploymentRequest()
+
+
 @pytest.mark.asyncio
 async def test_lock_deployment_async(
     transport: str = "grpc_asyncio", request_type=config.LockDeploymentRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -4790,15 +5555,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.lock_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.LockDeploymentRequest()
+        request = config.LockDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_lock_deployment_async_from_dict():
@@ -4972,15 +5738,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.unlock_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.UnlockDeploymentRequest()
+        request = config.UnlockDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_unlock_deployment_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -4996,14 +5763,64 @@
     ) as call:
         client.unlock_deployment()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.UnlockDeploymentRequest()
 
 
+def test_unlock_deployment_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.UnlockDeploymentRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.unlock_deployment), "__call__"
+    ) as call:
+        client.unlock_deployment(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.UnlockDeploymentRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_unlock_deployment_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.unlock_deployment), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.unlock_deployment()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.UnlockDeploymentRequest()
+
+
 @pytest.mark.asyncio
 async def test_unlock_deployment_async(
     transport: str = "grpc_asyncio", request_type=config.UnlockDeploymentRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -5022,15 +5839,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.unlock_deployment(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.UnlockDeploymentRequest()
+        request = config.UnlockDeploymentRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_unlock_deployment_async_from_dict():
@@ -5226,15 +6044,16 @@
             version="version_value",
         )
         response = client.export_lock_info(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportLockInfoRequest()
+        request = config.ExportLockInfoRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.LockInfo)
     assert response.lock_id == 725
     assert response.operation == "operation_value"
     assert response.info == "info_value"
     assert response.who == "who_value"
@@ -5253,14 +6072,66 @@
     with mock.patch.object(type(client.transport.export_lock_info), "__call__") as call:
         client.export_lock_info()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ExportLockInfoRequest()
 
 
+def test_export_lock_info_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ExportLockInfoRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_lock_info), "__call__") as call:
+        client.export_lock_info(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportLockInfoRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_export_lock_info_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.export_lock_info), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.LockInfo(
+                lock_id=725,
+                operation="operation_value",
+                info="info_value",
+                who="who_value",
+                version="version_value",
+            )
+        )
+        response = await client.export_lock_info()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportLockInfoRequest()
+
+
 @pytest.mark.asyncio
 async def test_export_lock_info_async(
     transport: str = "grpc_asyncio", request_type=config.ExportLockInfoRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -5283,15 +6154,16 @@
             )
         )
         response = await client.export_lock_info(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportLockInfoRequest()
+        request = config.ExportLockInfoRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.LockInfo)
     assert response.lock_id == 725
     assert response.operation == "operation_value"
     assert response.info == "info_value"
     assert response.who == "who_value"
@@ -5464,15 +6336,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.create_preview(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.CreatePreviewRequest()
+        request = config.CreatePreviewRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_create_preview_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -5486,14 +6359,62 @@
     with mock.patch.object(type(client.transport.create_preview), "__call__") as call:
         client.create_preview()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.CreatePreviewRequest()
 
 
+def test_create_preview_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.CreatePreviewRequest(
+        parent="parent_value",
+        preview_id="preview_id_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_preview), "__call__") as call:
+        client.create_preview(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.CreatePreviewRequest(
+            parent="parent_value",
+            preview_id="preview_id_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_create_preview_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.create_preview), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.create_preview()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.CreatePreviewRequest()
+
+
 @pytest.mark.asyncio
 async def test_create_preview_async(
     transport: str = "grpc_asyncio", request_type=config.CreatePreviewRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -5510,15 +6431,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.create_preview(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.CreatePreviewRequest()
+        request = config.CreatePreviewRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_create_preview_async_from_dict():
@@ -5726,35 +6648,40 @@
             service_account="service_account_value",
             artifacts_gcs_bucket="artifacts_gcs_bucket_value",
             worker_pool="worker_pool_value",
             error_code=config.Preview.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED,
             build="build_value",
             error_logs="error_logs_value",
             logs="logs_value",
+            tf_version="tf_version_value",
+            tf_version_constraint="tf_version_constraint_value",
         )
         response = client.get_preview(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetPreviewRequest()
+        request = config.GetPreviewRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Preview)
     assert response.name == "name_value"
     assert response.state == config.Preview.State.CREATING
     assert response.deployment == "deployment_value"
     assert response.preview_mode == config.Preview.PreviewMode.DEFAULT
     assert response.service_account == "service_account_value"
     assert response.artifacts_gcs_bucket == "artifacts_gcs_bucket_value"
     assert response.worker_pool == "worker_pool_value"
     assert response.error_code == config.Preview.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED
     assert response.build == "build_value"
     assert response.error_logs == "error_logs_value"
     assert response.logs == "logs_value"
+    assert response.tf_version == "tf_version_value"
+    assert response.tf_version_constraint == "tf_version_constraint_value"
 
 
 def test_get_preview_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
     # i.e. request == None and no flattened fields passed, work.
     client = ConfigClient(
         credentials=ga_credentials.AnonymousCredentials(),
@@ -5765,14 +6692,74 @@
     with mock.patch.object(type(client.transport.get_preview), "__call__") as call:
         client.get_preview()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.GetPreviewRequest()
 
 
+def test_get_preview_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.GetPreviewRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_preview), "__call__") as call:
+        client.get_preview(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetPreviewRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_preview_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.get_preview), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.Preview(
+                name="name_value",
+                state=config.Preview.State.CREATING,
+                deployment="deployment_value",
+                preview_mode=config.Preview.PreviewMode.DEFAULT,
+                service_account="service_account_value",
+                artifacts_gcs_bucket="artifacts_gcs_bucket_value",
+                worker_pool="worker_pool_value",
+                error_code=config.Preview.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED,
+                build="build_value",
+                error_logs="error_logs_value",
+                logs="logs_value",
+                tf_version="tf_version_value",
+                tf_version_constraint="tf_version_constraint_value",
+            )
+        )
+        response = await client.get_preview()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetPreviewRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_preview_async(
     transport: str = "grpc_asyncio", request_type=config.GetPreviewRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -5794,36 +6781,41 @@
                 service_account="service_account_value",
                 artifacts_gcs_bucket="artifacts_gcs_bucket_value",
                 worker_pool="worker_pool_value",
                 error_code=config.Preview.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED,
                 build="build_value",
                 error_logs="error_logs_value",
                 logs="logs_value",
+                tf_version="tf_version_value",
+                tf_version_constraint="tf_version_constraint_value",
             )
         )
         response = await client.get_preview(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetPreviewRequest()
+        request = config.GetPreviewRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.Preview)
     assert response.name == "name_value"
     assert response.state == config.Preview.State.CREATING
     assert response.deployment == "deployment_value"
     assert response.preview_mode == config.Preview.PreviewMode.DEFAULT
     assert response.service_account == "service_account_value"
     assert response.artifacts_gcs_bucket == "artifacts_gcs_bucket_value"
     assert response.worker_pool == "worker_pool_value"
     assert response.error_code == config.Preview.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED
     assert response.build == "build_value"
     assert response.error_logs == "error_logs_value"
     assert response.logs == "logs_value"
+    assert response.tf_version == "tf_version_value"
+    assert response.tf_version_constraint == "tf_version_constraint_value"
 
 
 @pytest.mark.asyncio
 async def test_get_preview_async_from_dict():
     await test_get_preview_async(request_type=dict)
 
 
@@ -5991,15 +6983,16 @@
             unreachable=["unreachable_value"],
         )
         response = client.list_previews(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListPreviewsRequest()
+        request = config.ListPreviewsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListPreviewsPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -6015,14 +7008,69 @@
     with mock.patch.object(type(client.transport.list_previews), "__call__") as call:
         client.list_previews()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ListPreviewsRequest()
 
 
+def test_list_previews_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ListPreviewsRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+        order_by="order_by_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_previews), "__call__") as call:
+        client.list_previews(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListPreviewsRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+            order_by="order_by_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_previews_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.list_previews), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.ListPreviewsResponse(
+                next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
+            )
+        )
+        response = await client.list_previews()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListPreviewsRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_previews_async(
     transport: str = "grpc_asyncio", request_type=config.ListPreviewsRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -6042,15 +7090,16 @@
             )
         )
         response = await client.list_previews(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListPreviewsRequest()
+        request = config.ListPreviewsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListPreviewsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -6414,15 +7463,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = operations_pb2.Operation(name="operations/spam")
         response = client.delete_preview(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.DeletePreviewRequest()
+        request = config.DeletePreviewRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 def test_delete_preview_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -6436,14 +7486,60 @@
     with mock.patch.object(type(client.transport.delete_preview), "__call__") as call:
         client.delete_preview()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.DeletePreviewRequest()
 
 
+def test_delete_preview_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.DeletePreviewRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_preview), "__call__") as call:
+        client.delete_preview(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.DeletePreviewRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_delete_preview_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(type(client.transport.delete_preview), "__call__") as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            operations_pb2.Operation(name="operations/spam")
+        )
+        response = await client.delete_preview()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.DeletePreviewRequest()
+
+
 @pytest.mark.asyncio
 async def test_delete_preview_async(
     transport: str = "grpc_asyncio", request_type=config.DeletePreviewRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -6460,15 +7556,16 @@
             operations_pb2.Operation(name="operations/spam")
         )
         response = await client.delete_preview(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.DeletePreviewRequest()
+        request = config.DeletePreviewRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, future.Future)
 
 
 @pytest.mark.asyncio
 async def test_delete_preview_async_from_dict():
@@ -6642,15 +7739,16 @@
         # Designate an appropriate return value for the call.
         call.return_value = config.ExportPreviewResultResponse()
         response = client.export_preview_result(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportPreviewResultRequest()
+        request = config.ExportPreviewResultRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.ExportPreviewResultResponse)
 
 
 def test_export_preview_result_empty_call():
     # This test is a coverage failsafe to make sure that totally empty calls,
@@ -6666,14 +7764,64 @@
     ) as call:
         client.export_preview_result()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ExportPreviewResultRequest()
 
 
+def test_export_preview_result_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ExportPreviewResultRequest(
+        parent="parent_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.export_preview_result), "__call__"
+    ) as call:
+        client.export_preview_result(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportPreviewResultRequest(
+            parent="parent_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_export_preview_result_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.export_preview_result), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.ExportPreviewResultResponse()
+        )
+        response = await client.export_preview_result()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ExportPreviewResultRequest()
+
+
 @pytest.mark.asyncio
 async def test_export_preview_result_async(
     transport: str = "grpc_asyncio", request_type=config.ExportPreviewResultRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -6692,15 +7840,16 @@
             config.ExportPreviewResultResponse()
         )
         response = await client.export_preview_result(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ExportPreviewResultRequest()
+        request = config.ExportPreviewResultRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.ExportPreviewResultResponse)
 
 
 @pytest.mark.asyncio
 async def test_export_preview_result_async_from_dict():
@@ -6799,15 +7948,16 @@
             unreachable=["unreachable_value"],
         )
         response = client.list_terraform_versions(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListTerraformVersionsRequest()
+        request = config.ListTerraformVersionsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListTerraformVersionsPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -6825,14 +7975,73 @@
     ) as call:
         client.list_terraform_versions()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.ListTerraformVersionsRequest()
 
 
+def test_list_terraform_versions_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.ListTerraformVersionsRequest(
+        parent="parent_value",
+        page_token="page_token_value",
+        filter="filter_value",
+        order_by="order_by_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_terraform_versions), "__call__"
+    ) as call:
+        client.list_terraform_versions(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListTerraformVersionsRequest(
+            parent="parent_value",
+            page_token="page_token_value",
+            filter="filter_value",
+            order_by="order_by_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_list_terraform_versions_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.list_terraform_versions), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.ListTerraformVersionsResponse(
+                next_page_token="next_page_token_value",
+                unreachable=["unreachable_value"],
+            )
+        )
+        response = await client.list_terraform_versions()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.ListTerraformVersionsRequest()
+
+
 @pytest.mark.asyncio
 async def test_list_terraform_versions_async(
     transport: str = "grpc_asyncio", request_type=config.ListTerraformVersionsRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -6854,15 +8063,16 @@
             )
         )
         response = await client.list_terraform_versions(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.ListTerraformVersionsRequest()
+        request = config.ListTerraformVersionsRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, pagers.ListTerraformVersionsAsyncPager)
     assert response.next_page_token == "next_page_token_value"
     assert response.unreachable == ["unreachable_value"]
 
 
@@ -7247,15 +8457,16 @@
             state=config.TerraformVersion.State.ACTIVE,
         )
         response = client.get_terraform_version(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls) == 1
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetTerraformVersionRequest()
+        request = config.GetTerraformVersionRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.TerraformVersion)
     assert response.name == "name_value"
     assert response.state == config.TerraformVersion.State.ACTIVE
 
 
@@ -7273,14 +8484,67 @@
     ) as call:
         client.get_terraform_version()
         call.assert_called()
         _, args, _ = call.mock_calls[0]
         assert args[0] == config.GetTerraformVersionRequest()
 
 
+def test_get_terraform_version_non_empty_request_with_auto_populated_field():
+    # This test is a coverage failsafe to make sure that UUID4 fields are
+    # automatically populated, according to AIP-4235, with non-empty requests.
+    client = ConfigClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc",
+    )
+
+    # Populate all string fields in the request which are not UUID4
+    # since we want to check that UUID4 are populated automatically
+    # if they meet the requirements of AIP 4235.
+    request = config.GetTerraformVersionRequest(
+        name="name_value",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_terraform_version), "__call__"
+    ) as call:
+        client.get_terraform_version(request=request)
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetTerraformVersionRequest(
+            name="name_value",
+        )
+
+
+@pytest.mark.asyncio
+async def test_get_terraform_version_empty_call_async():
+    # This test is a coverage failsafe to make sure that totally empty calls,
+    # i.e. request == None and no flattened fields passed, work.
+    client = ConfigAsyncClient(
+        credentials=ga_credentials.AnonymousCredentials(),
+        transport="grpc_asyncio",
+    )
+
+    # Mock the actual call within the gRPC stub, and fake the request.
+    with mock.patch.object(
+        type(client.transport.get_terraform_version), "__call__"
+    ) as call:
+        # Designate an appropriate return value for the call.
+        call.return_value = grpc_helpers_async.FakeUnaryUnaryCall(
+            config.TerraformVersion(
+                name="name_value",
+                state=config.TerraformVersion.State.ACTIVE,
+            )
+        )
+        response = await client.get_terraform_version()
+        call.assert_called()
+        _, args, _ = call.mock_calls[0]
+        assert args[0] == config.GetTerraformVersionRequest()
+
+
 @pytest.mark.asyncio
 async def test_get_terraform_version_async(
     transport: str = "grpc_asyncio", request_type=config.GetTerraformVersionRequest
 ):
     client = ConfigAsyncClient(
         credentials=ga_credentials.AnonymousCredentials(),
         transport=transport,
@@ -7302,15 +8566,16 @@
             )
         )
         response = await client.get_terraform_version(request)
 
         # Establish that the underlying gRPC stub method was called.
         assert len(call.mock_calls)
         _, args, _ = call.mock_calls[0]
-        assert args[0] == config.GetTerraformVersionRequest()
+        request = config.GetTerraformVersionRequest()
+        assert args[0] == request
 
     # Establish that the response is the type that we expect.
     assert isinstance(response, config.TerraformVersion)
     assert response.name == "name_value"
     assert response.state == config.TerraformVersion.State.ACTIVE
 
 
@@ -8162,14 +9427,15 @@
         "service_account": "service_account_value",
         "import_existing_resources": True,
         "worker_pool": "worker_pool_value",
         "lock_state": 1,
         "tf_version_constraint": "tf_version_constraint_value",
         "tf_version": "tf_version_value",
         "quota_validation": 1,
+        "annotations": {},
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = config.CreateDeploymentRequest.meta.fields["deployment"]
@@ -8585,14 +9851,15 @@
         "service_account": "service_account_value",
         "import_existing_resources": True,
         "worker_pool": "worker_pool_value",
         "lock_state": 1,
         "tf_version_constraint": "tf_version_constraint_value",
         "tf_version": "tf_version_value",
         "quota_validation": 1,
+        "annotations": {},
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = config.UpdateDeploymentRequest.meta.fields["deployment"]
@@ -12261,14 +13528,16 @@
         ],
         "error_logs": "error_logs_value",
         "preview_artifacts": {
             "content": "content_value",
             "artifacts": "artifacts_value",
         },
         "logs": "logs_value",
+        "tf_version": "tf_version_value",
+        "tf_version_constraint": "tf_version_constraint_value",
     }
     # The version of a generated dependency at test runtime may differ from the version used during generation.
     # Delete any fields which are not present in the current runtime dependency
     # See https://github.com/googleapis/gapic-generator-python/issues/1748
 
     # Determine if the message type is proto-plus or protobuf
     test_field = config.CreatePreviewRequest.meta.fields["preview"]
@@ -12629,14 +13898,16 @@
             service_account="service_account_value",
             artifacts_gcs_bucket="artifacts_gcs_bucket_value",
             worker_pool="worker_pool_value",
             error_code=config.Preview.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED,
             build="build_value",
             error_logs="error_logs_value",
             logs="logs_value",
+            tf_version="tf_version_value",
+            tf_version_constraint="tf_version_constraint_value",
         )
 
         # Wrap the value into a proper Response obj
         response_value = Response()
         response_value.status_code = 200
         # Convert return value to protobuf type
         return_value = config.Preview.pb(return_value)
@@ -12655,14 +13926,16 @@
     assert response.service_account == "service_account_value"
     assert response.artifacts_gcs_bucket == "artifacts_gcs_bucket_value"
     assert response.worker_pool == "worker_pool_value"
     assert response.error_code == config.Preview.ErrorCode.CLOUD_BUILD_PERMISSION_DENIED
     assert response.build == "build_value"
     assert response.error_logs == "error_logs_value"
     assert response.logs == "logs_value"
+    assert response.tf_version == "tf_version_value"
+    assert response.tf_version_constraint == "tf_version_constraint_value"
 
 
 def test_get_preview_rest_required_fields(request_type=config.GetPreviewRequest):
     transport_class = transports.ConfigRestTransport
 
     request_init = {}
     request_init["name"] = ""
```

