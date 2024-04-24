# Comparing `tmp/MorphIO-3.3.7.tar.gz` & `tmp/morphio-3.3.8-cp312-cp312-manylinux_2_27_x86_64.manylinux_2_28_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MorphIO-3.3.7.tar", last modified: Mon Dec 11 12:13:07 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

