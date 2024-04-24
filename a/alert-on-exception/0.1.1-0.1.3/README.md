# Comparing `tmp/alert_on_exception-0.1.1.tar.gz` & `tmp/alert_on_exception-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alert_on_exception-0.1.1.tar", last modified: Wed Apr 24 10:17:35 2024, max compression
+gzip compressed data, was "alert_on_exception-0.1.3.tar", last modified: Wed Apr 24 11:08:22 2024, max compression
```

## Comparing `alert_on_exception-0.1.1.tar` & `alert_on_exception-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,13 @@
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/
--rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.1/LICENSE
--rw-r--r--   0 user1     (1001) user1     (1001)     1100 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      864 2024-04-24 09:58:41.000000 alert_on_exception-0.1.1/README.md
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/alert_on_exception.egg-info/
--rw-r--r--   0 user1     (1001) user1     (1001)     1100 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/PKG-INFO
--rw-rw-r--   0 user1     (1001) user1     (1001)      292 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/SOURCES.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/dependency_links.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)       14 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/requires.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)        4 2024-04-24 10:17:35.000000 alert_on_exception-0.1.1/alert_on_exception.egg-info/top_level.txt
--rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.1/pyproject.toml
--rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/setup.cfg
--rw-rw-r--   0 user1     (1001) user1     (1001)      652 2024-04-24 10:17:30.000000 alert_on_exception-0.1.1/setup.py
-drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 10:17:35.272564 alert_on_exception-0.1.1/src/
--rw-rw-r--   0 user1     (1001) user1     (1001)       49 2024-04-24 09:54:19.000000 alert_on_exception-0.1.1/src/__init__.py
--rw-rw-r--   0 user1     (1001) user1     (1001)      987 2024-04-24 09:54:22.000000 alert_on_exception-0.1.1/src/alert_on_exception.py
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 11:08:22.186065 alert_on_exception-0.1.3/
+-rw-rw-r--   0 user1     (1001) user1     (1001)     1112 2024-04-24 09:35:45.000000 alert_on_exception-0.1.3/LICENSE
+-rw-r--r--   0 user1     (1001) user1     (1001)     1095 2024-04-24 11:08:22.186065 alert_on_exception-0.1.3/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      859 2024-04-24 11:06:44.000000 alert_on_exception-0.1.3/README.md
+drwxrwxr-x   0 user1     (1001) user1     (1001)        0 2024-04-24 11:08:22.186065 alert_on_exception-0.1.3/alert_on_exception.egg-info/
+-rw-r--r--   0 user1     (1001) user1     (1001)     1095 2024-04-24 11:08:22.000000 alert_on_exception-0.1.3/alert_on_exception.egg-info/PKG-INFO
+-rw-rw-r--   0 user1     (1001) user1     (1001)      250 2024-04-24 11:08:22.000000 alert_on_exception-0.1.3/alert_on_exception.egg-info/SOURCES.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-24 11:08:22.000000 alert_on_exception-0.1.3/alert_on_exception.egg-info/dependency_links.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)       14 2024-04-24 11:08:22.000000 alert_on_exception-0.1.3/alert_on_exception.egg-info/requires.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)        1 2024-04-24 11:08:22.000000 alert_on_exception-0.1.3/alert_on_exception.egg-info/top_level.txt
+-rw-rw-r--   0 user1     (1001) user1     (1001)       90 2024-04-24 09:33:49.000000 alert_on_exception-0.1.3/pyproject.toml
+-rw-rw-r--   0 user1     (1001) user1     (1001)       38 2024-04-24 11:08:22.186065 alert_on_exception-0.1.3/setup.cfg
+-rw-rw-r--   0 user1     (1001) user1     (1001)      652 2024-04-24 11:06:46.000000 alert_on_exception-0.1.3/setup.py
```

### Comparing `alert_on_exception-0.1.1/LICENSE` & `alert_on_exception-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `alert_on_exception-0.1.1/PKG-INFO` & `alert_on_exception-0.1.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert_on_exception
-Version: 0.1.1
+Version: 0.1.3
 Summary: A Python package to alert users about exceptions.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv
 
 # AlertOnException
@@ -19,24 +19,24 @@
 
 
 ## Installation
 
 Install using below pip command
 
 ```bash
-pip install alert_on_exception
+pip install alert-on-exception
 ```
 
 
 To use ExceptionNotifier, you need to configure it with your SMTP details and the recipient's information. Here's a quick example:
 
 
 ```bash
-from alert_on_exception import AlertOnException
+from alert_on_exception import alert
 
 # Create an instance of ExceptionNotifier
-notifier = AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
+notifier = alert.AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
 
 # Send a notification
 notifier.send_notification()
 
 ```
```

### Comparing `alert_on_exception-0.1.1/README.md` & `alert_on_exception-0.1.3/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -10,24 +10,24 @@
 
 
 ## Installation
 
 Install using below pip command
 
 ```bash
-pip install alert_on_exception
+pip install alert-on-exception
 ```
 
 
 To use ExceptionNotifier, you need to configure it with your SMTP details and the recipient's information. Here's a quick example:
 
 
 ```bash
-from alert_on_exception import AlertOnException
+from alert_on_exception import alert
 
 # Create an instance of ExceptionNotifier
-notifier = AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
+notifier = alert.AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
 
 # Send a notification
 notifier.send_notification()
 
 ```
```

### Comparing `alert_on_exception-0.1.1/alert_on_exception.egg-info/PKG-INFO` & `alert_on_exception-0.1.3/alert_on_exception.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: alert_on_exception
-Version: 0.1.1
+Version: 0.1.3
 Summary: A Python package to alert users about exceptions.
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: python-dotenv
 
 # AlertOnException
@@ -19,24 +19,24 @@
 
 
 ## Installation
 
 Install using below pip command
 
 ```bash
-pip install alert_on_exception
+pip install alert-on-exception
 ```
 
 
 To use ExceptionNotifier, you need to configure it with your SMTP details and the recipient's information. Here's a quick example:
 
 
 ```bash
-from alert_on_exception import AlertOnException
+from alert_on_exception import alert
 
 # Create an instance of ExceptionNotifier
-notifier = AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
+notifier = alert.AlertOnException("receiver@example.com", "Application Error", "An error has occurred!")
 
 # Send a notification
 notifier.send_notification()
 
 ```
```

### Comparing `alert_on_exception-0.1.1/setup.py` & `alert_on_exception-0.1.3/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 # Read the contents of your README file
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 setup(
     name="alert_on_exception",
-    version="0.1.1",
+    version="0.1.3",
     packages=find_packages(),
     install_requires=[
         "python-dotenv",  # List of packages required
     ],
     python_requires=">=3.6",
     description="A Python package to alert users about exceptions.",  # Short, concise description
     long_description=long_description,  # Detailed description
```

