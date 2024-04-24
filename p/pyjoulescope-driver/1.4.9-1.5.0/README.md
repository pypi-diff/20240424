# Comparing `tmp/pyjoulescope_driver-1.4.9.tar.gz` & `tmp/pyjoulescope_driver-1.5.0-cp311-cp311-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjoulescope_driver-1.4.9.tar", last modified: Mon Mar 18 20:55:01 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

