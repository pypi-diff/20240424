# Comparing `tmp/dynatrace_opentelemetry_gcf-1.287.2-py3-none-any.whl.zip` & `tmp/dynatrace_opentelemetry_gcf-1.289.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 12137 bytes, number of entries: 10
+Zip file size: 12139 bytes, number of entries: 10
 -rw-r--r--  2.0 unx      675 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/__init__.py
 -rw-r--r--  2.0 unx     4834 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_resource.py
 -rw-r--r--  2.0 unx     6676 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_trigger.py
 -rw-r--r--  2.0 unx     1938 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/_wrapper.py
 -rw-r--r--  2.0 unx        0 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/py.typed
 -rw-r--r--  2.0 unx       24 b- defN 20-Feb-02 00:00 dynatrace/opentelemetry/gcf/version.py
-?rw-r--r--  2.0 unx     1189 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.287.2.dist-info/METADATA
-?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.287.2.dist-info/WHEEL
-?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.287.2.dist-info/licenses/LICENSE
-?rw-r--r--  2.0 unx      959 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.287.2.dist-info/RECORD
-10 files, 27724 bytes uncompressed, 10455 bytes compressed:  62.3%
+?rw-r--r--  2.0 unx     1240 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.289.2.dist-info/METADATA
+?rw-r--r--  2.0 unx       87 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.289.2.dist-info/WHEEL
+?rw-r--r--  2.0 unx    11342 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.289.2.dist-info/licenses/LICENSE
+?rw-r--r--  2.0 unx      959 b- defN 20-Feb-02 00:00 dynatrace_opentelemetry_gcf-1.289.2.dist-info/RECORD
+10 files, 27775 bytes uncompressed, 10457 bytes compressed:  62.4%
```

## zipnote {}

```diff
@@ -12,20 +12,20 @@
 
 Filename: dynatrace/opentelemetry/gcf/py.typed
 Comment: 
 
 Filename: dynatrace/opentelemetry/gcf/version.py
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.287.2.dist-info/METADATA
+Filename: dynatrace_opentelemetry_gcf-1.289.2.dist-info/METADATA
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.287.2.dist-info/WHEEL
+Filename: dynatrace_opentelemetry_gcf-1.289.2.dist-info/WHEEL
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.287.2.dist-info/licenses/LICENSE
+Filename: dynatrace_opentelemetry_gcf-1.289.2.dist-info/licenses/LICENSE
 Comment: 
 
-Filename: dynatrace_opentelemetry_gcf-1.287.2.dist-info/RECORD
+Filename: dynatrace_opentelemetry_gcf-1.289.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## dynatrace/opentelemetry/gcf/version.py

```diff
@@ -1 +1 @@
-__version__ = "1.287.2"
+__version__ = "1.289.2"
```

## Comparing `dynatrace_opentelemetry_gcf-1.287.2.dist-info/METADATA` & `dynatrace_opentelemetry_gcf-1.289.2.dist-info/METADATA`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: dynatrace-opentelemetry-gcf
-Version: 1.287.2
+Version: 1.289.2
 Summary: Dynatrace OpenTelemetry package for Google Cloud Functions
 Project-URL: Homepage, https://www.dynatrace.com/technologies/python-monitoring/
 Author: Dynatrace
 License-Expression: Apache-2.0
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,17 +12,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Requires-Python: >=3.7
-Requires-Dist: dynatrace-opentelemetry-core==1.287.2
+Requires-Dist: dynatrace-opentelemetry-core==1.289.2
 Requires-Dist: flask<3.0,>=1.0
 Requires-Dist: opentelemetry-api~=1.3
 Provides-Extra: test
 Description-Content-Type: text/markdown
 
 # Dynatrace OpenTelemetry Tracing API For Python Google Cloud Functions
```

## Comparing `dynatrace_opentelemetry_gcf-1.287.2.dist-info/licenses/LICENSE` & `dynatrace_opentelemetry_gcf-1.289.2.dist-info/licenses/LICENSE`

 * *Files identical despite different names*

## Comparing `dynatrace_opentelemetry_gcf-1.287.2.dist-info/RECORD` & `dynatrace_opentelemetry_gcf-1.289.2.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 dynatrace/opentelemetry/gcf/__init__.py,sha256=pVCQ15ocBp7DACT2JC5wmLkyVRbeSqpF5nWkbypokL8,675
 dynatrace/opentelemetry/gcf/_resource.py,sha256=u2eY520ADxlgDir0OoapHkIf1Y9HdR-qSxxkcPkIV4I,4834
 dynatrace/opentelemetry/gcf/_trigger.py,sha256=8ATt5AkxQOzfNSwr531xBRFmBwD4H3B95-n_Mu35t6U,6676
 dynatrace/opentelemetry/gcf/_wrapper.py,sha256=aigZlgBBlF2Sxsd04xmzSr5nm3-rM61B0y4ttk_3r0c,1938
 dynatrace/opentelemetry/gcf/py.typed,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-dynatrace/opentelemetry/gcf/version.py,sha256=QzOEChxrQMlfXGe0Pi_npelWOm2Nzt1j2QAPCJB0mSM,24
-dynatrace_opentelemetry_gcf-1.287.2.dist-info/METADATA,sha256=nBrYNQygZbO7fIKvMYIMeCdy0NLLGnVhDtvvWPJgQTs,1189
-dynatrace_opentelemetry_gcf-1.287.2.dist-info/WHEEL,sha256=TJPnKdtrSue7xZ_AVGkp9YXcvDrobsjBds1du3Nx6dc,87
-dynatrace_opentelemetry_gcf-1.287.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
-dynatrace_opentelemetry_gcf-1.287.2.dist-info/RECORD,,
+dynatrace/opentelemetry/gcf/version.py,sha256=Y9A7I6XsG7FHtVRDTjoVmxJh-Cc_oWT6WseL3kzaL4o,24
+dynatrace_opentelemetry_gcf-1.289.2.dist-info/METADATA,sha256=LrPciD6hJ-dLZDC9ApSxT70XMNTErL2PKUqoditbzM0,1240
+dynatrace_opentelemetry_gcf-1.289.2.dist-info/WHEEL,sha256=bq9SyP5NxIRA9EpQgMCd-9RmPHWvbH-4lTDGwxgIR64,87
+dynatrace_opentelemetry_gcf-1.289.2.dist-info/licenses/LICENSE,sha256=OUyLShRPZFGLXlxbnRr7Of_8mNYYQ_qda632uhGSIaY,11342
+dynatrace_opentelemetry_gcf-1.289.2.dist-info/RECORD,,
```

