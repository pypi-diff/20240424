# Comparing `tmp/kuzu-0.3.3.dev44.tar.gz` & `tmp/kuzu-0.3.3.dev45-cp38-cp38-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kuzu-0.3.3.dev44.tar", last modified: Tue Apr 23 08:04:37 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

