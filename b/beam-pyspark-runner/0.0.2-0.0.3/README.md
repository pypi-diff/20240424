# Comparing `tmp/beam_pyspark_runner-0.0.2.tar.gz` & `tmp/beam_pyspark_runner-0.0.3-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "beam_pyspark_runner-0.0.2.tar", last modified: Tue Apr 23 15:32:27 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

