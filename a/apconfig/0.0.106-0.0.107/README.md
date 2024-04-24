# Comparing `tmp/apconfig-0.0.106.tar.gz` & `tmp/apconfig-0.0.107.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apconfig-0.0.106.tar", max compression
+gzip compressed data, was "apconfig-0.0.107.tar", max compression
```

## Comparing `apconfig-0.0.106.tar` & `apconfig-0.0.107.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.106/README.md
--rw-r--r--   0        0        0     3140 2024-04-06 06:41:58.360388 apconfig-0.0.106/apconfig/__init__.py
--rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.106/apconfig/utilities.py
--rw-r--r--   0        0        0      305 2024-04-06 06:41:58.332388 apconfig-0.0.106/pyproject.toml
--rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.106/PKG-INFO
+-rw-r--r--   0        0        0        0 2024-03-27 10:34:40.761324 apconfig-0.0.107/README.md
+-rw-r--r--   0        0        0     3214 2024-04-24 10:30:10.717114 apconfig-0.0.107/apconfig/__init__.py
+-rw-r--r--   0        0        0      114 2024-04-05 10:57:51.982200 apconfig-0.0.107/apconfig/utilities.py
+-rw-r--r--   0        0        0      305 2024-04-24 10:33:04.202613 apconfig-0.0.107/pyproject.toml
+-rw-r--r--   0        0        0      389 1970-01-01 00:00:00.000000 apconfig-0.0.107/PKG-INFO
```

### Comparing `apconfig-0.0.106/apconfig/__init__.py` & `apconfig-0.0.107/apconfig/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -94,7 +94,10 @@
 
 # Chain Feeds and Symbols
 all_chain_feeds = setup_data["assets"]
 all_chain_symbols = setup_data["symbols"]
 
 active_feed = os.getenv("FEED")
 # assert active_feed in all_chain_feeds, f"Feed {active_feed} not found in setup data. "
+
+# TSO Stuff
+submit_time_buffer = setup_data['tso']['submit_time_buffer']
```

