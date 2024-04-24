# Comparing `tmp/pymongo-4.6.3.tar.gz` & `tmp/pymongo-4.7.0-cp39-cp39-macosx_11_0_arm64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/mci/d2be42a062e3cd5a7f67fb663e338d8c/src/dist/.tmp-qm_3jf2v/pymongo-4.6.3.tar", last modified: Thu Mar 28 00:30:17 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

