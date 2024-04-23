# Comparing `tmp/runseq-0.0.4.tar.gz` & `tmp/runseq-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "runseq-0.0.4.tar", last modified: Tue Apr 23 15:47:55 2024, max compression
+gzip compressed data, was "runseq-0.1.0.tar", last modified: Tue Apr 23 23:20:35 2024, max compression
```

## Comparing `runseq-0.0.4.tar` & `runseq-0.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 15:47:55.083387 runseq-0.0.4/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.0.4/LICENSE
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43120 2024-04-23 15:47:55.083387 runseq-0.0.4/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2249 2024-04-23 15:46:52.000000 runseq-0.0.4/README.md
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-04-23 15:47:37.000000 runseq-0.0.4/pyproject.toml
-drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 15:47:55.083387 runseq-0.0.4/runseq.egg-info/
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43120 2024-04-23 15:47:55.000000 runseq-0.0.4/runseq.egg-info/PKG-INFO
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-04-23 15:47:55.000000 runseq-0.0.4/runseq.egg-info/SOURCES.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-04-23 15:47:55.000000 runseq-0.0.4/runseq.egg-info/dependency_links.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-04-23 15:47:55.000000 runseq-0.0.4/runseq.egg-info/entry_points.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-04-23 15:47:55.000000 runseq-0.0.4/runseq.egg-info/top_level.txt
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)     4445 2024-04-23 15:15:09.000000 runseq-0.0.4/runseq.py
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:47:55.083387 runseq-0.0.4/setup.cfg
--rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.0.4/setup.py
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 23:20:35.199044 runseq-0.1.0/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    35149 2024-04-23 13:58:13.000000 runseq-0.1.0/LICENSE
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43112 2024-04-23 23:20:35.199044 runseq-0.1.0/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     2241 2024-04-23 15:48:32.000000 runseq-0.1.0/README.md
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      469 2024-04-23 23:19:33.000000 runseq-0.1.0/pyproject.toml
+drwxr-xr-x   0 lgomes    (1000) lgomes    (1000)        0 2024-04-23 23:20:35.199044 runseq-0.1.0/runseq.egg-info/
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)    43112 2024-04-23 23:20:35.000000 runseq-0.1.0/runseq.egg-info/PKG-INFO
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)      216 2024-04-23 23:20:35.000000 runseq-0.1.0/runseq.egg-info/SOURCES.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        1 2024-04-23 23:20:35.000000 runseq-0.1.0/runseq.egg-info/dependency_links.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       39 2024-04-23 23:20:35.000000 runseq-0.1.0/runseq.egg-info/entry_points.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)        7 2024-04-23 23:20:35.000000 runseq-0.1.0/runseq.egg-info/top_level.txt
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)     4352 2024-04-23 23:19:56.000000 runseq-0.1.0/runseq.py
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 23:20:35.199044 runseq-0.1.0/setup.cfg
+-rw-r--r--   0 lgomes    (1000) lgomes    (1000)       38 2024-04-23 15:30:44.000000 runseq-0.1.0/setup.py
```

### Comparing `runseq-0.0.4/LICENSE` & `runseq-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `runseq-0.0.4/PKG-INFO` & `runseq-0.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.0.4
+Version: 0.1.0
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,16 +685,16 @@
 
 # runseq
 
 **Simple** job manager to run jobs sequentially in a Linux machine.
 
 This simple command line tool was created to solve a problem similar to the ones described here:
 
-    - https://stackoverflow.com/questions/72365506/how-to-change-a-sequence-of-bash-commands-while-running
-    - https://stackoverflow.com/questions/70946428/what-is-the-simplest-queue-job-manager-for-linux
+- https://stackoverflow.com/questions/72365506/how-to-change-a-sequence-of-bash-commands-while-running
+- https://stackoverflow.com/questions/70946428/what-is-the-simplest-queue-job-manager-for-linux
 
 Specifically, I wanted a way to execute long processing jobs sequentially and be able to modify the queue of upcomming jobs while a job was running.
 
 ## usage
 
 Using `--help` will show the tool usage:
```

### Comparing `runseq-0.0.4/README.md` & `runseq-0.1.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # runseq
 
 **Simple** job manager to run jobs sequentially in a Linux machine.
 
 This simple command line tool was created to solve a problem similar to the ones described here:
 
-    - https://stackoverflow.com/questions/72365506/how-to-change-a-sequence-of-bash-commands-while-running
-    - https://stackoverflow.com/questions/70946428/what-is-the-simplest-queue-job-manager-for-linux
+- https://stackoverflow.com/questions/72365506/how-to-change-a-sequence-of-bash-commands-while-running
+- https://stackoverflow.com/questions/70946428/what-is-the-simplest-queue-job-manager-for-linux
 
 Specifically, I wanted a way to execute long processing jobs sequentially and be able to modify the queue of upcomming jobs while a job was running.
 
 ## usage
 
 Using `--help` will show the tool usage:
```

### Comparing `runseq-0.0.4/runseq.egg-info/PKG-INFO` & `runseq-0.1.0/runseq.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: runseq
-Version: 0.0.4
+Version: 0.1.0
 Summary: Simple job manager to run jobs sequentially in a Linux machine.
 Author-email: Luís Gomes <luismsgomes@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -685,16 +685,16 @@
 
 # runseq
 
 **Simple** job manager to run jobs sequentially in a Linux machine.
 
 This simple command line tool was created to solve a problem similar to the ones described here:
 
-    - https://stackoverflow.com/questions/72365506/how-to-change-a-sequence-of-bash-commands-while-running
-    - https://stackoverflow.com/questions/70946428/what-is-the-simplest-queue-job-manager-for-linux
+- https://stackoverflow.com/questions/72365506/how-to-change-a-sequence-of-bash-commands-while-running
+- https://stackoverflow.com/questions/70946428/what-is-the-simplest-queue-job-manager-for-linux
 
 Specifically, I wanted a way to execute long processing jobs sequentially and be able to modify the queue of upcomming jobs while a job was running.
 
 ## usage
 
 Using `--help` will show the tool usage:
```

### Comparing `runseq-0.0.4/runseq.py` & `runseq-0.1.0/runseq.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,19 +6,14 @@
 import subprocess
 import sys
 import time
 
 from datetime import datetime
 
 
-__version__ = "0.0.2"
-__author__ = "Luís Gomes"
-__author_email__ = "luismsgomes@gmail.com"
-
-
 DB_PATH = os.environ.get("RUNSEQ_DB", "runseq.sqlite3")
 
 
 def db_connect():
     con = sqlite3.connect(DB_PATH)
     con.execute(
         "CREATE TABLE IF NOT EXISTS jobs("
@@ -136,15 +131,15 @@
         run_jobs()
     elif args.action == "add":
         command = " ".join([args.command] + args.args)
         add_job(priority=args.priority, command=command)
     elif args.action in ["list", "ls"]:
         list_jobs()
     elif args.action in ["remove", "rm"]:
-        remove_job(args.jobid)
+        remove_job(args.job_id)
     else:
         print("invalid action:", args.action, file=sys.stderr)
         sys.exit(2)
 
 
 if __name__ == "__main__":
     main()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

