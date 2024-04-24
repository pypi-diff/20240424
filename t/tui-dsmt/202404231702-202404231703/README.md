# Comparing `tmp/tui_dsmt-202404231702.tar.gz` & `tmp/tui_dsmt-202404231703-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tui_dsmt-202404231702.tar", last modified: Tue Apr 23 17:02:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

