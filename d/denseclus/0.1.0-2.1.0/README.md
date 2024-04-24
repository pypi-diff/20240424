# Comparing `tmp/denseclus-0.1.0.tar.gz` & `tmp/denseclus-2.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "denseclus-0.1.0.tar", last modified: Wed Apr 24 18:37:56 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

