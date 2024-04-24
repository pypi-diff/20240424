# Comparing `tmp/armis-1.0.18.tar.gz` & `tmp/armis-1.0.19.tar.gz`

## Comparing `armis-1.0.18.tar` & `armis-1.0.19.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 armis-1.0.18/requirements.txt
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 armis-1.0.18/src/armis/__about__.py
--rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 armis-1.0.18/src/armis/__init__.py
--rwxr-xr-x   0        0        0    40209 2020-02-02 00:00:00.000000 armis-1.0.18/src/armis/armiscloud.py
--rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_apicalls.py
--rwxr-xr-x   0        0        0      675 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_boundaries.py
--rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_ceiling.py
--rwxr-xr-x   0        0        0      500 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_collectors.py
--rwxr-xr-x   0        0        0     1516 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_devices.py
--rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_fixture.py
--rwxr-xr-x   0        0        0      785 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_integrations.py
--rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_notimplemented.py
--rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_objectcreation.py
--rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_sites.py
--rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 armis-1.0.18/tests/test_tagging.py
--rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 armis-1.0.18/.gitignore
--rw-r--r--   0        0        0     3233 2020-02-02 00:00:00.000000 armis-1.0.18/README.md
--rw-r--r--   0        0        0     4913 2020-02-02 00:00:00.000000 armis-1.0.18/pyproject.toml
--rw-r--r--   0        0        0     4506 2020-02-02 00:00:00.000000 armis-1.0.18/PKG-INFO
+-rw-r--r--   0        0        0       88 2020-02-02 00:00:00.000000 armis-1.0.19/requirements.txt
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 armis-1.0.19/src/armis/__about__.py
+-rw-r--r--   0        0        0      149 2020-02-02 00:00:00.000000 armis-1.0.19/src/armis/__init__.py
+-rwxr-xr-x   0        0        0    46696 2020-02-02 00:00:00.000000 armis-1.0.19/src/armis/armiscloud.py
+-rwxr-xr-x   0        0        0     3008 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_apicalls.py
+-rwxr-xr-x   0        0        0      801 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_boundaries.py
+-rwxr-xr-x   0        0        0      838 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_ceiling.py
+-rwxr-xr-x   0        0        0      500 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_collectors.py
+-rwxr-xr-x   0        0        0     1516 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_devices.py
+-rwxr-xr-x   0        0        0      722 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_fixture.py
+-rwxr-xr-x   0        0        0     1143 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_integrations.py
+-rwxr-xr-x   0        0        0      102 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_notimplemented.py
+-rwxr-xr-x   0        0        0     1643 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_objectcreation.py
+-rwxr-xr-x   0        0        0      414 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_sites.py
+-rwxr-xr-x   0        0        0     1299 2020-02-02 00:00:00.000000 armis-1.0.19/tests/test_tagging.py
+-rw-r--r--   0        0        0     1558 2020-02-02 00:00:00.000000 armis-1.0.19/.gitignore
+-rw-r--r--   0        0        0     4218 2020-02-02 00:00:00.000000 armis-1.0.19/README.md
+-rw-r--r--   0        0        0     4927 2020-02-02 00:00:00.000000 armis-1.0.19/pyproject.toml
+-rw-r--r--   0        0        0     5498 2020-02-02 00:00:00.000000 armis-1.0.19/PKG-INFO
```

### Comparing `armis-1.0.18/src/armis/armiscloud.py` & `armis-1.0.19/src/armis/armiscloud.py`

 * *Files 18% similar despite different names*

```diff
@@ -161,25 +161,38 @@
 
         return math.ceil(number / nearest) * nearest
 
     def _get_httpx_client(self):
         with contextlib.suppress(AttributeError):
             self.httpx_client.close()
 
-        httpx_client = httpx.Client(
+        return httpx.Client(
+            event_hooks={
+                "response": [self._httpx_callback_request_raise_4xx_5xx],
+            },
             follow_redirects=True,
             headers={
                 "user-agent": f"Armis Python Library {__version__}",
             },
             http2=True,
             limits=self._httpx_limits,
             timeout=self._http_timeout,
             trust_env=False,
         )
-        return httpx_client  # noqa: RET504
+
+    def _httpx_callback_request_raise_4xx_5xx(self, response):
+        self.log.debug(
+            "_httpx_callback_request_raise_4xx_5xx raising alert, status_code=%s",
+            response.status_code,
+        )
+
+        if response.status_code == httpx.codes.UNAUTHORIZED:
+            self.log.debug("401 unauthorized, our token probably expired")
+            self.authorization_token_expiration = 0
+            response.raise_for_status()
 
     def _api_http_request(self, **kwargs):
         """Wrap the request function and handles the authorization token.
 
         Parameters
         ----------
         method : str
@@ -322,14 +335,17 @@
                         )
                     else:
                         r = self.httpx_client.request(
                             "DELETE",
                             str(url),
                             headers=headers,
                         )
+                        # this usually returns a 204, so no text will be present
+                        # just return the result
+                        return r  # noqa: RET504
 
                 self.log.debug("response http version=%s", str(r.http_version))
 
                 try:
                     _ = self._json_decoder.decode(r.text)
                 except msgspec.DecodeError as err:
                     self.log.critical("exception: %s", str(err))
@@ -355,17 +371,17 @@
         self.log.debug("remaining_time=%s", str(remaining_time))
 
         if remaining_time < 1_000:
             self.log.debug("remaining_time < 1000")
             self.log.debug("expires=%s", str(self._authorization_token_expiration))
             self.log.debug("now > _authorization_token_expiration")
             self.log.debug("_authorization_token expired, getting new one")
-            url = str(self.TENANT_BASE_URL / "v1/access_token/")
+            url = self.TENANT_BASE_URL / "v1/access_token/"
             r = self.httpx_client.post(
-                url,
+                str(url),
                 data={
                     "secret_key": self.API_SECRET_KEY,
                 },
             )
             returnjson = self._json_decoder.decode(r.text)
             self.log.info("returnjson=%s", str(returnjson))
 
@@ -389,14 +405,116 @@
             self.log.debug("expires=%s", str(self._authorization_token_expiration))
             self.log.debug("now < _authorization_token_expiration")
 
         self.httpx_client.headers["Authorization"] = self._authorization_token
 
         self.log.debug("END")
 
+    def create_boundary(self, **kwargs) -> dict:
+        """Update a boundary given a boundary_id, name, and ruleaql.
+
+        Parameters
+        ----------
+        name : str
+            new name of the boundary
+        affected_sites : str|list, optional
+            sites affected
+        ruleaql : dict
+            aql to define the boundary
+
+        Returns
+        -------
+        creation_results : dict
+
+        Notes
+        -----
+        The cloud must be running at version >= R-23.3-S182.
+        """
+        self.log.debug("kwargs=%s", str(kwargs))
+
+        affected_sites = kwargs.get("affected_sites", None)
+        name = kwargs.get("name", None)
+        ruleaql = kwargs.get("ruleaql", None)
+
+        if name is None and ruleaql is None:
+            raise ValueError("name and ruleaql are required")
+        if name is None:
+            raise ValueError("name is required")
+        if ruleaql is None:
+            raise ValueError("ruleaql is required")
+
+        boundary_payload = {
+            "name": name,
+            "ruleAql": ruleaql,
+        }
+
+        if affected_sites is not None:
+            if isinstance(affected_sites, list):
+                self.log.debug(
+                    "affected_types was list, converting to a comma-delimited str",
+                )
+                # check if there is a comma in the name
+                # we can't update a boundary using an affected site with a comma in it
+                for affected_site in affected_sites:
+                    if "," in affected_site:
+                        raise ValueError(
+                            "Site '"
+                            + affected_site
+                            + "' contains a comma - Armis API doesn't support this",
+                        )
+
+                affected_sites = ",".join(affected_sites)
+
+            boundary_payload["affectedSites"] = affected_sites
+
+        self.log.debug("payload is now %s", str(boundary_payload))
+
+        # create the boundary
+        url = self.TENANT_BASE_URL / "v1/boundaries/"
+        self.log.debug("url=%s", str(url))
+        boundary_create = self._api_http_request(
+            method="POST",
+            url=url,
+            json=boundary_payload,
+        )
+        self.log.debug("return text=%s", str(boundary_create.text))
+        self.log.debug("status_code=%s", str(boundary_create.status_code))
+
+        # when creating a boundary, you get 201 back if it was created
+        if boundary_create.status_code != httpx.codes.CREATED:
+            self.log.info("FAILED boundary create for name: %s", str(name))
+            self.log.debug(boundary_create.text)
+            raise Exception("boundary update issue", boundary_create.text)
+
+        return self._json_decoder.decode(boundary_create.text)
+
+    def delete_boundary(self, boundary_id: int) -> dict:
+        """Delete a boundary given a boundary_id.
+
+        Parameters
+        ----------
+        boundary_id : int
+            The ID of the boundary tool to retrieve.
+
+        Returns
+        -------
+        delete_results : dict
+        """
+        url = self.TENANT_BASE_URL / f"v1/boundaries/{boundary_id}/"
+        self.log.debug("url=%s", str(url))
+        boundary_delete = self._api_http_request(method="DELETE", url=url)
+        if boundary_delete.status_code != httpx.codes.NO_CONTENT:
+            self.log.critical("STATUS CODE != 204")
+            self.log.critical("status_code=%s", str(boundary_delete.status_code))
+            raise Exception("boundary_delete issue", boundary_delete.text)
+
+        if boundary_delete.status_code == httpx.codes.NO_CONTENT:
+            return {"success": True}
+        return {"success": False}
+
     def get_boundary(self, boundary_id: int) -> dict:
         """Get a boundary given a boundary_id.
 
         Parameters
         ----------
         boundary_id : int
             The ID of the boundary tool to retrieve.
@@ -405,37 +523,40 @@
         -------
             boundary : dict
 
         Notes
         -----
         The cloud must be running at version >= R-23.3-S182.
         """
-        # boundary_id = kwargs.get("boundary_id", None)
-
         if boundary_id is None:
             raise ValueError("Need a boundary_id to continue")
 
-        url = self.TENANT_BASE_URL / "v1/boundaries" / str(boundary_id) / "/"
+        url = self.TENANT_BASE_URL / f"v1/boundaries/{boundary_id}/"
+
         self.log.debug("url=%s", str(url))
         boundary_details = self._api_http_request(method="GET", url=url)
 
         if boundary_details.status_code != httpx.codes.OK:
             self.log.critical("STATUS CODE != 200")
             self.log.critical("status_code=%s", str(boundary_details.status_code))
             self.log.critical("text=%s", boundary_details.text)
 
         return self._json_decoder.decode(boundary_details.text)["data"]
 
     def get_boundaries(self) -> dict:
-        """Get a list of boundaries.  Only works for cloud version >= R-23.3-S182.
+        """Get a list of boundaries.
 
         Returns
         -------
         boundaries : dict
             A dict of boundaries with the boundary_id as the key
+
+        Notes
+        -----
+        The cloud must be running at version >= R-23.3-S182.
         """
         url = self.TENANT_BASE_URL / "v1/boundaries/"
         url.args["from"] = 0
         url.args["length"] = self.ARMIS_API_PAGE_SIZE
         url.args["includeTotal"] = "true"
 
         boundaries = {}
@@ -468,22 +589,22 @@
 
         Parameters
         ----------
         boundary_id : int
             Armis boundary_id
         name : str
             new name of the boundary
-        affected_sites : str|list, optional
+        affected_sites : str | list, optional
             sites affected
         ruleaql : dict
             ASQ to define the boundary
 
         Notes
         -----
-        Only applies to cloud version >= R-23.3-S182.
+        The cloud must be running at version >= R-23.3-S182.
         """
         self.log.debug("kwargs=%s", str(kwargs))
 
         boundary_id = kwargs.get("boundary_id", None)
         if boundary_id is None:
             raise ValueError("No boundary_id provided")
 
@@ -529,15 +650,15 @@
                 if key not in boundary_update_payload:
                     self.log.debug('"%s" not in payload, adding it', key)
                     boundary_update_payload[key] = boundaryfromcloud[key]
 
         self.log.debug("payload is now %s", str(boundary_update_payload))
 
         # PATCH the boundary
-        url = self.TENANT_BASE_URL / "v1" / "boundaries" / str(boundary_id) / "/"
+        url = self.TENANT_BASE_URL / f"v1/boundaries/{boundary_id}/"
         self.log.debug("url=%s", str(url))
         boundary_update = self._api_http_request(
             method="PATCH",
             url=url,
             json=boundary_update_payload,
         )
         self.log.debug("return text=%s", str(boundary_update.text))
@@ -546,39 +667,183 @@
             self.log.info(
                 "FAILED boundary update for boundary_id: %s",
                 str(boundary_id),
             )
             self.log.debug(boundary_update.text)
             raise Exception("boundary update issue", boundary_update.text)
 
+    def get_collector(self, collector_id: int) -> dict:
+        """Get a collector given the collector_id.
+
+        Parameters
+        ----------
+        collector_id: int
+            The collector ID to fetch details about.
+
+        Returns
+        -------
+        collectors_dict: dict
+            A dictionary of a collector.
+        """
+        if collector_id is None:
+            raise ValueError("collector_id is required")
+
+        self.log.info("collector_id=%s", str(collector_id))
+        url = self.TENANT_BASE_URL / f"v1/collectors/{collector_id}/"
+
+        self.log.debug("url=%s", str(url))
+        collector_request = self._api_http_request(method="GET", url=url)
+        if collector_request.status_code != httpx.codes.OK:
+            raise Exception("collector issue", collector_request.text)
+
+        return self._json_decoder.decode(collector_request.text)["data"]
+
+    def get_collectors(self) -> dict:
+        """Get a dictionary of collectors.
+
+        Returns
+        -------
+        collectors_inventory: dict
+            A dictionary of collectors.
+
+        """
+        url = self.TENANT_BASE_URL / "v1/collectors/"
+        url.args["from"] = 0
+        url.args["length"] = self.ARMIS_API_PAGE_SIZE
+        collectors_inventory = {}
+
+        while url.args["from"] is not None:
+            self.log.info(
+                "fetching %s-%s",
+                str(url.args["from"]),
+                str(url.args["from"] + self.ARMIS_API_PAGE_SIZE),
+            )
+            get_collectors_request = self._api_http_request(method="GET", url=url)
+            if get_collectors_request.status_code != httpx.codes.OK:
+                self.log.critical("STATUS CODE != 200")
+                self.log.critical(
+                    "status_code=%s",
+                    str(get_collectors_request.status_code),
+                )
+                self.log.critical("text=%s", get_collectors_request.text)
+                self.log.critical("continuing")
+                continue
+
+            collectors_response = self._json_decoder.decode(get_collectors_request.text)
+            collectors_count = collectors_response["data"]["count"]
+            self.log.debug("retrieved %s collectors", str(collectors_count))
+
+            for collector in collectors_response["data"]["collectors"]:
+                collectornumber = collector["collectorNumber"]
+                collectors_inventory[collectornumber] = collector
+
+            self.log.debug(
+                "collectors next=%s",
+                str(collectors_response["data"]["next"]),
+            )
+            url.args["from"] = collectors_response["data"]["next"]
+
+        self.log.debug("collectors_inventory size=%s", str(len(collectors_inventory)))
+
+        if len(collectors_inventory) > 0:
+            collectors_inventory = dict(sorted(collectors_inventory.items()))
+        return collectors_inventory
+
+    def get_collectors_count(self) -> int:
+        """Get a count of collectors.
+
+        Returns
+        -------
+        collectors_count: int
+            A count of collectors.
+
+        """
+        self.log.info("get_collectors_count")
+        url = self.TENANT_BASE_URL / "v1/collectors/"
+        self.log.debug("url=%s", str(url))
+        url.args["length"] = 1
+        collectors_count_request = self._api_http_request(method="GET", url=url)
+        collectors_count = int(
+            self._json_decoder.decode(collectors_count_request.text)["data"]["total"],
+        )
+        self.log.debug("collectors_count=%s", str(collectors_count))
+        return collectors_count
+
+    def rename_collector(self, **kwargs) -> dict:
+        """Rename a collector given the collector_id.
+
+        Parameters
+        ----------
+        collector_id: int
+            The collector ID to rename
+        new_name: str
+            New name of the collector
+
+        Returns
+        -------
+        dict
+            JSON data as a dict.
+        """
+        collector_id = kwargs.get("collector_id", None)
+        new_name = kwargs.get("new_name", None)
+
+        if collector_id is None:
+            raise ValueError("collector_id is required")
+        if new_name is None:
+            raise ValueError("new_name is required")
+
+        # patch
+        url = self.TENANT_BASE_URL / f"v1/collectors/{collector_id}/"
+
+        rename_collector_payload = {
+            "name": new_name,
+        }
+        collector_update = self._api_http_request(
+            method="PATCH",
+            url=url,
+            json=rename_collector_payload,
+        )
+        self.log.debug("return text=%s", str(collector_update.text))
+        self.log.debug("status_code=%s", str(collector_update.status_code))
+        if collector_update.status_code != httpx.codes.OK:
+            self.log.info(
+                "FAILED collector rename for collector_id=%s, new_name=%s",
+                str(collector_id),
+                new_name,
+            )
+            self.log.debug(collector_update.text)
+            raise Exception("collector rename issue", collector_update.text)
+
+        return self._json_decoder.decode(collector_update.text)
+
     def get_devices(self, **kwargs: dict) -> list:
         """Get devices from inventory matching ASQ.
 
         Parameters
         ----------
         asq : str
             ASQ to execute.
         fields_wanted : list
             List of fields wanted.
 
         Returns
         -------
-        inventory: list
+        inventory : list
             Inventory items matching ASQ.
         """
         get_devices_start = pendulum.now()
         asq = kwargs.get("asq", None)
         if asq is None:
             raise ValueError("no asq provided")
         self.log.info("asq=%s", asq)
 
         fields_wanted = kwargs.get("fields_wanted", [])
         self.log.info("fields_wanted=%s", str(",".join(fields_wanted)))
 
-        url = self.TENANT_BASE_URL / "v1" / "devices/"
+        url = self.TENANT_BASE_URL / "v1/devices/"
         url.args["search"] = asq
         url.args["from"] = 0
         url.args["length"] = self.ARMIS_API_PAGE_SIZE
 
         # NOTE:
         # From the API Guide v1.8:
         # Iterating over a set of results it is recommended best practice to
@@ -741,15 +1006,15 @@
         """
         asq = kwargs.get("asq", None)
 
         if asq is None:
             raise ValueError("asq is required")
         self.log.info("asq=%s", asq)
 
-        url = self.TENANT_BASE_URL / "v1" / "devices/"
+        url = self.TENANT_BASE_URL / "v1/devices/"
         url.args["search"] = asq
         url.args["length"] = 1
         url.args["from"] = 0
         url.args["fields"] = "id"
         self.log.debug("url=%s", str(url))
 
         inventory_total_request = self._api_http_request(method="GET", url=url)
@@ -768,17 +1033,17 @@
     def tag_device(self, **kwargs: dict) -> None:
         """Add or remove a device from a deviceid.
 
         Parameters
         ----------
         device_id : int
             Device ID to tag.
-        tags: list|str
+        tags : list | str
             Tags to add to or remove from the device ID.
-        action: {'add', 'remove'}
+        action : {'add', 'remove'}
             Action to perform, one of add or remove.
         """
         self.log.debug("tag_device")
         device_id = kwargs.get("device_id", None)
         if device_id is None:
             raise ValueError("no device_id specified")
 
@@ -798,15 +1063,16 @@
 
         if len(tags) == 0:
             raise ValueError("no tag provided")
 
         if action not in {"add", "remove"}:
             raise ValueError("no valid action provided, should be one of add or remove")
 
-        url = self.TENANT_BASE_URL / "v1" / "devices" / str(device_id) / "tags/"
+        url = self.TENANT_BASE_URL / f"v1/devices/{device_id}/tags/"
+
         self.log.debug("url=%s", str(url))
 
         tag_payload = {"tags": tags}
         self.log.debug("json currently=%s", str(tag_payload))
         self.log.info(
             "tagging, action=%s, deviceid=%s, tags=%s",
             action,
@@ -832,90 +1098,14 @@
         if tag_device_update.status_code != httpx.codes.OK:
             self.log.info("FAILED DEVICE TAG for device ID: %s", str(device_id))
             self.log.debug(tag_device_update.text)
             raise Exception("tag_device_update issue", tag_device_update.text)
 
         return tag_device_update.text
 
-    def get_collector(self, collector_id: int) -> dict:
-        """Get a collector given the collector_id.
-
-        Parameters
-        ----------
-        collector_id : int
-            The collector ID to fetch details about.
-
-        Returns
-        -------
-        collectors_dict : dict
-            A dictionary of a collector.
-        """
-        if collector_id is None:
-            raise ValueError("collector_id is required")
-
-        self.log.info("collector_id=%s", str(collector_id))
-        url = self.TENANT_BASE_URL / "v1" / "collectors" / "/" / str(collector_id) / "/"
-        self.log.debug("url=%s", str(url))
-        collector_request = self._api_http_request(method="GET", url=url)
-        if collector_request.status_code != httpx.codes.OK:
-            raise Exception("collector issue", collector_request.text)
-
-        return self._json_decoder.decode(collector_request.text)["data"]
-
-    def get_collectors(self) -> dict:
-        """Get a dictionary of collectors.
-
-        Returns
-        -------
-        collectors_inventory : dict
-            A dictionary of collectors.
-
-        """
-        url = self.TENANT_BASE_URL / "v1" / "collectors/"
-        url.args["from"] = 0
-        url.args["length"] = self.ARMIS_API_PAGE_SIZE
-        collectors_inventory = {}
-
-        while url.args["from"] is not None:
-            self.log.info(
-                "fetching %s-%s",
-                str(url.args["from"]),
-                str(url.args["from"] + self.ARMIS_API_PAGE_SIZE),
-            )
-            get_collectors_request = self._api_http_request(method="GET", url=url)
-            if get_collectors_request.status_code != httpx.codes.OK:
-                self.log.critical("STATUS CODE != 200")
-                self.log.critical(
-                    "status_code=%s",
-                    str(get_collectors_request.status_code),
-                )
-                self.log.critical("text=%s", get_collectors_request.text)
-                self.log.critical("continuing")
-                continue
-
-            collectors_response = self._json_decoder.decode(get_collectors_request.text)
-            collectors_count = collectors_response["data"]["count"]
-            self.log.debug("retrieved %s collectors", str(collectors_count))
-
-            for collector in collectors_response["data"]["collectors"]:
-                collectornumber = collector["collectorNumber"]
-                collectors_inventory[collectornumber] = collector
-
-            self.log.debug(
-                "collectors next=%s",
-                str(collectors_response["data"]["next"]),
-            )
-            url.args["from"] = collectors_response["data"]["next"]
-
-        self.log.debug("collectors_inventory size=%s", str(len(collectors_inventory)))
-
-        if len(collectors_inventory) > 0:
-            collectors_inventory = dict(sorted(collectors_inventory.items()))
-        return collectors_inventory
-
     def get_integration(self, integration_id: int):
         """Get an integration given an integration_id.
 
         Parameters
         ----------
         integration_id : int
             Desired integration_id
@@ -924,21 +1114,20 @@
         -------
         integration : dict
             a dictionary of the requested integration
 
         Notes
         -----
         This method requires v2 of the API call which is only available in the
-        Armis Cloud version >= R-24.0.
+        Armis Cloud version >= R - 24.0.
         """
         if integration_id is None:
             raise ValueError("an integration_id is required")
 
-        url = self.TENANT_BASE_URL / "v2" / "integrations" / str(integration_id)
-        url = url / "/"
+        url = self.TENANT_BASE_URL / f"v2/integrations/{integration_id}/"
         url.args = {}
 
         integration_details = self._api_http_request(method="GET", url=url)
 
         if integration_details.status_code == httpx.codes.NOT_FOUND:
             self.log.debug("integration was not found")
             self.log.debug("text=%s", integration_details.text)
@@ -950,30 +1139,30 @@
                 "status_code=%s",
                 str(integration_details.status_code),
             )
             self.log.debug("text=%s", integration_details.text)
             raise Exception("integration_details issue", integration_details.text)
 
         integration = self._json_decoder.decode(integration_details.text)["data"][0]
-        return integration
+        return integration  # noqa: RET504
 
     def get_integrations(self) -> dict:
         """Get a list of integrations.
 
         Returns
         -------
         integrations : dict
             a dictionary of integrations
 
         Notes
         -----
         This method requires v2 of the API call which is only available in the
         Armis Cloud version >= R-24.0.
         """
-        url = self.TENANT_BASE_URL / "v2" / "integrations/"
+        url = self.TENANT_BASE_URL / "v2/integrations/"
         url.args["from"] = 0
         url.args["length"] = self.ARMIS_API_PAGE_SIZE
 
         integrations_count = self.get_integrations_count()
 
         integrations = {}
 
@@ -1021,15 +1210,15 @@
             A count of integrations.
 
         Notes
         -----
         This method requires v2 of the API call which is only available in the
         Armis Cloud version >= R-24.0.
         """
-        url = self.TENANT_BASE_URL / "v2" / "integrations/"
+        url = self.TENANT_BASE_URL / "v2/integrations/"
         url.args["length"] = 1
         self.log.debug("url=%s", str(url))
         count_request = self._api_http_request(method="GET", url=url)
         return int(self._json_decoder.decode(count_request.text)["data"]["total"])
 
     def get_sites(self) -> dict:
         """Get a list of sites.
@@ -1037,15 +1226,15 @@
         Returns
         -------
         sites : dict
             A dict of sites.
 
         Notes
         -----
-        Only applies to cloud version >= R-23.3-S182.
+        The cloud must be running at version >= R-23.3-S182.
         """
         url = self.TENANT_BASE_URL / "v1/sites/"
         url.args["from"] = 0
         url.args["length"] = self.ARMIS_API_PAGE_SIZE
         url.args["includeTotal"] = "true"
 
         sites = {}
@@ -1084,19 +1273,20 @@
             JSON data as a dict.
         """
         site_id = kwargs.get("site_id", None)
 
         if site_id is None:
             raise ValueError("site_id was not provided")
 
-        url = self.TENANT_BASE_URL / "v1" / "sites" / str(site_id) / "/"
+        url = self.TENANT_BASE_URL / f"v1/sites/{site_id}/"
+
         self.log.debug("url=%s", str(url))
 
         site_request = self._api_http_request(method="GET", url=url)
-        if site_request.status_code != 200:
+        if site_request.status_code != httpx.codes.OK:
             self.log.critical("STATUS CODE !=200")
             self.log.critical("status_code=%s", str(site_request.status_code))
             self.log.critical("text=%s", site_request.text)
             self.log.critical("continuing")
             raise Exception("dashboard http response !=200")
 
         if "data" in self._json_decoder.decode(site_request.text):
```

### Comparing `armis-1.0.18/tests/test_apicalls.py` & `armis-1.0.19/tests/test_apicalls.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.18/tests/test_boundaries.py` & `armis-1.0.19/tests/test_boundaries.py`

 * *Files 22% similar despite different names*

```diff
@@ -23,7 +23,12 @@
         boundaryid = random.choice(boundaryids)
         assert boundaryid == armis_object.get_boundary(boundary_id=boundaryid)["id"]
 
 
 def test_get_boundary_by_id_blank(armis_object):
     with pytest.raises(TypeError):
         armis_object.get_boundary()
+
+
+def test_get_boundary_by_id_none(armis_object):
+    with pytest.raises(ValueError):
+        armis_object.get_boundary(None)
```

### Comparing `armis-1.0.18/tests/test_ceiling.py` & `armis-1.0.19/tests/test_ceiling.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.18/tests/test_devices.py` & `armis-1.0.19/tests/test_devices.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.18/tests/test_fixture.py` & `armis-1.0.19/tests/test_fixture.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.18/tests/test_objectcreation.py` & `armis-1.0.19/tests/test_objectcreation.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.18/tests/test_tagging.py` & `armis-1.0.19/tests/test_tagging.py`

 * *Files identical despite different names*

### Comparing `armis-1.0.18/.gitignore` & `armis-1.0.19/.gitignore`

 * *Files identical despite different names*

### Comparing `armis-1.0.18/README.md` & `armis-1.0.19/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -15,40 +15,96 @@
 
 Install **armis** using pip:
 
 ```console
 $ pip install armis
 ```
 
-Now, let's get started:
+# A Quick Demo of Features
 
+## Getting Started
+First, let's create an ArmisCloud object:
 ```python
->>> from armis import ArmisCloud
->>> a = ArmisCloud(
-        api_secret_key="your-api-secret-key-here",
-        tenant_hostname="your-tenant-hostname-here.armis.com",
-        fields=["id", "ipAddress", "name", "firstSeen"]
-    )
->>> a.get_devices(asq='in:devices timeFrame:"10 Seconds"')
+from armis import ArmisCloud
+
+a = ArmisCloud(
+    api_secret_key="your-api-secret-key-here",
+    tenant_hostname="your-tenant-hostname-here.armis.com"
+)
+```
+
+## Device Operations
+Let's get a list of all devices matching our ASQ and only retrieve a few fields:
+
+```python
+devices = a.get_devices(
+    asq='in:devices timeFrame:"10 Seconds"',
+    fields=["id", "ipAddress", "name", "firstSeen"]
+)
+print(devices)
+
 [{"id": 15, "ipAddress": "10.1.2.3", "name": "super-pc", "firstSeen": "2019-05-15T13:00:00+00:00"}]
+```
 
+## Boundary Operations
+
+Let's get all of the boundaries known to the system:
+```python
+boundaries = a.get_boundaries()
+print(boundaries)
 
->>> a.get_boundaries()
 {1: {'affectedSites': '', 'id': 1, 'name': 'Corporate', 'ruleAql': {'or': ['ipAddress:10.0.0.0/8']}}, 2: {'affectedSites': '', 'id': 2, 'name': 'Guest', 'ruleAql': {'or': ['lastConnectedSsid:Guest']}}}
+```
 
+Let's get only one boundary by ID:
+```python
+boundaryone = a.get_boundary(boundary_id=1)
+print(boundaryone)
 
->>> a.get_boundary(boundary_id=1)
 {"data":{"affectedSites":"","id":1,"name":"Corporate","ruleAql":{"or":["ipAddress:10.0.0.0/8"]}},"success":true}
+```
 
+Deleting a boundary is easy:
+
+```python
+result = a.delete_boundary(boundary_id=3424234)
+print(result)
+{"success": True}
+```
+
+Creating a boundary is easy, though the syntax is not yet documented well here:
+```python
+result = a.create_boundary(
+    name="My New Boundary",
+    ruleaql={ "or": [
+        "ipAddress:10.0.0.0/24"
+        ]
+    }
+)
+print(result)
+{'data': {'id': 392309238}, 'success': True}
+```
+
+## Collector Operations
+
+Get a list of collectors:
+
+```python
+collectors = a.get_collectors()
+print(collectors)
 
->>> a.get_collectors()
 {1234: {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}}
+```
+
+Get the details for a specific collector:
 
+```python
+myimportantcollector = a.get_collector(collector_id=1234)
+print(myimportantcollector)
 
->>> a.get_collector(collector_id=1234)
 {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}
 
 ```
 
 ## Features
 
 **armis** gives you:
@@ -74,11 +130,9 @@
 **armis** relies on these excellent libraries:
 * [furl](https://github.com/gruns/furl) - provides easy-to-use URL parsing and updating
 * [httpx](https://github.com/encode/httpx/) - The underlying transport implementation for making HTTP requests
 * [msgspec](https://github.com/jcrist/msgspec) - for lightning fast decoding of JSON
 * [pendulum](https://github.com/sdispater/pendulum) - for easy date/time management
 * [tenacity](https://github.com/jd/tenacity) - retry management when things fail, with great retry/backoff options
 
-
 ## License
-
 `armis` is distributed under the terms of the [BSD-3-Clause](https://spdx.org/licenses/BSD-3-Clause.html) license.
```

#### html2text {}

```diff
@@ -1,30 +1,42 @@
 # Armis Python Library
         aarrmmiiss -- AA PPyytthhoonn lliibbrraarryy ffoorr iinntteerraaccttiinngg wwiitthh tthhee AArrmmiiss cclloouudd..
                                  _[_T_e_s_t_ _S_u_i_t_e_]
 **armis** is a Python client library for interacting with the Armis cloud. It
 connects using **HTTP/2** by default, falling back to **HTTP/1.1** when
 necessary. Python 3.8+ is supported. --- Install **armis** using pip:
-```console $ pip install armis ``` Now, let's get started: ```python >>> from
-armis import ArmisCloud >>> a = ArmisCloud( api_secret_key="your-api-secret-
-key-here", tenant_hostname="your-tenant-hostname-here.armis.com", fields=["id",
-"ipAddress", "name", "firstSeen"] ) >>> a.get_devices(asq='in:devices
-timeFrame:"10 Seconds"') [{"id": 15, "ipAddress": "10.1.2.3", "name": "super-
-pc", "firstSeen": "2019-05-15T13:00:00+00:00"}] >>> a.get_boundaries() {1:
-{'affectedSites': '', 'id': 1, 'name': 'Corporate', 'ruleAql': {'or':
-['ipAddress:10.0.0.0/8']}}, 2: {'affectedSites': '', 'id': 2, 'name': 'Guest',
-'ruleAql': {'or': ['lastConnectedSsid:Guest']}}} >>> a.get_boundary
-(boundary_id=1) {"data":{"affectedSites":"","id":1,"name":
-"Corporate","ruleAql":{"or":["ipAddress:10.0.0.0/8"]}},"success":true} >>>
-a.get_collectors() {1234: {'clusterId': 0, 'collectorNumber': 1234,
-'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress':
-'10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:
-56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/
-24', 'type': 'Physical'}} >>> a.get_collector(collector_id=1234) {'clusterId':
-0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted':
+```console $ pip install armis ``` # A Quick Demo of Features ## Getting
+Started First, let's create an ArmisCloud object: ```python from armis import
+ArmisCloud a = ArmisCloud( api_secret_key="your-api-secret-key-here",
+tenant_hostname="your-tenant-hostname-here.armis.com" ) ``` ## Device
+Operations Let's get a list of all devices matching our ASQ and only retrieve a
+few fields: ```python devices = a.get_devices( asq='in:devices timeFrame:"10
+Seconds"', fields=["id", "ipAddress", "name", "firstSeen"] ) print(devices) [
+{"id": 15, "ipAddress": "10.1.2.3", "name": "super-pc", "firstSeen": "2019-05-
+15T13:00:00+00:00"}] ``` ## Boundary Operations Let's get all of the boundaries
+known to the system: ```python boundaries = a.get_boundaries() print
+(boundaries) {1: {'affectedSites': '', 'id': 1, 'name': 'Corporate', 'ruleAql':
+{'or': ['ipAddress:10.0.0.0/8']}}, 2: {'affectedSites': '', 'id': 2, 'name':
+'Guest', 'ruleAql': {'or': ['lastConnectedSsid:Guest']}}} ``` Let's get only
+one boundary by ID: ```python boundaryone = a.get_boundary(boundary_id=1) print
+(boundaryone) {"data":{"affectedSites":"","id":1,"name":"Corporate","ruleAql":
+{"or":["ipAddress:10.0.0.0/8"]}},"success":true} ``` Deleting a boundary is
+easy: ```python result = a.delete_boundary(boundary_id=3424234) print(result)
+{"success": True} ``` Creating a boundary is easy, though the syntax is not yet
+documented well here: ```python result = a.create_boundary( name="My New
+Boundary", ruleaql={ "or": [ "ipAddress:10.0.0.0/24" ] } ) print(result)
+{'data': {'id': 392309238}, 'success': True} ``` ## Collector Operations Get a
+list of collectors: ```python collectors = a.get_collectors() print(collectors)
+{1234: {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1',
+'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:
+00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234',
+'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}} ``` Get the
+details for a specific collector: ```python myimportantcollector =
+a.get_collector(collector_id=1234) print(myimportantcollector) {'clusterId': 0,
+'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted':
 '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00',
 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status':
 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'} ``` ## Features
 **armis** gives you: * Easy connection to the Armis cloud using an API secret
 key. * A quick way to fetch devices from the cloud. * Retries in the event the
 cloud times out. This can happen with large queries that take more than 2
 minutes. This is the default for CloudFlare, which front-ends the cloud
```

### Comparing `armis-1.0.18/pyproject.toml` & `armis-1.0.19/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -72,14 +72,15 @@
 ]
 
 [tool.hatch.envs.types.scripts]
 check = "mypy --install-types --non-interactive {args:src/armis tests}"
 
 [tool.hatch.build.targets.sdist]
 exclude = [
+  "private*",
   ".coverage_report",
   "coverage_report",
   "docs/",
   "pytest.ini",
   ".dev",
   ".github",
   "mkdocs.yml",
```

### Comparing `armis-1.0.18/PKG-INFO` & `armis-1.0.19/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: armis
-Version: 1.0.18
+Version: 1.0.19
 Summary: Connect and perform actions with the Armis cloud
 Project-URL: Homepage, https://github.com/mmlange/armis-python/
 Project-URL: Issues, https://github.com/mmlange/armis-python/issues
 Project-URL: Source, https://github.com/mmlange/armis-python/
 Author-email: Matthew Lange <mmlange@gmail.com>
 Maintainer-email: Matthew Lange <mmlange@gmail.com>
 License-Expression: BSD-3-Clause
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Communications
 Classifier: Topic :: Software Development :: Libraries
 Requires-Python: >=3.8
 Requires-Dist: furl==2.1.3
-Requires-Dist: httpx[http2]==0.27.0
+Requires-Dist: httpx[brotli,http2]==0.27.0
 Requires-Dist: msgspec==0.18.6
 Requires-Dist: pendulum==3.0.0
 Requires-Dist: tenacity==8.2.3
 Description-Content-Type: text/markdown
 
 # Armis Python Library
 
@@ -46,40 +46,96 @@
 
 Install **armis** using pip:
 
 ```console
 $ pip install armis
 ```
 
-Now, let's get started:
+# A Quick Demo of Features
 
+## Getting Started
+First, let's create an ArmisCloud object:
 ```python
->>> from armis import ArmisCloud
->>> a = ArmisCloud(
-        api_secret_key="your-api-secret-key-here",
-        tenant_hostname="your-tenant-hostname-here.armis.com",
-        fields=["id", "ipAddress", "name", "firstSeen"]
-    )
->>> a.get_devices(asq='in:devices timeFrame:"10 Seconds"')
+from armis import ArmisCloud
+
+a = ArmisCloud(
+    api_secret_key="your-api-secret-key-here",
+    tenant_hostname="your-tenant-hostname-here.armis.com"
+)
+```
+
+## Device Operations
+Let's get a list of all devices matching our ASQ and only retrieve a few fields:
+
+```python
+devices = a.get_devices(
+    asq='in:devices timeFrame:"10 Seconds"',
+    fields=["id", "ipAddress", "name", "firstSeen"]
+)
+print(devices)
+
 [{"id": 15, "ipAddress": "10.1.2.3", "name": "super-pc", "firstSeen": "2019-05-15T13:00:00+00:00"}]
+```
 
+## Boundary Operations
+
+Let's get all of the boundaries known to the system:
+```python
+boundaries = a.get_boundaries()
+print(boundaries)
 
->>> a.get_boundaries()
 {1: {'affectedSites': '', 'id': 1, 'name': 'Corporate', 'ruleAql': {'or': ['ipAddress:10.0.0.0/8']}}, 2: {'affectedSites': '', 'id': 2, 'name': 'Guest', 'ruleAql': {'or': ['lastConnectedSsid:Guest']}}}
+```
 
+Let's get only one boundary by ID:
+```python
+boundaryone = a.get_boundary(boundary_id=1)
+print(boundaryone)
 
->>> a.get_boundary(boundary_id=1)
 {"data":{"affectedSites":"","id":1,"name":"Corporate","ruleAql":{"or":["ipAddress:10.0.0.0/8"]}},"success":true}
+```
 
+Deleting a boundary is easy:
+
+```python
+result = a.delete_boundary(boundary_id=3424234)
+print(result)
+{"success": True}
+```
+
+Creating a boundary is easy, though the syntax is not yet documented well here:
+```python
+result = a.create_boundary(
+    name="My New Boundary",
+    ruleaql={ "or": [
+        "ipAddress:10.0.0.0/24"
+        ]
+    }
+)
+print(result)
+{'data': {'id': 392309238}, 'success': True}
+```
+
+## Collector Operations
+
+Get a list of collectors:
+
+```python
+collectors = a.get_collectors()
+print(collectors)
 
->>> a.get_collectors()
 {1234: {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}}
+```
+
+Get the details for a specific collector:
 
+```python
+myimportantcollector = a.get_collector(collector_id=1234)
+print(myimportantcollector)
 
->>> a.get_collector(collector_id=1234)
 {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}
 
 ```
 
 ## Features
 
 **armis** gives you:
@@ -105,11 +161,9 @@
 **armis** relies on these excellent libraries:
 * [furl](https://github.com/gruns/furl) - provides easy-to-use URL parsing and updating
 * [httpx](https://github.com/encode/httpx/) - The underlying transport implementation for making HTTP requests
 * [msgspec](https://github.com/jcrist/msgspec) - for lightning fast decoding of JSON
 * [pendulum](https://github.com/sdispater/pendulum) - for easy date/time management
 * [tenacity](https://github.com/jd/tenacity) - retry management when things fail, with great retry/backoff options
 
-
 ## License
-
 `armis` is distributed under the terms of the [BSD-3-Clause](https://spdx.org/licenses/BSD-3-Clause.html) license.
```

#### html2text {}

```diff
@@ -1,47 +1,59 @@
-Metadata-Version: 2.3 Name: armis Version: 1.0.18 Summary: Connect and perform
+Metadata-Version: 2.3 Name: armis Version: 1.0.19 Summary: Connect and perform
 actions with the Armis cloud Project-URL: Homepage, https://github.com/mmlange/
 armis-python/ Project-URL: Issues, https://github.com/mmlange/armis-python/
 issues Project-URL: Source, https://github.com/mmlange/armis-python/ Author-
 email: Matthew Lange
 gmail.com> Maintainer-email: Matthew Lange
 gmail.com> License-Expression: BSD-3-Clause Keywords: api,armis,development
 Classifier: Development Status :: 4 - Beta Classifier: Intended Audience ::
 Developers Classifier: License :: OSI Approved :: BSD License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3 :: Only Classifier: Programming Language :: Python :: 3.8 Classifier:
 Programming Language :: Python :: 3.9 Classifier: Programming Language ::
 Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Classifier:
 Programming Language :: Python :: 3.12 Classifier: Topic :: Communications
 Classifier: Topic :: Software Development :: Libraries Requires-Python: >=3.8
-Requires-Dist: furl==2.1.3 Requires-Dist: httpx[http2]==0.27.0 Requires-Dist:
-msgspec==0.18.6 Requires-Dist: pendulum==3.0.0 Requires-Dist: tenacity==8.2.3
-Description-Content-Type: text/markdown # Armis Python Library
+Requires-Dist: furl==2.1.3 Requires-Dist: httpx[brotli,http2]==0.27.0 Requires-
+Dist: msgspec==0.18.6 Requires-Dist: pendulum==3.0.0 Requires-Dist:
+tenacity==8.2.3 Description-Content-Type: text/markdown # Armis Python Library
         aarrmmiiss -- AA PPyytthhoonn lliibbrraarryy ffoorr iinntteerraaccttiinngg wwiitthh tthhee AArrmmiiss cclloouudd..
                                  _[_T_e_s_t_ _S_u_i_t_e_]
 **armis** is a Python client library for interacting with the Armis cloud. It
 connects using **HTTP/2** by default, falling back to **HTTP/1.1** when
 necessary. Python 3.8+ is supported. --- Install **armis** using pip:
-```console $ pip install armis ``` Now, let's get started: ```python >>> from
-armis import ArmisCloud >>> a = ArmisCloud( api_secret_key="your-api-secret-
-key-here", tenant_hostname="your-tenant-hostname-here.armis.com", fields=["id",
-"ipAddress", "name", "firstSeen"] ) >>> a.get_devices(asq='in:devices
-timeFrame:"10 Seconds"') [{"id": 15, "ipAddress": "10.1.2.3", "name": "super-
-pc", "firstSeen": "2019-05-15T13:00:00+00:00"}] >>> a.get_boundaries() {1:
-{'affectedSites': '', 'id': 1, 'name': 'Corporate', 'ruleAql': {'or':
-['ipAddress:10.0.0.0/8']}}, 2: {'affectedSites': '', 'id': 2, 'name': 'Guest',
-'ruleAql': {'or': ['lastConnectedSsid:Guest']}}} >>> a.get_boundary
-(boundary_id=1) {"data":{"affectedSites":"","id":1,"name":
-"Corporate","ruleAql":{"or":["ipAddress:10.0.0.0/8"]}},"success":true} >>>
-a.get_collectors() {1234: {'clusterId': 0, 'collectorNumber': 1234,
-'defaultGateway': '10.0.0.1', 'httpsProxyRedacted': '', 'ipAddress':
-'10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00', 'macAddress': '00:12:34:
-56:78:90', 'name': 'Collector 1234', 'status': 'Offline', 'subnet': '10.0.0.0/
-24', 'type': 'Physical'}} >>> a.get_collector(collector_id=1234) {'clusterId':
-0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted':
+```console $ pip install armis ``` # A Quick Demo of Features ## Getting
+Started First, let's create an ArmisCloud object: ```python from armis import
+ArmisCloud a = ArmisCloud( api_secret_key="your-api-secret-key-here",
+tenant_hostname="your-tenant-hostname-here.armis.com" ) ``` ## Device
+Operations Let's get a list of all devices matching our ASQ and only retrieve a
+few fields: ```python devices = a.get_devices( asq='in:devices timeFrame:"10
+Seconds"', fields=["id", "ipAddress", "name", "firstSeen"] ) print(devices) [
+{"id": 15, "ipAddress": "10.1.2.3", "name": "super-pc", "firstSeen": "2019-05-
+15T13:00:00+00:00"}] ``` ## Boundary Operations Let's get all of the boundaries
+known to the system: ```python boundaries = a.get_boundaries() print
+(boundaries) {1: {'affectedSites': '', 'id': 1, 'name': 'Corporate', 'ruleAql':
+{'or': ['ipAddress:10.0.0.0/8']}}, 2: {'affectedSites': '', 'id': 2, 'name':
+'Guest', 'ruleAql': {'or': ['lastConnectedSsid:Guest']}}} ``` Let's get only
+one boundary by ID: ```python boundaryone = a.get_boundary(boundary_id=1) print
+(boundaryone) {"data":{"affectedSites":"","id":1,"name":"Corporate","ruleAql":
+{"or":["ipAddress:10.0.0.0/8"]}},"success":true} ``` Deleting a boundary is
+easy: ```python result = a.delete_boundary(boundary_id=3424234) print(result)
+{"success": True} ``` Creating a boundary is easy, though the syntax is not yet
+documented well here: ```python result = a.create_boundary( name="My New
+Boundary", ruleaql={ "or": [ "ipAddress:10.0.0.0/24" ] } ) print(result)
+{'data': {'id': 392309238}, 'success': True} ``` ## Collector Operations Get a
+list of collectors: ```python collectors = a.get_collectors() print(collectors)
+{1234: {'clusterId': 0, 'collectorNumber': 1234, 'defaultGateway': '10.0.0.1',
+'httpsProxyRedacted': '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:
+00:00+00:00', 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234',
+'status': 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'}} ``` Get the
+details for a specific collector: ```python myimportantcollector =
+a.get_collector(collector_id=1234) print(myimportantcollector) {'clusterId': 0,
+'collectorNumber': 1234, 'defaultGateway': '10.0.0.1', 'httpsProxyRedacted':
 '', 'ipAddress': '10.0.0.2', 'lastSeen': '2019-05-15T13:00:00+00:00',
 'macAddress': '00:12:34:56:78:90', 'name': 'Collector 1234', 'status':
 'Offline', 'subnet': '10.0.0.0/24', 'type': 'Physical'} ``` ## Features
 **armis** gives you: * Easy connection to the Armis cloud using an API secret
 key. * A quick way to fetch devices from the cloud. * Retries in the event the
 cloud times out. This can happen with large queries that take more than 2
 minutes. This is the default for CloudFlare, which front-ends the cloud
```

