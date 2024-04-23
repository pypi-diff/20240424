# Comparing `tmp/fudstop-2.5.3.tar.gz` & `tmp/fudstop-2.5.5-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fudstop-2.5.3.tar", last modified: Tue Apr 16 09:03:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

