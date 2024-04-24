# Comparing `tmp/girder-jobs-3.2.4.dev7.tar.gz` & `tmp/girder-jobs-5.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "girder-jobs-3.2.4.dev7.tar", last modified: Wed Apr 24 19:13:29 2024, max compression
+gzip compressed data, was "girder-jobs-5.0.0a2.tar", last modified: Fri Apr 12 16:31:14 2024, max compression
```

## Comparing `girder-jobs-3.2.4.dev7.tar` & `girder-jobs-5.0.0a2.tar`

### file list

```diff
@@ -1,59 +1,29 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.914469 girder-jobs-3.2.4.dev7/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-04-24 19:13:29.910469 girder-jobs-3.2.4.dev7/PKG-INFO
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.902469 girder-jobs-3.2.4.dev7/girder_jobs/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1275 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2053 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     9199 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/job_rest.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.902469 girder-jobs-3.2.4.dev7/girder_jobs/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    23250 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/models/job.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.906469 girder-jobs-3.2.4.dev7/girder_jobs/web_client/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2922 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/JobStatus.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.906469 girder-jobs-3.2.4.dev7/girder_jobs/web_client/collections/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      227 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/collections/JobCollection.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       76 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/collections/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      220 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      253 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/main.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.906469 girder-jobs-3.2.4.dev7/girder_jobs/web_client/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1405 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/models/JobModel.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/models/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      642 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/package.json
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1195 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/routes.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.906469 girder-jobs-3.2.4.dev7/girder_jobs/web_client/stylesheets/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      403 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/stylesheets/jobDetailsWidget.styl
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1274 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/stylesheets/jobListWidget.styl
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.906469 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       61 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/adminViewMenuItem.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)       80 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/headerUserViewMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      290 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/jobCheckBoxContent.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      200 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/jobCheckBoxMenu.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2232 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/jobDetailsWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1940 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/jobList.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      880 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/jobListWidget.pug
--rw-r--r--   0 circleci  (1001) circleci  (1002)      174 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/templates/jobsGraphWidget.pug
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.910469 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      399 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/AdminView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2192 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/CheckBoxMenu.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      654 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/HeaderUserView.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4906 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/JobDetailsWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8414 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/JobGraphWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    12083 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/JobListWidget.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)      210 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/index.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8304 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/timeChartConfig.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    11782 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/girder_jobs/web_client/views/timingHistoryChartConfig.js
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.910469 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      613 2024-04-24 19:13:29.000000 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1802 2024-04-24 19:13:29.000000 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:29.000000 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-04-24 19:13:29.000000 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-24 19:13:29.000000 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-24 19:13:29.000000 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-04-24 19:13:29.000000 girder-jobs-3.2.4.dev7/girder_jobs.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/plugin.cmake
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:13:29.910469 girder-jobs-3.2.4.dev7/plugin_tests/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/plugin_tests/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    21567 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/plugin_tests/jobsSpec.js
--rw-r--r--   0 circleci  (1001) circleci  (1002)    24932 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/plugin_tests/jobs_test.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/plugin_tests/local_job_impl.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-24 19:13:29.914469 girder-jobs-3.2.4.dev7/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2024-04-24 19:11:47.000000 girder-jobs-3.2.4.dev7/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      138 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/PKG-INFO
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/girder_jobs/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1551 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/girder_jobs/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2053 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/girder_jobs/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9199 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/girder_jobs/job_rest.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/girder_jobs/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/girder_jobs/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    23109 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/girder_jobs/models/job.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:14.428818 girder-jobs-5.0.0a2/girder_jobs/web_client/
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/girder_jobs/web_client/dist/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   501838 2024-04-12 16:28:33.000000 girder-jobs-5.0.0a2/girder_jobs/web_client/dist/girder-plugin-jobs.umd.cjs
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1917 2024-04-12 16:28:32.000000 girder-jobs-5.0.0a2/girder_jobs/web_client/dist/style.css
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/girder_jobs.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      610 2024-04-12 16:31:14.000000 girder-jobs-5.0.0a2/girder_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      584 2024-04-12 16:31:14.000000 girder-jobs-5.0.0a2/girder_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:14.000000 girder-jobs-5.0.0a2/girder_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       46 2024-04-12 16:31:14.000000 girder-jobs-5.0.0a2/girder_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-04-12 16:31:14.000000 girder-jobs-5.0.0a2/girder_jobs.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       10 2024-04-12 16:31:14.000000 girder-jobs-5.0.0a2/girder_jobs.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2024-04-12 16:31:14.000000 girder-jobs-5.0.0a2/girder_jobs.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       49 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/plugin.cmake
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/plugin_tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/plugin_tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    24932 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/plugin_tests/jobs_test.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      156 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/plugin_tests/local_job_impl.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-04-12 16:31:14.432818 girder-jobs-5.0.0a2/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1667 2024-04-12 16:27:18.000000 girder-jobs-5.0.0a2/setup.py
```

### Comparing `girder-jobs-3.2.4.dev7/PKG-INFO` & `girder-jobs-5.0.0a2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-jobs
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: A general purpose plugin for managing offline jobs.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#jobs
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-jobs-3.2.4.dev7/girder_jobs/__init__.py` & `girder-jobs-5.0.0a2/girder_jobs/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import importlib
+from pathlib import Path
 
 from girder import events
-from girder.plugin import GirderPlugin
+from girder.plugin import GirderPlugin, registerPluginStaticContent
 from girder.utility.model_importer import ModelImporter
 
 from . import constants, job_rest
 from .models.job import Job
 
 
 def scheduleLocal(event):
@@ -26,13 +27,19 @@
         module = importlib.import_module(job['module'])
         fn = getattr(module, job.get('function', 'run'))
         fn(job)
 
 
 class JobsPlugin(GirderPlugin):
     DISPLAY_NAME = 'Jobs'
-    CLIENT_SOURCE_PATH = 'web_client'
 
     def load(self, info):
         ModelImporter.registerModel('job', Job, 'jobs')
         info['apiRoot'].job = job_rest.Job()
         events.bind('jobs.schedule', 'jobs', scheduleLocal)
+        registerPluginStaticContent(
+            plugin='jobs',
+            css=['/style.css'],
+            js=['/girder-plugin-jobs.umd.cjs'],
+            staticDir=Path(__file__).parent / 'web_client' / 'dist',
+            tree=info['serverRoot'],
+        )
```

### Comparing `girder-jobs-3.2.4.dev7/girder_jobs/constants.py` & `girder-jobs-5.0.0a2/girder_jobs/constants.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.4.dev7/girder_jobs/job_rest.py` & `girder-jobs-5.0.0a2/girder_jobs/job_rest.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.4.dev7/girder_jobs/models/job.py` & `girder-jobs-5.0.0a2/girder_jobs/models/job.py`

 * *Files 1% similar despite different names*

```diff
@@ -311,18 +311,15 @@
 
     def scheduleJob(self, job):
         """
         Trigger the event to schedule this job. Other plugins are in charge of
         actually scheduling and/or executing the job, except in the case when
         the handler is 'local'.
         """
-        if job.get('asynchronous', job.get('async')) is True:
-            events.daemon.trigger('jobs.schedule', info=job)
-        else:
-            events.trigger('jobs.schedule', info=job)
+        events.trigger('jobs.schedule', info=job)
 
     def createJobToken(self, job, days=7):
         """
         Create a token that can be used just for the management of an individual
         job, e.g. updating job info, progress, logs, status.
         """
         return Token().createToken(days=days, scope='jobs.job_' + str(job['_id']))
```

### Comparing `girder-jobs-3.2.4.dev7/girder_jobs.egg-info/PKG-INFO` & `girder-jobs-5.0.0a2/girder_jobs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: girder-jobs
-Version: 3.2.4.dev7
+Version: 5.0.0a2
 Summary: A general purpose plugin for managing offline jobs.
 Home-page: http://girder.readthedocs.io/en/latest/plugins.html#jobs
 Author: Kitware, Inc.
 Author-email: kitware@kitware.com
 License: Apache 2.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Web Environment
```

### Comparing `girder-jobs-3.2.4.dev7/plugin_tests/jobs_test.py` & `girder-jobs-5.0.0a2/plugin_tests/jobs_test.py`

 * *Files identical despite different names*

### Comparing `girder-jobs-3.2.4.dev7/setup.py` & `girder-jobs-5.0.0a2/setup.py`

 * *Files identical despite different names*

