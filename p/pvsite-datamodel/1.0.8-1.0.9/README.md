# Comparing `tmp/pvsite_datamodel-1.0.8.tar.gz` & `tmp/pvsite_datamodel-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pvsite_datamodel-1.0.8.tar", max compression
+gzip compressed data, was "pvsite_datamodel-1.0.9.tar", max compression
```

## Comparing `pvsite_datamodel-1.0.8.tar` & `pvsite_datamodel-1.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
--rw-r--r--   0        0        0     1073 2024-01-17 10:40:24.708088 pvsite_datamodel-1.0.8/LICENSE
--rw-r--r--   0        0        0     3759 2024-01-17 10:40:24.708088 pvsite_datamodel-1.0.8/README.md
--rw-r--r--   0        0        0      290 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/__init__.py
--rw-r--r--   0        0        0      854 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/connection.py
--rw-r--r--   0        0        0        0 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/py.typed
--rw-r--r--   0        0        0     1004 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/pydantic_models.py
--rw-r--r--   0        0        0      499 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/read/__init__.py
--rw-r--r--   0        0        0     4396 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/read/generation.py
--rw-r--r--   0        0        0     3672 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/read/latest_forecast_values.py
--rw-r--r--   0        0        0     3949 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/read/site.py
--rw-r--r--   0        0        0      640 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/read/status.py
--rw-r--r--   0        0        0     2297 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/read/user.py
--rw-r--r--   0        0        0    12163 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/sqlmodels.py
--rw-r--r--   0        0        0       10 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno/dno.cpg
--rw-r--r--   0        0        0     2636 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno/dno.dbf
--rw-r--r--   0        0        0      417 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno/dno.prj
--rw-r--r--   0        0        0   956812 2024-01-17 10:40:24.720088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno/dno.shp
--rw-r--r--   0        0        0      212 2024-01-17 10:40:24.720088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno/dno.shx
--rw-r--r--   0        0        0     1398 2024-01-17 10:40:24.712088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno.py
--rw-r--r--   0        0        0       10 2024-01-17 10:40:24.720088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.cpg
--rw-r--r--   0        0        0    53711 2024-01-17 10:40:24.720088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.dbf
--rw-r--r--   0        0        0      417 2024-01-17 10:40:24.720088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.prj
--rw-r--r--   0        0        0  6013616 2024-01-17 10:40:24.748088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.shp
--rw-r--r--   0        0        0     2764 2024-01-17 10:40:24.748088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.shx
--rw-r--r--   0        0        0     1289 2024-01-17 10:40:24.720088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp.py
--rw-r--r--   0        0        0     8420 2024-01-17 10:40:24.748088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp_new_ids_and_names-edited.csv
--rw-r--r--   0        0        0     1621 2024-01-17 10:40:24.748088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/utils.py
--rw-r--r--   0        0        0     2186 2024-01-17 10:40:24.748088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/generation.py
--rw-r--r--   0        0        0     9003 2024-01-17 10:40:24.748088 pvsite_datamodel-1.0.8/pvsite_datamodel/write/user_and_site.py
--rw-r--r--   0        0        0     1658 2024-01-17 10:40:24.748088 pvsite_datamodel-1.0.8/pyproject.toml
--rw-r--r--   0        0        0     4328 1970-01-01 00:00:00.000000 pvsite_datamodel-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-01-17 16:06:10.785713 pvsite_datamodel-1.0.9/LICENSE
+-rw-r--r--   0        0        0     3782 2024-01-17 16:06:10.785713 pvsite_datamodel-1.0.9/README.md
+-rw-r--r--   0        0        0      290 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/__init__.py
+-rw-r--r--   0        0        0      854 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/connection.py
+-rw-r--r--   0        0        0        0 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/py.typed
+-rw-r--r--   0        0        0     1004 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/pydantic_models.py
+-rw-r--r--   0        0        0      525 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/read/__init__.py
+-rw-r--r--   0        0        0     4396 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/read/generation.py
+-rw-r--r--   0        0        0     3672 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/read/latest_forecast_values.py
+-rw-r--r--   0        0        0     4562 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/read/site.py
+-rw-r--r--   0        0        0      640 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/read/status.py
+-rw-r--r--   0        0        0     2297 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/read/user.py
+-rw-r--r--   0        0        0    12313 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/sqlmodels.py
+-rw-r--r--   0        0        0       10 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno/dno.cpg
+-rw-r--r--   0        0        0     2636 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno/dno.dbf
+-rw-r--r--   0        0        0      417 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno/dno.prj
+-rw-r--r--   0        0        0   956812 2024-01-17 16:06:10.797713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno/dno.shp
+-rw-r--r--   0        0        0      212 2024-01-17 16:06:10.797713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno/dno.shx
+-rw-r--r--   0        0        0     1398 2024-01-17 16:06:10.789713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno.py
+-rw-r--r--   0        0        0       10 2024-01-17 16:06:10.797713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.cpg
+-rw-r--r--   0        0        0    53711 2024-01-17 16:06:10.797713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.dbf
+-rw-r--r--   0        0        0      417 2024-01-17 16:06:10.797713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.prj
+-rw-r--r--   0        0        0  6013616 2024-01-17 16:06:10.825714 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.shp
+-rw-r--r--   0        0        0     2764 2024-01-17 16:06:10.825714 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.shx
+-rw-r--r--   0        0        0     1289 2024-01-17 16:06:10.797713 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp.py
+-rw-r--r--   0        0        0     8420 2024-01-17 16:06:10.825714 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp_new_ids_and_names-edited.csv
+-rw-r--r--   0        0        0     1621 2024-01-17 16:06:10.825714 pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/utils.py
+-rw-r--r--   0        0        0     2186 2024-01-17 16:06:10.825714 pvsite_datamodel-1.0.9/pvsite_datamodel/write/generation.py
+-rw-r--r--   0        0        0     9158 2024-01-17 16:06:10.825714 pvsite_datamodel-1.0.9/pvsite_datamodel/write/user_and_site.py
+-rw-r--r--   0        0        0     1658 2024-01-17 16:06:10.825714 pvsite_datamodel-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4351 1970-01-01 00:00:00.000000 pvsite_datamodel-1.0.9/PKG-INFO
```

### Comparing `pvsite_datamodel-1.0.8/LICENSE` & `pvsite_datamodel-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/README.md` & `pvsite_datamodel-1.0.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 
 - get_user_by_email
 - get_pv_generation_by_sites
 - get_site_by_uuid
 - get_site_by_client_site_id
 - get_site_by_client_site_name
 - get_all_sites
+- get_sites_by_country
 - get_site_group_by_name
 - get_latest_status
 - get_latest_forecast_values_by_site
 
 
 ### Write package functions
```

#### html2text {}

```diff
@@ -9,19 +9,19 @@
 SQLAlchemy definitions of table schemas tests: # External tests package ``` ###
 Top-level functions Classes specifying table schemas: - APIRequestSQL -
 GenerationSQL - ForecastSQL - ForecastValueSQL - UserSQL - SiteSQL -
 SiteGroupSQL - StatusSQL Database connection objects: - DatabaseConnection ###
 Read package functions Currently available functions accessible via `from
 pvsite_datamodel.read import `: - get_user_by_email -
 get_pv_generation_by_sites - get_site_by_uuid - get_site_by_client_site_id -
-get_site_by_client_site_name - get_all_sites - get_site_group_by_name -
-get_latest_status - get_latest_forecast_values_by_site ### Write package
-functions Currently available write functions accessible via `from
-pvsite_datamodels.write import `: - insert_generation_values - create_site -
-create_site_group - create_user - add_site_to_site_group -
+get_site_by_client_site_name - get_all_sites - get_sites_by_country -
+get_site_group_by_name - get_latest_status - get_latest_forecast_values_by_site
+### Write package functions Currently available write functions accessible via
+`from pvsite_datamodels.write import `: - insert_generation_values -
+create_site - create_site_group - create_user - add_site_to_site_group -
 change_user_site_group - update_user_site_group - delete_site - delete_user -
 delete_site_group - make_fake_site ## Install the dependencies (requires
 [poetry][poetry]) poetry install ## Coding style Format the code **in place**.
 make format Lint the code make lint ## Running the tests make test ## Multiple
 Clients We have the ability to have these different scenarios 1. one user - can
 add or view one site 2. one user, can add or view multiple sites 3. Two users
 (for example from the sample company), want to look at one site 4. Two users,
```

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/connection.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/connection.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/pydantic_models.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/pydantic_models.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/read/generation.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/read/generation.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/read/latest_forecast_values.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/read/latest_forecast_values.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/read/site.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/read/site.py`

 * *Files 8% similar despite different names*

```diff
@@ -82,28 +82,54 @@
 
     return site
 
 
 def get_all_sites(session: Session) -> List[SiteSQL]:
     """Get all sites from the sites table.
 
-    :param session: database sessions
+    :param session: database session
     :return: site object
     """
     logger.debug("Getting all sites")
 
     # start main query
     query = session.query(SiteSQL)
 
     # order by uuuid
     query = query.order_by(SiteSQL.site_uuid)
 
     # get all results
     sites = query.all()
 
+    logger.debug(f"Found {len(sites)} sites")
+
+    return sites
+
+
+def get_sites_by_country(session: Session, country: str) -> List[SiteSQL]:
+    """Get sites for specific country from the sites table.
+
+    :param session: database session
+    :param country: country name
+    :return: site object
+    """
+    logger.debug(f"Getting sites by country={country}")
+
+    # start main query
+    query = session.query(SiteSQL)
+
+    # filter by country
+    query = query.filter(SiteSQL.country == country)
+
+    # order by uuuid
+    query = query.order_by(SiteSQL.site_uuid)
+
+    # get all results
+    sites = query.all()
+
     logger.debug(f"Found {len(sites)} sites")
 
     return sites
 
 
 def get_sites_from_user(session, user, lat_lon_limits: Optional[LatitudeLongitudeLimits] = None):
     """
```

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/read/status.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/read/status.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/read/user.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/read/user.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/sqlmodels.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/sqlmodels.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,20 @@
     client_site_id = sa.Column(
         sa.Integer, index=True, comment="The ID of the site as given by the providing client"
     )
     client_site_name = sa.Column(
         sa.String(255), index=True, comment="The ID of the site as given by the providing client"
     )
 
-    region = sa.Column(sa.String(255), comment="The region in the UK in which the site is located")
+    country = sa.Column(
+        sa.String(255), server_default="uk", comment="The country in which the site is located"
+    )
+    region = sa.Column(
+        sa.String(255), comment="The region within the country in which the site is located"
+    )
     dno = sa.Column(sa.String(255), comment="The Distribution Node Operator that owns the site")
     gsp = sa.Column(sa.String(255), comment="The Grid Supply Point in which the site is located")
 
     asset_type = sa.Column(
         sa.Enum(SiteAssetType, name="site_asset_type"),
         nullable=False,
         server_default=SiteAssetType.pv.name,
```

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno/dno.dbf` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno/dno.dbf`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno/dno.shp` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno/dno.shp`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/dno.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/dno.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.dbf` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.dbf`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.shp` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.shp`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp/gsp.shx` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp/gsp.shx`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/gsp_new_ids_and_names-edited.csv` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/gsp_new_ids_and_names-edited.csv`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/data/utils.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/data/utils.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/generation.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/generation.py`

 * *Files identical despite different names*

### Comparing `pvsite_datamodel-1.0.8/pvsite_datamodel/write/user_and_site.py` & `pvsite_datamodel-1.0.9/pvsite_datamodel/write/user_and_site.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,14 +61,15 @@
     client_site_id: int,
     client_site_name: str,
     latitude: float,
     longitude: float,
     capacity_kw: float,
     dno: Optional[str] = None,
     gsp: Optional[str] = None,
+    country: Optional[str] = "uk",
     region: Optional[str] = None,
     asset_type: Optional[str] = SiteAssetType.pv.name,
     orientation: Optional[float] = None,
     tilt: Optional[float] = None,
     inverter_capacity_kw: Optional[float] = None,
     module_capacity_kw: Optional[float] = None,
 ) -> [SiteSQL, str]:
@@ -79,29 +80,33 @@
     :param client_site_id: id the client uses for the site
     :param client_site_name: name the client uses for the site
     :param latitude: latitude of site as an integer
     :param longitude: longitude of site as an integer
     :param capacity_kw: capacity of site in kw
     :param dno: dno of site
     :param gsp: gsp of site
-    :param region: region of site, deafut is uk
+    :param country: country of site, default is uk
+    :param region: region of site
     :param asset_type: type of asset (accepts "pv" or "wind")
     :param orientation: orientation of site, default is 180
     :param tilt: tilt of site, default is 35
     :param inverter_capacity_kw: inverter capacity of site in kw
     :param module_capacity_kw: module capacity of site in kw
 
     """
     max_ml_id = session.query(func.max(SiteSQL.ml_id)).scalar()
 
     if max_ml_id is None:
         max_ml_id = 0
 
-    if region in [None, ""]:
-        region = "uk"
+    if country in [None, ""]:
+        country = "uk"
+
+    # if region in [None, ""]:
+    #     region = "uk"
 
     if asset_type not in SiteAssetType.__members__:
         raise ValueError(
             f"""Invalid asset_type. Received: {asset_type},
             but must one of ({', '.join(map(lambda type: type.name, SiteAssetType))})"""
         )
 
@@ -130,14 +135,15 @@
         client_site_id=client_site_id,
         client_site_name=client_site_name,
         latitude=latitude,
         longitude=longitude,
         capacity_kw=capacity_kw,
         dno=dno,
         gsp=gsp,
+        country=country,
         region=region,
         asset_type=asset_type,
         orientation=orientation,
         tilt=tilt,
         inverter_capacity_kw=inverter_capacity_kw,
         module_capacity_kw=module_capacity_kw,
     )
```

### Comparing `pvsite_datamodel-1.0.8/pyproject.toml` & `pvsite_datamodel-1.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pvsite-datamodel"
-version = "1.0.8"
+version = "1.0.9"
 description = "SDK for interacting with the PVSite database"
 authors = ["Open Climate Fix"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.11"
 sqlalchemy = "1.4.46"
```

### Comparing `pvsite_datamodel-1.0.8/PKG-INFO` & `pvsite_datamodel-1.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pvsite-datamodel
-Version: 1.0.8
+Version: 1.0.9
 Summary: SDK for interacting with the PVSite database
 Author: Open Climate Fix
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: geopandas (>=0.14.2,<0.15.0)
@@ -60,14 +60,15 @@
 
 - get_user_by_email
 - get_pv_generation_by_sites
 - get_site_by_uuid
 - get_site_by_client_site_id
 - get_site_by_client_site_name
 - get_all_sites
+- get_sites_by_country
 - get_site_group_by_name
 - get_latest_status
 - get_latest_forecast_values_by_site
 
 
 ### Write package functions
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pvsite-datamodel Version: 1.0.8 Summary: SDK for
+Metadata-Version: 2.1 Name: pvsite-datamodel Version: 1.0.9 Summary: SDK for
 interacting with the PVSite database Author: Open Climate Fix Requires-Python:
 >=3.11,<4.0 Classifier: Programming Language :: Python :: 3 Classifier:
 Programming Language :: Python :: 3.11 Classifier: Programming Language ::
 Python :: 3.12 Requires-Dist: geopandas (>=0.14.2,<0.15.0) Requires-Dist:
 pandas (>=1.5.3,<2.0.0) Requires-Dist: psycopg2-binary (>=2.9.5,<3.0.0)
 Requires-Dist: pydantic (>=2.3.0,<3.0.0) Requires-Dist: sqlalchemy (==1.4.46)
 Description-Content-Type: text/markdown
@@ -17,19 +17,19 @@
 SQLAlchemy definitions of table schemas tests: # External tests package ``` ###
 Top-level functions Classes specifying table schemas: - APIRequestSQL -
 GenerationSQL - ForecastSQL - ForecastValueSQL - UserSQL - SiteSQL -
 SiteGroupSQL - StatusSQL Database connection objects: - DatabaseConnection ###
 Read package functions Currently available functions accessible via `from
 pvsite_datamodel.read import `: - get_user_by_email -
 get_pv_generation_by_sites - get_site_by_uuid - get_site_by_client_site_id -
-get_site_by_client_site_name - get_all_sites - get_site_group_by_name -
-get_latest_status - get_latest_forecast_values_by_site ### Write package
-functions Currently available write functions accessible via `from
-pvsite_datamodels.write import `: - insert_generation_values - create_site -
-create_site_group - create_user - add_site_to_site_group -
+get_site_by_client_site_name - get_all_sites - get_sites_by_country -
+get_site_group_by_name - get_latest_status - get_latest_forecast_values_by_site
+### Write package functions Currently available write functions accessible via
+`from pvsite_datamodels.write import `: - insert_generation_values -
+create_site - create_site_group - create_user - add_site_to_site_group -
 change_user_site_group - update_user_site_group - delete_site - delete_user -
 delete_site_group - make_fake_site ## Install the dependencies (requires
 [poetry][poetry]) poetry install ## Coding style Format the code **in place**.
 make format Lint the code make lint ## Running the tests make test ## Multiple
 Clients We have the ability to have these different scenarios 1. one user - can
 add or view one site 2. one user, can add or view multiple sites 3. Two users
 (for example from the sample company), want to look at one site 4. Two users,
```

