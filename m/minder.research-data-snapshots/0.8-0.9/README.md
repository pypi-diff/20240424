# Comparing `tmp/minder.research_data_snapshots-0.8-py3-none-any.whl.zip` & `tmp/minder.research_data_snapshots-0.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 3605 bytes, number of entries: 6
--rw-r--r--  2.0 unx     2909 b- defN 24-Mar-19 09:59 minder/research_data_snapshots/__init__.py
+Zip file size: 3596 bytes, number of entries: 6
+-rw-r--r--  2.0 unx     2564 b- defN 24-Mar-20 15:15 minder/research_data_snapshots/__init__.py
 -rw-r--r--  2.0 unx      756 b- defN 24-Mar-19 09:59 minder/research_data_snapshots/__main__.py
--rw-r--r--  2.0 unx     1966 b- defN 24-Mar-19 09:59 minder.research_data_snapshots-0.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-19 09:59 minder.research_data_snapshots-0.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Mar-19 09:59 minder.research_data_snapshots-0.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      578 b- defN 24-Mar-19 09:59 minder.research_data_snapshots-0.8.dist-info/RECORD
-6 files, 6308 bytes uncompressed, 2535 bytes compressed:  59.8%
+-rw-r--r--  2.0 unx     1966 b- defN 24-Mar-20 15:24 minder.research_data_snapshots-0.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Mar-20 15:24 minder.research_data_snapshots-0.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-Mar-20 15:24 minder.research_data_snapshots-0.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      578 b- defN 24-Mar-20 15:24 minder.research_data_snapshots-0.9.dist-info/RECORD
+6 files, 5963 bytes uncompressed, 2526 bytes compressed:  57.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: minder/research_data_snapshots/__init__.py
 Comment: 
 
 Filename: minder/research_data_snapshots/__main__.py
 Comment: 
 
-Filename: minder.research_data_snapshots-0.8.dist-info/METADATA
+Filename: minder.research_data_snapshots-0.9.dist-info/METADATA
 Comment: 
 
-Filename: minder.research_data_snapshots-0.8.dist-info/WHEEL
+Filename: minder.research_data_snapshots-0.9.dist-info/WHEEL
 Comment: 
 
-Filename: minder.research_data_snapshots-0.8.dist-info/top_level.txt
+Filename: minder.research_data_snapshots-0.9.dist-info/top_level.txt
 Comment: 
 
-Filename: minder.research_data_snapshots-0.8.dist-info/RECORD
+Filename: minder.research_data_snapshots-0.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## minder/research_data_snapshots/__init__.py

```diff
@@ -2,37 +2,30 @@
 from pathlib import Path
 
 import platformdirs
 import requests
 from tqdm import tqdm
 
 
-def download_dataset(
+def _download_dataset(
     dataset: str,
     organization: str,
-    folder: Path | None = None,
-    refresh: bool = False,
-    token_path: Path | None = None,
+    folder: Path,
+    refresh: bool,
+    token: str,
+    api: str,
 ) -> Path:
-    if not folder:
-        folder = platformdirs.user_cache_path("research-data-snapshots")
     file = (folder / organization / dataset).with_suffix(".parquet")
     if file.exists() and not refresh:
         return file
     file.parent.mkdir(parents=True, exist_ok=True)
-    RESEARCH_PORTAL_API = os.getenv("RESEARCH_PORTAL_API", "https://research.minder.care/api")
-    MINDER_TOKEN = (
-        os.environ["MINDER_TOKEN"]
-        if "MINDER_TOKEN" in os.environ
-        else Path(token_path or os.environ["RESEARCH_PORTAL_TOKEN_PATH"]).read_text("utf-8").rstrip()
-    )
     with file.open(mode="wb") as f:
         response = requests.get(
-            f"{RESEARCH_PORTAL_API}/data/organization/{organization}/{dataset}.parquet",
-            headers={"Authorization": f"Bearer {MINDER_TOKEN}"},
+            f"{api}/data/organization/{organization}/{dataset}.parquet",
+            headers={"Authorization": f"Bearer {token}"},
             stream=True,
             timeout=None,
         )
         response.raise_for_status()
         progress = tqdm(
             desc=str(file),
             total=int(response.headers.get("content-length", -1)),
@@ -50,30 +43,32 @@
     datasets: list[str],
     organizations: list[str] | None = None,
     folder: Path | None = None,
     refresh: bool = False,
     token_path: Path | None = None,
     csv: bool = False,
 ) -> list[Path]:
+    RESEARCH_PORTAL_API = os.getenv("RESEARCH_PORTAL_API", "https://research.minder.care/api")
+    MINDER_TOKEN = (
+        os.environ["MINDER_TOKEN"]
+        if "MINDER_TOKEN" in os.environ
+        else Path(token_path or os.environ["RESEARCH_PORTAL_TOKEN_PATH"]).read_text("utf-8").rstrip()
+    )
     if organizations is None:
-        RESEARCH_PORTAL_API = os.getenv("RESEARCH_PORTAL_API", "https://research.minder.care/api")
-        MINDER_TOKEN = (
-            os.environ["MINDER_TOKEN"]
-            if "MINDER_TOKEN" in os.environ
-            else Path(token_path or os.environ["RESEARCH_PORTAL_TOKEN_PATH"]).read_text("utf-8").rstrip()
-        )
         response = requests.get(
             f"{RESEARCH_PORTAL_API}/info/organizations",
             headers={"Authorization": f"Bearer {MINDER_TOKEN}"},
             timeout=None,
         )
         response.raise_for_status()
         organizations = [organization["id"] for organization in response.json()["organizations"]]
+    if folder is None:
+        folder = platformdirs.user_cache_path("research-data-snapshots")
     parquets = [
-        download_dataset(dataset, organization, folder, refresh, token_path)
+        _download_dataset(dataset, organization, folder, refresh, MINDER_TOKEN, RESEARCH_PORTAL_API)
         for dataset in datasets
         for organization in organizations
     ]
     if csv:
         import pyarrow.csv
         import pyarrow.parquet
```

## Comparing `minder.research_data_snapshots-0.8.dist-info/METADATA` & `minder.research_data_snapshots-0.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: minder.research-data-snapshots
-Version: 0.8
+Version: 0.9
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: platformdirs ==4.2.0
 Requires-Dist: requests ==2.31.0
 Requires-Dist: tqdm ==4.66.2
 Provides-Extra: csv
 Requires-Dist: pyarrow ; extra == 'csv'
```

## Comparing `minder.research_data_snapshots-0.8.dist-info/RECORD` & `minder.research_data_snapshots-0.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,6 +1,6 @@
-minder/research_data_snapshots/__init__.py,sha256=_yUfA2FY728O2PrMexzLbWcFcbTkvowILsxjzEq9s3w,2909
+minder/research_data_snapshots/__init__.py,sha256=KSqmqXCTfGaWhn6YNLWr-oD3-1w4vdejApI7ia0INF4,2564
 minder/research_data_snapshots/__main__.py,sha256=tvlU26fnzecodl06Pq0SGE9vT31PgQX6hHbd7a-G7Vc,756
-minder.research_data_snapshots-0.8.dist-info/METADATA,sha256=nMarN26lPAUO-e0flH0-6Nh1tFsXuGz7EolN2eLIsI4,1966
-minder.research_data_snapshots-0.8.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-minder.research_data_snapshots-0.8.dist-info/top_level.txt,sha256=hmIcu2oEHK3sAZZC9kYXgv92pMEHwa7lumv4VmdswFI,7
-minder.research_data_snapshots-0.8.dist-info/RECORD,,
+minder.research_data_snapshots-0.9.dist-info/METADATA,sha256=pQPFhWKM0yY1keFWa1Q8fYBtrceEQRZOnqguNAcAHyU,1966
+minder.research_data_snapshots-0.9.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+minder.research_data_snapshots-0.9.dist-info/top_level.txt,sha256=hmIcu2oEHK3sAZZC9kYXgv92pMEHwa7lumv4VmdswFI,7
+minder.research_data_snapshots-0.9.dist-info/RECORD,,
```

