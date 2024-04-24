# Comparing `tmp/SilverStreamingApplicationPoC-1.8-py3-none-any.whl.zip` & `tmp/SilverStreamingApplicationPoC-1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,16 +1,16 @@
-Zip file size: 12993 bytes, number of entries: 14
--rw-r--r--  2.0 unx    13828 b- defN 24-Feb-16 08:03 com/phida/main/Operations.py
--rw-r--r--  2.0 unx    15864 b- defN 24-Feb-24 20:43 com/phida/main/SilverMerge.py
+Zip file size: 13116 bytes, number of entries: 14
+-rw-r--r--  2.0 unx    13829 b- defN 24-Feb-28 10:17 com/phida/main/Operations.py
+-rw-r--r--  2.0 unx    15865 b- defN 24-Feb-28 10:17 com/phida/main/SilverMerge.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-18 02:29 com/phida/main/__init__.py
 -rw-r--r--  2.0 unx     1374 b- defN 24-Feb-15 12:09 com/phida/main/logging.py
--rw-r--r--  2.0 unx     1146 b- defN 24-Feb-27 21:29 com/phida/main/sparksession.py
--rw-r--r--  2.0 unx     2035 b- defN 24-Feb-22 10:07 com/phida/main/utils.py
+-rw-r--r--  2.0 unx     2040 b- defN 24-Feb-28 12:26 com/phida/main/sparksession.py
+-rw-r--r--  2.0 unx     2036 b- defN 24-Feb-28 10:17 com/phida/main/utils.py
 -rw-r--r--  2.0 unx     5765 b- defN 24-Feb-06 06:49 com/phida/tests/OperationsTest.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-06 06:49 com/phida/tests/__init__.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-06 06:49 com/phida/tests/main_test.py
 -rw-r--r--  2.0 unx        0 b- defN 24-Feb-06 06:49 com/phida/tests/utils_test.py
--rw-r--r--  2.0 unx      190 b- defN 24-Feb-27 21:32 SilverStreamingApplicationPoC-1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-27 21:32 SilverStreamingApplicationPoC-1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        4 b- defN 24-Feb-27 21:32 SilverStreamingApplicationPoC-1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1214 b- defN 24-Feb-27 21:32 SilverStreamingApplicationPoC-1.8.dist-info/RECORD
-14 files, 41512 bytes uncompressed, 10935 bytes compressed:  73.7%
+-rw-r--r--  2.0 unx      168 b- defN 24-Feb-28 12:30 SilverStreamingApplicationPoC-1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Feb-28 12:30 SilverStreamingApplicationPoC-1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        4 b- defN 24-Feb-28 12:30 SilverStreamingApplicationPoC-1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1214 b- defN 24-Feb-28 12:30 SilverStreamingApplicationPoC-1.9.dist-info/RECORD
+14 files, 42387 bytes uncompressed, 11058 bytes compressed:  73.9%
```

## zipnote {}

```diff
@@ -24,20 +24,20 @@
 
 Filename: com/phida/tests/main_test.py
 Comment: 
 
 Filename: com/phida/tests/utils_test.py
 Comment: 
 
-Filename: SilverStreamingApplicationPoC-1.8.dist-info/METADATA
+Filename: SilverStreamingApplicationPoC-1.9.dist-info/METADATA
 Comment: 
 
-Filename: SilverStreamingApplicationPoC-1.8.dist-info/WHEEL
+Filename: SilverStreamingApplicationPoC-1.9.dist-info/WHEEL
 Comment: 
 
-Filename: SilverStreamingApplicationPoC-1.8.dist-info/top_level.txt
+Filename: SilverStreamingApplicationPoC-1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: SilverStreamingApplicationPoC-1.8.dist-info/RECORD
+Filename: SilverStreamingApplicationPoC-1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## com/phida/main/Operations.py

```diff
@@ -1,9 +1,9 @@
 from pyspark.sql.utils import AnalysisException
-from com.phida.main.sparksession import spark
+#from com.phida.main.sparksession import spark
 from pyspark.sql.functions import col
 
 
 def tableExists(dbName, tblName):
     """
     desc:
         A static function for checking whether a given table exists.
```

## com/phida/main/SilverMerge.py

```diff
@@ -1,8 +1,8 @@
-from com.phida.main.sparksession import spark, logger
+#from com.phida.main.sparksession import spark, logger
 from com.phida.main.Operations import tableExists, addDerivedColumns, createDeltaTable, alterDeltaTable, \
     dropColumns, getDerivedColumnsList, schemaDiff, getKeyCols, buildJoinCondition, buildColumnsDict, hiveDDL, schemaDataTypeDiff
 from com.phida.main.utils import pathExists, convertStrToList
 from pyspark.sql.functions import row_number, col, broadcast
 from pyspark.sql.window import Window
 from delta.tables import DeltaTable
 from time import sleep
```

## com/phida/main/sparksession.py

```diff
@@ -9,23 +9,42 @@
 
 ###############Above lines are commented and Below lines are added by Shilton#########
 import pyspark
 import base64
 from pyspark.sql import SparkSession
 from com.phida.main import logging
 
-with open("/mnt/secrets/azure-secret.txt", "rb") as file:
-    storage_account_key = file.read().strip()
+def create_spark_session(app_name):
+    with open("/mnt/secrets/azure-secret.txt", "rb") as file:
+        storage_account_key = file.read().strip()
 
-decoded_key = base64.b64decode(storage_account_key).decode("utf-8")
+    decoded_key = base64.b64decode(storage_account_key).decode("utf-8")
 
-#This 'sparkAppName' is substituted by the arguments section of the SparkApplication.
-spark = SparkSession.builder \
-    .appName(sparkAppName) \
-    .config('spark.jars.packages', 'org.apache.hadoop:hadoop-azure:3.3.1') \
-    .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension") \
-    .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog") \
-    .config("fs.azure.account.auth.type.eabase.dfs.core.windows.net", "SharedKey") \
-    .config("fs.azure.account.key.eabase.dfs.core.windows.net", decoded_key) \
-    .getOrCreate()
+    # Pass 'app_name' as an argument to appName method
+    spark = SparkSession.builder \
+        .appName(app_name) \
+        .config('spark.jars.packages', 'org.apache.hadoop:hadoop-azure:3.3.1') \
+        .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension") \
+        .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog") \
+        .config("fs.azure.account.auth.type.eabase.dfs.core.windows.net", "SharedKey") \
+        .config("fs.azure.account.key.eabase.dfs.core.windows.net", decoded_key) \
+        .getOrCreate()
 
-logger = logging.Log4j(spark)
+    logger = logging.Log4j(spark)
+
+    return spark, logger
+# with open("/mnt/secrets/azure-secret.txt", "rb") as file:
+#     storage_account_key = file.read().strip()
+
+# decoded_key = base64.b64decode(storage_account_key).decode("utf-8")
+
+# #This 'sparkAppName' is substituted by the arguments section of the SparkApplication.
+# spark = SparkSession.builder \
+#     .appName("SilverMerge") \
+#     .config('spark.jars.packages', 'org.apache.hadoop:hadoop-azure:3.3.1') \
+#     .config("spark.sql.extensions", "io.delta.sql.DeltaSparkSessionExtension") \
+#     .config("spark.sql.catalog.spark_catalog", "org.apache.spark.sql.delta.catalog.DeltaCatalog") \
+#     .config("fs.azure.account.auth.type.eabase.dfs.core.windows.net", "SharedKey") \
+#     .config("fs.azure.account.key.eabase.dfs.core.windows.net", decoded_key) \
+#     .getOrCreate()
+
+# logger = logging.Log4j(spark)
```

## com/phida/main/utils.py

```diff
@@ -1,9 +1,9 @@
 import os
-from com.phida.main.sparksession import spark
+#from com.phida.main.sparksession import spark
 from pyspark.sql.utils import AnalysisException
 
 def convertToUnixPath(path):
     """
     desc:
         A Function for converting dbfs path to equivalent unix path with just a dbfs prefix.
         Converting to unix path is to make sure that even if the source path has wild characters,
```

