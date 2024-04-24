# Comparing `tmp/ocean_spark_connect-0.3.4.tar.gz` & `tmp/ocean_spark_connect-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ocean_spark_connect-0.3.4.tar", max compression
+gzip compressed data, was "ocean_spark_connect-0.3.5.tar", max compression
```

## Comparing `ocean_spark_connect-0.3.4.tar` & `ocean_spark_connect-0.3.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0      607 2024-02-02 14:22:56.752244 ocean_spark_connect-0.3.4/README.md
--rw-r--r--   0        0        0       25 2024-02-02 14:22:56.752244 ocean_spark_connect-0.3.4/ocean_spark_connect/__init__.py
--rw-r--r--   0        0        0     5019 2024-02-02 14:22:56.752244 ocean_spark_connect-0.3.4/ocean_spark_connect/inverse_websockify.py
--rw-r--r--   0        0        0    11335 2024-02-02 14:22:56.752244 ocean_spark_connect-0.3.4/ocean_spark_connect/ocean_spark_session.py
--rw-r--r--   0        0        0        0 2024-02-02 14:22:56.752244 ocean_spark_connect-0.3.4/ocean_spark_connect/py.typed
--rw-r--r--   0        0        0      544 2024-02-02 14:22:56.752244 ocean_spark_connect-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     1407 1970-01-01 00:00:00.000000 ocean_spark_connect-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0      607 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/README.md
+-rw-r--r--   0        0        0       25 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/__init__.py
+-rw-r--r--   0        0        0     4986 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/inverse_websockify.py
+-rw-r--r--   0        0        0    11221 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/ocean_spark_session.py
+-rw-r--r--   0        0        0        0 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/ocean_spark_connect/py.typed
+-rw-r--r--   0        0        0      538 2024-04-24 09:52:52.203616 ocean_spark_connect-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     1388 1970-01-01 00:00:00.000000 ocean_spark_connect-0.3.5/PKG-INFO
```

### Comparing `ocean_spark_connect-0.3.4/README.md` & `ocean_spark_connect-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `ocean_spark_connect-0.3.4/ocean_spark_connect/inverse_websockify.py` & `ocean_spark_connect-0.3.5/ocean_spark_connect/inverse_websockify.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,14 @@
                 extra_headers={"Authorization": f"Bearer {self.token}"},
             ) as ws:
                 print(f"{peer} connected to {self.url} on {self.addr}:{self.port}")
 
                 def r_reader() -> Any:
                     return r.read(65536)
 
-                self.writer = w
-
                 tcp_to_ws = self.loop.create_task(self.copy(r_reader, ws.send))
                 ws_to_tcp = self.loop.create_task(self.copy(ws.recv, w.write))
                 done, pending = await asyncio.wait(
                     [tcp_to_ws, ws_to_tcp], return_when=asyncio.FIRST_COMPLETED
                 )
                 for x in done:
                     try:
```

### Comparing `ocean_spark_connect-0.3.4/ocean_spark_connect/ocean_spark_session.py` & `ocean_spark_connect-0.3.5/ocean_spark_connect/ocean_spark_session.py`

 * *Files 2% similar despite different names*

```diff
@@ -279,18 +279,15 @@
         spark_0 = OceanSparkSession.Builder() \
             .cluster_id("osc-739db584") \
             .appid("spark-connect-40982-foxes") \
             .profile("default") \
             .getOrCreate()
 
         spark_0.sql("select random()").show()
-        spark_0.stop()
         # spark = OceanSparkSession.Builder().getOrCreate()
         # spark.ai("create a dataframe of random gaussian distributed numbers using pyspark. the length of the new dataframe should be 10000").show()
         # spark.ai("from the jaffle schema, select all columns in the customers table and generate a random gender").show()
         # spark.ai("show me the names of the tables joined with their column names in the jaffle schema").show()
         # asyncio.all_tasks()
     finally:
-        print("erm", file=sys.stderr)
-        #    print("erm", file=sys.stderr)
-        #    if spark_0 is not None:
-        #        spark_0.stop()
+        if spark_0 is not None:
+            spark_0.stop()
```

### Comparing `ocean_spark_connect-0.3.4/pyproject.toml` & `ocean_spark_connect-0.3.5/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "ocean-spark-connect"
-version = "0.3.4"
+version = "0.3.5"
 description = "Spark Connect adapter for Ocean Spark"
 authors = ["Sigmar Stefansson <sigmar@netapp.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
-pyspark = "^3.5.0"
+pyspark = "^3.4.0"
 websockets = "^11.0.3"
 pandas = "^2.0.3"
-pyarrow = "^13.0.0"
+pyarrow = "*"
 grpcio = "^1.57.0"
 googleapis-common-protos = "^1.60.0"
 grpcio-status = "^1.57.0"
 
 [tool.setuptools.packages.find]
 where = ["ocean_spark_connect"]
```

### Comparing `ocean_spark_connect-0.3.4/PKG-INFO` & `ocean_spark_connect-0.3.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: ocean-spark-connect
-Version: 0.3.4
+Version: 0.3.5
 Summary: Spark Connect adapter for Ocean Spark
 Author: Sigmar Stefansson
 Author-email: sigmar@netapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: googleapis-common-protos (>=1.60.0,<2.0.0)
 Requires-Dist: grpcio (>=1.57.0,<2.0.0)
 Requires-Dist: grpcio-status (>=1.57.0,<2.0.0)
 Requires-Dist: pandas (>=2.0.3,<3.0.0)
-Requires-Dist: pyarrow (>=13.0.0,<14.0.0)
-Requires-Dist: pyspark (>=3.5.0,<4.0.0)
+Requires-Dist: pyarrow
+Requires-Dist: pyspark (>=3.4.0,<4.0.0)
 Requires-Dist: websockets (>=11.0.3,<12.0.0)
 Description-Content-Type: text/markdown
 
 ## Wrapper to create Spark Connect session for Spark Applications in Ocean
 
 ```
 from ocean_spark_connect.ocean_spark_session import OceanSparkSession
```

