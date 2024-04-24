# Comparing `tmp/DockerBuildSystem-1.1.8-py2.py3-none-any.whl.zip` & `tmp/DockerBuildSystem-1.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 6636 bytes, number of entries: 13
+Zip file size: 6646 bytes, number of entries: 13
 -rw-rw-rw-  2.0 fat     3146 b- defN 18-May-16 15:15 DockerBuildSystem/DockerComposeTools.py
 -rw-rw-rw-  2.0 fat     1231 b- defN 18-May-08 08:12 DockerBuildSystem/DockerImageTools.py
--rw-rw-rw-  2.0 fat     2162 b- defN 18-May-08 08:12 DockerBuildSystem/DockerSwarmTools.py
+-rw-rw-rw-  2.0 fat     2233 b- defN 18-May-18 13:54 DockerBuildSystem/DockerSwarmTools.py
 -rw-rw-rw-  2.0 fat     2299 b- defN 18-May-11 08:15 DockerBuildSystem/TerminalTools.py
 -rw-rw-rw-  2.0 fat      712 b- defN 18-May-14 06:44 DockerBuildSystem/VersionTools.py
 -rw-rw-rw-  2.0 fat        0 b- defN 18-May-08 08:12 DockerBuildSystem/__init__.py
--rw-rw-rw-  2.0 fat       24 b- defN 18-May-18 11:45 DockerBuildSystem-1.1.8.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat     1085 b- defN 18-May-18 11:45 DockerBuildSystem-1.1.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat      619 b- defN 18-May-18 11:45 DockerBuildSystem-1.1.8.dist-info/metadata.json
--rw-rw-rw-  2.0 fat       18 b- defN 18-May-18 11:45 DockerBuildSystem-1.1.8.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat      116 b- defN 18-May-18 11:45 DockerBuildSystem-1.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      431 b- defN 18-May-18 11:45 DockerBuildSystem-1.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1207 b- defN 18-May-18 11:45 DockerBuildSystem-1.1.8.dist-info/RECORD
-13 files, 13050 bytes uncompressed, 4590 bytes compressed:  64.8%
+-rw-rw-rw-  2.0 fat       24 b- defN 18-May-18 13:55 DockerBuildSystem-1.1.9.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1085 b- defN 18-May-18 13:55 DockerBuildSystem-1.1.9.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat      619 b- defN 18-May-18 13:55 DockerBuildSystem-1.1.9.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       18 b- defN 18-May-18 13:55 DockerBuildSystem-1.1.9.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      116 b- defN 18-May-18 13:55 DockerBuildSystem-1.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      431 b- defN 18-May-18 13:55 DockerBuildSystem-1.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1207 b- defN 18-May-18 13:55 DockerBuildSystem-1.1.9.dist-info/RECORD
+13 files, 13121 bytes uncompressed, 4600 bytes compressed:  64.9%
```

## zipnote {}

```diff
@@ -12,29 +12,29 @@
 
 Filename: DockerBuildSystem/VersionTools.py
 Comment: 
 
 Filename: DockerBuildSystem/__init__.py
 Comment: 
 
-Filename: DockerBuildSystem-1.1.8.dist-info/DESCRIPTION.rst
+Filename: DockerBuildSystem-1.1.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: DockerBuildSystem-1.1.8.dist-info/LICENSE.txt
+Filename: DockerBuildSystem-1.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: DockerBuildSystem-1.1.8.dist-info/metadata.json
+Filename: DockerBuildSystem-1.1.9.dist-info/metadata.json
 Comment: 
 
-Filename: DockerBuildSystem-1.1.8.dist-info/top_level.txt
+Filename: DockerBuildSystem-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: DockerBuildSystem-1.1.8.dist-info/WHEEL
+Filename: DockerBuildSystem-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: DockerBuildSystem-1.1.8.dist-info/METADATA
+Filename: DockerBuildSystem-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: DockerBuildSystem-1.1.8.dist-info/RECORD
+Filename: DockerBuildSystem-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## DockerBuildSystem/DockerSwarmTools.py

```diff
@@ -1,13 +1,14 @@
 from DockerBuildSystem import TerminalTools
 import os
 
 
-def DeployStack(composeFile, stackName, environmentVariablesFile = '.env'):
-    TerminalTools.LoadEnvironmentVariables(environmentVariablesFile)
+def DeployStack(composeFile, stackName, environmentVariablesFiles = ['.env']):
+    for environmentVariablesFile in environmentVariablesFiles:
+        TerminalTools.LoadEnvironmentVariables(environmentVariablesFile)
     print("Deploying stack: " + stackName)
     dockerCommand = "docker stack deploy -c " + composeFile + " " + stackName
     TerminalTools.ExecuteTerminalCommands([dockerCommand], True)
 
 
 def RemoveStack(stackName):
     print("Removing stack: " + stackName)
```

## Comparing `DockerBuildSystem-1.1.8.dist-info/LICENSE.txt` & `DockerBuildSystem-1.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `DockerBuildSystem-1.1.8.dist-info/metadata.json` & `DockerBuildSystem-1.1.9.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'1.1.9'"}*

```diff
@@ -41,9 +41,9 @@
             "requires": [
                 "python-dotenv",
                 "pyyaml"
             ]
         }
     ],
     "summary": "A Docker build system for managing docker.",
-    "version": "1.1.8"
+    "version": "1.1.9"
 }
```

## Comparing `DockerBuildSystem-1.1.8.dist-info/RECORD` & `DockerBuildSystem-1.1.9.dist-info/RECORD`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 DockerBuildSystem/DockerComposeTools.py,sha256=JyJqEMICxFqfdZa9oHfzOFEMMVpcureI2yh1KqLMlfQ,3146
 DockerBuildSystem/DockerImageTools.py,sha256=4Ns6lTOr3mHIH0af3K4CGsLuPNx0UhVdTwKAkReJz2A,1231
-DockerBuildSystem/DockerSwarmTools.py,sha256=KODlI5zKoXbfxZZcxdIQx3VGQxYG7dcLgm0p1Ex0MKQ,2162
+DockerBuildSystem/DockerSwarmTools.py,sha256=8YgBwBRdFZL2M-V_TDrG_5RKkbE-8ahv9P4AvMGzDAE,2233
 DockerBuildSystem/TerminalTools.py,sha256=7JGcryL4OfEdIuvwoFBfPRPhp0qrCPTxlN_WIgFF2KE,2299
 DockerBuildSystem/VersionTools.py,sha256=M2P_NGMkEA9dLiN6QnAZNcaUKbvANQsenGF1GoUwMHE,712
 DockerBuildSystem/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-DockerBuildSystem-1.1.8.dist-info/DESCRIPTION.rst,sha256=I9iR4aUA4wr-ihV24uALgDOpzqqpN0Gi-xkjdr6Hf0w,24
-DockerBuildSystem-1.1.8.dist-info/LICENSE.txt,sha256=tqisjHbgCfhQ5neJeaNnxAy4o_Usg1yot8AXCSf__QY,1085
-DockerBuildSystem-1.1.8.dist-info/METADATA,sha256=EuSotkiI6Gj73TmlnFrkb6LQ864FF0hD-mrTR8cnFvw,431
-DockerBuildSystem-1.1.8.dist-info/RECORD,,
-DockerBuildSystem-1.1.8.dist-info/WHEEL,sha256=9Z5Xm-eel1bTS7e6ogYiKz0zmPEqDwIypurdHN1hR40,116
-DockerBuildSystem-1.1.8.dist-info/metadata.json,sha256=U6k642rO5VeLqGg_G5smQSa1wj5UmcVl_B9gSaQyBMY,619
-DockerBuildSystem-1.1.8.dist-info/top_level.txt,sha256=swY3T2tQMNuNrXkVqjyM4Lq6X6mrZel0hLNc69HhyPQ,18
+DockerBuildSystem-1.1.9.dist-info/DESCRIPTION.rst,sha256=I9iR4aUA4wr-ihV24uALgDOpzqqpN0Gi-xkjdr6Hf0w,24
+DockerBuildSystem-1.1.9.dist-info/LICENSE.txt,sha256=tqisjHbgCfhQ5neJeaNnxAy4o_Usg1yot8AXCSf__QY,1085
+DockerBuildSystem-1.1.9.dist-info/METADATA,sha256=VKNsIv9BDNjhIafyHFLCwG4HKFQCC5gu7H3x0MefiX0,431
+DockerBuildSystem-1.1.9.dist-info/RECORD,,
+DockerBuildSystem-1.1.9.dist-info/WHEEL,sha256=9Z5Xm-eel1bTS7e6ogYiKz0zmPEqDwIypurdHN1hR40,116
+DockerBuildSystem-1.1.9.dist-info/metadata.json,sha256=ITJ6lEGzAKZRZAWGDYguPKwaOJwxceL0DC1PuSL2eYY,619
+DockerBuildSystem-1.1.9.dist-info/top_level.txt,sha256=swY3T2tQMNuNrXkVqjyM4Lq6X6mrZel0hLNc69HhyPQ,18
```

