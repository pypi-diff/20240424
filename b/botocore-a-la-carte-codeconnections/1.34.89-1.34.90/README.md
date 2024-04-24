# Comparing `tmp/botocore-a-la-carte-codeconnections-1.34.89.tar.gz` & `tmp/botocore_a_la_carte_codeconnections-1.34.90-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-codeconnections-1.34.89.tar", last modified: Tue Apr 23 01:01:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```
