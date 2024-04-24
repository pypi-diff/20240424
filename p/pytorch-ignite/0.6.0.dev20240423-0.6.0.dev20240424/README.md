# Comparing `tmp/pytorch-ignite-0.6.0.dev20240423.tar.gz` & `tmp/pytorch_ignite-0.6.0.dev20240424-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytorch-ignite-0.6.0.dev20240423.tar", last modified: Tue Apr 23 00:13:32 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

