# Comparing `tmp/cdsapi-0.5.1.tar.gz` & `tmp/cdsapi-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsapi-0.5.1.tar", last modified: Tue Feb  9 17:12:28 2021, max compression
+gzip compressed data, was "cdsapi-0.6.1.tar", last modified: Thu Mar 16 14:34:55 2023, max compression
```

## Comparing `cdsapi-0.5.1.tar` & `cdsapi-0.6.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 17:12:28.153052 cdsapi-0.5.1/
--rw-r--r--   0 runner    (1001) docker     (116)     1134 2021-02-09 17:12:18.000000 cdsapi-0.5.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (116)    10174 2021-02-09 17:12:18.000000 cdsapi-0.5.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (116)      204 2021-02-09 17:12:18.000000 cdsapi-0.5.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     3079 2021-02-09 17:12:28.153052 cdsapi-0.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     1736 2021-02-09 17:12:18.000000 cdsapi-0.5.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 17:12:28.153052 cdsapi-0.5.1/cdsapi/
--rw-r--r--   0 runner    (1001) docker     (116)      946 2021-02-09 17:12:18.000000 cdsapi-0.5.1/cdsapi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    18844 2021-02-09 17:12:18.000000 cdsapi-0.5.1/cdsapi/api.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 17:12:28.153052 cdsapi-0.5.1/cdsapi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     3079 2021-02-09 17:12:27.000000 cdsapi-0.5.1/cdsapi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      362 2021-02-09 17:12:28.000000 cdsapi-0.5.1/cdsapi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-09 17:12:27.000000 cdsapi-0.5.1/cdsapi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       21 2021-02-09 17:12:27.000000 cdsapi-0.5.1/cdsapi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)        7 2021-02-09 17:12:27.000000 cdsapi-0.5.1/cdsapi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2021-02-09 17:12:27.000000 cdsapi-0.5.1/cdsapi.egg-info/zip-safe
--rwxr-xr-x   0 runner    (1001) docker     (116)      675 2021-02-09 17:12:18.000000 cdsapi-0.5.1/example-era5.py
--rwxr-xr-x   0 runner    (1001) docker     (116)      564 2021-02-09 17:12:18.000000 cdsapi-0.5.1/example-glaciers.py
--rw-r--r--   0 runner    (1001) docker     (116)      227 2021-02-09 17:12:28.153052 cdsapi-0.5.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     2122 2021-02-09 17:12:18.000000 cdsapi-0.5.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2021-02-09 17:12:28.153052 cdsapi-0.5.1/tests/
--rw-r--r--   0 runner    (1001) docker     (116)       94 2021-02-09 17:12:18.000000 cdsapi-0.5.1/tests/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (116)      374 2021-02-09 17:12:18.000000 cdsapi-0.5.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (116)      437 2021-02-09 17:12:18.000000 cdsapi-0.5.1/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:34:55.768443 cdsapi-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-03-16 14:34:45.000000 cdsapi-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-03-16 14:34:45.000000 cdsapi-0.6.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-03-16 14:34:45.000000 cdsapi-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-03-16 14:34:55.768443 cdsapi-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1746 2023-03-16 14:34:45.000000 cdsapi-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:34:55.764443 cdsapi-0.6.1/cdsapi/
+-rw-r--r--   0 runner    (1001) docker     (123)      946 2023-03-16 14:34:45.000000 cdsapi-0.6.1/cdsapi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19579 2023-03-16 14:34:45.000000 cdsapi-0.6.1/cdsapi/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:34:55.764443 cdsapi-0.6.1/cdsapi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3092 2023-03-16 14:34:55.000000 cdsapi-0.6.1/cdsapi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-16 14:34:55.000000 cdsapi-0.6.1/cdsapi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 14:34:55.000000 cdsapi-0.6.1/cdsapi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-03-16 14:34:55.000000 cdsapi-0.6.1/cdsapi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-03-16 14:34:55.000000 cdsapi-0.6.1/cdsapi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-16 14:34:55.000000 cdsapi-0.6.1/cdsapi.egg-info/zip-safe
+-rwxr-xr-x   0 runner    (1001) docker     (123)      675 2023-03-16 14:34:45.000000 cdsapi-0.6.1/example-era5.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      564 2023-03-16 14:34:45.000000 cdsapi-0.6.1/example-glaciers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      227 2023-03-16 14:34:55.768443 cdsapi-0.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-03-16 14:34:45.000000 cdsapi-0.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-16 14:34:55.768443 cdsapi-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-03-16 14:34:45.000000 cdsapi-0.6.1/tests/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-03-16 14:34:45.000000 cdsapi-0.6.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-03-16 14:34:45.000000 cdsapi-0.6.1/tox.ini
```

### Comparing `cdsapi-0.5.1/CONTRIBUTING.rst` & `cdsapi-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cdsapi-0.5.1/LICENSE.txt` & `cdsapi-0.6.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cdsapi-0.5.1/PKG-INFO` & `cdsapi-0.6.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdsapi
-Version: 0.5.1
+Version: 0.6.1
 Summary: Climate Data Store API
 Home-page: https://github.com/ecmwf/cdsapi
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description: 
         Install
@@ -14,15 +14,15 @@
         
             $ pip install cdsapi
         
         
         Configure
         ---------
         
-        Get your UID and API key from the CDS portal at the address https://cds.climate.copernicus.eu/user
+        Get your user ID (UID) and API key from the CDS portal at the address https://cds.climate.copernicus.eu/user
         and write it into the configuration file, so it looks like::
         
             $ cat ~/.cdsapirc
             url: https://cds.climate.copernicus.eu/api/v2
             key: <UID>:<API key>
             verify: 0
         
@@ -66,19 +66,19 @@
         limitations under the License.
         
         In applying this licence, ECMWF does not waive the privileges and immunities
         granted to it by virtue of its status as an intergovernmental organisation nor
         does it submit to any jurisdiction.
         
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
```

### Comparing `cdsapi-0.5.1/README.rst` & `cdsapi-0.6.1/README.rst`

 * *Files 5% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     $ pip install cdsapi
 
 
 Configure
 ---------
 
-Get your UID and API key from the CDS portal at the address https://cds.climate.copernicus.eu/user
+Get your user ID (UID) and API key from the CDS portal at the address https://cds.climate.copernicus.eu/user
 and write it into the configuration file, so it looks like::
 
     $ cat ~/.cdsapirc
     url: https://cds.climate.copernicus.eu/api/v2
     key: <UID>:<API key>
     verify: 0
```

### Comparing `cdsapi-0.5.1/cdsapi/__init__.py` & `cdsapi-0.6.1/cdsapi/__init__.py`

 * *Files identical despite different names*

### Comparing `cdsapi-0.5.1/cdsapi/api.py` & `cdsapi-0.6.1/cdsapi/api.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,18 +5,20 @@
 # In applying this licence, ECMWF does not waive the privileges and immunities
 # granted to it by virtue of its status as an intergovernmental organisation nor
 # does it submit to any jurisdiction.
 
 from __future__ import absolute_import, division, print_function, unicode_literals
 
 import json
-import time
-import os
 import logging
+import os
+import time
 import uuid
+
+import pkg_resources
 import requests
 
 try:
     from urllib.parse import urljoin
 except ImportError:
     from urlparse import urljoin
 
@@ -31,24 +33,23 @@
         i += 1
     return "%g%s" % (int(n * 10 + 0.5) / 10.0, u[i])
 
 
 def read_config(path):
     config = {}
     with open(path) as f:
-        for l in f.readlines():
-            if ":" in l:
-                k, v = l.strip().split(":", 1)
+        for line in f.readlines():
+            if ":" in line:
+                k, v = line.strip().split(":", 1)
                 if k in ("url", "key", "verify"):
                     config[k] = v.strip()
     return config
 
 
 def toJSON(obj):
-
     to_json = getattr(obj, "toJSON", None)
     if callable(to_json):
         return to_json()
 
     if isinstance(obj, (list, tuple)):
         return [toJSON(x) for x in obj]
 
@@ -59,15 +60,14 @@
         return r
 
     return obj
 
 
 class Result(object):
     def __init__(self, client, reply):
-
         self.reply = reply
 
         self._url = client.url
 
         self.session = client.session
         self.robust = client.robust
         self.verify = client.verify
@@ -91,29 +91,27 @@
             contentType=self.content_type,
             contentLength=self.content_length,
             location=self.location,
         )
         return r
 
     def _download(self, url, size, target):
-
         if target is None:
             target = url.split("/")[-1]
 
         self.info("Downloading %s to %s (%s)", url, target, bytes_to_string(size))
         start = time.time()
 
         mode = "wb"
         total = 0
         sleep = 10
         tries = 0
         headers = None
 
         while tries < self.retry_max:
-
             r = self.robust(self.session.get)(
                 url,
                 stream=True,
                 verify=self.verify,
                 headers=headers,
                 timeout=self.timeout,
             )
@@ -202,30 +200,33 @@
 
     def update(self, request_id=None):
         if request_id is None:
             request_id = self.reply["request_id"]
         task_url = "%s/tasks/%s" % (self._url, request_id)
         self.debug("GET %s", task_url)
 
-        result = self.robust(self.session.get)(task_url, verify=self.verify)
+        result = self.robust(self.session.get)(
+            task_url, verify=self.verify, timeout=self.timeout
+        )
         result.raise_for_status()
         self.reply = result.json()
 
     def delete(self):
-
         if self._deleted:
             return
 
         if "request_id" in self.reply:
             rid = self.reply["request_id"]
 
             task_url = "%s/tasks/%s" % (self._url, rid)
             self.debug("DELETE %s", task_url)
 
-            delete = self.session.delete(task_url, verify=self.verify)
+            delete = self.session.delete(
+                task_url, verify=self.verify, timeout=self.timeout
+            )
             self.debug("DELETE returns %s %s", delete.status_code, delete.reason)
 
             try:
                 delete.raise_for_status()
             except Exception:
                 self.warning(
                     "DELETE %s returns %s %s",
@@ -241,15 +242,14 @@
             if self.cleanup:
                 self.delete()
         except Exception as e:
             print(e)
 
 
 class Client(object):
-
     logger = logging.getLogger("cdsapi")
 
     def __init__(
         self,
         url=os.environ.get("CDSAPI_URL"),
         key=os.environ.get("CDSAPI_KEY"),
         quiet=False,
@@ -266,44 +266,51 @@
         warning_callback=None,
         error_callback=None,
         debug_callback=None,
         metadata=None,
         forget=False,
         session=requests.Session(),
     ):
-
         if not quiet:
-
             if debug:
                 level = logging.DEBUG
             else:
                 level = logging.INFO
 
-            logging.basicConfig(
-                level=level, format="%(asctime)s %(levelname)s %(message)s"
-            )
+            self.logger.setLevel(level)
+
+            # avoid duplicate handlers when creating more than one Client
+            if not self.logger.handlers:
+                formatter = logging.Formatter("%(asctime)s %(levelname)s %(message)s")
+                handler = logging.StreamHandler()
+                handler.setFormatter(formatter)
+                self.logger.addHandler(handler)
 
         dotrc = os.environ.get("CDSAPI_RC", os.path.expanduser("~/.cdsapirc"))
 
         if url is None or key is None:
             if os.path.exists(dotrc):
                 config = read_config(dotrc)
 
                 if key is None:
                     key = config.get("key")
 
                 if url is None:
                     url = config.get("url")
 
                 if verify is None:
-                    verify = int(config.get("verify", 1))
+                    verify = bool(int(config.get("verify", 1)))
 
         if url is None or key is None or key is None:
             raise Exception("Missing/incomplete configuration file: %s" % (dotrc))
 
+        # If verify is still None, then we set to default value of True
+        if verify is None:
+            verify = True
+
         self.url = url
         self.key = key
 
         self.quiet = quiet
         self.progress = progress and not quiet
 
         self.verify = True if verify else False
@@ -318,14 +325,23 @@
         self.debug_callback = debug_callback
         self.warning_callback = warning_callback
         self.info_callback = info_callback
         self.error_callback = error_callback
 
         self.session = session
         self.session.auth = tuple(self.key.split(":", 2))
+        self.session.headers = {
+            "User-Agent": "cdsapi/%s"
+            % pkg_resources.get_distribution("cdsapi").version,
+        }
+
+        assert len(self.session.auth) == 2, (
+            "The cdsapi key provided is not the correct format, please ensure it conforms to:\n"
+            "<UID>:<APIKEY>"
+        )
 
         self.metadata = metadata
         self.forget = forget
 
         self.debug(
             "CDSAPI %s",
             dict(
@@ -349,15 +365,15 @@
         if target is not None:
             result.download(target)
         return result
 
     def service(self, name, *args, **kwargs):
         self.delete = False  # Don't delete results
         name = "/".join(name.split("."))
-        mimic_ui = kwargs.pop('mimic_ui', False)
+        mimic_ui = kwargs.pop("mimic_ui", False)
         # To mimic the CDS ui the request should be populated directly with the kwargs
         if mimic_ui:
             request = kwargs
         else:
             request = dict(args=args, kwargs=kwargs)
 
         if self.metadata:
@@ -373,15 +389,15 @@
     def workflow(self, code, *args, **kwargs):
         workflow_name = kwargs.pop("workflow_name", "application")
         params = dict(code=code, args=args, kwargs=kwargs, workflow_name=workflow_name)
         return self.service("tool.toolbox.orchestrator.run_workflow", params)
 
     def status(self, context=None):
         url = "%s/status.json" % (self.url,)
-        r = self.session.get(url, verify=self.verify)
+        r = self.session.get(url, verify=self.verify, timeout=self.timeout)
         r.raise_for_status()
         return r.json()
 
     def _status(self, url):
         try:
             status = self.status(url)
 
@@ -397,15 +413,14 @@
             for w in warning:
                 self.warning("%s", w)
 
         except Exception:
             pass
 
     def _api(self, url, request, method):
-
         self._status(url)
 
         session = self.session
 
         self.info("Sending request to %s", url)
         self.debug("%s %s %s", method, url, json.dumps(request))
 
@@ -423,15 +438,14 @@
 
         reply = None
 
         try:
             result.raise_for_status()
             reply = result.json()
         except Exception:
-
             if reply is None:
                 try:
                     reply = result.json()
                 except Exception:
                     reply = dict(message=result.text)
 
             self.debug(json.dumps(reply))
@@ -453,15 +467,14 @@
 
         if not self.wait_until_complete:
             return Result(self, reply)
 
         sleep = 1
 
         while True:
-
             self.debug("REPLY %s", reply)
 
             if reply["state"] != self.last_state:
                 self.info("Request is %s" % (reply["state"],))
                 self.last_state = reply["state"]
 
             if reply["state"] == "completed":
@@ -531,27 +544,25 @@
     def debug(self, *args, **kwargs):
         if self.debug_callback:
             self.debug_callback(*args, **kwargs)
         else:
             self.logger.debug(*args, **kwargs)
 
     def _download(self, results, targets=None):
-
         if isinstance(results, Result):
             if targets:
                 path = targets.pop(0)
             else:
                 path = None
             return results.download(path)
 
         if isinstance(results, (list, tuple)):
             return [self._download(x, targets) for x in results]
 
         if isinstance(results, dict):
-
             if "location" in results and "contentLength" in results:
                 reply = dict(
                     location=results["location"],
                     content_length=results["contentLength"],
                     content_type=results.get("contentType"),
                 )
 
@@ -582,59 +593,53 @@
             content_length=r.headers["Content-Length"],
             content_type=r.headers["Content-Type"],
         )
         return Result(self, reply)
 
     def robust(self, call):
         def retriable(code, reason):
-
             if code in [
                 requests.codes.internal_server_error,
                 requests.codes.bad_gateway,
                 requests.codes.service_unavailable,
                 requests.codes.gateway_timeout,
                 requests.codes.too_many_requests,
                 requests.codes.request_timeout,
             ]:
                 return True
 
             return False
 
         def wrapped(*args, **kwargs):
             tries = 0
-            while tries < self.retry_max:
+            while True:
+                txt = "Error"
                 try:
-                    r = call(*args, **kwargs)
+                    resp = call(*args, **kwargs)
                 except (
                     requests.exceptions.ConnectionError,
                     requests.exceptions.ReadTimeout,
                 ) as e:
-                    r = None
-                    self.warning(
-                        "Recovering from connection error [%s], attemps %s of %s",
-                        e,
-                        tries,
-                        self.retry_max,
-                    )
-
-                if r is not None:
-                    if not retriable(r.status_code, r.reason):
-                        return r
+                    resp = None
+                    txt = f"Connection error: [{e}]"
+
+                if resp is not None:
+                    if not retriable(resp.status_code, resp.reason):
+                        break
                     try:
-                        self.warning(r.json()["reason"])
+                        self.warning(resp.json()["reason"])
                     except Exception:
                         pass
-                    self.warning(
-                        "Recovering from HTTP error [%s %s], attemps %s of %s",
-                        r.status_code,
-                        r.reason,
-                        tries,
-                        self.retry_max,
-                    )
+                    txt = f"HTTP error: [{resp.status_code} {resp.reason}]"
 
                 tries += 1
+                self.warning(txt + f". Attempt {tries} of {self.retry_max}.")
+                if tries < self.retry_max:
+                    self.warning(f"Retrying in {self.sleep_max} seconds")
+                    time.sleep(self.sleep_max)
+                    self.info("Retrying now...")
+                else:
+                    raise Exception("Could not connect")
 
-                self.warning("Retrying in %s seconds", self.sleep_max)
-                time.sleep(self.sleep_max)
-                self.info("Retrying now...")
+            return resp
 
         return wrapped
```

### Comparing `cdsapi-0.5.1/cdsapi.egg-info/PKG-INFO` & `cdsapi-0.6.1/cdsapi.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: cdsapi
-Version: 0.5.1
+Version: 0.6.1
 Summary: Climate Data Store API
 Home-page: https://github.com/ecmwf/cdsapi
 Author: ECMWF
 Author-email: software.support@ecmwf.int
 License: Apache 2.0
 Description: 
         Install
@@ -14,15 +14,15 @@
         
             $ pip install cdsapi
         
         
         Configure
         ---------
         
-        Get your UID and API key from the CDS portal at the address https://cds.climate.copernicus.eu/user
+        Get your user ID (UID) and API key from the CDS portal at the address https://cds.climate.copernicus.eu/user
         and write it into the configuration file, so it looks like::
         
             $ cat ~/.cdsapirc
             url: https://cds.climate.copernicus.eu/api/v2
             key: <UID>:<API key>
             verify: 0
         
@@ -66,19 +66,19 @@
         limitations under the License.
         
         In applying this licence, ECMWF does not waive the privileges and immunities
         granted to it by virtue of its status as an intergovernmental organisation nor
         does it submit to any jurisdiction.
         
 Platform: UNKNOWN
-Classifier: Development Status :: 3 - Alpha
+Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 2
-Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Operating System :: OS Independent
```

### Comparing `cdsapi-0.5.1/example-era5.py` & `cdsapi-0.6.1/example-era5.py`

 * *Files identical despite different names*

### Comparing `cdsapi-0.5.1/example-glaciers.py` & `cdsapi-0.6.1/example-glaciers.py`

 * *Files identical despite different names*

### Comparing `cdsapi-0.5.1/setup.py` & `cdsapi-0.6.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
 
 def read(fname):
     file_path = os.path.join(os.path.dirname(__file__), fname)
     return io.open(file_path, encoding="utf-8").read()
 
 
-version = "0.5.1"
+version = "0.6.1"
 
 
 setuptools.setup(
     name="cdsapi",
     version=version,
     author="ECMWF",
     author_email="software.support@ecmwf.int",
@@ -46,21 +46,21 @@
     include_package_data=True,
     install_requires=[
         "requests>=2.5.0",
         "tqdm",
     ],
     zip_safe=True,
     classifiers=[
-        "Development Status :: 3 - Alpha",
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
-        "Programming Language :: Python :: 2",
-        "Programming Language :: Python :: 2.7",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.4",
-        "Programming Language :: Python :: 3.5",
-        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Operating System :: OS Independent",
     ],
 )
```

