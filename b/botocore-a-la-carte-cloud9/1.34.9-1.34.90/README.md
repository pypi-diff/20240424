# Comparing `tmp/botocore-a-la-carte-cloud9-1.34.9.tar.gz` & `tmp/botocore_a_la_carte_cloud9-1.34.90-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-cloud9-1.34.9.tar", last modified: Thu Dec 28 01:06:34 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

