# Comparing `tmp/matter_observability-2.0.1-py3-none-any.whl.zip` & `tmp/matter_observability-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11310 bytes, number of entries: 21
+Zip file size: 11383 bytes, number of entries: 21
 -rw-r--r--  2.0 unx      134 b- defN 20-Feb-02 00:00 matter_observability/__about__.py
 -rw-r--r--  2.0 unx      112 b- defN 20-Feb-02 00:00 matter_observability/__init__.py
 -rw-r--r--  2.0 unx      331 b- defN 20-Feb-02 00:00 matter_observability/config.py
 -rw-r--r--  2.0 unx      132 b- defN 20-Feb-02 00:00 matter_observability/exceptions.py
 -rw-r--r--  2.0 unx      133 b- defN 20-Feb-02 00:00 matter_observability/fastapi/__init__.py
 -rw-r--r--  2.0 unx      641 b- defN 20-Feb-02 00:00 matter_observability/fastapi/request_id.py
 -rw-r--r--  2.0 unx      536 b- defN 20-Feb-02 00:00 matter_observability/fastapi/utils.py
@@ -12,12 +12,12 @@
 -rw-r--r--  2.0 unx      868 b- defN 20-Feb-02 00:00 matter_observability/metrics/custom_metrics.py
 -rw-r--r--  2.0 unx     2428 b- defN 20-Feb-02 00:00 matter_observability/metrics/decorators.py
 -rw-r--r--  2.0 unx      473 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_counter.py
 -rw-r--r--  2.0 unx      489 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge.py
 -rw-r--r--  2.0 unx      708 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_gauge_duration.py
 -rw-r--r--  2.0 unx      421 b- defN 20-Feb-02 00:00 matter_observability/metrics/labeled_metric.py
 -rw-r--r--  2.0 unx      900 b- defN 20-Feb-02 00:00 matter_observability/metrics/utils.py
-?rw-r--r--  2.0 unx     5897 b- defN 20-Feb-02 00:00 matter_observability-2.0.1.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-2.0.1.dist-info/WHEEL
-?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-2.0.1.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-2.0.1.dist-info/RECORD
-21 files, 20171 bytes uncompressed, 7944 bytes compressed:  60.6%
+?rw-r--r--  2.0 unx     6027 b- defN 20-Feb-02 00:00 matter_observability-2.0.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 matter_observability-2.0.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx     1068 b- defN 20-Feb-02 00:00 matter_observability-2.0.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx     1999 b- defN 20-Feb-02 00:00 matter_observability-2.0.2.dist-info/RECORD
+21 files, 20301 bytes uncompressed, 8017 bytes compressed:  60.5%
```

## zipnote {}

```diff
@@ -45,20 +45,20 @@
 
 Filename: matter_observability/metrics/labeled_metric.py
 Comment: 
 
 Filename: matter_observability/metrics/utils.py
 Comment: 
 
-Filename: matter_observability-2.0.1.dist-info/METADATA
+Filename: matter_observability-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: matter_observability-2.0.1.dist-info/WHEEL
+Filename: matter_observability-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: matter_observability-2.0.1.dist-info/licenses/LICENSE
+Filename: matter_observability-2.0.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: matter_observability-2.0.1.dist-info/RECORD
+Filename: matter_observability-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## matter_observability/__about__.py

```diff
@@ -1,4 +1,4 @@
 # SPDX-FileCopyrightText: 2023-present Rômulo Jales <romulo@thisismatter.com>
 #
 # SPDX-License-Identifier: MIT
-__version__ = "2.0.1"
+__version__ = "2.0.2"
```

## Comparing `matter_observability-2.0.1.dist-info/METADATA` & `matter_observability-2.0.2.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: matter-observability
-Version: 2.0.1
+Version: 2.0.2
 Summary: A template for Matter's observability library
 Project-URL: Documentation, https://github.com/Matter-Tech/matter-observability#readme
 Project-URL: Issues, https://github.com/Matter-Tech/matter-observability/issues
 Project-URL: Source, https://github.com/Matter-Tech/matter-observability
 Author-email: Tomer Sasson <tomer@thisismatter.com>
 License-Expression: MIT
 License-File: LICENSE
@@ -178,23 +178,26 @@
 ```
 
 Make sure that you have set the following ENV values:
 ```env
 SERVER_LOG_LEVEL=debug
 PROMETHEUS_PUSH_GATEWAY_HOST=localhost
 INSTANCE_NAME=observability_instance
+ENABLE_METRICS=true
 ```
+The last one is required for the API metrics endpoint to be exposed - they are not enabled by default!
 
 
 ## Contributing
 
 Make sure you have all supported python versions installed in your machine:
 
 * 3.10
 * 3.11
+* 3.12
 
 ### Install hatch in your system
 
 ```https://hatch.pypa.io/latest/install/```
 
 ### Create the environment
```

## Comparing `matter_observability-2.0.1.dist-info/licenses/LICENSE` & `matter_observability-2.0.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `matter_observability-2.0.1.dist-info/RECORD` & `matter_observability-2.0.2.dist-info/RECORD`

 * *Files 18% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-matter_observability/__about__.py,sha256=PUxRIZJJ4cTHqB6m1DOzeE3lL4QPyOkQshyVxicDngs,134
+matter_observability/__about__.py,sha256=uVEBPzvzLMjJ_cWa7GsT69XJqJ-AyShRDnJh7Tj2JtU,134
 matter_observability/__init__.py,sha256=3w1lcMfVq_KzRTAJVSrwL5vGSnu2BzERE4WFHCGvzFY,112
 matter_observability/config.py,sha256=UKORWKu3BE9FvzuLYT8HbCAtvwuB5Lxu24ho1ft73fs,331
 matter_observability/exceptions.py,sha256=vc3AZT1ZsrkTgnkeoiOFsAgsSIlCkywHryUnm-APVQo,132
 matter_observability/fastapi/__init__.py,sha256=TBGRRAMg7Q2Ov_a6sUZuWIoH9ITxWF036CYLVn-K25g,133
 matter_observability/fastapi/request_id.py,sha256=frjbfIr6U3J6ElbA5ZDnNFiz7eKerCGStevHHZu78P0,641
 matter_observability/fastapi/utils.py,sha256=VOux21KI6HJMZgPDWoozLV7lHiaoh6WHT0LKf6kp6W4,536
 matter_observability/logging/__init__.py,sha256=Xz1akGf5QHmMHjF9PpQ6Ljx8V5VI28N1tjom11jEKnQ,73
@@ -11,11 +11,11 @@
 matter_observability/metrics/custom_metrics.py,sha256=2DCMSyAwnSf8hfNeRCAKdWLm5BGFp3C0vRQHvNVVCSM,868
 matter_observability/metrics/decorators.py,sha256=LdnXq5dpxrBsjw6iOtFys3DLHmBhSK59FiusIkp8kHM,2428
 matter_observability/metrics/labeled_counter.py,sha256=SO7h6_4MAhO_AzQJOMhl2puB3vBBY6YQeVFhbYlPeH8,473
 matter_observability/metrics/labeled_gauge.py,sha256=MYJRPuqsvrjdBmDIiBaxzA66CUjJVI1KOGvzRRhDas0,489
 matter_observability/metrics/labeled_gauge_duration.py,sha256=mXVxqHi5RKL1-e6pC7i8-huopt53D1KfrMRcCEZbe_Y,708
 matter_observability/metrics/labeled_metric.py,sha256=Qn4psWuJJTyALay8-wU0vK2Y0epp25JWPSoZ8BQK8hM,421
 matter_observability/metrics/utils.py,sha256=TjhMxm3hj8PrOpJxuBHkwqexvXDuZPx7Oiul3EDlcUA,900
-matter_observability-2.0.1.dist-info/METADATA,sha256=U56slc3JBOMvbGiF23f6FaPg_eltpLILu6jTBfk2g9g,5897
-matter_observability-2.0.1.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
-matter_observability-2.0.1.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
-matter_observability-2.0.1.dist-info/RECORD,,
+matter_observability-2.0.2.dist-info/METADATA,sha256=8hYs5COgo7Ct5AIkZbywdqI8OGg-pkSq8ruAE7Dq3dg,6027
+matter_observability-2.0.2.dist-info/WHEEL,sha256=zEMcRr9Kr03x1ozGwg5v9NQBKn3kndp6LSoSlVg-jhU,87
+matter_observability-2.0.2.dist-info/licenses/LICENSE,sha256=bqRY4B_u4xSKzKFb3ML8l0nCWvMXyzEGwY2B2hteV8g,1068
+matter_observability-2.0.2.dist-info/RECORD,,
```

