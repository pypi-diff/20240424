# Comparing `tmp/shelltool-0.1.2.tar.gz` & `tmp/shelltool-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shelltool-0.1.2.tar", last modified: Sun Apr 21 07:45:41 2024, max compression
+gzip compressed data, was "shelltool-0.2.2.tar", last modified: Tue Apr 23 22:28:31 2024, max compression
```

## Comparing `shelltool-0.1.2.tar` & `shelltool-0.2.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-04-21 07:45:41.101956 shelltool-0.1.2/
--rw-rw-rw-   0        0        0     1070 2024-04-21 05:33:02.000000 shelltool-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     6298 2024-04-21 07:45:41.100959 shelltool-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     5772 2024-04-21 07:43:52.000000 shelltool-0.1.2/README.md
--rw-rw-rw-   0        0        0      593 2024-04-21 07:45:32.000000 shelltool-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-21 07:45:41.101956 shelltool-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-21 07:45:41.099960 shelltool-0.1.2/shelltool.egg-info/
--rw-rw-rw-   0        0        0     6298 2024-04-21 07:45:41.000000 shelltool-0.1.2/shelltool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      177 2024-04-21 07:45:41.000000 shelltool-0.1.2/shelltool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-21 07:45:41.000000 shelltool-0.1.2/shelltool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2024-04-21 07:45:41.000000 shelltool-0.1.2/shelltool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4957 2024-04-21 07:42:24.000000 shelltool-0.1.2/shelltool.py
+drwxrwxrwx   0        0        0        0 2024-04-23 22:28:31.074418 shelltool-0.2.2/
+-rw-rw-rw-   0        0        0     1070 2024-04-21 05:33:02.000000 shelltool-0.2.2/LICENSE
+-rw-rw-rw-   0        0        0     8855 2024-04-23 22:28:31.072419 shelltool-0.2.2/PKG-INFO
+-rw-rw-rw-   0        0        0     8329 2024-04-23 22:27:07.000000 shelltool-0.2.2/README.md
+-rw-rw-rw-   0        0        0      593 2024-04-23 22:27:57.000000 shelltool-0.2.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-23 22:28:31.074418 shelltool-0.2.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-23 22:28:31.072419 shelltool-0.2.2/shelltool.egg-info/
+-rw-rw-rw-   0        0        0     8855 2024-04-23 22:28:31.000000 shelltool-0.2.2/shelltool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      177 2024-04-23 22:28:31.000000 shelltool-0.2.2/shelltool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-23 22:28:31.000000 shelltool-0.2.2/shelltool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2024-04-23 22:28:31.000000 shelltool-0.2.2/shelltool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     9961 2024-04-23 22:09:48.000000 shelltool-0.2.2/shelltool.py
```

### Comparing `shelltool-0.1.2/LICENSE` & `shelltool-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `shelltool-0.1.2/PKG-INFO` & `shelltool-0.2.2/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: shelltool
-Version: 0.1.2
-Summary: A better way to compose shell-like commands in python.
-Author: William L.
-Project-URL: Homepage, https://github.com/FrewtyPebbles/Shellify.py
-Project-URL: Issues, https://github.com/FrewtyPebbles/Shellify.py/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.10
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Shelltool
 
 Shelltool is an api that makes dealing with and composing subprocesses in python easier, more readable, and more immediately useful.  It accomplishes this by utilizing syntax that makes it feel more like composing procedures in Bash rather than dealing with things like `Popen` or `Thread(target=lambda:subprocess.run())`.
 
 Heres an example of the syntax.  
 ```py
 if __name__ == "__main__":
@@ -117,24 +103,24 @@
 ```py
 cat_to_grep_cmd = SHELL.SHELL() @ SHELL.grep("SHELL")
 cat_to_grep_cmd.run()
 
 print(cat_to_grep_cmd.stdout.decode())
 ```
 
-## The Tilda Operator
+## The Tilde Operator
 
 `~`
 
-The *Tilda* operator runs the supplied process on a separate thread:
+The *Tilde* operator runs the supplied process on a separate thread:
 
 ```py
 # Lets pretend we need to run a slow subprocess.
 
-# By just adding a tilda, we can instantly move this subprocess to a separate concurrent thread.
+# By just adding a tilde, we can instantly move this subprocess to a separate concurrent thread.
 cat_to_grep_cmd = ~(SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
 
 # Now lets run our slow subprocess/spawn our thread.
 cat_to_grep_cmd.run()
 
 # Now that our process is happening off of the main thread we can do other computations while we wait for it to finish
 while cat_to_grep_cmd.running:
@@ -142,14 +128,83 @@
     print(f"Currently doing concurrent tasks while running subprocess with pid: {cat_to_grep_cmd.pid}")
 
 # Finally we've finished our other tasks, so lets get our long awaited stdout and stderr data from our subprocess.  Accessing either stdout or stderr on our process will join our thread back to its spawning thread, or in this case the main thread.
 print(cat_to_grep_cmd.stdout.decode())
 print(cat_to_grep_cmd.stderr.decode())
 ```
 
+## The & Operator
+
+`&`
+
+The *&* operator runs process on its left hand side before its process on its right hand side:
+
+```py
+cat_to_grep_cmd = ~(SHELL.sleep(5) & SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
+# This will sleep 5 seconds before calling `cat ./shelltool.py | grep shell`
+
+cat_to_grep_cmd.run()
+
+# Now we can do some other tasks while the the terminal is sleeping then cat-ing to grep-ing
+while cat_to_grep_cmd.running:
+    # do some other tasks...
+    print(f"Currently doing concurrent tasks while running subprocess with pid: {cat_to_grep_cmd.pid}")
+
+# Finally we've finished our other tasks, so lets get our long awaited stdout and stderr data from our subprocess.  Accessing either stdout or stderr on our process will join our thread back to its spawning thread, or in this case the main thread.
+print(cat_to_grep_cmd.stdout.decode())
+print(cat_to_grep_cmd.stderr.decode())
+```
+
+## But how do I get my stdout and stderr as my program runs?
+
+`process_variable.next_stream_line()`
+
+`.next_stream_line()` grabs the next line of stdout and stderr as they are emitted from the process in real time.  It returns these lines as a tuple of bytes `(stdout:bytes | None, stderr:bytes | None)`.  You can check if there are any available lines of stdout and stderr from your process with the boolean property `process.stream_empty`.
+
+example:
+
+Lets say we have the following python program `test.py`:
+
+```py
+from time import sleep
+import sys
+for i in range(10):
+    if i % 2 == 0:
+        print(i, file=sys.stderr)
+    else:
+        print(i)
+    sleep(0.5)
+```
+
+Now here is our code running our python program:
+
+```py
+process = ~(SHELL.python("-u", "test.py"))
+# This runs test.py with unbuffered writes to IO
+
+process.run()
+
+while process.running or not process.stream_empty:
+    # while the process is running or there are stdouts and stderrs left from our process.
+
+    out, err = process.next_stream_line() #grab any potential incoming stdout and stderr
+
+    if out: # if stdout line is not none:
+        print(f"PROCESS RUNNING: {process.running}")
+        sys.stdout.write(f"out:\n{out.decode()}")
+
+    if err: # if stderr line is not none:
+        print(f"PROCESS RUNNING: {process.running}")
+        sys.stdout.write(f"err:\n{err.decode()}")
+```
+
+***Incase anyone needs to know***: 
+
+This function itterates to the next output buffer in the stream.  So if you want to itterate through each write to the stdout, you will need to make sure your writes are unbuffered.
+
 ## Help! My subprocess is out of controll! (How to Kill Your Subprocess) 
 
 Killing your rogue subprocess is as simple as `.kill()`.
 
 ```py
 cat_to_grep_cmd = ~(SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
 cat_to_grep_cmd.run()
@@ -194,8 +249,8 @@
 process, process_err = ~((p1 := (SHELL.echo("SHELL") | SHELL.tee("/dev/stderr"))) | SHELL.grep("SHELL")), ~(p1 @ SHELL.grep("SHELL"))
 p1.run()
 process.run()
 process_err.run()
 
 print(f"p_out:\n{process.stdout.decode()}")
 print(f"p_err:\n{process_err.stdout.decode()}")
-```
+```
```

### Comparing `shelltool-0.1.2/pyproject.toml` & `shelltool-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shelltool"
-version = "0.1.2"
+version = "0.2.2"
 authors = [
   { name="William L." },
 ]
 description = "A better way to compose shell-like commands in python."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `shelltool-0.1.2/shelltool.egg-info/PKG-INFO` & `shelltool-0.2.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shelltool
-Version: 0.1.2
+Version: 0.2.2
 Summary: A better way to compose shell-like commands in python.
 Author: William L.
 Project-URL: Homepage, https://github.com/FrewtyPebbles/Shellify.py
 Project-URL: Issues, https://github.com/FrewtyPebbles/Shellify.py/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -117,24 +117,24 @@
 ```py
 cat_to_grep_cmd = SHELL.SHELL() @ SHELL.grep("SHELL")
 cat_to_grep_cmd.run()
 
 print(cat_to_grep_cmd.stdout.decode())
 ```
 
-## The Tilda Operator
+## The Tilde Operator
 
 `~`
 
-The *Tilda* operator runs the supplied process on a separate thread:
+The *Tilde* operator runs the supplied process on a separate thread:
 
 ```py
 # Lets pretend we need to run a slow subprocess.
 
-# By just adding a tilda, we can instantly move this subprocess to a separate concurrent thread.
+# By just adding a tilde, we can instantly move this subprocess to a separate concurrent thread.
 cat_to_grep_cmd = ~(SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
 
 # Now lets run our slow subprocess/spawn our thread.
 cat_to_grep_cmd.run()
 
 # Now that our process is happening off of the main thread we can do other computations while we wait for it to finish
 while cat_to_grep_cmd.running:
@@ -142,14 +142,83 @@
     print(f"Currently doing concurrent tasks while running subprocess with pid: {cat_to_grep_cmd.pid}")
 
 # Finally we've finished our other tasks, so lets get our long awaited stdout and stderr data from our subprocess.  Accessing either stdout or stderr on our process will join our thread back to its spawning thread, or in this case the main thread.
 print(cat_to_grep_cmd.stdout.decode())
 print(cat_to_grep_cmd.stderr.decode())
 ```
 
+## The & Operator
+
+`&`
+
+The *&* operator runs process on its left hand side before its process on its right hand side:
+
+```py
+cat_to_grep_cmd = ~(SHELL.sleep(5) & SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
+# This will sleep 5 seconds before calling `cat ./shelltool.py | grep shell`
+
+cat_to_grep_cmd.run()
+
+# Now we can do some other tasks while the the terminal is sleeping then cat-ing to grep-ing
+while cat_to_grep_cmd.running:
+    # do some other tasks...
+    print(f"Currently doing concurrent tasks while running subprocess with pid: {cat_to_grep_cmd.pid}")
+
+# Finally we've finished our other tasks, so lets get our long awaited stdout and stderr data from our subprocess.  Accessing either stdout or stderr on our process will join our thread back to its spawning thread, or in this case the main thread.
+print(cat_to_grep_cmd.stdout.decode())
+print(cat_to_grep_cmd.stderr.decode())
+```
+
+## But how do I get my stdout and stderr as my program runs?
+
+`process_variable.next_stream_line()`
+
+`.next_stream_line()` grabs the next line of stdout and stderr as they are emitted from the process in real time.  It returns these lines as a tuple of bytes `(stdout:bytes | None, stderr:bytes | None)`.  You can check if there are any available lines of stdout and stderr from your process with the boolean property `process.stream_empty`.
+
+example:
+
+Lets say we have the following python program `test.py`:
+
+```py
+from time import sleep
+import sys
+for i in range(10):
+    if i % 2 == 0:
+        print(i, file=sys.stderr)
+    else:
+        print(i)
+    sleep(0.5)
+```
+
+Now here is our code running our python program:
+
+```py
+process = ~(SHELL.python("-u", "test.py"))
+# This runs test.py with unbuffered writes to IO
+
+process.run()
+
+while process.running or not process.stream_empty:
+    # while the process is running or there are stdouts and stderrs left from our process.
+
+    out, err = process.next_stream_line() #grab any potential incoming stdout and stderr
+
+    if out: # if stdout line is not none:
+        print(f"PROCESS RUNNING: {process.running}")
+        sys.stdout.write(f"out:\n{out.decode()}")
+
+    if err: # if stderr line is not none:
+        print(f"PROCESS RUNNING: {process.running}")
+        sys.stdout.write(f"err:\n{err.decode()}")
+```
+
+***Incase anyone needs to know***: 
+
+This function itterates to the next output buffer in the stream.  So if you want to itterate through each write to the stdout, you will need to make sure your writes are unbuffered.
+
 ## Help! My subprocess is out of controll! (How to Kill Your Subprocess) 
 
 Killing your rogue subprocess is as simple as `.kill()`.
 
 ```py
 cat_to_grep_cmd = ~(SHELL.cat("./shelltool.py") | SHELL.grep("SHELL"))
 cat_to_grep_cmd.run()
```

