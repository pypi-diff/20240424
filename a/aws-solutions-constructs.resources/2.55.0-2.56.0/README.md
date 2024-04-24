# Comparing `tmp/aws-solutions-constructs.resources-2.55.0.tar.gz` & `tmp/aws_solutions_constructs.resources-2.56.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aws-solutions-constructs.resources-2.55.0.tar", last modified: Fri Apr 12 16:15:38 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

## Comparing `aws-solutions-constructs.resources-2.55.0.tar` & `aws_solutions_constructs/resources/_jsii/resources@2.56.0.jsii.tgz`

 * *Files 8% similar despite different names*

### file list

```diff
@@ -1,22 +1,52 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.512487 aws-solutions-constructs.resources-2.55.0/
--rw-r--r--   0 root         (0) root         (0)    10279 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2425 2024-04-12 16:15:38.512487 aws-solutions-constructs.resources-2.55.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1554 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/README.md
--rw-r--r--   0 root         (0) root         (0)      234 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-12 16:15:38.512487 aws-solutions-constructs.resources-2.55.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1891 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.504487 aws-solutions-constructs.resources-2.55.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.504487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.508487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/
--rw-r--r--   0 root         (0) root         (0)    19179 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.508487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/
--rw-r--r--   0 root         (0) root         (0)      584 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2063939 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/_jsii/resources@2.55.0.jsii.tgz
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 16:15:07.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs/resources/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-12 16:15:38.508487 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2425 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      589 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      188 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       25 2024-04-12 16:15:38.000000 aws-solutions-constructs.resources-2.55.0/src/aws_solutions_constructs.resources.egg-info/top_level.txt
+-rw-r--r--   0        0        0       89 1985-10-26 08:15:00.000000 package/.eslintignore
+-rw-r--r--   0        0        0   121661 1985-10-26 08:15:00.000000 package/.jsii
+-rw-r--r--   0        0        0  9373310 1985-10-26 08:15:00.000000 package/test/template/large-sample-template
+-rw-r--r--   0        0        0      125 1985-10-26 08:15:00.000000 package/lib/placeholder
+-rw-r--r--   0        0        0       26 1985-10-26 08:15:00.000000 package/test/template/sample-template
+-rw-r--r--   0        0        0  9373310 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/asset.122da676fba68619def0d539ff80855eaa0ba3686fb37faa298ce277c4feb8f8
+-rw-r--r--   0        0        0      125 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/asset.7dbcd6245c5c6f70da313d31e9bd533af2214c565d855fb2f669666e927c125e
+-rw-r--r--   0        0        0      125 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/asset.7dbcd6245c5c6f70da313d31e9bd533af2214c565d855fb2f669666e927c125e
+-rw-r--r--   0        0        0       26 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/asset.97cd237b0ae069fe0711bcc6a711e213fdaf0956421de5b964de9ccd0d2b23a1
+-rw-r--r--   0        0        0     2457 1985-10-26 08:15:00.000000 package/index.js
+-rw-r--r--   0        0        0    18035 1985-10-26 08:15:00.000000 package/lib/key-policy-updater-custom-resource/index.js
+-rw-r--r--   0        0        0     8860 1985-10-26 08:15:00.000000 package/lib/template-writer-custom-resource/index.js
+-rw-r--r--   0        0        0     8860 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/asset.b1223f33e5124fdec3dc7988012c02ed49e285da9c1b8bcd2ce2d2c7c5d09ee7/index.js
+-rw-r--r--   0        0        0     8860 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/asset.b1223f33e5124fdec3dc7988012c02ed49e285da9c1b8bcd2ce2d2c7c5d09ee7/index.js
+-rw-r--r--   0        0        0     5051 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js
+-rw-r--r--   0        0        0     7032 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js
+-rw-r--r--   0        0        0     9748 1985-10-26 08:15:00.000000 package/lib/key-policy-updater.js
+-rw-r--r--   0        0        0    23955 1985-10-26 08:15:00.000000 package/test/kms-key-policy-updater.test.js
+-rw-r--r--   0        0        0    15953 1985-10-26 08:15:00.000000 package/lib/template-writer.js
+-rw-r--r--   0        0        0     8607 1985-10-26 08:15:00.000000 package/test/template-writer.test.js
+-rw-r--r--   0        0        0     4712 1985-10-26 08:15:00.000000 package/lib/utils.js
+-rw-r--r--   0        0        0      111 1985-10-26 08:15:00.000000 package/integ.config.json
+-rw-r--r--   0        0        0      346 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/integ.json
+-rw-r--r--   0        0        0      369 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/integ.json
+-rw-r--r--   0        0        0     6511 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/manifest.json
+-rw-r--r--   0        0        0     6661 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/manifest.json
+-rw-r--r--   0        0        0     2626 1985-10-26 08:15:00.000000 package/package.json
+-rw-r--r--   0        0        0     3330 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/template-writer-from-asset.assets.json
+-rw-r--r--   0        0        0    10535 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/template-writer-from-asset.template.json
+-rw-r--r--   0        0        0     3336 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/template-writer-from-large-asset.assets.json
+-rw-r--r--   0        0        0    10800 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/template-writer-from-large-asset.template.json
+-rw-r--r--   0        0        0      703 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/templatewriterfromassetIntegDefaultTestDeployAssert3AE00E9B.assets.json
+-rw-r--r--   0        0        0      770 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/templatewriterfromassetIntegDefaultTestDeployAssert3AE00E9B.template.json
+-rw-r--r--   0        0        0      708 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/templatewriterfromlargeassetIntegDefaultTestDeployAssertA02D2FEC.assets.json
+-rw-r--r--   0        0        0      770 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/templatewriterfromlargeassetIntegDefaultTestDeployAssertA02D2FEC.template.json
+-rw-r--r--   0        0        0    29166 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/tree.json
+-rw-r--r--   0        0        0    29505 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/tree.json
+-rw-r--r--   0        0        0     1553 1985-10-26 08:15:00.000000 package/README.md
+-rw-r--r--   0        0        0       20 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/cdk.out
+-rw-r--r--   0        0        0       20 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/cdk.out
+-rw-r--r--   0        0        0      665 1985-10-26 08:15:00.000000 package/index.d.ts
+-rw-r--r--   0        0        0     1507 1985-10-26 08:15:00.000000 package/lib/key-policy-updater-custom-resource/index.d.ts
+-rw-r--r--   0        0        0      807 1985-10-26 08:15:00.000000 package/lib/template-writer-custom-resource/index.d.ts
+-rw-r--r--   0        0        0      807 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.js.snapshot/asset.b1223f33e5124fdec3dc7988012c02ed49e285da9c1b8bcd2ce2d2c7c5d09ee7/index.d.ts
+-rw-r--r--   0        0        0      807 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.js.snapshot/asset.b1223f33e5124fdec3dc7988012c02ed49e285da9c1b8bcd2ce2d2c7c5d09ee7/index.d.ts
+-rw-r--r--   0        0        0      595 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-asset.d.ts
+-rw-r--r--   0        0        0      595 1985-10-26 08:15:00.000000 package/test/integ.template-writer-from-large-asset.d.ts
+-rw-r--r--   0        0        0     1333 1985-10-26 08:15:00.000000 package/lib/key-policy-updater.d.ts
+-rw-r--r--   0        0        0      595 1985-10-26 08:15:00.000000 package/test/kms-key-policy-updater.test.d.ts
+-rw-r--r--   0        0        0     2833 1985-10-26 08:15:00.000000 package/lib/template-writer.d.ts
+-rw-r--r--   0        0        0      595 1985-10-26 08:15:00.000000 package/test/template-writer.test.d.ts
+-rw-r--r--   0        0        0      738 1985-10-26 08:15:00.000000 package/lib/utils.d.ts
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+gzip compressed data, max compression
```

### filetype from diffoscope

```diff
@@ -1 +1 @@
-TarFile
+GzipFile
```
