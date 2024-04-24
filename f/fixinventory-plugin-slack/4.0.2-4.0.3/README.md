# Comparing `tmp/fixinventory-plugin-slack-4.0.2.tar.gz` & `tmp/fixinventory_plugin_slack-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fixinventory-plugin-slack-4.0.2.tar", last modified: Fri Apr 12 12:17:55 2024, max compression
+gzip compressed data, was "fixinventory_plugin_slack-4.0.3.tar", last modified: Wed Apr 24 10:35:45 2024, max compression
```

## Comparing `fixinventory-plugin-slack-4.0.2.tar` & `fixinventory_plugin_slack-4.0.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.833978 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/
--rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/fix_plugin_slack/resources.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-12 12:16:06.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-12 12:17:55.000000 fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-12 12:17:55.837978 fixinventory-plugin-slack-4.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-12 12:14:47.000000 fixinventory-plugin-slack-4.0.2/test/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:35:45.910831 fixinventory_plugin_slack-4.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-24 10:32:49.000000 fixinventory_plugin_slack-4.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 10:35:45.910831 fixinventory_plugin_slack-4.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-24 10:32:49.000000 fixinventory_plugin_slack-4.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:35:45.910831 fixinventory_plugin_slack-4.0.3/fix_plugin_slack/
+-rw-r--r--   0 runner    (1001) docker     (127)    11688 2024-04-24 10:32:49.000000 fixinventory_plugin_slack-4.0.3/fix_plugin_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-24 10:32:49.000000 fixinventory_plugin_slack-4.0.3/fix_plugin_slack/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10615 2024-04-24 10:32:49.000000 fixinventory_plugin_slack-4.0.3/fix_plugin_slack/resources.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:35:45.910831 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1053 2024-04-24 10:35:45.000000 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-24 10:35:45.000000 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:35:45.000000 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-24 10:35:45.000000 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 10:33:57.000000 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-24 10:35:45.000000 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-24 10:35:45.000000 fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1369 2024-04-24 10:32:49.000000 fixinventory_plugin_slack-4.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-04-24 10:35:45.910831 fixinventory_plugin_slack-4.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 10:35:45.910831 fixinventory_plugin_slack-4.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-24 10:32:49.000000 fixinventory_plugin_slack-4.0.3/test/test_config.py
```

### Comparing `fixinventory-plugin-slack-4.0.2/PKG-INFO` & `fixinventory_plugin_slack-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-slack
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Slack Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: slack-sdk
 Requires-Dist: retrying
 
 # fix-plugin-slack
 Slack collector for Fix
 
 ## License
```

### Comparing `fixinventory-plugin-slack-4.0.2/fix_plugin_slack/__init__.py` & `fixinventory_plugin_slack-4.0.3/fix_plugin_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-slack-4.0.2/fix_plugin_slack/resources.py` & `fixinventory_plugin_slack-4.0.3/fix_plugin_slack/resources.py`

 * *Files identical despite different names*

### Comparing `fixinventory-plugin-slack-4.0.2/fixinventory_plugin_slack.egg-info/PKG-INFO` & `fixinventory_plugin_slack-4.0.3/fixinventory_plugin_slack.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fixinventory-plugin-slack
-Version: 4.0.2
+Version: 4.0.3
 Summary: Fix Slack Plugin
 Author: Some Engineering Inc.
 License: AGPLv3
 Project-URL: Documentation, https://inventory.fix.security
 Project-URL: Source, https://github.com/someengineering/fix/tree/main/plugins/slack
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
@@ -15,15 +15,15 @@
 Classifier: Operating System :: Unix
 Classifier: Environment :: Console
 Classifier: Natural Language :: English
 Classifier: Topic :: Security
 Classifier: Topic :: Utilities
 Requires-Python: >=3.11
 Description-Content-Type: text/markdown
-Requires-Dist: fixinventorylib==4.0.2
+Requires-Dist: fixinventorylib==4.0.3
 Requires-Dist: slack-sdk
 Requires-Dist: retrying
 
 # fix-plugin-slack
 Slack collector for Fix
 
 ## License
```

### Comparing `fixinventory-plugin-slack-4.0.2/pyproject.toml` & `fixinventory_plugin_slack-4.0.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [project]
 name = "fixinventory-plugin-slack"
 description = "Fix Slack Plugin"
-version = "4.0.2"
+version = "4.0.3"
 authors = [{name="Some Engineering Inc."}]
 license = { text="AGPLv3" }
 requires-python = ">=3.11"
 classifiers = [
     # Current project status
     "Development Status :: 4 - Beta",
     # Audience
@@ -23,15 +23,15 @@
     "Natural Language :: English",
     "Topic :: Security",
     "Topic :: Utilities",
 ]
 readme = {file="README.md", content-type="text/markdown"}
 
 dependencies = [
-    "fixinventorylib==4.0.2",
+    "fixinventorylib==4.0.3",
     "slack-sdk",
     "retrying",
 ]
 
 [project.entry-points."fix.plugins"]
 slack_bot = "fix_plugin_slack:SlackBotPlugin"
 slack_collector = "fix_plugin_slack:SlackCollectorPlugin"
```

