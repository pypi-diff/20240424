# Comparing `tmp/oteltest-0.8.0.tar.gz` & `tmp/oteltest-0.9.0.tar.gz`

## Comparing `oteltest-0.8.0.tar` & `oteltest-0.9.0.tar`

### file list

```diff
@@ -1,19 +1,15 @@
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/client_server.0.json
--rw-r--r--   0        0        0     4256 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/client_server.1.json
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/client_server.py
--rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/simple_loop.0.json
--rw-r--r--   0        0        0     7637 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/simple_loop.1.json
--rwxr-xr-x   0        0        0     1438 2020-02-02 00:00:00.000000 oteltest-0.8.0/example_scripts/simple_loop.py
--rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/__init__.py
--rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/main.py
--rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/private.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/version.py
--rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/sink/__init__.py
--rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.8.0/src/oteltest/sink/private.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.8.0/tests/__init__.py
--rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 oteltest-0.8.0/tests/test_oteltest.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.8.0/.gitignore
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.8.0/LICENSE.txt
--rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 oteltest-0.8.0/README.md
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 oteltest-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 oteltest-0.9.0/example_scripts/client_server.py
+-rwxr-xr-x   0        0        0     1438 2020-02-02 00:00:00.000000 oteltest-0.9.0/example_scripts/simple_loop.py
+-rw-r--r--   0        0        0     6168 2020-02-02 00:00:00.000000 oteltest-0.9.0/src/oteltest/__init__.py
+-rw-r--r--   0        0        0     1408 2020-02-02 00:00:00.000000 oteltest-0.9.0/src/oteltest/main.py
+-rw-r--r--   0        0        0     6767 2020-02-02 00:00:00.000000 oteltest-0.9.0/src/oteltest/private.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 oteltest-0.9.0/src/oteltest/version.py
+-rw-r--r--   0        0        0     3729 2020-02-02 00:00:00.000000 oteltest-0.9.0/src/oteltest/sink/__init__.py
+-rw-r--r--   0        0        0     1672 2020-02-02 00:00:00.000000 oteltest-0.9.0/src/oteltest/sink/private.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.9.0/tests/__init__.py
+-rw-r--r--   0        0        0      616 2020-02-02 00:00:00.000000 oteltest-0.9.0/tests/test_oteltest.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 oteltest-0.9.0/.gitignore
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 oteltest-0.9.0/LICENSE.txt
+-rw-r--r--   0        0        0     3606 2020-02-02 00:00:00.000000 oteltest-0.9.0/README.md
+-rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 oteltest-0.9.0/pyproject.toml
+-rw-r--r--   0        0        0     4728 2020-02-02 00:00:00.000000 oteltest-0.9.0/PKG-INFO
```

### Comparing `oteltest-0.8.0/example_scripts/client_server.py` & `oteltest-0.9.0/example_scripts/client_server.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/example_scripts/simple_loop.py` & `oteltest-0.9.0/example_scripts/simple_loop.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/src/oteltest/__init__.py` & `oteltest-0.9.0/src/oteltest/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/src/oteltest/main.py` & `oteltest-0.9.0/src/oteltest/main.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/src/oteltest/private.py` & `oteltest-0.9.0/src/oteltest/private.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/src/oteltest/version.py` & `oteltest-0.9.0/tests/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,9 +7,7 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
-
-__version__ = "0.8.0"
```

### Comparing `oteltest-0.8.0/src/oteltest/sink/__init__.py` & `oteltest-0.9.0/src/oteltest/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/src/oteltest/sink/private.py` & `oteltest-0.9.0/src/oteltest/sink/private.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/tests/__init__.py` & `oteltest-0.9.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/tests/test_oteltest.py` & `oteltest-0.9.0/tests/test_oteltest.py`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/.gitignore` & `oteltest-0.9.0/.gitignore`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/LICENSE.txt` & `oteltest-0.9.0/src/oteltest/version.py`

 * *Files 26% similar despite different names*

```diff
@@ -7,7 +7,9 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+
+__version__ = "0.9.0"
```

### Comparing `oteltest-0.8.0/README.md` & `oteltest-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/pyproject.toml` & `oteltest-0.9.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `oteltest-0.8.0/PKG-INFO` & `oteltest-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: oteltest
-Version: 0.8.0
+Version: 0.9.0
 Summary: OpenTelemetry Tester
 Project-URL: Documentation, https://github.com/open-telemetry/opentelemetry-python#readme
 Project-URL: Issues, https://github.com/open-telemetry/opentelemetry-python/issues
 Project-URL: Source, https://github.com/open-telemetry/opentelemetry-python/
 Author-email: OpenTelemetry Authors <cncf-opentelemetry-contributors@lists.cncf.io>
 License-Expression: Apache-2.0
 License-File: LICENSE.txt
```

