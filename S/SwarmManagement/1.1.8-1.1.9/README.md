# Comparing `tmp/SwarmManagement-1.1.8-py2.py3-none-any.whl.zip` & `tmp/SwarmManagement-1.1.9-py2.py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 9617 bytes, number of entries: 15
+Zip file size: 9614 bytes, number of entries: 15
 -rw-rw-rw-  2.0 fat     2882 b- defN 18-May-18 12:57 SwarmManagement/SwarmConfigs.py
 -rw-rw-rw-  2.0 fat     2869 b- defN 18-May-18 13:13 SwarmManagement/SwarmManager.py
 -rw-rw-rw-  2.0 fat     2961 b- defN 18-May-18 12:56 SwarmManagement/SwarmNetworks.py
 -rw-rw-rw-  2.0 fat     2874 b- defN 18-May-18 12:56 SwarmManagement/SwarmSecrets.py
 -rw-rw-rw-  2.0 fat     2975 b- defN 18-May-18 13:49 SwarmManagement/SwarmStacks.py
--rw-rw-rw-  2.0 fat     3942 b- defN 18-May-18 13:53 SwarmManagement/SwarmTools.py
+-rw-rw-rw-  2.0 fat     3943 b- defN 18-May-18 14:03 SwarmManagement/SwarmTools.py
 -rw-rw-rw-  2.0 fat      644 b- defN 18-May-08 08:11 SwarmManagement/__init__.py
--rw-rw-rw-  2.0 fat       28 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/DESCRIPTION.rst
--rw-rw-rw-  2.0 fat     1085 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/LICENSE.txt
--rw-rw-rw-  2.0 fat       58 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/entry_points.txt
--rw-rw-rw-  2.0 fat      779 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/metadata.json
--rw-rw-rw-  2.0 fat       16 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/top_level.txt
--rw-rw-rw-  2.0 fat      116 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/WHEEL
--rw-rw-rw-  2.0 fat      429 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/METADATA
--rw-rw-rw-  2.0 fat     1360 b- defN 18-May-18 14:01 SwarmManagement-1.1.8.dist-info/RECORD
-15 files, 23018 bytes uncompressed, 7347 bytes compressed:  68.1%
+-rw-rw-rw-  2.0 fat       28 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/DESCRIPTION.rst
+-rw-rw-rw-  2.0 fat     1085 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/LICENSE.txt
+-rw-rw-rw-  2.0 fat       58 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/entry_points.txt
+-rw-rw-rw-  2.0 fat      779 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/metadata.json
+-rw-rw-rw-  2.0 fat       16 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/top_level.txt
+-rw-rw-rw-  2.0 fat      116 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat      429 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/METADATA
+-rw-rw-rw-  2.0 fat     1360 b- defN 18-May-18 14:03 SwarmManagement-1.1.9.dist-info/RECORD
+15 files, 23019 bytes uncompressed, 7344 bytes compressed:  68.1%
```

## zipnote {}

```diff
@@ -15,32 +15,32 @@
 
 Filename: SwarmManagement/SwarmTools.py
 Comment: 
 
 Filename: SwarmManagement/__init__.py
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/DESCRIPTION.rst
+Filename: SwarmManagement-1.1.9.dist-info/DESCRIPTION.rst
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/LICENSE.txt
+Filename: SwarmManagement-1.1.9.dist-info/LICENSE.txt
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/entry_points.txt
+Filename: SwarmManagement-1.1.9.dist-info/entry_points.txt
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/metadata.json
+Filename: SwarmManagement-1.1.9.dist-info/metadata.json
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/top_level.txt
+Filename: SwarmManagement-1.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/WHEEL
+Filename: SwarmManagement-1.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/METADATA
+Filename: SwarmManagement-1.1.9.dist-info/METADATA
 Comment: 
 
-Filename: SwarmManagement-1.1.8.dist-info/RECORD
+Filename: SwarmManagement-1.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## SwarmManagement/SwarmTools.py

```diff
@@ -55,15 +55,15 @@
 
 def GetEnvironmnetVariablesFiles(arguments):
     envFiles = GetArgumentValues(arguments, '-env')
     envFiles += GetArgumentValues(arguments, '-e')
     if len(envFiles) == 0:
         swarmManagementYamlData = GetSwarmManagementYamlData(arguments)
         if 'env_files' in swarmManagementYamlData:
-            envFiles = swarmManagementYamlData['env_file']
+            envFiles = swarmManagementYamlData['env_files']
         else:
             envFiles.append('.env')
     return envFiles
 
 
 def GetProperties(arguments, propertyType, errorInfoMsg):
     swarmManagementYamlData = GetSwarmManagementYamlData(arguments)
```

## Comparing `SwarmManagement-1.1.8.dist-info/LICENSE.txt` & `SwarmManagement-1.1.9.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `SwarmManagement-1.1.8.dist-info/metadata.json` & `SwarmManagement-1.1.9.dist-info/metadata.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9375%*

 * *Differences: {"'version'": "'1.1.9'"}*

```diff
@@ -51,9 +51,9 @@
             "extra": "test",
             "requires": [
                 "coverage"
             ]
         }
     ],
     "summary": "A library for managing Docker Swarm.",
-    "version": "1.1.8"
+    "version": "1.1.9"
 }
```

## Comparing `SwarmManagement-1.1.8.dist-info/RECORD` & `SwarmManagement-1.1.9.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 SwarmManagement/SwarmConfigs.py,sha256=q82qcL3jQDUIdsB7DrpTypy2q0ft7FZzdJRRQq02pJo,2882
 SwarmManagement/SwarmManager.py,sha256=8TpFlLAO9IO0pvCRsxaMK4DWUP5uHDH3prk5-NexwJ4,2869
 SwarmManagement/SwarmNetworks.py,sha256=ZBAyo0BYfmpeoQmCXwc8bvEWnSfzhFXpPiboa_b-7FY,2961
 SwarmManagement/SwarmSecrets.py,sha256=sSzYdDorEBbKamLNpwBOQP6DeGZ_1Zx3VICV_7kBaL4,2874
 SwarmManagement/SwarmStacks.py,sha256=2Tk8b8pcKA3eO8X2cs5y9YdvX4UMpCwaDMtvRXZwxNY,2975
-SwarmManagement/SwarmTools.py,sha256=rE3-OgVsL9pRFREtVxaZSWX2xpnPVFGAO6mGqKwGgaI,3942
+SwarmManagement/SwarmTools.py,sha256=NwnaQHWGdLvbfnLHU7cc9mUgJr6B_eb2yBv6m7tiqyU,3943
 SwarmManagement/__init__.py,sha256=0LpQhq5K9y5C8zu1B82_e-dWcweHI8A4gCgw3mHWeuw,644
-SwarmManagement-1.1.8.dist-info/DESCRIPTION.rst,sha256=ghBQ_qMHiRPVsHFt_p9LG9bRl3QM0mCbkTKJVn9rL-c,28
-SwarmManagement-1.1.8.dist-info/LICENSE.txt,sha256=tqisjHbgCfhQ5neJeaNnxAy4o_Usg1yot8AXCSf__QY,1085
-SwarmManagement-1.1.8.dist-info/METADATA,sha256=WmUq9YYoJAvr0oEdkOyPtqGaFCGMOKjZAmjO2CuRAco,429
-SwarmManagement-1.1.8.dist-info/RECORD,,
-SwarmManagement-1.1.8.dist-info/WHEEL,sha256=9Z5Xm-eel1bTS7e6ogYiKz0zmPEqDwIypurdHN1hR40,116
-SwarmManagement-1.1.8.dist-info/entry_points.txt,sha256=ZjqwGb6OUUGMXx8LgbCt7_qyxc3CZJxkswUxGp__3nI,58
-SwarmManagement-1.1.8.dist-info/metadata.json,sha256=x4ArIArUhift1OHFdWpDnC5CIL2rSB131Zdc7gMIFdE,779
-SwarmManagement-1.1.8.dist-info/top_level.txt,sha256=BEE-4fa552HXeuK7o4VXX1h4jPhySc2Q67cdweUn2lY,16
+SwarmManagement-1.1.9.dist-info/DESCRIPTION.rst,sha256=ghBQ_qMHiRPVsHFt_p9LG9bRl3QM0mCbkTKJVn9rL-c,28
+SwarmManagement-1.1.9.dist-info/LICENSE.txt,sha256=tqisjHbgCfhQ5neJeaNnxAy4o_Usg1yot8AXCSf__QY,1085
+SwarmManagement-1.1.9.dist-info/METADATA,sha256=f5v13qYZLSPexzgqG3sfpKjK_0gFbCA30ODt2A9vxjU,429
+SwarmManagement-1.1.9.dist-info/RECORD,,
+SwarmManagement-1.1.9.dist-info/WHEEL,sha256=9Z5Xm-eel1bTS7e6ogYiKz0zmPEqDwIypurdHN1hR40,116
+SwarmManagement-1.1.9.dist-info/entry_points.txt,sha256=ZjqwGb6OUUGMXx8LgbCt7_qyxc3CZJxkswUxGp__3nI,58
+SwarmManagement-1.1.9.dist-info/metadata.json,sha256=BGP50-J-VVryLeCgI4yLbQoXYW6sfyRtMkSLNTC9DIs,779
+SwarmManagement-1.1.9.dist-info/top_level.txt,sha256=BEE-4fa552HXeuK7o4VXX1h4jPhySc2Q67cdweUn2lY,16
```

