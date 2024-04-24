# Comparing `tmp/botocore-a-la-carte-omics-1.34.89.tar.gz` & `tmp/botocore-a-la-carte-omics-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-omics-1.34.89.tar", last modified: Tue Apr 23 01:02:11 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-omics-1.34.9.tar", last modified: Thu Dec 28 01:06:54 2023, max compression
```

## Comparing `botocore-a-la-carte-omics-1.34.89.tar` & `botocore-a-la-carte-omics-1.34.9.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:11.477760 botocore-a-la-carte-omics-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-23 01:02:11.000000 botocore-a-la-carte-omics-1.34.89/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-23 01:02:11.477760 botocore-a-la-carte-omics-1.34.89/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:11.473760 botocore-a-la-carte-omics-1.34.89/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:11.473760 botocore-a-la-carte-omics-1.34.89/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:11.473760 botocore-a-la-carte-omics-1.34.89/botocore/data/omics/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:11.473760 botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/
--rw-r--r--   0 runner    (1001) docker     (127)    17620 2024-04-23 01:01:45.000000 botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     3466 2024-04-23 01:01:45.000000 botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   281236 2024-04-23 01:01:45.000000 botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)    14692 2024-04-23 01:01:45.000000 botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:11.477760 botocore-a-la-carte-omics-1.34.89/botocore_a_la_carte_omics.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-04-23 01:02:11.000000 botocore-a-la-carte-omics-1.34.89/botocore_a_la_carte_omics.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-23 01:02:11.000000 botocore-a-la-carte-omics-1.34.89/botocore_a_la_carte_omics.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:02:11.000000 botocore-a-la-carte-omics-1.34.89/botocore_a_la_carte_omics.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 01:02:11.000000 botocore-a-la-carte-omics-1.34.89/botocore_a_la_carte_omics.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:02:11.477760 botocore-a-la-carte-omics-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-23 01:02:11.000000 botocore-a-la-carte-omics-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:54.318378 botocore-a-la-carte-omics-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:54.000000 botocore-a-la-carte-omics-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-12-28 01:06:54.318378 botocore-a-la-carte-omics-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:54.314378 botocore-a-la-carte-omics-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:54.314378 botocore-a-la-carte-omics-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:54.314378 botocore-a-la-carte-omics-1.34.9/botocore/data/omics/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:54.318378 botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/
+-rw-r--r--   0 runner    (1001) docker     (127)    17620 2023-12-28 01:06:26.000000 botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3466 2023-12-28 01:06:26.000000 botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   279011 2023-12-28 01:06:26.000000 botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14692 2023-12-28 01:06:26.000000 botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:54.318378 botocore-a-la-carte-omics-1.34.9/botocore_a_la_carte_omics.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      953 2023-12-28 01:06:54.000000 botocore-a-la-carte-omics-1.34.9/botocore_a_la_carte_omics.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2023-12-28 01:06:54.000000 botocore-a-la-carte-omics-1.34.9/botocore_a_la_carte_omics.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:54.000000 botocore-a-la-carte-omics-1.34.9/botocore_a_la_carte_omics.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:54.000000 botocore-a-la-carte-omics-1.34.9/botocore_a_la_carte_omics.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:54.318378 botocore-a-la-carte-omics-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2023-12-28 01:06:54.000000 botocore-a-la-carte-omics-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-omics-1.34.89/LICENSE.txt` & `botocore-a-la-carte-omics-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-omics-1.34.89/PKG-INFO` & `botocore-a-la-carte-omics-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-omics
-Version: 1.34.89
+Version: 1.34.9
 Summary: omics data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/endpoint-rule-set-1.json` & `botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/paginators-1.json` & `botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/service-2.json` & `botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/service-2.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9986804300814679%*

 * *Differences: {"'operations'": "{'AbortMultipartReadSetUpload': {'documentation': '<p> Stops a multipart upload. "*

 * *                 "</p>'}, 'CompleteMultipartReadSetUpload': {'documentation': '<p> Concludes a "*

 * *                 "multipart upload once you have uploaded all the components. </p>'}, "*

 * *                 "'CreateMultipartReadSetUpload': {'documentation': '<p> Begins a multipart read "*

 * *                 "set upload. </p>'}, 'ListMultipartReadSetUploads': {'documentation': '<p> Lists "*

 * *                 'multipart […]*

```diff
@@ -9,15 +9,15 @@
         "serviceId": "Omics",
         "signatureVersion": "v4",
         "signingName": "omics",
         "uid": "omics-2022-11-28"
     },
     "operations": {
         "AbortMultipartReadSetUpload": {
-            "documentation": "<p>Stops a multipart upload.</p>",
+            "documentation": "<p> Stops a multipart upload. </p>",
             "endpoint": {
                 "hostPrefix": "control-storage-"
             },
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
@@ -246,15 +246,15 @@
             },
             "name": "CancelVariantImportJob",
             "output": {
                 "shape": "CancelVariantImportResponse"
             }
         },
         "CompleteMultipartReadSetUpload": {
-            "documentation": "<p>Concludes a multipart upload once you have uploaded all the components.</p>",
+            "documentation": "<p> Concludes a multipart upload once you have uploaded all the components. </p>",
             "endpoint": {
                 "hostPrefix": "storage-"
             },
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
@@ -372,15 +372,15 @@
             },
             "name": "CreateAnnotationStoreVersion",
             "output": {
                 "shape": "CreateAnnotationStoreVersionResponse"
             }
         },
         "CreateMultipartReadSetUpload": {
-            "documentation": "<p>Begins a multipart read set upload.</p>",
+            "documentation": "<p> Begins a multipart read set upload. </p>",
             "endpoint": {
                 "hostPrefix": "control-storage-"
             },
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
@@ -1959,15 +1959,15 @@
             },
             "name": "ListAnnotationStores",
             "output": {
                 "shape": "ListAnnotationStoresResponse"
             }
         },
         "ListMultipartReadSetUploads": {
-            "documentation": "<p>Lists multipart read set uploads and for in progress uploads. Once the upload is completed, a read set is created and the upload will no longer be returned in the response.</p>",
+            "documentation": "<p> Lists multipart read set uploads and for in progress uploads. Once the upload is completed, a read set is created and the upload will no longer be returned in the respone. </p>",
             "endpoint": {
                 "hostPrefix": "control-storage-"
             },
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
@@ -2117,15 +2117,15 @@
             },
             "name": "ListReadSetImportJobs",
             "output": {
                 "shape": "ListReadSetImportJobsResponse"
             }
         },
         "ListReadSetUploadParts": {
-            "documentation": "<p>This operation will list all parts in a requested multipart upload for a sequence store.</p>",
+            "documentation": "<p> This operation will list all parts in a requested multipart upload for a sequence store. </p>",
             "endpoint": {
                 "hostPrefix": "control-storage-"
             },
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
@@ -3237,15 +3237,15 @@
             "input": {
                 "shape": "UpdateWorkflowRequest"
             },
             "name": "UpdateWorkflow"
         },
         "UploadReadSetPart": {
             "authtype": "v4-unsigned-body",
-            "documentation": "<p>This operation uploads a specific part of a read set. If you upload a new part using a previously used part number, the previously uploaded part will be overwritten.</p>",
+            "documentation": "<p> This operation uploads a specific part of a read set. If you upload a new part using a previously used part number, the previously uploaded part will be overwritten. </p>",
             "endpoint": {
                 "hostPrefix": "storage-"
             },
             "errors": [
                 {
                     "shape": "InternalServerException"
                 },
@@ -3285,21 +3285,21 @@
             }
         }
     },
     "shapes": {
         "AbortMultipartReadSetUploadRequest": {
             "members": {
                 "sequenceStoreId": {
-                    "documentation": "<p>The sequence store ID for the store involved in the multipart upload.</p>",
+                    "documentation": "<p> The sequence store ID for the store involved in the multipart upload. </p>",
                     "location": "uri",
                     "locationName": "sequenceStoreId",
                     "shape": "SequenceStoreId"
                 },
                 "uploadId": {
-                    "documentation": "<p>The ID for the multipart upload.</p>",
+                    "documentation": "<p> The ID for the multipart upload. </p>",
                     "location": "uri",
                     "locationName": "uploadId",
                     "shape": "UploadId"
                 }
             },
             "required": [
                 "sequenceStoreId",
@@ -3839,25 +3839,25 @@
             "max": 1,
             "min": 1,
             "type": "string"
         },
         "CompleteMultipartReadSetUploadRequest": {
             "members": {
                 "parts": {
-                    "documentation": "<p>The individual uploads or parts of a multipart upload.</p>",
+                    "documentation": "<p> The individual uploads or parts of a multipart upload. </p>",
                     "shape": "CompleteReadSetUploadPartList"
                 },
                 "sequenceStoreId": {
-                    "documentation": "<p>The sequence store ID for the store involved in the multipart upload.</p>",
+                    "documentation": "<p> The sequence store ID for the store involved in the multipart upload. </p>",
                     "location": "uri",
                     "locationName": "sequenceStoreId",
                     "shape": "SequenceStoreId"
                 },
                 "uploadId": {
-                    "documentation": "<p>The ID for the multipart upload.</p>",
+                    "documentation": "<p> The ID for the multipart upload. </p>",
                     "location": "uri",
                     "locationName": "uploadId",
                     "shape": "UploadId"
                 }
             },
             "required": [
                 "sequenceStoreId",
@@ -3865,15 +3865,15 @@
                 "parts"
             ],
             "type": "structure"
         },
         "CompleteMultipartReadSetUploadResponse": {
             "members": {
                 "readSetId": {
-                    "documentation": "<p>The read set ID created for an uploaded read set.</p>",
+                    "documentation": "<p> The read set ID created for an uploaded read set. </p>",
                     "shape": "ReadSetId"
                 }
             },
             "required": [
                 "readSetId"
             ],
             "type": "structure"
@@ -3885,15 +3885,15 @@
             "type": "list"
         },
         "CompleteReadSetUploadPartListItem": {
             "documentation": "<p> Part of the response to the CompleteReadSetUpload API, including metadata. </p>",
             "members": {
                 "checksum": {
                     "documentation": "<p> A unique identifier used to confirm that parts are being added to the correct upload. </p>",
-                    "shape": "CompleteReadSetUploadPartListItemChecksumString"
+                    "shape": "String"
                 },
                 "partNumber": {
                     "documentation": "<p> A number identifying the part in a read set upload. </p>",
                     "shape": "CompleteReadSetUploadPartListItemPartNumberInteger"
                 },
                 "partSource": {
                     "documentation": "<p> The source file of the part being uploaded. </p>",
@@ -3903,20 +3903,14 @@
             "required": [
                 "partNumber",
                 "partSource",
                 "checksum"
             ],
             "type": "structure"
         },
-        "CompleteReadSetUploadPartListItemChecksumString": {
-            "max": 100,
-            "min": 1,
-            "pattern": "[\\p{L}||\\p{M}||\\p{Z}||\\p{S}||\\p{N}||\\p{P}]+",
-            "type": "string"
-        },
         "CompleteReadSetUploadPartListItemPartNumberInteger": {
             "box": true,
             "max": 10000,
             "min": 1,
             "type": "integer"
         },
         "CompletionTime": {
@@ -4095,53 +4089,53 @@
                 "creationTime"
             ],
             "type": "structure"
         },
         "CreateMultipartReadSetUploadRequest": {
             "members": {
                 "clientToken": {
-                    "documentation": "<p>An idempotency token that can be used to avoid triggering multiple multipart uploads.</p>",
+                    "documentation": "<p> An idempotency token that can be used to avoid triggering multiple multipart uploads. </p>",
                     "shape": "ClientToken"
                 },
                 "description": {
-                    "documentation": "<p>The description of the read set.</p>",
+                    "documentation": "<p> The description of the read set. </p>",
                     "shape": "ReadSetDescription"
                 },
                 "generatedFrom": {
-                    "documentation": "<p>Where the source originated.</p>",
+                    "documentation": "<p> Where the source originated. </p>",
                     "shape": "GeneratedFrom"
                 },
                 "name": {
-                    "documentation": "<p>The name of the read set.</p>",
+                    "documentation": "<p> The name of the read set. </p>",
                     "shape": "ReadSetName"
                 },
                 "referenceArn": {
-                    "documentation": "<p>The ARN of the reference.</p>",
+                    "documentation": "<p> The ARN of the reference. </p>",
                     "shape": "ReferenceArn"
                 },
                 "sampleId": {
-                    "documentation": "<p>The source's sample ID.</p>",
+                    "documentation": "<p> The source's sample ID. </p>",
                     "shape": "SampleId"
                 },
                 "sequenceStoreId": {
-                    "documentation": "<p>The sequence store ID for the store that is the destination of the multipart uploads.</p>",
+                    "documentation": "<p> The sequence store ID for the store that is the destination of the multipart uploads. </p>",
                     "location": "uri",
                     "locationName": "sequenceStoreId",
                     "shape": "SequenceStoreId"
                 },
                 "sourceFileType": {
-                    "documentation": "<p>The type of file being uploaded.</p>",
+                    "documentation": "<p> The type of file being uploaded. </p>",
                     "shape": "FileType"
                 },
                 "subjectId": {
-                    "documentation": "<p>The source's subject ID.</p>",
+                    "documentation": "<p> The source's subject ID. </p>",
                     "shape": "SubjectId"
                 },
                 "tags": {
-                    "documentation": "<p>Any tags to add to the read set.</p>",
+                    "documentation": "<p> Any tags to add to the read set. </p>",
                     "shape": "TagMap"
                 }
             },
             "required": [
                 "sequenceStoreId",
                 "sourceFileType",
                 "subjectId",
@@ -4149,55 +4143,55 @@
                 "name"
             ],
             "type": "structure"
         },
         "CreateMultipartReadSetUploadResponse": {
             "members": {
                 "creationTime": {
-                    "documentation": "<p>The creation time of the multipart upload.</p>",
+                    "documentation": "<p> The creation time of the multipart upload. </p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "description": {
-                    "documentation": "<p>The description of the read set.</p>",
+                    "documentation": "<p> The description of the read set. </p>",
                     "shape": "ReadSetDescription"
                 },
                 "generatedFrom": {
-                    "documentation": "<p>The source of the read set.</p>",
+                    "documentation": "<p> The source of the read set. </p>",
                     "shape": "GeneratedFrom"
                 },
                 "name": {
-                    "documentation": "<p>The name of the read set.</p>",
+                    "documentation": "<p> The name of the read set. </p>",
                     "shape": "ReadSetName"
                 },
                 "referenceArn": {
-                    "documentation": "<p>The read set source's reference ARN.</p>",
+                    "documentation": "<p> The read set source's reference ARN. </p>",
                     "shape": "ReferenceArn"
                 },
                 "sampleId": {
-                    "documentation": "<p>The source's sample ID.</p>",
+                    "documentation": "<p> The source's sample ID. </p>",
                     "shape": "SampleId"
                 },
                 "sequenceStoreId": {
-                    "documentation": "<p>The sequence store ID for the store that the read set will be created in.</p>",
+                    "documentation": "<p> The sequence store ID for the store that the read set will be created in. </p>",
                     "shape": "SequenceStoreId"
                 },
                 "sourceFileType": {
-                    "documentation": "<p>The file type of the read set source.</p>",
+                    "documentation": "<p> The file type of the read set source. </p>",
                     "shape": "FileType"
                 },
                 "subjectId": {
-                    "documentation": "<p>The source's subject ID.</p>",
+                    "documentation": "<p> The source's subject ID. </p>",
                     "shape": "SubjectId"
                 },
                 "tags": {
-                    "documentation": "<p>The tags to add to the read set.</p>",
+                    "documentation": "<p> The tags to add to the read set. </p>",
                     "shape": "TagMap"
                 },
                 "uploadId": {
-                    "documentation": "<p>The ID for the initiated multipart upload.</p>",
+                    "documentation": "<p> he ID for the initiated multipart upload. </p>",
                     "shape": "UploadId"
                 }
             },
             "required": [
                 "sequenceStoreId",
                 "uploadId",
                 "sourceFileType",
@@ -4277,15 +4271,15 @@
                     "shape": "CreateRunGroupRequestMaxCpusInteger"
                 },
                 "maxDuration": {
                     "documentation": "<p>A maximum run time for the group in minutes.</p>",
                     "shape": "CreateRunGroupRequestMaxDurationInteger"
                 },
                 "maxGpus": {
-                    "documentation": "<p>The maximum GPUs that can be used by a run group.</p>",
+                    "documentation": "<p> The maximum GPUs that can be used by a run group. </p>",
                     "shape": "CreateRunGroupRequestMaxGpusInteger"
                 },
                 "maxRuns": {
                     "documentation": "<p>The maximum number of concurrent runs for the group.</p>",
                     "shape": "CreateRunGroupRequestMaxRunsInteger"
                 },
                 "name": {
@@ -4354,20 +4348,16 @@
                     "documentation": "<p>To ensure that requests don't run multiple times, specify a unique token for each request.</p>",
                     "shape": "ClientToken"
                 },
                 "description": {
                     "documentation": "<p>A description for the store.</p>",
                     "shape": "SequenceStoreDescription"
                 },
-                "eTagAlgorithmFamily": {
-                    "documentation": "<p>The ETag algorithm family to use for ingested read sets.</p>",
-                    "shape": "ETagAlgorithmFamily"
-                },
                 "fallbackLocation": {
-                    "documentation": "<p>An S3 location that is used to store files that have failed a direct upload.</p>",
+                    "documentation": "<p> An S3 location that is used to store files that have failed a direct upload. </p>",
                     "shape": "S3Destination"
                 },
                 "name": {
                     "documentation": "<p>A name for the store.</p>",
                     "shape": "SequenceStoreName"
                 },
                 "sseConfig": {
@@ -4394,20 +4384,16 @@
                     "documentation": "<p>When the store was created.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "description": {
                     "documentation": "<p>The store's description.</p>",
                     "shape": "SequenceStoreDescription"
                 },
-                "eTagAlgorithmFamily": {
-                    "documentation": "<p>The algorithm family of the ETag.</p>",
-                    "shape": "ETagAlgorithmFamily"
-                },
                 "fallbackLocation": {
-                    "documentation": "<p>An S3 location that is used to store files that have failed a direct upload.</p>",
+                    "documentation": "<p> An S3 location that is used to store files that have failed a direct upload. </p>",
                     "shape": "S3Destination"
                 },
                 "id": {
                     "documentation": "<p>The store's ID.</p>",
                     "shape": "SequenceStoreId"
                 },
                 "name": {
@@ -4522,15 +4508,15 @@
                 "creationTime"
             ],
             "type": "structure"
         },
         "CreateWorkflowRequest": {
             "members": {
                 "accelerators": {
-                    "documentation": "<p>The computational accelerator specified to run the workflow.</p>",
+                    "documentation": "<p> The computational accelerator specified to run the workflow. </p>",
                     "shape": "Accelerators"
                 },
                 "definitionUri": {
                     "documentation": "<p>The URI of a definition for the workflow.</p>",
                     "shape": "WorkflowDefinition"
                 },
                 "definitionZip": {
@@ -4840,50 +4826,36 @@
         },
         "Description": {
             "max": 500,
             "min": 0,
             "type": "string"
         },
         "ETag": {
-            "documentation": "<p>The entity tag (ETag) is a hash of the object representing its semantic content.</p>",
+            "documentation": "<p> The entity tag (ETag) is a hash of the object representing its semantic content. </p>",
             "members": {
                 "algorithm": {
-                    "documentation": "<p>The algorithm used to calculate the read set\u2019s ETag(s).</p>",
+                    "documentation": "<p> The algorithm used to calculate the read set\u2019s ETag(s). </p>",
                     "shape": "ETagAlgorithm"
                 },
                 "source1": {
-                    "documentation": "<p>The ETag hash calculated on Source1 of the read set.</p>",
+                    "documentation": "<p> The ETag hash calculated on Source1 of the read set. </p>",
                     "shape": "String"
                 },
                 "source2": {
-                    "documentation": "<p>The ETag hash calculated on Source2 of the read set.</p>",
+                    "documentation": "<p> The ETag hash calculated on Source2 of the read set. </p>",
                     "shape": "String"
                 }
             },
             "type": "structure"
         },
         "ETagAlgorithm": {
             "enum": [
                 "FASTQ_MD5up",
                 "BAM_MD5up",
-                "CRAM_MD5up",
-                "FASTQ_SHA256up",
-                "BAM_SHA256up",
-                "CRAM_SHA256up",
-                "FASTQ_SHA512up",
-                "BAM_SHA512up",
-                "CRAM_SHA512up"
-            ],
-            "type": "string"
-        },
-        "ETagAlgorithmFamily": {
-            "enum": [
-                "MD5up",
-                "SHA256up",
-                "SHA512up"
+                "CRAM_MD5up"
             ],
             "type": "string"
         },
         "Encoding": {
             "max": 20,
             "min": 1,
             "type": "string"
@@ -5021,18 +4993,14 @@
                     "documentation": "<p>The file's content length.</p>",
                     "shape": "FileInformationContentLengthLong"
                 },
                 "partSize": {
                     "documentation": "<p>The file's part size.</p>",
                     "shape": "FileInformationPartSizeLong"
                 },
-                "s3Access": {
-                    "documentation": "<p>The S3 URI metadata of a sequence store.</p>",
-                    "shape": "ReadSetS3Access"
-                },
                 "totalParts": {
                     "documentation": "<p>The file's total parts.</p>",
                     "shape": "FileInformationTotalPartsInteger"
                 }
             },
             "type": "structure"
         },
@@ -5136,15 +5104,15 @@
                 "jobId"
             ],
             "type": "structure"
         },
         "GetAnnotationImportResponse": {
             "members": {
                 "annotationFields": {
-                    "documentation": "<p>The annotation schema generated by the parsed annotation data.</p>",
+                    "documentation": "<p> The annotation schema generated by the parsed annotation data. </p>",
                     "shape": "AnnotationFieldMap"
                 },
                 "completionTime": {
                     "documentation": "<p>When the job completed.</p>",
                     "shape": "CompletionTime"
                 },
                 "creationTime": {
@@ -5620,15 +5588,15 @@
                     "shape": "CreationType"
                 },
                 "description": {
                     "documentation": "<p>The read set's description.</p>",
                     "shape": "ReadSetDescription"
                 },
                 "etag": {
-                    "documentation": "<p>The entity tag (ETag) is a hash of the object meant to represent its semantic content.</p>",
+                    "documentation": "<p> The entity tag (ETag) is a hash of the object meant to represent its semantic content. </p>",
                     "shape": "ETag"
                 },
                 "fileType": {
                     "documentation": "<p>The read set's file type.</p>",
                     "shape": "FileType"
                 },
                 "files": {
@@ -5660,15 +5628,15 @@
                     "shape": "SequenceStoreId"
                 },
                 "status": {
                     "documentation": "<p>The read set's status.</p>",
                     "shape": "ReadSetStatus"
                 },
                 "statusMessage": {
-                    "documentation": "<p>The status message for a read set. It provides more detail as to why the read set has a status. </p>",
+                    "documentation": "<p> The status message for a read set. It provides more detail as to why the read set has a status. </p>",
                     "shape": "ReadSetStatusMessage"
                 },
                 "subjectId": {
                     "documentation": "<p>The read set's subject ID.</p>",
                     "shape": "SubjectId"
                 }
             },
@@ -6009,15 +5977,15 @@
                     "shape": "GetRunGroupResponseMaxCpusInteger"
                 },
                 "maxDuration": {
                     "documentation": "<p>The group's maximum run time in minutes.</p>",
                     "shape": "GetRunGroupResponseMaxDurationInteger"
                 },
                 "maxGpus": {
-                    "documentation": "<p>The maximum GPUs that can be used by a run group.</p>",
+                    "documentation": "<p> The maximum GPUs that can be used by a run group. </p>",
                     "shape": "GetRunGroupResponseMaxGpusInteger"
                 },
                 "maxRuns": {
                     "documentation": "<p>The maximum number of concurrent runs for the group.</p>",
                     "shape": "GetRunGroupResponseMaxRunsInteger"
                 },
                 "name": {
@@ -6074,15 +6042,15 @@
                 "id"
             ],
             "type": "structure"
         },
         "GetRunResponse": {
             "members": {
                 "accelerators": {
-                    "documentation": "<p>The computational accelerator used to run the workflow.</p>",
+                    "documentation": "<p> The computational accelerator used to run the workflow. </p>",
                     "shape": "Accelerators"
                 },
                 "arn": {
                     "documentation": "<p>The run's ARN.</p>",
                     "shape": "RunArn"
                 },
                 "creationTime": {
@@ -6094,27 +6062,27 @@
                     "shape": "WorkflowDefinition"
                 },
                 "digest": {
                     "documentation": "<p>The run's digest.</p>",
                     "shape": "WorkflowDigest"
                 },
                 "failureReason": {
-                    "documentation": "<p>The reason a run has failed.</p>",
+                    "documentation": "<p> The reason a run has failed. </p>",
                     "shape": "RunFailureReason"
                 },
                 "id": {
                     "documentation": "<p>The run's ID.</p>",
                     "shape": "RunId"
                 },
                 "logLevel": {
                     "documentation": "<p>The run's log level.</p>",
                     "shape": "RunLogLevel"
                 },
                 "logLocation": {
-                    "documentation": "<p>The location of the run log.</p>",
+                    "documentation": "<p> The location of the run log. </p>",
                     "shape": "RunLogLocation"
                 },
                 "name": {
                     "documentation": "<p>The run's name.</p>",
                     "shape": "RunName"
                 },
                 "outputUri": {
@@ -6146,15 +6114,15 @@
                     "shape": "RunGroupId"
                 },
                 "runId": {
                     "documentation": "<p>The run's ID.</p>",
                     "shape": "RunId"
                 },
                 "runOutputUri": {
-                    "documentation": "<p>The destination for workflow outputs.</p>",
+                    "documentation": "<p> The destination for workflow outputs. </p>",
                     "shape": "RunOutputUri"
                 },
                 "startTime": {
                     "documentation": "<p>When the run started.</p>",
                     "shape": "RunTimestamp"
                 },
                 "startedBy": {
@@ -6178,15 +6146,15 @@
                     "shape": "GetRunResponseStorageCapacityInteger"
                 },
                 "tags": {
                     "documentation": "<p>The run's tags.</p>",
                     "shape": "TagMap"
                 },
                 "uuid": {
-                    "documentation": "<p>The universally unique identifier for a run.</p>",
+                    "documentation": "<p> The universally unique identifier for a run. </p>",
                     "shape": "RunUuid"
                 },
                 "workflowId": {
                     "documentation": "<p>The run's workflow ID.</p>",
                     "shape": "WorkflowId"
                 },
                 "workflowType": {
@@ -6236,23 +6204,23 @@
                     "shape": "GetRunTaskResponseCpusInteger"
                 },
                 "creationTime": {
                     "documentation": "<p>When the task was created.</p>",
                     "shape": "TaskTimestamp"
                 },
                 "failureReason": {
-                    "documentation": "<p>The reason a task has failed.</p>",
+                    "documentation": "<p> The reason a task has failed. </p>",
                     "shape": "TaskFailureReason"
                 },
                 "gpus": {
-                    "documentation": "<p>The number of Graphics Processing Units (GPU) specified in the task.</p>",
+                    "documentation": "<p> The number of Graphics Processing Units (GPU) specified in the task. </p>",
                     "shape": "GetRunTaskResponseGpusInteger"
                 },
                 "instanceType": {
-                    "documentation": "<p>The instance type for a task.</p>",
+                    "documentation": "<p> The instance type for a task. </p>",
                     "shape": "TaskInstanceType"
                 },
                 "logStream": {
                     "documentation": "<p>The task's log stream.</p>",
                     "shape": "TaskLogStream"
                 },
                 "memory": {
@@ -6325,34 +6293,26 @@
                     "documentation": "<p>When the store was created.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "description": {
                     "documentation": "<p>The store's description.</p>",
                     "shape": "SequenceStoreDescription"
                 },
-                "eTagAlgorithmFamily": {
-                    "documentation": "<p>The algorithm family of the ETag.</p>",
-                    "shape": "ETagAlgorithmFamily"
-                },
                 "fallbackLocation": {
-                    "documentation": "<p>An S3 location that is used to store files that have failed a direct upload.</p>",
+                    "documentation": "<p> An S3 location that is used to store files that have failed a direct upload. </p>",
                     "shape": "S3Destination"
                 },
                 "id": {
                     "documentation": "<p>The store's ID.</p>",
                     "shape": "SequenceStoreId"
                 },
                 "name": {
                     "documentation": "<p>The store's name.</p>",
                     "shape": "SequenceStoreName"
                 },
-                "s3Access": {
-                    "documentation": "<p>The S3 metadata of a sequence store, including the ARN and S3 URI of the S3 bucket.</p>",
-                    "shape": "SequenceStoreS3Access"
-                },
                 "sseConfig": {
                     "documentation": "<p>The store's server-side encryption (SSE) settings.</p>",
                     "shape": "SseConfig"
                 }
             },
             "required": [
                 "id",
@@ -6397,15 +6357,15 @@
                 "jobId"
             ],
             "type": "structure"
         },
         "GetVariantImportResponse": {
             "members": {
                 "annotationFields": {
-                    "documentation": "<p>The annotation schema generated by the parsed annotation data.</p>",
+                    "documentation": "<p> The annotation schema generated by the parsed annotation data. </p>",
                     "shape": "AnnotationFieldMap"
                 },
                 "completionTime": {
                     "documentation": "<p>When the job completed.</p>",
                     "shape": "CompletionTime"
                 },
                 "creationTime": {
@@ -6564,15 +6524,15 @@
                 "id"
             ],
             "type": "structure"
         },
         "GetWorkflowResponse": {
             "members": {
                 "accelerators": {
-                    "documentation": "<p>The computational accelerator specified to run the workflow. </p>",
+                    "documentation": "<p> The computational accelerator specified to run the workflow. </p>",
                     "shape": "Accelerators"
                 },
                 "arn": {
                     "documentation": "<p>The workflow's ARN.</p>",
                     "shape": "WorkflowArn"
                 },
                 "creationTime": {
@@ -6600,15 +6560,15 @@
                     "shape": "WorkflowId"
                 },
                 "main": {
                     "documentation": "<p>The path of the main definition file for the workflow.</p>",
                     "shape": "WorkflowMain"
                 },
                 "metadata": {
-                    "documentation": "<p>Gets metadata for workflow.</p>",
+                    "documentation": "<p> Gets metadata for workflow. </p>",
                     "shape": "WorkflowMetadata"
                 },
                 "name": {
                     "documentation": "<p>The workflow's name.</p>",
                     "shape": "WorkflowName"
                 },
                 "parameterTemplate": {
@@ -7127,27 +7087,27 @@
                 }
             },
             "type": "structure"
         },
         "ListMultipartReadSetUploadsRequest": {
             "members": {
                 "maxResults": {
-                    "documentation": "<p>The maximum number of multipart uploads returned in a page.</p>",
+                    "documentation": "<p> The maximum number of multipart uploads returned in a page. </p>",
                     "location": "querystring",
                     "locationName": "maxResults",
                     "shape": "ListMultipartReadSetUploadsRequestMaxResultsInteger"
                 },
                 "nextToken": {
-                    "documentation": "<p>Next token returned in the response of a previous ListMultipartReadSetUploads call. Used to get the next page of results.</p>",
+                    "documentation": "<p> Next token returned in the response of a previous ListMultipartReadSetUploads call. Used to get the next page of results. </p>",
                     "location": "querystring",
                     "locationName": "nextToken",
                     "shape": "NextToken"
                 },
                 "sequenceStoreId": {
-                    "documentation": "<p>The Sequence Store ID used for the multipart uploads.</p>",
+                    "documentation": "<p> The Sequence Store ID used for the multipart uploads. </p>",
                     "location": "uri",
                     "locationName": "sequenceStoreId",
                     "shape": "SequenceStoreId"
                 }
             },
             "required": [
                 "sequenceStoreId"
@@ -7159,19 +7119,19 @@
             "max": 100,
             "min": 1,
             "type": "integer"
         },
         "ListMultipartReadSetUploadsResponse": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>Next token returned in the response of a previous ListMultipartReadSetUploads call. Used to get the next page of results.</p>",
+                    "documentation": "<p> Next token returned in the response of a previous ListMultipartReadSetUploads call. Used to get the next page of results. </p>",
                     "shape": "NextToken"
                 },
                 "uploads": {
-                    "documentation": "<p>An array of multipart uploads.</p>",
+                    "documentation": "<p> An array of multipart uploads. </p>",
                     "shape": "MultipartReadSetUploadList"
                 }
             },
             "type": "structure"
         },
         "ListReadSetActivationJobsRequest": {
             "members": {
@@ -7319,41 +7279,41 @@
                 }
             },
             "type": "structure"
         },
         "ListReadSetUploadPartsRequest": {
             "members": {
                 "filter": {
-                    "documentation": "<p>Attributes used to filter for a specific subset of read set part uploads.</p>",
+                    "documentation": "<p> Attributes used to filter for a specific subset of read set part uploads. </p>",
                     "shape": "ReadSetUploadPartListFilter"
                 },
                 "maxResults": {
-                    "documentation": "<p>The maximum number of read set upload parts returned in a page.</p>",
+                    "documentation": "<p> The maximum number of read set upload parts returned in a page. </p>",
                     "location": "querystring",
                     "locationName": "maxResults",
                     "shape": "ListReadSetUploadPartsRequestMaxResultsInteger"
                 },
                 "nextToken": {
-                    "documentation": "<p>Next token returned in the response of a previous ListReadSetUploadPartsRequest call. Used to get the next page of results.</p>",
+                    "documentation": "<p> Next token returned in the response of a previous ListReadSetUploadPartsRequest call. Used to get the next page of results. </p>",
                     "location": "querystring",
                     "locationName": "nextToken",
                     "shape": "NextToken"
                 },
                 "partSource": {
-                    "documentation": "<p>The source file for the upload part.</p>",
+                    "documentation": "<p> The source file for the upload part. </p>",
                     "shape": "ReadSetPartSource"
                 },
                 "sequenceStoreId": {
-                    "documentation": "<p>The Sequence Store ID used for the multipart uploads.</p>",
+                    "documentation": "<p> The Sequence Store ID used for the multipart uploads. </p>",
                     "location": "uri",
                     "locationName": "sequenceStoreId",
                     "shape": "SequenceStoreId"
                 },
                 "uploadId": {
-                    "documentation": "<p>The ID for the initiated multipart upload.</p>",
+                    "documentation": "<p> The ID for the initiated multipart upload. </p>",
                     "location": "uri",
                     "locationName": "uploadId",
                     "shape": "UploadId"
                 }
             },
             "required": [
                 "sequenceStoreId",
@@ -7367,19 +7327,19 @@
             "max": 100,
             "min": 1,
             "type": "integer"
         },
         "ListReadSetUploadPartsResponse": {
             "members": {
                 "nextToken": {
-                    "documentation": "<p>Next token returned in the response of a previous ListReadSetUploadParts call. Used to get the next page of results.</p>",
+                    "documentation": "<p> Next token returned in the response of a previous ListReadSetUploadParts call. Used to get the next page of results. </p>",
                     "shape": "NextToken"
                 },
                 "parts": {
-                    "documentation": "<p>An array of upload parts.</p>",
+                    "documentation": "<p> An array of upload parts. </p>",
                     "shape": "ReadSetUploadPartList"
                 }
             },
             "type": "structure"
         },
         "ListReadSetsRequest": {
             "members": {
@@ -7693,15 +7653,15 @@
                 "startingToken": {
                     "documentation": "<p>Specify the pagination token from a previous request to retrieve the next page of results.</p>",
                     "location": "querystring",
                     "locationName": "startingToken",
                     "shape": "RunListToken"
                 },
                 "status": {
-                    "documentation": "<p>The status of a run.</p>",
+                    "documentation": "<p> The status of a run. </p>",
                     "location": "querystring",
                     "locationName": "status",
                     "shape": "RunStatus"
                 }
             },
             "type": "structure"
         },
@@ -8409,15 +8369,15 @@
                     "shape": "CreationType"
                 },
                 "description": {
                     "documentation": "<p>The read set's description.</p>",
                     "shape": "ReadSetDescription"
                 },
                 "etag": {
-                    "documentation": "<p>The entity tag (ETag) is a hash of the object representing its semantic content.</p>",
+                    "documentation": "<p> The entity tag (ETag) is a hash of the object representing its semantic content. </p>",
                     "shape": "ETag"
                 },
                 "fileType": {
                     "documentation": "<p>The read set's file type.</p>",
                     "shape": "FileType"
                 },
                 "id": {
@@ -8480,24 +8440,14 @@
             "type": "string"
         },
         "ReadSetPartStreamingBlob": {
             "requiresLength": true,
             "streaming": true,
             "type": "blob"
         },
-        "ReadSetS3Access": {
-            "documentation": "<p>The S3 URI for each read set file.</p>",
-            "members": {
-                "s3Uri": {
-                    "documentation": "<p>The S3 URI for each read set file.</p>",
-                    "shape": "S3Uri"
-                }
-            },
-            "type": "structure"
-        },
         "ReadSetStatus": {
             "enum": [
                 "ARCHIVED",
                 "ACTIVATING",
                 "ACTIVE",
                 "DELETING",
                 "DELETED",
@@ -9113,22 +9063,22 @@
                 "ALL"
             ],
             "max": 64,
             "min": 1,
             "type": "string"
         },
         "RunLogLocation": {
-            "documentation": "<p>The URI for the run log.</p>",
+            "documentation": "<p> The URI for the run log. </p>",
             "members": {
                 "engineLogStream": {
-                    "documentation": "<p>The log stream ARN for the engine log.</p>",
+                    "documentation": "<p> The log stream ARN for the engine log. </p>",
                     "shape": "EngineLogStream"
                 },
                 "runLogStream": {
-                    "documentation": "<p>The log stream ARN for the run log.</p>",
+                    "documentation": "<p> The log stream ARN for the run log. </p>",
                     "shape": "RunLogStream"
                 }
             },
             "type": "structure"
         },
         "RunLogStream": {
             "pattern": "[\\p{L}||\\p{M}||\\p{Z}||\\p{S}||\\p{N}||\\p{P}]+",
@@ -9223,20 +9173,14 @@
         },
         "RunUuid": {
             "max": 128,
             "min": 1,
             "pattern": "[\\p{L}||\\p{M}||\\p{Z}||\\p{S}||\\p{N}||\\p{P}]+",
             "type": "string"
         },
-        "S3AccessPointArn": {
-            "max": 1024,
-            "min": 1,
-            "pattern": "arn:[^:]*:s3:[^:]*:[^:]*:accesspoint/.*",
-            "type": "string"
-        },
         "S3Destination": {
             "pattern": "s3://([a-z0-9][a-z0-9-.]{1,61}[a-z0-9])/?((.{1,1024})/)?",
             "type": "string"
         },
         "S3Uri": {
             "pattern": "s3://([a-z0-9][a-z0-9-.]{1,61}[a-z0-9])/(.{1,1024})",
             "type": "string"
@@ -9323,18 +9267,14 @@
                     "documentation": "<p>When the store was created.</p>",
                     "shape": "SyntheticTimestamp_date_time"
                 },
                 "description": {
                     "documentation": "<p>The store's description.</p>",
                     "shape": "SequenceStoreDescription"
                 },
-                "eTagAlgorithmFamily": {
-                    "documentation": "<p>The algorithm family of the ETag.</p>",
-                    "shape": "ETagAlgorithmFamily"
-                },
                 "fallbackLocation": {
                     "documentation": "<p> An S3 location that is used to store files that have failed a direct upload. </p>",
                     "shape": "S3Destination"
                 },
                 "id": {
                     "documentation": "<p>The store's ID.</p>",
                     "shape": "SequenceStoreId"
@@ -9387,28 +9327,14 @@
         },
         "SequenceStoreName": {
             "max": 127,
             "min": 1,
             "pattern": "[\\p{L}||\\p{M}||\\p{Z}||\\p{S}||\\p{N}||\\p{P}]+",
             "type": "string"
         },
-        "SequenceStoreS3Access": {
-            "documentation": "<p>The S3 access metadata of the sequence store.</p>",
-            "members": {
-                "s3AccessPointArn": {
-                    "documentation": "<p>This is ARN of the access point associated with the S3 bucket storing read sets.</p>",
-                    "shape": "S3AccessPointArn"
-                },
-                "s3Uri": {
-                    "documentation": "<p>The S3 URI of the sequence store.</p>",
-                    "shape": "S3Uri"
-                }
-            },
-            "type": "structure"
-        },
         "ServiceQuotaExceededException": {
             "documentation": "<p>The request exceeds a service quota.</p>",
             "error": {
                 "httpStatusCode": 402,
                 "senderFault": true
             },
             "exception": true,
@@ -9526,15 +9452,15 @@
             "min": 20,
             "pattern": ".*arn:([^: ]*):([^: ]*):([^: ]*):([0-9]{12}):([^: ]*).*",
             "type": "string"
         },
         "StartAnnotationImportRequest": {
             "members": {
                 "annotationFields": {
-                    "documentation": "<p>The annotation schema generated by the parsed annotation data.</p>",
+                    "documentation": "<p> The annotation schema generated by the parsed annotation data. </p>",
                     "shape": "AnnotationFieldMap"
                 },
                 "destinationName": {
                     "documentation": "<p>A destination annotation store for the job.</p>",
                     "shape": "StoreName"
                 },
                 "formatOptions": {
@@ -9971,15 +9897,15 @@
                     "shape": "RunGroupId"
                 },
                 "runId": {
                     "documentation": "<p>The ID of a run to duplicate.</p>",
                     "shape": "RunId"
                 },
                 "storageCapacity": {
-                    "documentation": "<p>A storage capacity for the run in gibibytes.</p>",
+                    "documentation": "<p>A storage capacity for the run in gigabytes.</p>",
                     "shape": "StartRunRequestStorageCapacityInteger"
                 },
                 "tags": {
                     "documentation": "<p>Tags for the run.</p>",
                     "shape": "TagMap"
                 },
                 "workflowId": {
@@ -10016,36 +9942,36 @@
                     "shape": "RunArn"
                 },
                 "id": {
                     "documentation": "<p>The run's ID.</p>",
                     "shape": "RunId"
                 },
                 "runOutputUri": {
-                    "documentation": "<p>The destination for workflow outputs.</p>",
+                    "documentation": "<p> The destination for workflow outputs. </p>",
                     "shape": "RunOutputUri"
                 },
                 "status": {
                     "documentation": "<p>The run's status.</p>",
                     "shape": "RunStatus"
                 },
                 "tags": {
                     "documentation": "<p>The run's tags.</p>",
                     "shape": "TagMap"
                 },
                 "uuid": {
-                    "documentation": "<p>The universally unique identifier for a run.</p>",
+                    "documentation": "<p> The universally unique identifier for a run. </p>",
                     "shape": "RunUuid"
                 }
             },
             "type": "structure"
         },
         "StartVariantImportRequest": {
             "members": {
                 "annotationFields": {
-                    "documentation": "<p>The annotation schema generated by the parsed annotation data.</p>",
+                    "documentation": "<p> The annotation schema generated by the parsed annotation data. </p>",
                     "shape": "AnnotationFieldMap"
                 },
                 "destinationName": {
                     "documentation": "<p>The destination variant store for the job.</p>",
                     "shape": "StoreName"
                 },
                 "items": {
@@ -10240,15 +10166,15 @@
                     "shape": "TaskTimestamp"
                 },
                 "gpus": {
                     "documentation": "<p> The number of Graphics Processing Units (GPU) specified for the task. </p>",
                     "shape": "TaskListItemGpusInteger"
                 },
                 "instanceType": {
-                    "documentation": "<p> The instance type for a task.</p>",
+                    "documentation": "<p> The instance type for a task. </p>",
                     "shape": "TaskInstanceType"
                 },
                 "memory": {
                     "documentation": "<p>The task's memory use in gigabyes.</p>",
                     "shape": "TaskListItemMemoryInteger"
                 },
                 "name": {
@@ -10586,15 +10512,15 @@
                     "shape": "UpdateRunGroupRequestMaxCpusInteger"
                 },
                 "maxDuration": {
                     "documentation": "<p>A maximum run time for the group in minutes.</p>",
                     "shape": "UpdateRunGroupRequestMaxDurationInteger"
                 },
                 "maxGpus": {
-                    "documentation": "<p>The maximum GPUs that can be used by a run group.</p>",
+                    "documentation": "<p> The maximum GPUs that can be used by a run group. </p>",
                     "shape": "UpdateRunGroupRequestMaxGpusInteger"
                 },
                 "maxRuns": {
                     "documentation": "<p>The maximum number of concurrent runs for the group.</p>",
                     "shape": "UpdateRunGroupRequestMaxRunsInteger"
                 },
                 "name": {
@@ -10722,37 +10648,37 @@
             "min": 10,
             "pattern": "[0-9]+",
             "type": "string"
         },
         "UploadReadSetPartRequest": {
             "members": {
                 "partNumber": {
-                    "documentation": "<p>The number of the part being uploaded.</p>",
+                    "documentation": "<p> The number of the part being uploaded. </p>",
                     "location": "querystring",
                     "locationName": "partNumber",
                     "shape": "UploadReadSetPartRequestPartNumberInteger"
                 },
                 "partSource": {
-                    "documentation": "<p>The source file for an upload part.</p>",
+                    "documentation": "<p> The source file for an upload part. </p>",
                     "location": "querystring",
                     "locationName": "partSource",
                     "shape": "ReadSetPartSource"
                 },
                 "payload": {
-                    "documentation": "<p>The read set data to upload for a part.</p>",
+                    "documentation": "<p> The read set data to upload for a part. </p>",
                     "shape": "ReadSetPartStreamingBlob"
                 },
                 "sequenceStoreId": {
-                    "documentation": "<p>The Sequence Store ID used for the multipart upload.</p>",
+                    "documentation": "<p> The Sequence Store ID used for the multipart upload. </p>",
                     "location": "uri",
                     "locationName": "sequenceStoreId",
                     "shape": "SequenceStoreId"
                 },
                 "uploadId": {
-                    "documentation": "<p>The ID for the initiated multipart upload.</p>",
+                    "documentation": "<p> The ID for the initiated multipart upload. </p>",
                     "location": "uri",
                     "locationName": "uploadId",
                     "shape": "UploadId"
                 }
             },
             "payload": "payload",
             "required": [
@@ -10769,15 +10695,15 @@
             "max": 10000,
             "min": 1,
             "type": "integer"
         },
         "UploadReadSetPartResponse": {
             "members": {
                 "checksum": {
-                    "documentation": "<p>An identifier used to confirm that parts are being added to the intended upload.</p>",
+                    "documentation": "<p> An identifier used to confirm that parts are being added to the intended upload. </p>",
                     "shape": "String"
                 }
             },
             "required": [
                 "checksum"
             ],
             "type": "structure"
```

### Comparing `botocore-a-la-carte-omics-1.34.89/botocore/data/omics/2022-11-28/waiters-2.json` & `botocore-a-la-carte-omics-1.34.9/botocore/data/omics/2022-11-28/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-omics-1.34.89/botocore_a_la_carte_omics.egg-info/PKG-INFO` & `botocore-a-la-carte-omics-1.34.9/botocore_a_la_carte_omics.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-omics
-Version: 1.34.89
+Version: 1.34.9
 Summary: omics data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-omics-1.34.89/setup.py` & `botocore-a-la-carte-omics-1.34.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-omics',
-    version="1.34.89",
+    version="1.34.9",
     description='omics data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/omics/*/*.json'],
```

