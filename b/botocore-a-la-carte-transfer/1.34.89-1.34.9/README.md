# Comparing `tmp/botocore-a-la-carte-transfer-1.34.89.tar.gz` & `tmp/botocore-a-la-carte-transfer-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-transfer-1.34.89.tar", last modified: Tue Apr 23 01:02:15 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-transfer-1.34.9.tar", last modified: Thu Dec 28 01:07:04 2023, max compression
```

## Comparing `botocore-a-la-carte-transfer-1.34.89.tar` & `botocore-a-la-carte-transfer-1.34.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:15.605734 botocore-a-la-carte-transfer-1.34.89/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-23 01:02:15.000000 botocore-a-la-carte-transfer-1.34.89/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-23 01:02:15.601734 botocore-a-la-carte-transfer-1.34.89/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:15.601734 botocore-a-la-carte-transfer-1.34.89/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:15.601734 botocore-a-la-carte-transfer-1.34.89/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:15.601734 botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:15.601734 botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/
--rw-r--r--   0 runner    (1001) docker     (127)    13734 2024-04-23 01:01:45.000000 botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-23 01:01:45.000000 botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/examples-1.json
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-04-23 01:01:45.000000 botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   302241 2024-04-23 01:01:45.000000 botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/service-2.json
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-04-23 01:01:45.000000 botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/waiters-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-23 01:02:15.601734 botocore-a-la-carte-transfer-1.34.89/botocore_a_la_carte_transfer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      960 2024-04-23 01:02:15.000000 botocore-a-la-carte-transfer-1.34.89/botocore_a_la_carte_transfer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-04-23 01:02:15.000000 botocore-a-la-carte-transfer-1.34.89/botocore_a_la_carte_transfer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-23 01:02:15.000000 botocore-a-la-carte-transfer-1.34.89/botocore_a_la_carte_transfer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-23 01:02:15.000000 botocore-a-la-carte-transfer-1.34.89/botocore_a_la_carte_transfer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-23 01:02:15.605734 botocore-a-la-carte-transfer-1.34.89/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1145 2024-04-23 01:02:15.000000 botocore-a-la-carte-transfer-1.34.89/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:07:04.000000 botocore-a-la-carte-transfer-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/
+-rw-r--r--   0 runner    (1001) docker     (127)    13734 2023-12-28 01:06:26.000000 botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2023-12-28 01:06:26.000000 botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/examples-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2023-12-28 01:06:26.000000 botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)   290456 2023-12-28 01:06:26.000000 botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/service-2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      868 2023-12-28 01:06:26.000000 botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/waiters-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/botocore_a_la_carte_transfer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2023-12-28 01:07:04.000000 botocore-a-la-carte-transfer-1.34.9/botocore_a_la_carte_transfer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2023-12-28 01:07:04.000000 botocore-a-la-carte-transfer-1.34.9/botocore_a_la_carte_transfer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:07:04.000000 botocore-a-la-carte-transfer-1.34.9/botocore_a_la_carte_transfer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:07:04.000000 botocore-a-la-carte-transfer-1.34.9/botocore_a_la_carte_transfer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:07:04.834461 botocore-a-la-carte-transfer-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2023-12-28 01:07:04.000000 botocore-a-la-carte-transfer-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-transfer-1.34.89/LICENSE.txt` & `botocore-a-la-carte-transfer-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.89/PKG-INFO` & `botocore-a-la-carte-transfer-1.34.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-transfer
-Version: 1.34.89
+Version: 1.34.9
 Summary: transfer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json` & `botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/paginators-1.json` & `botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/paginators-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/service-2.json` & `botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/service-2.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9944462015007158%*

 * *Differences: {"'operations'": "{'CreateConnector': {'documentation': '<p>Creates the connector, which captures "*

 * *                 'the parameters for a connection for the AS2 or SFTP protocol. For AS2, the '*

 * *                 'connector is required for sending files to an externally hosted AS2 server. For '*

 * *                 'SFTP, the connector is required when sending files to an SFTP server or '*

 * *                 'receiving files from an SFTP server. For more details about connectors, see <a '*

 * *                 'href="ht […]*

```diff
@@ -76,15 +76,15 @@
             },
             "name": "CreateAgreement",
             "output": {
                 "shape": "CreateAgreementResponse"
             }
         },
         "CreateConnector": {
-            "documentation": "<p>Creates the connector, which captures the parameters for a connection for the AS2 or SFTP protocol. For AS2, the connector is required for sending files to an externally hosted AS2 server. For SFTP, the connector is required when sending files to an SFTP server or receiving files from an SFTP server. For more details about connectors, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/configure-as2-connector.html\">Configure AS2 connectors</a> and <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/configure-sftp-connector.html\">Create SFTP connectors</a>.</p> <note> <p>You must specify exactly one configuration object: either for AS2 (<code>As2Config</code>) or SFTP (<code>SftpConfig</code>).</p> </note>",
+            "documentation": "<p>Creates the connector, which captures the parameters for a connection for the AS2 or SFTP protocol. For AS2, the connector is required for sending files to an externally hosted AS2 server. For SFTP, the connector is required when sending files to an SFTP server or receiving files from an SFTP server. For more details about connectors, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/create-b2b-server.html#configure-as2-connector\">Create AS2 connectors</a> and <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/configure-sftp-connector.html\">Create SFTP connectors</a>.</p> <note> <p>You must specify exactly one configuration object: either for AS2 (<code>As2Config</code>) or SFTP (<code>SftpConfig</code>).</p> </note>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "InvalidRequestException"
                 },
@@ -701,15 +701,15 @@
             },
             "name": "DescribeProfile",
             "output": {
                 "shape": "DescribeProfileResponse"
             }
         },
         "DescribeSecurityPolicy": {
-            "documentation": "<p>Describes the security policy that is attached to your server or SFTP connector. The response contains a description of the security policy's properties. For more information about security policies, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies.html\">Working with security policies for servers</a> or <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies-connectors.html\">Working with security policies for SFTP connectors</a>.</p>",
+            "documentation": "<p>Describes the security policy that is attached to your file transfer protocol-enabled server. The response contains a description of the security policy's properties. For more information about security policies, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies.html\">Working with security policies</a>.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "InvalidRequestException"
                 },
@@ -1126,15 +1126,15 @@
             },
             "name": "ListProfiles",
             "output": {
                 "shape": "ListProfilesResponse"
             }
         },
         "ListSecurityPolicies": {
-            "documentation": "<p>Lists the security policies that are attached to your servers and SFTP connectors. For more information about security policies, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies.html\">Working with security policies for servers</a> or <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies-connectors.html\">Working with security policies for SFTP connectors</a>.</p>",
+            "documentation": "<p>Lists the security policies that are attached to your file transfer protocol-enabled servers.</p>",
             "errors": [
                 {
                     "shape": "InvalidRequestException"
                 },
                 {
                     "shape": "InternalServiceError"
                 },
@@ -1302,47 +1302,16 @@
                 "shape": "SendWorkflowStepStateRequest"
             },
             "name": "SendWorkflowStepState",
             "output": {
                 "shape": "SendWorkflowStepStateResponse"
             }
         },
-        "StartDirectoryListing": {
-            "documentation": "<p>Retrieves a list of the contents of a directory from a remote SFTP server. You specify the connector ID, the output path, and the remote directory path. You can also specify the optional <code>MaxItems</code> value to control the maximum number of items that are listed from the remote directory. This API returns a list of all files and directories in the remote directory (up to the maximum value), but does not return files or folders in sub-directories. That is, it only returns a list of files and directories one-level deep.</p> <p>After you receive the listing file, you can provide the files that you want to transfer to the <code>RetrieveFilePaths</code> parameter of the <code>StartFileTransfer</code> API call.</p> <p>The naming convention for the output file is <code> <i>connector-ID</i>-<i>listing-ID</i>.json</code>. The output file contains the following information:</p> <ul> <li> <p> <code>filePath</code>: the complete path of a remote file, relative to the directory of the listing request for your SFTP connector on the remote server.</p> </li> <li> <p> <code>modifiedTimestamp</code>: the last time the file was modified, in UTC time format. This field is optional. If the remote file attributes don't contain a timestamp, it is omitted from the file listing.</p> </li> <li> <p> <code>size</code>: the size of the file, in bytes. This field is optional. If the remote file attributes don't contain a file size, it is omitted from the file listing.</p> </li> <li> <p> <code>path</code>: the complete path of a remote directory, relative to the directory of the listing request for your SFTP connector on the remote server.</p> </li> <li> <p> <code>truncated</code>: a flag indicating whether the list output contains all of the items contained in the remote directory or not. If your <code>Truncated</code> output value is true, you can increase the value provided in the optional <code>max-items</code> input attribute to be able to list more items (up to the maximum allowed list size of 10,000 items).</p> </li> </ul>",
-            "errors": [
-                {
-                    "shape": "ResourceNotFoundException"
-                },
-                {
-                    "shape": "InvalidRequestException"
-                },
-                {
-                    "shape": "ThrottlingException"
-                },
-                {
-                    "shape": "InternalServiceError"
-                },
-                {
-                    "shape": "ServiceUnavailableException"
-                }
-            ],
-            "http": {
-                "method": "POST",
-                "requestUri": "/"
-            },
-            "input": {
-                "shape": "StartDirectoryListingRequest"
-            },
-            "name": "StartDirectoryListing",
-            "output": {
-                "shape": "StartDirectoryListingResponse"
-            }
-        },
         "StartFileTransfer": {
-            "documentation": "<p>Begins a file transfer between local Amazon Web Services storage and a remote AS2 or SFTP server.</p> <ul> <li> <p>For an AS2 connector, you specify the <code>ConnectorId</code> and one or more <code>SendFilePaths</code> to identify the files you want to transfer.</p> </li> <li> <p>For an SFTP connector, the file transfer can be either outbound or inbound. In both cases, you specify the <code>ConnectorId</code>. Depending on the direction of the transfer, you also specify the following items:</p> <ul> <li> <p>If you are transferring file from a partner's SFTP server to Amazon Web Services storage, you specify one or more <code>RetrieveFilePaths</code> to identify the files you want to transfer, and a <code>LocalDirectoryPath</code> to specify the destination folder.</p> </li> <li> <p>If you are transferring file to a partner's SFTP server from Amazon Web Services storage, you specify one or more <code>SendFilePaths</code> to identify the files you want to transfer, and a <code>RemoteDirectoryPath</code> to specify the destination folder.</p> </li> </ul> </li> </ul>",
+            "documentation": "<p>Begins a file transfer between local Amazon Web Services storage and a remote AS2 or SFTP server.</p> <ul> <li> <p>For an AS2 connector, you specify the <code>ConnectorId</code> and one or more <code>SendFilePaths</code> to identify the files you want to transfer.</p> </li> <li> <p>For an SFTP connector, the file transfer can be either outbound or inbound. In both cases, you specify the <code>ConnectorId</code>. Depending on the direction of the transfer, you also specify the following items:</p> <ul> <li> <p>If you are transferring file from a partner's SFTP server to Amazon Web Services storage, you specify one or more <code>RetreiveFilePaths</code> to identify the files you want to transfer, and a <code>LocalDirectoryPath</code> to specify the destination folder.</p> </li> <li> <p>If you are transferring file to a partner's SFTP server from Amazon Web Services storage, you specify one or more <code>SendFilePaths</code> to identify the files you want to transfer, and a <code>RemoteDirectoryPath</code> to specify the destination folder.</p> </li> </ul> </li> </ul>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "InvalidRequestException"
                 },
@@ -1762,15 +1731,15 @@
             },
             "name": "UpdateServer",
             "output": {
                 "shape": "UpdateServerResponse"
             }
         },
         "UpdateUser": {
-            "documentation": "<p>Assigns new properties to a user. Parameters you pass modify any or all of the following: the home directory, role, and policy for the <code>UserName</code> and <code>ServerId</code> you specify.</p> <p>The response returns the <code>ServerId</code> and the <code>UserName</code> for the updated user.</p> <p>In the console, you can select <i>Restricted</i> when you create or update a user. This ensures that the user can't access anything outside of their home directory. The programmatic way to configure this behavior is to update the user. Set their <code>HomeDirectoryType</code> to <code>LOGICAL</code>, and specify <code>HomeDirectoryMappings</code> with <code>Entry</code> as root (<code>/</code>) and <code>Target</code> as their home directory.</p> <p>For example, if the user's home directory is <code>/test/admin-user</code>, the following command updates the user so that their configuration in the console shows the <i>Restricted</i> flag as selected.</p> <p> <code> aws transfer update-user --server-id &lt;server-id&gt; --user-name admin-user --home-directory-type LOGICAL --home-directory-mappings \"[{\\\"Entry\\\":\\\"/\\\", \\\"Target\\\":\\\"/test/admin-user\\\"}]\"</code> </p>",
+            "documentation": "<p>Assigns new properties to a user. Parameters you pass modify any or all of the following: the home directory, role, and policy for the <code>UserName</code> and <code>ServerId</code> you specify.</p> <p>The response returns the <code>ServerId</code> and the <code>UserName</code> for the updated user.</p>",
             "errors": [
                 {
                     "shape": "ResourceNotFoundException"
                 },
                 {
                     "shape": "InvalidRequestException"
                 },
@@ -1844,15 +1813,15 @@
                     "shape": "As2ConnectorSecretId"
                 },
                 "Compression": {
                     "documentation": "<p>Specifies whether the AS2 file is compressed.</p>",
                     "shape": "CompressionEnum"
                 },
                 "EncryptionAlgorithm": {
-                    "documentation": "<p>The algorithm that is used to encrypt the file.</p> <p>Note the following:</p> <ul> <li> <p>Do not use the <code>DES_EDE3_CBC</code> algorithm unless you must support a legacy client that requires it, as it is a weak encryption algorithm.</p> </li> <li> <p>You can only specify <code>NONE</code> if the URL for your connector uses HTTPS. Using HTTPS ensures that no traffic is sent in clear text.</p> </li> </ul>",
+                    "documentation": "<p>The algorithm that is used to encrypt the file.</p> <note> <p>You can only specify <code>NONE</code> if the URL for your connector uses HTTPS. This ensures that no traffic is sent in clear text.</p> </note>",
                     "shape": "EncryptionAlg"
                 },
                 "LocalProfileId": {
                     "documentation": "<p>A unique identifier for the AS2 local profile.</p>",
                     "shape": "ProfileId"
                 },
                 "MdnResponse": {
@@ -1963,16 +1932,15 @@
                 "CERTIFICATE_WITH_PRIVATE_KEY"
             ],
             "type": "string"
         },
         "CertificateUsageType": {
             "enum": [
                 "SIGNING",
-                "ENCRYPTION",
-                "TLS"
+                "ENCRYPTION"
             ],
             "type": "string"
         },
         "CompressionEnum": {
             "enum": [
                 "ZLIB",
                 "DISABLED"
@@ -1994,20 +1962,14 @@
         },
         "ConnectorId": {
             "max": 19,
             "min": 19,
             "pattern": "c-([0-9a-f]{17})",
             "type": "string"
         },
-        "ConnectorSecurityPolicyName": {
-            "max": 100,
-            "min": 0,
-            "pattern": "TransferSFTPConnectorSecurityPolicy-[A-Za-z0-9-]+",
-            "type": "string"
-        },
         "CopyStepDetails": {
             "documentation": "<p>Each step type has its own <code>StepDetails</code> structure.</p>",
             "members": {
                 "DestinationFileLocation": {
                     "documentation": "<p>Specifies the location for the file being copied. Use <code>${Transfer:UserName}</code> or <code>${Transfer:UploadDate}</code> in this field to parametrize the destination prefix by username or uploaded date.</p> <ul> <li> <p>Set the value of <code>DestinationFileLocation</code> to <code>${Transfer:UserName}</code> to copy uploaded files to an Amazon S3 bucket that is prefixed with the name of the Transfer Family user that uploaded the file.</p> </li> <li> <p>Set the value of <code>DestinationFileLocation</code> to <code>${Transfer:UploadDate}</code> to copy uploaded files to an Amazon S3 bucket that is prefixed with the date of the upload.</p> <note> <p>The system resolves <code>UploadDate</code> to a date format of <i>YYYY-MM-DD</i>, based on the date the file is uploaded in UTC.</p> </note> </li> </ul>",
                     "shape": "InputFileLocation"
                 },
@@ -2150,18 +2112,14 @@
                     "documentation": "<p>A structure that contains the parameters for an AS2 connector object.</p>",
                     "shape": "As2ConnectorConfig"
                 },
                 "LoggingRole": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role that allows a connector to turn on CloudWatch logging for Amazon S3 events. When set, you can view connector activity in your CloudWatch logs.</p>",
                     "shape": "Role"
                 },
-                "SecurityPolicyName": {
-                    "documentation": "<p>Specifies the name of the security policy for the connector.</p>",
-                    "shape": "ConnectorSecurityPolicyName"
-                },
                 "SftpConfig": {
                     "documentation": "<p>A structure that contains the parameters for an SFTP connector object.</p>",
                     "shape": "SftpConnectorConfig"
                 },
                 "Tags": {
                     "documentation": "<p>Key-value pairs that can be used to group and search for connectors. Tags are metadata attached to connectors for any purpose.</p>",
                     "shape": "Tags"
@@ -2277,15 +2235,15 @@
                     "shape": "Protocols"
                 },
                 "S3StorageOptions": {
                     "documentation": "<p>Specifies whether or not performance for your Amazon S3 directories is optimized. This is disabled by default.</p> <p>By default, home directory mappings have a <code>TYPE</code> of <code>DIRECTORY</code>. If you enable this option, you would then need to explicitly set the <code>HomeDirectoryMapEntry</code> <code>Type</code> to <code>FILE</code> if you want a mapping to have a file target.</p>",
                     "shape": "S3StorageOptions"
                 },
                 "SecurityPolicyName": {
-                    "documentation": "<p>Specifies the name of the security policy for the server.</p>",
+                    "documentation": "<p>Specifies the name of the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyName"
                 },
                 "StructuredLogDestinations": {
                     "documentation": "<p>Specifies the log groups to which your server logs are sent.</p> <p>To specify a log group, you must provide the ARN for an existing log group. In this case, the format of the log group is as follows:</p> <p> <code>arn:aws:logs:region-name:amazon-account-id:log-group:log-group-name:*</code> </p> <p>For example, <code>arn:aws:logs:us-east-1:111122223333:log-group:mytestgroup:*</code> </p> <p>If you have previously specified a log group for a server, you can clear it, and in effect turn off structured logging, by providing an empty value for this parameter in an <code>update-server</code> call. For example:</p> <p> <code>update-server --server-id s-1234567890abcdef0 --structured-log-destinations</code> </p>",
                     "shape": "StructuredLogDestinations"
                 },
                 "Tags": {
@@ -2849,15 +2807,15 @@
                 "Profile"
             ],
             "type": "structure"
         },
         "DescribeSecurityPolicyRequest": {
             "members": {
                 "SecurityPolicyName": {
-                    "documentation": "<p>Specify the text name of the security policy for which you want the details.</p>",
+                    "documentation": "<p>Specifies the name of the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyName"
                 }
             },
             "required": [
                 "SecurityPolicyName"
             ],
             "type": "structure"
@@ -3122,22 +3080,14 @@
                     "documentation": "<p>The unique identifier for the connector.</p>",
                     "shape": "ConnectorId"
                 },
                 "LoggingRole": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role that allows a connector to turn on CloudWatch logging for Amazon S3 events. When set, you can view connector activity in your CloudWatch logs.</p>",
                     "shape": "Role"
                 },
-                "SecurityPolicyName": {
-                    "documentation": "<p>The text name of the security policy for the specified connector.</p>",
-                    "shape": "ConnectorSecurityPolicyName"
-                },
-                "ServiceManagedEgressIpAddresses": {
-                    "documentation": "<p>The list of egress IP addresses of this connector. These IP addresses are assigned automatically when you create the connector.</p>",
-                    "shape": "ServiceManagedEgressIpAddresses"
-                },
                 "SftpConfig": {
                     "documentation": "<p>A structure that contains the parameters for an SFTP connector object.</p>",
                     "shape": "SftpConnectorConfig"
                 },
                 "Tags": {
                     "documentation": "<p>Key-value pairs that can be used to group and search for connectors.</p>",
                     "shape": "Tags"
@@ -3256,69 +3206,53 @@
             },
             "required": [
                 "Arn"
             ],
             "type": "structure"
         },
         "DescribedSecurityPolicy": {
-            "documentation": "<p>Describes the properties of a security policy that you specify. For more information about security policies, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies.html\">Working with security policies for servers</a> or <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies-connectors.html\">Working with security policies for SFTP connectors</a>.</p>",
+            "documentation": "<p>Describes the properties of a security policy that was specified. For more information about security policies, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/security-policies.html\">Working with security policies</a>.</p>",
             "members": {
                 "Fips": {
-                    "documentation": "<p>Specifies whether this policy enables Federal Information Processing Standards (FIPS). This parameter applies to both server and connector security policies.</p>",
+                    "documentation": "<p>Specifies whether this policy enables Federal Information Processing Standards (FIPS).</p>",
                     "shape": "Fips"
                 },
-                "Protocols": {
-                    "documentation": "<p>Lists the file transfer protocols that the security policy applies to.</p>",
-                    "shape": "SecurityPolicyProtocols"
-                },
                 "SecurityPolicyName": {
-                    "documentation": "<p>The text name of the specified security policy.</p>",
+                    "documentation": "<p>Specifies the name of the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyName"
                 },
                 "SshCiphers": {
-                    "documentation": "<p>Lists the enabled Secure Shell (SSH) cipher encryption algorithms in the security policy that is attached to the server or connector. This parameter applies to both server and connector security policies.</p>",
-                    "shape": "SecurityPolicyOptions"
-                },
-                "SshHostKeyAlgorithms": {
-                    "documentation": "<p>Lists the host key algorithms for the security policy.</p> <note> <p>This parameter only applies to security policies for connectors.</p> </note>",
+                    "documentation": "<p>Specifies the enabled Secure Shell (SSH) cipher encryption algorithms in the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyOptions"
                 },
                 "SshKexs": {
-                    "documentation": "<p>Lists the enabled SSH key exchange (KEX) encryption algorithms in the security policy that is attached to the server or connector. This parameter applies to both server and connector security policies.</p>",
+                    "documentation": "<p>Specifies the enabled SSH key exchange (KEX) encryption algorithms in the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyOptions"
                 },
                 "SshMacs": {
-                    "documentation": "<p>Lists the enabled SSH message authentication code (MAC) encryption algorithms in the security policy that is attached to the server or connector. This parameter applies to both server and connector security policies.</p>",
+                    "documentation": "<p>Specifies the enabled SSH message authentication code (MAC) encryption algorithms in the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyOptions"
                 },
                 "TlsCiphers": {
-                    "documentation": "<p>Lists the enabled Transport Layer Security (TLS) cipher encryption algorithms in the security policy that is attached to the server.</p> <note> <p>This parameter only applies to security policies for servers.</p> </note>",
+                    "documentation": "<p>Specifies the enabled Transport Layer Security (TLS) cipher encryption algorithms in the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyOptions"
-                },
-                "Type": {
-                    "documentation": "<p>The resource type to which the security policy applies, either server or connector.</p>",
-                    "shape": "SecurityPolicyResourceType"
                 }
             },
             "required": [
                 "SecurityPolicyName"
             ],
             "type": "structure"
         },
         "DescribedServer": {
             "documentation": "<p>Describes the properties of a file transfer protocol-enabled server that was specified.</p>",
             "members": {
                 "Arn": {
                     "documentation": "<p>Specifies the unique Amazon Resource Name (ARN) of the server.</p>",
                     "shape": "Arn"
                 },
-                "As2ServiceManagedEgressIpAddresses": {
-                    "documentation": "<p>The list of egress IP addresses of this server. These IP addresses are only relevant for servers that use the AS2 protocol. They are used for sending asynchronous MDNs.</p> <p>These IP addresses are assigned automatically when you create an AS2 server. Additionally, if you update an existing server and add the AS2 protocol, static IP addresses are assigned as well.</p>",
-                    "shape": "ServiceManagedEgressIpAddresses"
-                },
                 "Certificate": {
                     "documentation": "<p>Specifies the ARN of the Amazon Web ServicesCertificate Manager (ACM) certificate. Required when <code>Protocols</code> is set to <code>FTPS</code>.</p>",
                     "shape": "Certificate"
                 },
                 "Domain": {
                     "documentation": "<p>Specifies the domain of the storage system that is used for file transfers.</p>",
                     "shape": "Domain"
@@ -3364,15 +3298,15 @@
                     "shape": "Protocols"
                 },
                 "S3StorageOptions": {
                     "documentation": "<p>Specifies whether or not performance for your Amazon S3 directories is optimized. This is disabled by default.</p> <p>By default, home directory mappings have a <code>TYPE</code> of <code>DIRECTORY</code>. If you enable this option, you would then need to explicitly set the <code>HomeDirectoryMapEntry</code> <code>Type</code> to <code>FILE</code> if you want a mapping to have a file target.</p>",
                     "shape": "S3StorageOptions"
                 },
                 "SecurityPolicyName": {
-                    "documentation": "<p>Specifies the name of the security policy for the server.</p>",
+                    "documentation": "<p>Specifies the name of the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyName"
                 },
                 "ServerId": {
                     "documentation": "<p>Specifies the unique system-assigned identifier for a server that you instantiate.</p>",
                     "shape": "ServerId"
                 },
                 "State": {
@@ -3537,30 +3471,29 @@
             "type": "string"
         },
         "EncryptionAlg": {
             "enum": [
                 "AES128_CBC",
                 "AES192_CBC",
                 "AES256_CBC",
-                "DES_EDE3_CBC",
                 "NONE"
             ],
             "type": "string"
         },
         "EncryptionType": {
             "enum": [
                 "PGP"
             ],
             "type": "string"
         },
         "EndpointDetails": {
             "documentation": "<p>The virtual private cloud (VPC) endpoint settings that are configured for your file transfer protocol-enabled server. With a VPC endpoint, you can restrict access to your server and resources only within your VPC. To control incoming internet traffic, invoke the <code>UpdateServer</code> API and attach an Elastic IP address to your server's endpoint.</p> <note> <p> After May 19, 2021, you won't be able to create a server using <code>EndpointType=VPC_ENDPOINT</code> in your Amazon Web Servicesaccount if your account hasn't already done so before May 19, 2021. If you have already created servers with <code>EndpointType=VPC_ENDPOINT</code> in your Amazon Web Servicesaccount on or before May 19, 2021, you will not be affected. After this date, use <code>EndpointType</code>=<code>VPC</code>.</p> <p>For more information, see https://docs.aws.amazon.com/transfer/latest/userguide/create-server-in-vpc.html#deprecate-vpc-endpoint.</p> </note>",
             "members": {
                 "AddressAllocationIds": {
-                    "documentation": "<p>A list of address allocation IDs that are required to attach an Elastic IP address to your server's endpoint.</p> <p>An address allocation ID corresponds to the allocation ID of an Elastic IP address. This value can be retrieved from the <code>allocationId</code> field from the Amazon EC2 <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_Address.html\">Address</a> data type. One way to retrieve this value is by calling the EC2 <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_DescribeAddresses.html\">DescribeAddresses</a> API.</p> <p>This parameter is optional. Set this parameter if you want to make your VPC endpoint public-facing. For details, see <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/create-server-in-vpc.html#create-internet-facing-endpoint\">Create an internet-facing endpoint for your server</a>.</p> <note> <p>This property can only be set as follows:</p> <ul> <li> <p> <code>EndpointType</code> must be set to <code>VPC</code> </p> </li> <li> <p>The Transfer Family server must be offline.</p> </li> <li> <p>You cannot set this parameter for Transfer Family servers that use the FTP protocol.</p> </li> <li> <p>The server must already have <code>SubnetIds</code> populated (<code>SubnetIds</code> and <code>AddressAllocationIds</code> cannot be updated simultaneously).</p> </li> <li> <p> <code>AddressAllocationIds</code> can't contain duplicates, and must be equal in length to <code>SubnetIds</code>. For example, if you have three subnet IDs, you must also specify three address allocation IDs.</p> </li> <li> <p>Call the <code>UpdateServer</code> API to set or change this parameter.</p> </li> </ul> </note>",
+                    "documentation": "<p>A list of address allocation IDs that are required to attach an Elastic IP address to your server's endpoint.</p> <note> <p>This property can only be set when <code>EndpointType</code> is set to <code>VPC</code> and it is only valid in the <code>UpdateServer</code> API.</p> </note>",
                     "shape": "AddressAllocationIds"
                 },
                 "SecurityGroupIds": {
                     "documentation": "<p>A list of security groups IDs that are available to attach to your server's endpoint.</p> <note> <p>This property can only be set when <code>EndpointType</code> is set to <code>VPC</code>.</p> <p>You can edit the <code>SecurityGroupIds</code> property in the <a href=\"https://docs.aws.amazon.com/transfer/latest/userguide/API_UpdateServer.html\">UpdateServer</a> API only if you are changing the <code>EndpointType</code> from <code>PUBLIC</code> or <code>VPC_ENDPOINT</code> to <code>VPC</code>. To change security groups associated with your server's VPC endpoint after creation, use the Amazon EC2 <a href=\"https://docs.aws.amazon.com/AWSEC2/latest/APIReference/API_ModifyVpcEndpoint.html\">ModifyVpcEndpoint</a> API.</p> </note>",
                     "shape": "SecurityGroupIds"
                 },
                 "SubnetIds": {
@@ -3786,15 +3719,15 @@
         "HostKeyType": {
             "type": "string"
         },
         "IdentityProviderDetails": {
             "documentation": "<p>Returns information related to the type of user authentication that is in use for a file transfer protocol-enabled server's users. A server can have only one method of authentication.</p>",
             "members": {
                 "DirectoryId": {
-                    "documentation": "<p>The identifier of the Directory Service directory that you want to use as your identity provider.</p>",
+                    "documentation": "<p>The identifier of the Directory Service directory that you want to stop sharing.</p>",
                     "shape": "DirectoryId"
                 },
                 "Function": {
                     "documentation": "<p>The ARN for a Lambda function to use for the Identity provider.</p>",
                     "shape": "Function"
                 },
                 "InvocationRole": {
@@ -4768,20 +4701,14 @@
         },
         "ListedWorkflows": {
             "member": {
                 "shape": "ListedWorkflow"
             },
             "type": "list"
         },
-        "ListingId": {
-            "max": 512,
-            "min": 1,
-            "pattern": "[0-9a-zA-Z./-]+",
-            "type": "string"
-        },
         "LogGroupName": {
             "max": 512,
             "min": 1,
             "pattern": "[\\.\\-_/#A-Za-z0-9]*",
             "type": "string"
         },
         "LoggingConfiguration": {
@@ -4813,20 +4740,14 @@
         "MapType": {
             "enum": [
                 "FILE",
                 "DIRECTORY"
             ],
             "type": "string"
         },
-        "MaxItems": {
-            "box": true,
-            "max": 10000,
-            "min": 1,
-            "type": "integer"
-        },
         "MaxResults": {
             "box": true,
             "max": 1000,
             "min": 1,
             "type": "integer"
         },
         "MdnResponse": {
@@ -4879,20 +4800,14 @@
             "max": 1,
             "member": {
                 "shape": "WorkflowDetail"
             },
             "min": 0,
             "type": "list"
         },
-        "OutputFileName": {
-            "max": 537,
-            "min": 26,
-            "pattern": "c-([0-9a-f]{17})-[0-9a-zA-Z./-]+.json",
-            "type": "string"
-        },
         "OverwriteExisting": {
             "enum": [
                 "TRUE",
                 "FALSE"
             ],
             "type": "string"
         },
@@ -5197,15 +5112,15 @@
                 "shape": "SecurityGroupId"
             },
             "type": "list"
         },
         "SecurityPolicyName": {
             "max": 100,
             "min": 0,
-            "pattern": "Transfer[A-Za-z0-9]*SecurityPolicy-[A-Za-z0-9-]+",
+            "pattern": "TransferSecurityPolicy-.+",
             "type": "string"
         },
         "SecurityPolicyNames": {
             "member": {
                 "shape": "SecurityPolicyName"
             },
             "type": "list"
@@ -5217,36 +5132,14 @@
         },
         "SecurityPolicyOptions": {
             "member": {
                 "shape": "SecurityPolicyOption"
             },
             "type": "list"
         },
-        "SecurityPolicyProtocol": {
-            "enum": [
-                "SFTP",
-                "FTPS"
-            ],
-            "type": "string"
-        },
-        "SecurityPolicyProtocols": {
-            "max": 5,
-            "member": {
-                "shape": "SecurityPolicyProtocol"
-            },
-            "min": 1,
-            "type": "list"
-        },
-        "SecurityPolicyResourceType": {
-            "enum": [
-                "SERVER",
-                "CONNECTOR"
-            ],
-            "type": "string"
-        },
         "SendWorkflowStepStateRequest": {
             "members": {
                 "ExecutionId": {
                     "documentation": "<p>A unique identifier for the execution of a workflow.</p>",
                     "shape": "ExecutionId"
                 },
                 "Status": {
@@ -5279,24 +5172,14 @@
             "min": 19,
             "pattern": "s-([0-9a-f]{17})",
             "type": "string"
         },
         "ServiceErrorMessage": {
             "type": "string"
         },
-        "ServiceManagedEgressIpAddress": {
-            "pattern": "\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}",
-            "type": "string"
-        },
-        "ServiceManagedEgressIpAddresses": {
-            "member": {
-                "shape": "ServiceManagedEgressIpAddress"
-            },
-            "type": "list"
-        },
         "ServiceMetadata": {
             "documentation": "<p>A container object for the session details that are associated with a workflow.</p>",
             "members": {
                 "UserDetails": {
                     "documentation": "<p>The Server ID (<code>ServerId</code>), Session ID (<code>SessionId</code>) and user (<code>UserName</code>) make up the <code>UserDetails</code>.</p>",
                     "shape": "UserDetails"
                 }
@@ -5336,18 +5219,18 @@
                 "PUBLIC_KEY",
                 "PUBLIC_KEY_OR_PASSWORD",
                 "PUBLIC_KEY_AND_PASSWORD"
             ],
             "type": "string"
         },
         "SftpConnectorConfig": {
-            "documentation": "<p>Contains the details for an SFTP connector object. The connector object is used for transferring files to and from a partner's SFTP server.</p> <note> <p>Because the <code>SftpConnectorConfig</code> data type is used for both creating and updating SFTP connectors, its parameters, <code>TrustedHostKeys</code> and <code>UserSecretId</code> are marked as not required. This is a bit misleading, as they are not required when you are updating an existing SFTP connector, but <i>are required</i> when you are creating a new SFTP connector.</p> </note>",
+            "documentation": "<p>Contains the details for an SFTP connector object. The connector object is used for transferring files to and from a partner's SFTP server.</p>",
             "members": {
                 "TrustedHostKeys": {
-                    "documentation": "<p>The public portion of the host key, or keys, that are used to identify the external server to which you are connecting. You can use the <code>ssh-keyscan</code> command against the SFTP server to retrieve the necessary key.</p> <p>The three standard SSH public key format elements are <code>&lt;key type&gt;</code>, <code>&lt;body base64&gt;</code>, and an optional <code>&lt;comment&gt;</code>, with spaces between each element. Specify only the <code>&lt;key type&gt;</code> and <code>&lt;body base64&gt;</code>: do not enter the <code>&lt;comment&gt;</code> portion of the key.</p> <p>For the trusted host key, Transfer Family accepts RSA and ECDSA keys.</p> <ul> <li> <p>For RSA keys, the <code>&lt;key type&gt;</code> string is <code>ssh-rsa</code>.</p> </li> <li> <p>For ECDSA keys, the <code>&lt;key type&gt;</code> string is either <code>ecdsa-sha2-nistp256</code>, <code>ecdsa-sha2-nistp384</code>, or <code>ecdsa-sha2-nistp521</code>, depending on the size of the key you generated.</p> </li> </ul> <p>Run this command to retrieve the SFTP server host key, where your SFTP server name is <code>ftp.host.com</code>.</p> <p> <code>ssh-keyscan ftp.host.com</code> </p> <p>This prints the public host key to standard output.</p> <p> <code>ftp.host.com ssh-rsa AAAAB3Nza...&lt;long-string-for-public-key</code> </p> <p>Copy and paste this string into the <code>TrustedHostKeys</code> field for the <code>create-connector</code> command or into the <b>Trusted host keys</b> field in the console.</p>",
+                    "documentation": "<p>The public portion of the host key, or keys, that are used to identify the external server to which you are connecting. You can use the <code>ssh-keyscan</code> command against the SFTP server to retrieve the necessary key.</p> <p>The three standard SSH public key format elements are <code>&lt;key type&gt;</code>, <code>&lt;body base64&gt;</code>, and an optional <code>&lt;comment&gt;</code>, with spaces between each element. Specify only the <code>&lt;key type&gt;</code> and <code>&lt;body base64&gt;</code>: do not enter the <code>&lt;comment&gt;</code> portion of the key.</p> <p>For the trusted host key, Transfer Family accepts RSA and ECDSA keys.</p> <ul> <li> <p>For RSA keys, the <code>&lt;key type&gt;</code> string is <code>ssh-rsa</code>.</p> </li> <li> <p>For ECDSA keys, the <code>&lt;key type&gt;</code> string is either <code>ecdsa-sha2-nistp256</code>, <code>ecdsa-sha2-nistp384</code>, or <code>ecdsa-sha2-nistp521</code>, depending on the size of the key you generated.</p> </li> </ul>",
                     "shape": "SftpConnectorTrustedHostKeyList"
                 },
                 "UserSecretId": {
                     "documentation": "<p>The identifier for the secret (in Amazon Web Services Secrets Manager) that contains the SFTP user's private key, password, or both. The identifier must be the Amazon Resource Name (ARN) of the secret.</p>",
                     "shape": "SecretId"
                 }
             },
@@ -5430,57 +5313,14 @@
             "max": 5,
             "member": {
                 "shape": "SshPublicKey"
             },
             "min": 0,
             "type": "list"
         },
-        "StartDirectoryListingRequest": {
-            "members": {
-                "ConnectorId": {
-                    "documentation": "<p>The unique identifier for the connector.</p>",
-                    "shape": "ConnectorId"
-                },
-                "MaxItems": {
-                    "documentation": "<p>An optional parameter where you can specify the maximum number of file/directory names to retrieve. The default value is 1,000.</p>",
-                    "shape": "MaxItems"
-                },
-                "OutputDirectoryPath": {
-                    "documentation": "<p>Specifies the path (bucket and prefix) in Amazon S3 storage to store the results of the directory listing.</p>",
-                    "shape": "FilePath"
-                },
-                "RemoteDirectoryPath": {
-                    "documentation": "<p>Specifies the directory on the remote SFTP server for which you want to list its contents.</p>",
-                    "shape": "FilePath"
-                }
-            },
-            "required": [
-                "ConnectorId",
-                "RemoteDirectoryPath",
-                "OutputDirectoryPath"
-            ],
-            "type": "structure"
-        },
-        "StartDirectoryListingResponse": {
-            "members": {
-                "ListingId": {
-                    "documentation": "<p>Returns a unique identifier for the directory listing call.</p>",
-                    "shape": "ListingId"
-                },
-                "OutputFileName": {
-                    "documentation": "<p>Returns the file name where the results are stored. This is a combination of the connector ID and the listing ID: <code>&lt;connector-id&gt;-&lt;listing-id&gt;.json</code>.</p>",
-                    "shape": "OutputFileName"
-                }
-            },
-            "required": [
-                "ListingId",
-                "OutputFileName"
-            ],
-            "type": "structure"
-        },
         "StartFileTransferRequest": {
             "members": {
                 "ConnectorId": {
                     "documentation": "<p>The unique identifier for the connector.</p>",
                     "shape": "ConnectorId"
                 },
                 "LocalDirectoryPath": {
@@ -5944,18 +5784,14 @@
                     "documentation": "<p>The unique identifier for the connector.</p>",
                     "shape": "ConnectorId"
                 },
                 "LoggingRole": {
                     "documentation": "<p>The Amazon Resource Name (ARN) of the Identity and Access Management (IAM) role that allows a connector to turn on CloudWatch logging for Amazon S3 events. When set, you can view connector activity in your CloudWatch logs.</p>",
                     "shape": "Role"
                 },
-                "SecurityPolicyName": {
-                    "documentation": "<p>Specifies the name of the security policy for the connector.</p>",
-                    "shape": "ConnectorSecurityPolicyName"
-                },
                 "SftpConfig": {
                     "documentation": "<p>A structure that contains the parameters for an SFTP connector object.</p>",
                     "shape": "SftpConnectorConfig"
                 },
                 "Url": {
                     "documentation": "<p>The URL of the partner's AS2 or SFTP endpoint.</p>",
                     "shape": "Url"
@@ -6088,15 +5924,15 @@
                     "shape": "Protocols"
                 },
                 "S3StorageOptions": {
                     "documentation": "<p>Specifies whether or not performance for your Amazon S3 directories is optimized. This is disabled by default.</p> <p>By default, home directory mappings have a <code>TYPE</code> of <code>DIRECTORY</code>. If you enable this option, you would then need to explicitly set the <code>HomeDirectoryMapEntry</code> <code>Type</code> to <code>FILE</code> if you want a mapping to have a file target.</p>",
                     "shape": "S3StorageOptions"
                 },
                 "SecurityPolicyName": {
-                    "documentation": "<p>Specifies the name of the security policy for the server.</p>",
+                    "documentation": "<p>Specifies the name of the security policy that is attached to the server.</p>",
                     "shape": "SecurityPolicyName"
                 },
                 "ServerId": {
                     "documentation": "<p>A system-assigned unique identifier for a server instance that the Transfer Family user is assigned to.</p>",
                     "shape": "ServerId"
                 },
                 "StructuredLogDestinations": {
```

### Comparing `botocore-a-la-carte-transfer-1.34.89/botocore/data/transfer/2018-11-05/waiters-2.json` & `botocore-a-la-carte-transfer-1.34.9/botocore/data/transfer/2018-11-05/waiters-2.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-transfer-1.34.89/botocore_a_la_carte_transfer.egg-info/PKG-INFO` & `botocore-a-la-carte-transfer-1.34.9/botocore_a_la_carte_transfer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-transfer
-Version: 1.34.89
+Version: 1.34.9
 Summary: transfer data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-transfer-1.34.89/setup.py` & `botocore-a-la-carte-transfer-1.34.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-transfer',
-    version="1.34.89",
+    version="1.34.9",
     description='transfer data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/transfer/*/*.json'],
```

