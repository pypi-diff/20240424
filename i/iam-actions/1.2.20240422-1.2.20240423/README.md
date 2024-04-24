# Comparing `tmp/iam_actions-1.2.20240422.tar.gz` & `tmp/iam_actions-1.2.20240423.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_actions-1.2.20240422.tar", max compression
+gzip compressed data, was "iam_actions-1.2.20240423.tar", max compression
```

## Comparing `iam_actions-1.2.20240422.tar` & `iam_actions-1.2.20240423.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1071 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/LICENSE
--rw-r--r--   0        0        0     2302 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/README.md
--rw-r--r--   0        0        0      228 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/__init__.py
--rw-r--r--   0        0        0  4805273 2024-04-22 02:21:18.913228 iam_actions-1.2.20240422/iam_actions/actions.json
--rw-r--r--   0        0        0      496 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/data.py
--rw-r--r--   0        0        0       80 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/generate/__init__.py
--rw-r--r--   0        0        0     3097 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/generate/action_map.py
--rw-r--r--   0        0        0    23329 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/generate/aws_docs.py
--rw-r--r--   0        0        0     3739 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/generate/generate.py
--rw-r--r--   0        0        0     3272 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/generate/notifier.py
--rw-r--r--   0        0        0     1902 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/generate/resource_type.py
--rw-r--r--   0        0        0     2277 2024-04-22 02:19:25.321197 iam_actions-1.2.20240422/iam_actions/generate/services.py
--rw-r--r--   0        0        0   624345 2024-04-22 02:21:18.913228 iam_actions-1.2.20240422/iam_actions/policies.json
--rw-r--r--   0        0        0   208291 2024-04-22 02:21:18.913228 iam_actions-1.2.20240422/iam_actions/resourcetypes.json
--rw-r--r--   0        0        0   605709 2024-04-22 02:21:18.913228 iam_actions-1.2.20240422/iam_actions/services.json
--rw-r--r--   0        0        0     1154 2024-04-22 02:21:19.557227 iam_actions-1.2.20240422/pyproject.toml
--rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240422/setup.py
--rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240422/PKG-INFO
+-rw-r--r--   0        0        0     1071 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/LICENSE
+-rw-r--r--   0        0        0     2302 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/README.md
+-rw-r--r--   0        0        0      228 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/__init__.py
+-rw-r--r--   0        0        0  4809276 2024-04-23 02:20:35.221037 iam_actions-1.2.20240423/iam_actions/actions.json
+-rw-r--r--   0        0        0      496 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/data.py
+-rw-r--r--   0        0        0       80 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/generate/__init__.py
+-rw-r--r--   0        0        0     3097 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/generate/action_map.py
+-rw-r--r--   0        0        0    23329 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/generate/aws_docs.py
+-rw-r--r--   0        0        0     3739 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/generate/generate.py
+-rw-r--r--   0        0        0     3272 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/generate/notifier.py
+-rw-r--r--   0        0        0     1902 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/generate/resource_type.py
+-rw-r--r--   0        0        0     2277 2024-04-23 02:19:32.308711 iam_actions-1.2.20240423/iam_actions/generate/services.py
+-rw-r--r--   0        0        0   625264 2024-04-23 02:20:35.221037 iam_actions-1.2.20240423/iam_actions/policies.json
+-rw-r--r--   0        0        0   208315 2024-04-23 02:20:35.221037 iam_actions-1.2.20240423/iam_actions/resourcetypes.json
+-rw-r--r--   0        0        0   606627 2024-04-23 02:20:35.221037 iam_actions-1.2.20240423/iam_actions/services.json
+-rw-r--r--   0        0        0     1154 2024-04-23 02:20:35.869041 iam_actions-1.2.20240423/pyproject.toml
+-rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 iam_actions-1.2.20240423/setup.py
+-rw-r--r--   0        0        0     2915 1970-01-01 00:00:00.000000 iam_actions-1.2.20240423/PKG-INFO
```

### Comparing `iam_actions-1.2.20240422/LICENSE` & `iam_actions-1.2.20240423/LICENSE`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/README.md` & `iam_actions-1.2.20240423/README.md`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/iam_actions/actions.json` & `iam_actions-1.2.20240423/iam_actions/actions.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9973457861405431%*

 * *Differences: {"'appmesh'": "{'GetMeshPolicy': {'access_level': 'Read', 'description': 'Grants permission to "*

 * *              "read the RAM access control policy for a mesh', 'resources': ['mesh']}, "*

 * *              "'DeleteMeshPolicy': {'access_level': 'Write', 'description': 'Grants permission to "*

 * *              "delete the RAM access control policy for a mesh', 'resources': ['mesh']}, "*

 * *              "'PutMeshPolicy': {'access_level': 'Write', 'description': 'Grants permission to "*

 * *              "define the RAM access c […]*

```diff
@@ -5680,20 +5680,22 @@
             "description": "Grants permission to delete an existing service mesh",
             "orphan": false,
             "resources": [
                 "mesh"
             ]
         },
         "DeleteMeshPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "DeleteMeshPolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to delete the RAM access control policy for a mesh",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "mesh"
+            ]
         },
         "DeleteRoute": {
             "access_level": "Write",
             "action": "DeleteRoute",
             "condition_keys": [],
             "description": "Grants permission to delete an existing route",
             "orphan": false,
@@ -5808,20 +5810,22 @@
             "description": "Grants permission to describe an existing virtual service",
             "orphan": false,
             "resources": [
                 "virtualService"
             ]
         },
         "GetMeshPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Read",
             "action": "GetMeshPolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to read the RAM access control policy for a mesh",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "mesh"
+            ]
         },
         "ListGatewayRoutes": {
             "access_level": "List",
             "action": "ListGatewayRoutes",
             "condition_keys": [],
             "description": "Grants permission to list existing gateway routes in a service mesh",
             "orphan": false,
@@ -5900,20 +5904,22 @@
             "description": "Grants permission to list existing virtual services in a service mesh",
             "orphan": false,
             "resources": [
                 "mesh"
             ]
         },
         "PutMeshPolicy": {
-            "access_level": "Undocumented",
+            "access_level": "Write",
             "action": "PutMeshPolicy",
             "condition_keys": [],
-            "description": "Not Documented by AWS",
+            "description": "Grants permission to define the RAM access control policy for a mesh",
             "orphan": false,
-            "resources": []
+            "resources": [
+                "mesh"
+            ]
         },
         "StreamAggregatedResources": {
             "access_level": "Read",
             "action": "StreamAggregatedResources",
             "condition_keys": [],
             "description": "Grants permission to receive streamed resources for an App Mesh endpoint (VirtualNode/VirtualGateway)",
             "orphan": false,
@@ -133368,14 +133374,22 @@
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
             ],
             "description": "Grants permission to create a trust anchor",
             "orphan": false,
             "resources": []
         },
+        "DeleteAttributeMapping": {
+            "access_level": "Undocumented",
+            "action": "DeleteAttributeMapping",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "DeleteCrl": {
             "access_level": "Write",
             "action": "DeleteCrl",
             "condition_keys": [],
             "description": "Grants permission to delete a certificate revocation list (crl)",
             "orphan": false,
             "resources": [
@@ -133549,14 +133563,22 @@
             "access_level": "List",
             "action": "ListTrustAnchors",
             "condition_keys": [],
             "description": "Grants permission to list trust anchors",
             "orphan": false,
             "resources": []
         },
+        "PutAttributeMapping": {
+            "access_level": "Undocumented",
+            "action": "PutAttributeMapping",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
         "PutNotificationSettings": {
             "access_level": "Write",
             "action": "PutNotificationSettings",
             "condition_keys": [],
             "description": "Grants permission to attach notification settings to a trust anchor",
             "orphan": false,
             "resources": [
@@ -135215,14 +135237,144 @@
             "action": "ViewBilling",
             "condition_keys": [],
             "description": "Grants permission to get all the domain-related billing records for the current AWS account for a specified period",
             "orphan": false,
             "resources": []
         }
     },
+    "route53profiles": {
+        "AssociateProfile": {
+            "access_level": "Undocumented",
+            "action": "AssociateProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "AssociateResourceToProfile": {
+            "access_level": "Undocumented",
+            "action": "AssociateResourceToProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "CreateProfile": {
+            "access_level": "Undocumented",
+            "action": "CreateProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DeleteProfile": {
+            "access_level": "Undocumented",
+            "action": "DeleteProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DisassociateProfile": {
+            "access_level": "Undocumented",
+            "action": "DisassociateProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "DisassociateResourceFromProfile": {
+            "access_level": "Undocumented",
+            "action": "DisassociateResourceFromProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetProfile": {
+            "access_level": "Undocumented",
+            "action": "GetProfile",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetProfileAssociation": {
+            "access_level": "Undocumented",
+            "action": "GetProfileAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "GetProfileResourceAssociation": {
+            "access_level": "Undocumented",
+            "action": "GetProfileResourceAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListProfileAssociations": {
+            "access_level": "Undocumented",
+            "action": "ListProfileAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListProfileResourceAssociations": {
+            "access_level": "Undocumented",
+            "action": "ListProfileResourceAssociations",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListProfiles": {
+            "access_level": "Undocumented",
+            "action": "ListProfiles",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "ListTagsForResource": {
+            "access_level": "Undocumented",
+            "action": "ListTagsForResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "TagResource": {
+            "access_level": "Undocumented",
+            "action": "TagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UntagResource": {
+            "access_level": "Undocumented",
+            "action": "UntagResource",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        },
+        "UpdateProfileResourceAssociation": {
+            "access_level": "Undocumented",
+            "action": "UpdateProfileResourceAssociation",
+            "condition_keys": [],
+            "description": "Not Documented by AWS",
+            "orphan": false,
+            "resources": []
+        }
+    },
     "route53resolver": {
         "AssociateFirewallRuleGroup": {
             "access_level": "Write",
             "action": "AssociateFirewallRuleGroup",
             "condition_keys": [
                 "aws:RequestTag/${TagKey}",
                 "aws:TagKeys"
```

### Comparing `iam_actions-1.2.20240422/iam_actions/generate/action_map.py` & `iam_actions-1.2.20240423/iam_actions/generate/action_map.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/iam_actions/generate/aws_docs.py` & `iam_actions-1.2.20240423/iam_actions/generate/aws_docs.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/iam_actions/generate/generate.py` & `iam_actions-1.2.20240423/iam_actions/generate/generate.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/iam_actions/generate/notifier.py` & `iam_actions-1.2.20240423/iam_actions/generate/notifier.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/iam_actions/generate/resource_type.py` & `iam_actions-1.2.20240423/iam_actions/generate/resource_type.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/iam_actions/generate/services.py` & `iam_actions-1.2.20240423/iam_actions/generate/services.py`

 * *Files identical despite different names*

### Comparing `iam_actions-1.2.20240422/iam_actions/policies.json` & `iam_actions-1.2.20240423/iam_actions/policies.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9997548220592231%*

 * *Differences: {"'serviceMap'": "{'AWS Identity and Access Management Roles Anywhere': {'Actions': {insert: [(2, "*

 * *                 "'DeleteAttributeMapping'), (22, 'PutAttributeMapping')]}}, 'Amazon Route 53 "*

 * *                 "Profiles enables sharing DNS settings with VPCs': OrderedDict([('StringPrefix', "*

 * *                 "'route53profiles'), ('Actions', ['AssociateProfile', "*

 * *                 "'AssociateResourceToProfile', 'CreateProfile', 'DeleteProfile', "*

 * *                 "'DisassociateProfile', 'DisassociateResou […]*

```diff
@@ -5927,14 +5927,15 @@
         },
         "AWS Identity and Access Management Roles Anywhere": {
             "ARNFormat": "arn:aws:rolesanywhere:${Region}:${Account}:${ResourceType}/${ResourceId}",
             "ARNRegex": "^arn:aws:rolesanywhere:.+:.+:.+",
             "Actions": [
                 "CreateProfile",
                 "CreateTrustAnchor",
+                "DeleteAttributeMapping",
                 "DeleteCrl",
                 "DeleteProfile",
                 "DeleteTrustAnchor",
                 "DisableCrl",
                 "DisableProfile",
                 "DisableTrustAnchor",
                 "EnableCrl",
@@ -5946,14 +5947,15 @@
                 "GetTrustAnchor",
                 "ImportCrl",
                 "ListCrls",
                 "ListProfiles",
                 "ListSubjects",
                 "ListTagsForResource",
                 "ListTrustAnchors",
+                "PutAttributeMapping",
                 "PutNotificationSettings",
                 "ResetNotificationSettings",
                 "TagResource",
                 "UntagResource",
                 "UpdateCrl",
                 "UpdateProfile",
                 "UpdateTrustAnchor"
@@ -19957,14 +19959,43 @@
                 "UpdateDomainNameservers",
                 "UpdateTagsForDomain",
                 "ViewBilling"
             ],
             "HasResource": false,
             "StringPrefix": "route53domains"
         },
+        "Amazon Route 53 Profiles enables sharing DNS settings with VPCs": {
+            "ARNFormat": "arn:aws:route53profiles:${Region}:${Account}:${ResourceType}/${ResourceId}",
+            "ARNRegex": "^arn:aws:route53profiles:.+:.+:.+",
+            "Actions": [
+                "AssociateProfile",
+                "AssociateResourceToProfile",
+                "CreateProfile",
+                "DeleteProfile",
+                "DisassociateProfile",
+                "DisassociateResourceFromProfile",
+                "GetProfile",
+                "GetProfileAssociation",
+                "GetProfileResourceAssociation",
+                "ListProfileAssociations",
+                "ListProfileResourceAssociations",
+                "ListProfiles",
+                "ListTagsForResource",
+                "TagResource",
+                "UntagResource",
+                "UpdateProfileResourceAssociation"
+            ],
+            "HasResource": true,
+            "StringPrefix": "route53profiles",
+            "conditionKeys": [
+                "aws:RequestTag/${TagKey}",
+                "aws:ResourceTag/${TagKey}",
+                "aws:TagKeys"
+            ]
+        },
         "Amazon Route 53 Recovery Cluster": {
             "ARNFormat": "arn:aws:route53-recovery-control::${Account}:${ResourceType}/${ResourceName}",
             "ARNRegex": "^arn:aws:route53-recovery-control::.+:.+",
             "Actions": [
                 "GetRoutingControlState",
                 "ListRoutingControls",
                 "UpdateRoutingControlState",
```

### Comparing `iam_actions-1.2.20240422/iam_actions/resourcetypes.json` & `iam_actions-1.2.20240423/iam_actions/resourcetypes.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9974424552429667%*

 * *Differences: {"'route53profiles'": 'OrderedDict()'}*

```diff
@@ -5670,14 +5670,15 @@
         },
         "resourceset": {
             "arn_pattern": "arn:*:route53-recovery-readiness::*:resource-set/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         }
     },
     "route53domains": {},
+    "route53profiles": {},
     "route53resolver": {
         "firewall-config": {
             "arn_pattern": "arn:*:route53resolver:*:*:firewall-config/*",
             "condition_keys": "aws:ResourceTag/${TagKey}"
         },
         "firewall-domain-list": {
             "arn_pattern": "arn:*:route53resolver:*:*:firewall-domain-list/*",
```

### Comparing `iam_actions-1.2.20240422/iam_actions/services.json` & `iam_actions-1.2.20240423/iam_actions/services.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.997435350951975%*

 * *Differences: {"'rolesanywhere'": "{'Actions': {insert: [(2, 'DeleteAttributeMapping'), (22, "*

 * *                    "'PutAttributeMapping')]}}",*

 * * "'route53profiles'": "OrderedDict([('Actions', ['AssociateProfile', 'AssociateResourceToProfile', "*

 * *                      "'CreateProfile', 'DeleteProfile', 'DisassociateProfile', "*

 * *                      "'DisassociateResourceFromProfile', 'GetProfile', 'GetProfileAssociation', "*

 * *                      "'GetProfileResourceAssociation', 'ListProfileAssociations', "*

 * *                […]*

```diff
@@ -18782,14 +18782,15 @@
         ],
         "ARNRegexes": [
             "^arn:aws:rolesanywhere:.+:.+:.+"
         ],
         "Actions": [
             "CreateProfile",
             "CreateTrustAnchor",
+            "DeleteAttributeMapping",
             "DeleteCrl",
             "DeleteProfile",
             "DeleteTrustAnchor",
             "DisableCrl",
             "DisableProfile",
             "DisableTrustAnchor",
             "EnableCrl",
@@ -18801,14 +18802,15 @@
             "GetTrustAnchor",
             "ImportCrl",
             "ListCrls",
             "ListProfiles",
             "ListSubjects",
             "ListTagsForResource",
             "ListTrustAnchors",
+            "PutAttributeMapping",
             "PutNotificationSettings",
             "ResetNotificationSettings",
             "TagResource",
             "UntagResource",
             "UpdateCrl",
             "UpdateProfile",
             "UpdateTrustAnchor"
@@ -19069,14 +19071,49 @@
         ],
         "ConditionKeys": [],
         "HasResource": false,
         "ServiceNames": [
             "Amazon Route 53 Domains"
         ]
     },
+    "route53profiles": {
+        "ARNFormats": [
+            "arn:aws:route53profiles:${Region}:${Account}:${ResourceType}/${ResourceId}"
+        ],
+        "ARNRegexes": [
+            "^arn:aws:route53profiles:.+:.+:.+"
+        ],
+        "Actions": [
+            "AssociateProfile",
+            "AssociateResourceToProfile",
+            "CreateProfile",
+            "DeleteProfile",
+            "DisassociateProfile",
+            "DisassociateResourceFromProfile",
+            "GetProfile",
+            "GetProfileAssociation",
+            "GetProfileResourceAssociation",
+            "ListProfileAssociations",
+            "ListProfileResourceAssociations",
+            "ListProfiles",
+            "ListTagsForResource",
+            "TagResource",
+            "UntagResource",
+            "UpdateProfileResourceAssociation"
+        ],
+        "ConditionKeys": [
+            "aws:RequestTag/${TagKey}",
+            "aws:ResourceTag/${TagKey}",
+            "aws:TagKeys"
+        ],
+        "HasResource": true,
+        "ServiceNames": [
+            "Amazon Route 53 Profiles enables sharing DNS settings with VPCs"
+        ]
+    },
     "route53resolver": {
         "ARNFormats": [
             "arn:aws:route53resolver:${Region}:${Account}:${ResourceType}/${ResourceId}"
         ],
         "ARNRegexes": [
             "^arn:aws:route53resolver:.+:.+:.+"
         ],
```

### Comparing `iam_actions-1.2.20240422/pyproject.toml` & `iam_actions-1.2.20240423/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "iam-actions"
-version = "1.2.20240422"
+version = "1.2.20240423"
 description = "JSON of AWS policy components"
 authors = ["Constable <info@constableapp.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/constableapp/iam_actions"
 packages = [{include = "iam_actions"}]
```

### Comparing `iam_actions-1.2.20240422/setup.py` & `iam_actions-1.2.20240423/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['iam_actions', 'iam_actions.generate']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'iam-actions',
-    'version': '1.2.20240422',
+    'version': '1.2.20240423',
     'description': 'JSON of AWS policy components',
     'long_description': '# iam_actions\n\n`iam_actions` is a python module which contains a dictionary of AWS IAM information. Ideally, it is a complete catalog of all AWS services, actions, and resource types. The information is scraped from the AWS documentation pages.\n\nNightly, the scraping service runs, and publishes a new version with the date appended. \n\nThe package is meant to be used as a consumable package, but it also contains the code to generate the definitions for packaging.\n\nThere are three "roots" that you can consume: actions, resource_types, and services. They all currently return as dict\'s. *However, in a future release, it will be returned as python data structures*\n\n## Actions\n\nActions is a listing of all the actions for a given service. The structure is as follows:\n```\n{\n    "service_name": {\n        "action_name: {\n            "access_level": access_level,\n            "action": action_name,\n            "condition_keys": [condition_key1, ...],\n            "description": description\n        }\n    }\n}\n```\n\nTherefore, you can find information about an action as follows\n\n```\n>>> iam_actions.actions[\'s3\'][\'GetObject\']\n{\'access_level\': \'Read\', \'action\': \'GetObject\', \'condition_keys\': [\'s3:AccessPointNetworkOrigin\', \'s3:DataAccessPointAccount\', \'s3:DataAccessPointArn\', \'s3:ExistingObjectTag/<key>\', \'s3:ResourceAccount\', \'s3:TlsVersion\', \'s3:authType\', \'s3:signatureAge\', \'s3:signatureversion\', \'s3:x-amz-content-sha256\'], \'description\': \'Grants permission to retrieve objects from Amazon S3\', \'orphan\': False, \'resources\': [\'object\']}\n```\n\n## Services\n\nServices list information about the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "Actions": [action1, ...]\n        "ServiceNames": [service_name1, ...]\n        "ARNFormats": [arn_format1, ...]\n        "ConditionKeys": [condition_key1, ...]\n        "HasResource": bool\n    }\n}\n```\n\n## Resource Types\n\nResource Types list information about the resource types for the service. The structure is as follows:\n\n```\n{\n    "service_name": {\n        "resource_name": {\n            "arn_pattern": arn_pattern,\n            "condition_keys": [condition_key1, ...]\n        }\n    }\n}\n```\n\n## Usage\n\n```python\nimport iam_actions\n\nprint(item_actions.services)\nprint(item_actions.actions)\nprint(item_actions.resource_types)\n```\n',
     'author': 'Constable',
     'author_email': 'info@constableapp.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://github.com/constableapp/iam_actions',
```

### Comparing `iam_actions-1.2.20240422/PKG-INFO` & `iam_actions-1.2.20240423/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam-actions
-Version: 1.2.20240422
+Version: 1.2.20240423
 Summary: JSON of AWS policy components
 Home-page: https://github.com/constableapp/iam_actions
 License: MIT
 Author: Constable
 Author-email: info@constableapp.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

