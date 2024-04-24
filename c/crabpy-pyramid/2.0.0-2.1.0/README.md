# Comparing `tmp/crabpy_pyramid-2.0.0.tar.gz` & `tmp/crabpy_pyramid-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crabpy_pyramid-2.0.0.tar", last modified: Wed Dec 13 07:49:14 2023, max compression
+gzip compressed data, was "crabpy_pyramid-2.1.0.tar", last modified: Wed Apr 24 12:24:04 2024, max compression
```

## Comparing `crabpy_pyramid-2.0.0.tar` & `crabpy_pyramid-2.1.0.tar`

### file list

```diff
@@ -1,32 +1,33 @@
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5012 2023-12-13 07:49:13.000000 crabpy_pyramid-2.0.0/CHANGES.rst
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/LICENSE
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/MANIFEST.in
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7042 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/README.rst
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/crabpy_pyramid/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     9628 2023-12-13 07:49:13.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/__init__.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/crabpy_pyramid/renderers/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/renderers/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6961 2023-12-12 15:17:34.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/renderers/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/renderers/capakey.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/crabpy_pyramid/routes/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/routes/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3685 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/routes/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/routes/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/utils.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/crabpy_pyramid/views/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/views/__init__.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    12365 2023-12-12 15:17:34.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/views/adressenregister.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/views/capakey.py
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-11-24 09:37:50.000000 crabpy_pyramid-2.0.0/crabpy_pyramid/views/exceptions.py
-drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7042 2023-12-13 07:49:14.000000 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/PKG-INFO
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      747 2023-12-13 07:49:14.000000 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/SOURCES.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-12-13 07:49:14.000000 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/dependency_links.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2023-12-13 07:49:14.000000 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/entry_points.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-11-24 14:00:28.000000 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/not-zip-safe
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       43 2023-12-13 07:49:14.000000 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/requires.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2023-12-13 07:49:14.000000 crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/top_level.txt
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2023-12-13 07:49:14.987567 crabpy_pyramid-2.0.0/setup.cfg
--rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1485 2023-12-13 07:49:13.000000 crabpy_pyramid-2.0.0/setup.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-24 12:24:04.457818 crabpy_pyramid-2.1.0/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5185 2024-04-24 12:23:47.000000 crabpy_pyramid-2.1.0/CHANGES.rst
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1089 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/LICENSE
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       39 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/MANIFEST.in
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7215 2024-04-24 12:24:04.457818 crabpy_pyramid-2.1.0/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1326 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/README.rst
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-24 12:24:04.457818 crabpy_pyramid-2.1.0/crabpy_pyramid/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     9628 2024-04-24 08:14:54.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/__init__.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-24 12:24:04.457818 crabpy_pyramid-2.1.0/crabpy_pyramid/renderers/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/renderers/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     6961 2023-12-12 15:17:34.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/renderers/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3726 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/renderers/capakey.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-24 12:24:04.457818 crabpy_pyramid-2.1.0/crabpy_pyramid/routes/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/routes/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     3685 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/routes/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1901 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/routes/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     2735 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/utils.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-24 12:24:04.457818 crabpy_pyramid-2.1.0/crabpy_pyramid/views/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        0 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/views/__init__.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)    12696 2024-04-24 12:23:47.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/views/adressenregister.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     5610 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/views/capakey.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      599 2023-11-24 09:37:50.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/views/exceptions.py
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1503 2024-04-24 12:23:47.000000 crabpy_pyramid-2.1.0/crabpy_pyramid/views/utils.py
+drwxrwxr-x   0 claeyswo  (1001) claeyswo  (1001)        0 2024-04-24 12:24:04.457818 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     7215 2024-04-24 12:24:04.000000 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/PKG-INFO
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      777 2024-04-24 12:24:04.000000 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/SOURCES.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2024-04-24 12:24:04.000000 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/dependency_links.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       47 2024-04-24 12:24:04.000000 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/entry_points.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)        1 2023-11-24 14:00:28.000000 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/not-zip-safe
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       43 2024-04-24 12:24:04.000000 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/requires.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)       15 2024-04-24 12:24:04.000000 crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/top_level.txt
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)      173 2024-04-24 12:24:04.461818 crabpy_pyramid-2.1.0/setup.cfg
+-rw-rw-r--   0 claeyswo  (1001) claeyswo  (1001)     1485 2024-04-24 12:23:47.000000 crabpy_pyramid-2.1.0/setup.py
```

### Comparing `crabpy_pyramid-2.0.0/CHANGES.rst` & `crabpy_pyramid-2.1.0/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+2.1.0 (24-04-2024)
+------------------
+
+- HTTPNotFound niet altijd raisen bij lege list responses. (#196)
+- Query params ondersteunen bij zoeken in adressenregister (#195)
+
+
 2.0.0 (13-12-2023)
 ------------------
 
 - Remove crab (#208)
 
 1.8.0 (12-12-2023)
 ------------------
```

### Comparing `crabpy_pyramid-2.0.0/LICENSE` & `crabpy_pyramid-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/PKG-INFO` & `crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crabpy_pyramid
-Version: 2.0.0
+Name: crabpy-pyramid
+Version: 2.1.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,21 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+2.1.0 (24-04-2024)
+------------------
+
+- HTTPNotFound niet altijd raisen bij lege list responses. (#196)
+- Query params ondersteunen bij zoeken in adressenregister (#195)
+
+
 2.0.0 (13-12-2023)
 ------------------
 
 - Remove crab (#208)
 
 1.8.0 (12-12-2023)
 ------------------
```

### Comparing `crabpy_pyramid-2.0.0/README.rst` & `crabpy_pyramid-2.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/__init__.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/__init__.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/renderers/adressenregister.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/renderers/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/renderers/capakey.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/renderers/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/routes/adressenregister.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/routes/adressenregister.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/routes/capakey.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/routes/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/utils.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/utils.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/views/adressenregister.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/views/adressenregister.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,40 +1,23 @@
+import inspect
 import logging
 import re
 
 import pycountry
-from crabpy.client import AdressenRegisterClientException
-from pyramid.httpexceptions import HTTPBadRequest
 from pyramid.httpexceptions import HTTPNotFound
 from pyramid.view import view_config
 
 from crabpy_pyramid.utils import range_return
 from crabpy_pyramid.utils import set_http_caching
+from crabpy_pyramid.views.utils import extract_valid_params
+from crabpy_pyramid.views.utils import handle_gateway_response
 
 log = logging.getLogger(__name__)
 
 
-def handle_gateway_response(gateway_method, *args, **kwargs):
-    try:
-        result = gateway_method(*args, **kwargs)
-        if not result:
-            raise HTTPNotFound()
-        return result
-    except AdressenRegisterClientException as ae:
-        cause = ae.__cause__
-        if hasattr(cause, "response"):
-            status_code = cause.response.status_code
-            if status_code == 404:
-                raise HTTPNotFound()
-            if status_code == 400:
-                detail = getattr(cause.response, "text", "")
-                raise HTTPBadRequest(detail=detail)
-        raise ae
-
-
 @view_config(
     route_name="adressenregister_list_gewesten",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def list_gewesten(request):
     request = set_http_caching(request, "adressenregister", "long")
@@ -60,14 +43,15 @@
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def list_provincies(request):
     request = set_http_caching(request, "adressenregister", "permanent")
     Gateway = request.adressenregister_gateway()
     gewest_niscode = request.matchdict.get("gewest_niscode")
+    handle_gateway_response(Gateway.get_gewest_by_niscode, gewest_niscode)
     provincies = handle_gateway_response(Gateway.list_provincies, gewest_niscode)
     return range_return(request, provincies)
 
 
 @view_config(
     route_name="adressenregister_get_provincie",
     renderer="adresreg_itemjson",
@@ -130,31 +114,34 @@
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def list_gemeenten_by_provincie(request):
     request = set_http_caching(request, "adressenregister", "long")
     Gateway = request.adressenregister_gateway()
     provincie_id = request.matchdict.get("provincie_niscode")
-    gemeenten = handle_gateway_response(
-        Gateway.list_gemeenten_by_provincie, provincie_id
-    )
+    provincie = handle_gateway_response(Gateway.get_provincie_by_niscode, provincie_id)
+    gemeenten = handle_gateway_response(Gateway.list_gemeenten_by_provincie, provincie)
 
     return range_return(request, gemeenten)
 
 
 @view_config(
     route_name="list_gemeenten_adressenregister",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def list_gemeenten_adressenregister(request):
     request = set_http_caching(request, "adressenregister", "long")
     Gateway = request.adressenregister_gateway()
+    method = Gateway.list_gemeenten
     gewest_niscode = request.matchdict.get("gewest_niscode")
-    gemeenten = handle_gateway_response(Gateway.list_gemeenten, gewest_niscode)
+    handle_gateway_response(Gateway.get_gewest_by_niscode, gewest_niscode)
+    kwargs = extract_valid_params(method, request)
+    kwargs["gewest_niscode"] = gewest_niscode
+    gemeenten = handle_gateway_response(method, **kwargs)
 
     return range_return(request, gemeenten)
 
 
 @view_config(
     route_name="get_gemeente_adressenregister",
     renderer="adresreg_itemjson",
@@ -172,19 +159,22 @@
     route_name="adressenregister_list_straten",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def list_straten(request):
     request = set_http_caching(request, "adressenregister", "short")
     Gateway = request.adressenregister_gateway()
+    method = Gateway.list_straten
     gemeente_niscode = request.matchdict.get("niscode")
-    include_homoniem = True if request.params.get("include_homoniem") else False
-    straten = handle_gateway_response(
-        Gateway.list_straten, gemeente_niscode, include_homoniem=include_homoniem
+    gemeente = handle_gateway_response(
+        Gateway.get_gemeente_by_niscode, gemeente_niscode
     )
+    kwargs = extract_valid_params(method, request)
+    kwargs["gemeente"] = gemeente
+    straten = handle_gateway_response(method, **kwargs)
 
     return range_return(request, straten)
 
 
 @view_config(
     route_name="adressenregister_get_straat_by_id",
     renderer="adresreg_itemjson",
@@ -202,59 +192,59 @@
     route_name="adressenregister_list_adressen",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def list_adressen_by_straat(request):
     request = set_http_caching(request, "adressenregister", "short")
     Gateway = request.adressenregister_gateway()
+    method = Gateway.list_adressen_with_params
     straat_id = request.matchdict.get("straat_id")
-    straten = handle_gateway_response(
-        Gateway.list_adressen_with_params, straatnaamObjectId=straat_id
-    )
+    handle_gateway_response(Gateway.get_straat_by_id, straat_id)
+    kwargs = extract_valid_params(method, request)
+    kwargs["straatnaamObjectId"] = straat_id
+    straten = handle_gateway_response(method, **kwargs)
 
     return range_return(request, straten)
 
 
 @view_config(
     route_name="adressenregister_get_adres_by_straat_and_huisnummer",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def adressenregister_get_adres_by_straat_huisnummer(request):
     request = set_http_caching(request, "adressenregister", "short")
     Gateway = request.adressenregister_gateway()
+    method = Gateway.list_adressen_with_params
     straat_id = request.matchdict.get("straat_id")
-    huisnummer = request.matchdict.get("huisnummer")
-    adressen = handle_gateway_response(
-        Gateway.list_adressen_with_params,
-        straatnaamObjectId=straat_id,
-        huisnummer=huisnummer,
-    )
+    handle_gateway_response(Gateway.get_straat_by_id, straat_id)
+    kwargs = extract_valid_params(method, request)
+    kwargs["straatnaamObjectId"] = straat_id
+    kwargs["huisnummer"] = request.matchdict.get("huisnummer")
+    adressen = handle_gateway_response(method, **kwargs)
 
     return range_return(request, adressen)
 
 
 @view_config(
     route_name="adressenregister_get_adres_by_straat_and_huisnummer_and_busnummer",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def adressenregister_get_adres_by_straat_huisnummer_busnummer(request):
     request = set_http_caching(request, "adressenregister", "short")
     Gateway = request.adressenregister_gateway()
+    method = Gateway.list_adressen_with_params
     straat_id = request.matchdict.get("straat_id")
-    huisnummer = request.matchdict.get("huisnummer")
-    busnummer = request.matchdict.get("busnummer")
-    adressen = handle_gateway_response(
-        Gateway.list_adressen_with_params,
-        straatnaamObjectId=straat_id,
-        huisnummer=huisnummer,
-        busnummer=busnummer,
-    )
-
+    handle_gateway_response(Gateway.get_straat_by_id, straat_id)
+    kwargs = extract_valid_params(method, request)
+    kwargs["straatnaamObjectId"] = straat_id
+    kwargs["huisnummer"] = request.matchdict.get("huisnummer")
+    kwargs["busnummer"] = request.matchdict.get("busnummer")
+    adressen = handle_gateway_response(method, **kwargs)
     return range_return(request, adressen)
 
 
 @view_config(
     route_name="adressenregister_get_adres_by_id",
     renderer="adresreg_itemjson",
     accept="application/json",
@@ -271,18 +261,20 @@
     route_name="adressenregister_list_percelen_by_adres",
     renderer="adresreg_listjson",
     accept="application/json",
 )
 def adressenregister_list_percelen_by_adres(request):
     request = set_http_caching(request, "adressenregister", "short")
     Gateway = request.adressenregister_gateway()
+    method = Gateway.list_percelen_with_params
     adres_id = request.matchdict.get("adres_id")
-    adressen = handle_gateway_response(
-        Gateway.list_percelen_with_params, adresObjectId=adres_id
-    )
+    handle_gateway_response(Gateway.get_adres_by_id, adres_id)
+    kwargs = extract_valid_params(method, request)
+    kwargs["adresObjectId"] = adres_id
+    adressen = handle_gateway_response(method, **kwargs)
 
     return range_return(request, adressen)
 
 
 @view_config(
     route_name="adressenregister_get_perceel_by_id",
     renderer="adresreg_itemjson",
```

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/views/capakey.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/views/capakey.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid/views/exceptions.py` & `crabpy_pyramid-2.1.0/crabpy_pyramid/views/exceptions.py`

 * *Files identical despite different names*

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/PKG-INFO` & `crabpy_pyramid-2.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: crabpy-pyramid
-Version: 2.0.0
+Name: crabpy_pyramid
+Version: 2.1.0
 Summary: Bindings for the CRABpy webservices and the Pyramid framework.
 Home-page: http://github.com/OnroerendErfgoed/crabpy_pyramid
 Author: Onroerend Erfgoed
 Author-email: ict@onroerenderfgoed.be
 License: MIT
 Keywords: web wsgi pyramid CRAB CAPAKEY AGIV
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,14 +48,21 @@
     # activate your virtual env
     $ pip install sphinx sphinxcontrib-httpdomain
     $ python setup.py develop
     $ cd docs
     $ make html
 
 
+2.1.0 (24-04-2024)
+------------------
+
+- HTTPNotFound niet altijd raisen bij lege list responses. (#196)
+- Query params ondersteunen bij zoeken in adressenregister (#195)
+
+
 2.0.0 (13-12-2023)
 ------------------
 
 - Remove crab (#208)
 
 1.8.0 (12-12-2023)
 ------------------
```

### Comparing `crabpy_pyramid-2.0.0/crabpy_pyramid.egg-info/SOURCES.txt` & `crabpy_pyramid-2.1.0/crabpy_pyramid.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -18,8 +18,9 @@
 crabpy_pyramid/renderers/capakey.py
 crabpy_pyramid/routes/__init__.py
 crabpy_pyramid/routes/adressenregister.py
 crabpy_pyramid/routes/capakey.py
 crabpy_pyramid/views/__init__.py
 crabpy_pyramid/views/adressenregister.py
 crabpy_pyramid/views/capakey.py
-crabpy_pyramid/views/exceptions.py
+crabpy_pyramid/views/exceptions.py
+crabpy_pyramid/views/utils.py
```

### Comparing `crabpy_pyramid-2.0.0/setup.py` & `crabpy_pyramid-2.1.0/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     'coverage',
     'webtest'
 ]
 
 testing_extras = tests_requires + []
 
 setup(name='crabpy_pyramid',
-      version='2.0.0',
+      version='2.1.0',
       description='Bindings for the CRABpy webservices and the Pyramid framework.',
       long_description=README + '\n\n' + CHANGES,
       classifiers=[
         'Development Status :: 5 - Production/Stable',
         "Programming Language :: Python",
         'Programming Language :: Python :: 3.8',
         "Framework :: Pyramid",
```

