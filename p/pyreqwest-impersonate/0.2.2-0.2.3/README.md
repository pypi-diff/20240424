# Comparing `tmp/pyreqwest_impersonate-0.2.2.tar.gz` & `tmp/pyreqwest_impersonate-0.2.3.tar.gz`

## Comparing `pyreqwest_impersonate-0.2.2.tar` & `pyreqwest_impersonate-0.2.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.2.2/Cargo.toml
--rw-r--r--   0     1001      127     5412 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/.gitignore
--rw-r--r--   0     1001      127     7501 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/README.md
--rw-r--r--   0     1001      127      271 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/benchmark/1_threads.csv
--rw-r--r--   0     1001      127      273 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/benchmark/4_threads.csv
--rw-r--r--   0     1001      127      343 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/benchmark/README.md
--rw-r--r--   0     1001      127     3299 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/benchmark/benchmark.py
--rw-r--r--   0     1001      127       83 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/benchmark/requirements.txt
--rw-r--r--   0     1001      127      799 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/benchmark/server.py
--rw-r--r--   0     1001      127    18795 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/src/lib.rs
--rw-r--r--   0     1001      127     2964 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/src/response.rs
--rw-r--r--   0     1001      127     3800 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/tests/test_client.py
--rw-r--r--   0     1001      127    47243 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/Cargo.lock
--rw-r--r--   0     1001      127     1151 2024-04-22 11:01:27.000000 pyreqwest_impersonate-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     8570 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      991 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.2.3/Cargo.toml
+-rw-r--r--   0     1001      127     5412 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/.gitignore
+-rw-r--r--   0     1001      127     7466 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/README.md
+-rw-r--r--   0     1001      127      272 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/benchmark/1_threads.csv
+-rw-r--r--   0     1001      127      273 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/benchmark/4_threads.csv
+-rw-r--r--   0     1001      127      343 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/benchmark/README.md
+-rw-r--r--   0     1001      127     3299 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/benchmark/benchmark.py
+-rw-r--r--   0     1001      127       83 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      799 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/benchmark/server.py
+-rw-r--r--   0     1001      127    19543 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/src/lib.rs
+-rw-r--r--   0     1001      127     3036 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/src/response.rs
+-rw-r--r--   0     1001      127     3800 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/tests/test_client.py
+-rw-r--r--   0     1001      127    47243 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/Cargo.lock
+-rw-r--r--   0     1001      127     1151 2024-04-24 19:12:11.000000 pyreqwest_impersonate-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     8535 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.2.3/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.2.2/Cargo.toml` & `pyreqwest_impersonate-0.2.3/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.2.2"
+version = "0.2.3"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
```

### Comparing `pyreqwest_impersonate-0.2.2/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.2.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.2.2/.gitignore` & `pyreqwest_impersonate-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.2.2/README.md` & `pyreqwest_impersonate-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,14 @@
 data = {"key1": "value1", "key2": "value2"}
 auth = ("user", "password")
 resp = client.post(url="https://httpbin.org/anything", data=data, auth=auth)
 print(response.content)  # Get the content as bytes
 print(response.cookies)  # Access cookies
 print(response.headers)  # Access headers
 print(response.json())  # Parse the content as JSON
-print(response.raw) # Raw response
 print(response.status_code)  # Access the status code
 print(response.text)  # Decode the content as text
 print(response.url)  # Access the URL
 ```
 ### II. AsyncClient
 
 TODO
```

### Comparing `pyreqwest_impersonate-0.2.2/benchmark/benchmark.py` & `pyreqwest_impersonate-0.2.3/benchmark/benchmark.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.2.2/benchmark/server.py` & `pyreqwest_impersonate-0.2.3/benchmark/server.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.2.2/src/lib.rs` & `pyreqwest_impersonate-0.2.3/src/lib.rs`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use std::collections::HashMap;
 use std::str::FromStr;
 use std::time::Duration;
 
 use pyo3::exceptions;
 use pyo3::prelude::*;
+use pyo3::types::PyBytes;
+use pyo3::types::{PyDict, PyString};
 use reqwest_impersonate::blocking::multipart;
 use reqwest_impersonate::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest_impersonate::impersonate::Impersonate;
 use reqwest_impersonate::redirect::Policy;
 use reqwest_impersonate::Method;
 
 mod response;
@@ -202,14 +204,15 @@
     /// * `Response` - A response object containing the server's response to the request.
     ///
     /// # Errors
     ///
     /// * `PyException` - If there is an error making the request.
     fn request(
         &self,
+        py: Python,
         method: &str,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<HashMap<String, String>>,
         files: Option<HashMap<String, String>>,
@@ -303,144 +306,163 @@
         }
 
         // Timeout
         if let Some(seconds) = timeout {
             request_builder = request_builder.timeout(Duration::from_secs_f64(seconds));
         }
 
-        // Send request
-        let mut resp = Python::with_gil(|py| {
-            py.allow_threads(|| {
-                request_builder.send().map_err(|e| {
-                    PyErr::new::<exceptions::PyException, _>(format!("Error in request: {}", e))
-                })
+        // Send request | release GIL
+        let resp = py.allow_threads(|| {
+            request_builder.send().map_err(|e| {
+                PyErr::new::<exceptions::PyException, _>(format!("Error in request: {}", e))
             })
         })?;
 
         // Response items
-        let mut raw: Vec<u8> = vec![];
-        resp.copy_to(&mut raw).map_err(|e| {
-            PyErr::new::<exceptions::PyIOError, _>(format!("Error in get resp.raw: {}", e))
-        })?;
-        let cookies: HashMap<String, String> = resp
-            .cookies()
-            .map(|cookie| (cookie.name().to_string(), cookie.value().to_string()))
-            .collect();
+        let cookies_dict = PyDict::new_bound(py);
+        for cookie in resp.cookies() {
+            let key = cookie.name().to_string();
+            let value = cookie.value().to_string();
+            cookies_dict.set_item(key, value)?;
+        }
+        let cookies = cookies_dict.unbind();
+
         // Encoding from "Content-Type" header or "UTF-8"
-        let encoding = resp
-            .headers()
-            .get("Content-Type")
-            .and_then(|ct| ct.to_str().ok())
-            .and_then(|ct| {
-                ct.split(';').find_map(|param| {
-                    let mut kv = param.splitn(2, '=');
-                    let key = kv.next()?.trim();
-                    let value = kv.next()?.trim();
-                    if key.eq_ignore_ascii_case("charset") {
-                        Some(value.to_string())
-                    } else {
-                        None
-                    }
+        let encoding = {
+            let encoding_str = resp
+                .headers()
+                .get("Content-Type")
+                .and_then(|ct| ct.to_str().ok())
+                .and_then(|ct| {
+                    ct.split(';').find_map(|param| {
+                        let mut kv = param.splitn(2, '=');
+                        let key = kv.next()?.trim();
+                        let value = kv.next()?.trim();
+                        if key.eq_ignore_ascii_case("charset") {
+                            Some(value.to_string())
+                        } else {
+                            None
+                        }
+                    })
                 })
-            })
-            .unwrap_or("UTF-8".to_string());
-        let headers: HashMap<String, String> = resp
-            .headers()
-            .iter()
-            .map(|(k, v)| (k.as_str().to_string(), v.to_str().unwrap_or("").to_string()))
-            .collect();
-        let status_code = resp.status().as_u16();
-        let url = resp.url().to_string();
+                .unwrap_or("UTF-8".to_string());
+            PyString::new_bound(py, &encoding_str).unbind()
+        };
+
+        let headers_dict = PyDict::new_bound(py);
+        for (key, value) in resp.headers().iter() {
+            let key_str = key.as_str();
+            let value_str = value.to_str().unwrap_or("");
+            headers_dict.set_item(key_str, value_str)?;
+        }
+        let headers = headers_dict.unbind();
+
+        let status_code = resp.status().as_u16().into_py(py);
+
+        let url = PyString::new_bound(py, &resp.url().to_string()).into();
+
+        let buf = resp.bytes().map_err(|e| {
+            PyErr::new::<exceptions::PyException, _>(format!("Error reading response bytes: {}", e))
+        })?;
+        let content = PyBytes::new_bound(py, &buf).unbind();
 
         Ok(Response {
+            content,
             cookies,
             encoding,
             headers,
-            raw,
             status_code,
             url,
         })
     }
 
     fn get(
         &self,
         url: &str,
+        py: Python,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
+            py,
             "GET",
             url,
             params,
             headers,
             None,
             None,
             None,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn head(
         &self,
+        py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
+            py,
             "HEAD",
             url,
             params,
             headers,
             None,
             None,
             None,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn options(
         &self,
+        py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
+            py,
             "OPTIONS",
             url,
             params,
             headers,
             None,
             None,
             None,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn delete(
         &self,
+        py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
+            py,
             "DELETE",
             url,
             params,
             headers,
             None,
             None,
             None,
@@ -448,75 +470,81 @@
             auth_bearer,
             timeout,
         )
     }
 
     fn post(
         &self,
+        py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<HashMap<String, String>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
+            py,
             "POST",
             url,
             params,
             headers,
             content,
             data,
             files,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn put(
         &self,
+        py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<HashMap<String, String>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
+            py,
             "PUT",
             url,
             params,
             headers,
             content,
             data,
             files,
             auth,
             auth_bearer,
             timeout,
         )
     }
     fn patch(
         &self,
+        py: Python,
         url: &str,
         params: Option<HashMap<String, String>>,
         headers: Option<HashMap<String, String>>,
         content: Option<Vec<u8>>,
         data: Option<HashMap<String, String>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
         self.request(
+            py,
             "PATCH",
             url,
             params,
             headers,
             content,
             data,
             files,
```

### Comparing `pyreqwest_impersonate-0.2.2/src/response.rs` & `pyreqwest_impersonate-0.2.3/src/response.rs`

 * *Files 14% similar despite different names*

```diff
@@ -1,85 +1,83 @@
-use std::collections::HashMap;
-
 use encoding_rs::*;
 use pyo3::exceptions;
 use pyo3::prelude::*;
-use pyo3::types::PyBytes;
+use pyo3::types::{PyBytes, PyDict, PyString};
 use pythonize::pythonize;
 use serde_json::{Error as SerdeError, Value};
 
 /// A struct representing an HTTP response.
 ///
 /// This struct provides methods to access various parts of an HTTP response, such as headers, cookies, status code, and the response body.
 /// It also supports decoding the response body as text or JSON, with the ability to specify the character encoding.
 #[pyclass]
 pub struct Response {
     #[pyo3(get)]
-    pub cookies: HashMap<String, String>,
+    pub content: Py<PyBytes>,
     #[pyo3(get)]
-    pub encoding: String,
+    pub cookies: Py<PyDict>,
     #[pyo3(get)]
-    pub headers: HashMap<String, String>,
+    pub encoding: Py<PyString>,
     #[pyo3(get)]
-    pub raw: Vec<u8>,
+    pub headers: Py<PyDict>,
     #[pyo3(get)]
-    pub status_code: u16,
+    pub status_code: Py<PyAny>,
     #[pyo3(get)]
-    pub url: String,
+    pub url: Py<PyAny>,
 }
 
 #[pymethods]
 impl Response {
     #[getter]
-    fn content(&mut self) -> PyResult<PyObject> {
-        Python::with_gil(|py| {
-            // Convert the raw response body to PyBytes
-            let py_bytes = PyBytes::new_bound(py, &self.raw);
+    fn text(&mut self, py: Python) -> PyResult<String> {
+        // Access the string data as bytes
+        let encoding_bytes = &self.encoding.bind(py).to_string().as_bytes().to_vec();
+
+        // Convert Py<PyBytes> to &[u8]
+        let raw_bytes = &self.content.bind(py).as_bytes();
+
+        // Release the GIL here because decoding can be CPU-intensive
+        let (decoded_str, detected_encoding_name) = py.allow_threads(move || {
+            let encoding = Encoding::for_label(&encoding_bytes).ok_or_else(|| {
+                PyErr::new::<exceptions::PyValueError, _>(format!(
+                    "Unsupported charset: {}",
+                    String::from_utf8_lossy(&encoding_bytes)
+                ))
+            })?;
+            let (decoded_str, detected_encoding, _) = encoding.decode(&raw_bytes);
+            // Return the decoded string and the name of the detected encoding
+            Ok::<(String, String), PyErr>((
+                decoded_str.to_string(),
+                detected_encoding.name().to_string(),
+            ))
+        })?;
+
+        // Update self.encoding based on the detected encoding
+        if self.encoding.bind(py).to_string() != detected_encoding_name {
+            self.encoding = PyString::new_bound(py, &detected_encoding_name).into();
+        }
 
-            // Convert the PyBytes to a Python object
-            Ok(py_bytes.into())
-        })
+        Ok(decoded_str)
     }
 
-    #[getter]
-    fn text(&mut self) -> PyResult<String> {
-        Python::with_gil(|py| {
-            // Release the GIL here because decoding can be CPU-intensive.
-            py.allow_threads(|| {
-                let encoding = Encoding::for_label(&self.encoding.as_bytes()).ok_or_else(|| {
-                    PyErr::new::<exceptions::PyValueError, _>(format!(
-                        "Unsupported charset: {}",
-                        self.encoding
-                    ))
-                })?;
-                let (decoded_str, detected_encoding, _) = encoding.decode(&self.raw);
-                // Redefine resp.encoding if detected_encoding != charset
-                if detected_encoding != encoding {
-                    self.encoding = detected_encoding.name().to_string();
-                }
-                Ok(decoded_str.to_string())
-            })
-        })
-    }
-
-    fn json(&mut self) -> PyResult<PyObject> {
-        Python::with_gil(|py| {
-            // Directly parse the raw response body as JSON
-            // We release the GIL here because JSON parsing can be CPU-intensive.
-            let value: Result<Value, SerdeError> =
-                py.allow_threads(|| serde_json::from_slice(&self.raw));
-
-            // Manually convert the serde_json::Error into a pyo3::PyErr
-            let json_value = value.map_err(|e| {
-                PyErr::new::<exceptions::PyValueError, _>(format!("Failed to parse JSON: {}", e))
-            })?;
-
-            // Convert the parsed JSON into a Python object using pythonize
-            pythonize(py, &json_value).map_err(|e| {
-                PyErr::new::<exceptions::PyValueError, _>(format!(
-                    "Failed to convert JSON to Python object: {}",
-                    e
-                ))
-            })
+    fn json(&mut self, py: Python) -> PyResult<PyObject> {
+        // Convert Py<PyBytes> to &[u8]
+        let raw_bytes = &self.content.bind(py).as_bytes();
+
+        // Release the GIL here because JSON parsing can be CPU-intensive
+        let value: Result<Value, SerdeError> =
+            py.allow_threads(|| serde_json::from_slice(raw_bytes));
+
+        // Manually convert the serde_json::Error into a pyo3::PyErr
+        let json_value = value.map_err(|e| {
+            PyErr::new::<exceptions::PyValueError, _>(format!("Failed to parse JSON: {}", e))
+        })?;
+
+        // Convert the parsed JSON into a Python object using pythonize
+        pythonize(py, &json_value).map_err(|e| {
+            PyErr::new::<exceptions::PyValueError, _>(format!(
+                "Failed to convert JSON to Python object: {}",
+                e
+            ))
         })
     }
 }
```

### Comparing `pyreqwest_impersonate-0.2.2/tests/test_client.py` & `pyreqwest_impersonate-0.2.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.2.2/Cargo.lock` & `pyreqwest_impersonate-0.2.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1003,15 +1003,15 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.2.2"
+version = "0.2.3"
 dependencies = [
  "encoding_rs",
  "pyo3",
  "pythonize",
  "reqwest-impersonate",
  "serde_json",
 ]
```

### Comparing `pyreqwest_impersonate-0.2.2/pyproject.toml` & `pyreqwest_impersonate-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.2.2/PKG-INFO` & `pyreqwest_impersonate-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.2.2
+Version: 0.2.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -142,15 +142,14 @@
 data = {"key1": "value1", "key2": "value2"}
 auth = ("user", "password")
 resp = client.post(url="https://httpbin.org/anything", data=data, auth=auth)
 print(response.content)  # Get the content as bytes
 print(response.cookies)  # Access cookies
 print(response.headers)  # Access headers
 print(response.json())  # Parse the content as JSON
-print(response.raw) # Raw response
 print(response.status_code)  # Access the status code
 print(response.text)  # Decode the content as text
 print(response.url)  # Access the URL
 ```
 ### II. AsyncClient
 
 TODO
```

