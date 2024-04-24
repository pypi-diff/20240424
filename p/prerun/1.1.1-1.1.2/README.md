# Comparing `tmp/prerun-1.1.1.tar.gz` & `tmp/prerun-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prerun-1.1.1.tar", last modified: Wed Apr 17 00:07:19 2024, max compression
+gzip compressed data, was "prerun-1.1.2.tar", last modified: Wed Apr 24 05:10:38 2024, max compression
```

## Comparing `prerun-1.1.1.tar` & `prerun-1.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:07:19.712029 prerun-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-17 00:07:15.000000 prerun-1.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-17 00:07:19.712029 prerun-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-17 00:07:15.000000 prerun-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-17 00:07:15.000000 prerun-1.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 00:07:19.712029 prerun-1.1.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:07:19.708029 prerun-1.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:07:19.712029 prerun-1.1.1/src/prerun/
--rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-17 00:07:15.000000 prerun-1.1.1/src/prerun/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-17 00:07:15.000000 prerun-1.1.1/src/prerun/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-17 00:07:15.000000 prerun-1.1.1/src/prerun/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-17 00:07:15.000000 prerun-1.1.1/src/prerun/recv_bytes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5527 2024-04-17 00:07:15.000000 prerun-1.1.1/src/prerun/server.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-17 00:07:15.000000 prerun-1.1.1/src/prerun/sigint.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 00:07:19.712029 prerun-1.1.1/src/prerun.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-17 00:07:19.000000 prerun-1.1.1/src/prerun.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-17 00:07:19.000000 prerun-1.1.1/src/prerun.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 00:07:19.000000 prerun-1.1.1/src/prerun.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-17 00:07:19.000000 prerun-1.1.1/src/prerun.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-17 00:07:19.000000 prerun-1.1.1/src/prerun.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-17 00:07:19.000000 prerun-1.1.1/src/prerun.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:10:38.407529 prerun-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-24 05:10:33.000000 prerun-1.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-24 05:10:38.407529 prerun-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-24 05:10:33.000000 prerun-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      536 2024-04-24 05:10:33.000000 prerun-1.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 05:10:38.407529 prerun-1.1.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:10:38.403529 prerun-1.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:10:38.403529 prerun-1.1.2/src/prerun/
+-rw-r--r--   0 runner    (1001) docker     (127)      706 2024-04-24 05:10:33.000000 prerun-1.1.2/src/prerun/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-24 05:10:33.000000 prerun-1.1.2/src/prerun/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-04-24 05:10:33.000000 prerun-1.1.2/src/prerun/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      218 2024-04-24 05:10:33.000000 prerun-1.1.2/src/prerun/recv_bytes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6211 2024-04-24 05:10:33.000000 prerun-1.1.2/src/prerun/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-04-24 05:10:33.000000 prerun-1.1.2/src/prerun/sigint.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 05:10:38.407529 prerun-1.1.2/src/prerun.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-04-24 05:10:38.000000 prerun-1.1.2/src/prerun.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      372 2024-04-24 05:10:38.000000 prerun-1.1.2/src/prerun.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 05:10:38.000000 prerun-1.1.2/src/prerun.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-24 05:10:38.000000 prerun-1.1.2/src/prerun.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-24 05:10:38.000000 prerun-1.1.2/src/prerun.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-24 05:10:38.000000 prerun-1.1.2/src/prerun.egg-info/top_level.txt
```

### Comparing `prerun-1.1.1/LICENSE` & `prerun-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `prerun-1.1.1/PKG-INFO` & `prerun-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 1.1.1
+Version: 1.1.2
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

### Comparing `prerun-1.1.1/pyproject.toml` & `prerun-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "prerun"
-version = "1.1.1"
+version = "1.1.2"
 description = "Prerun"
 readme = "README.md"
 requires-python = ">=3.9"
 license = {file = "LICENSE"}
 keywords = ["development"]
 classifiers = [
   "Development Status :: 3 - Alpha",
```

### Comparing `prerun-1.1.1/src/prerun/__init__.py` & `prerun-1.1.2/src/prerun/__init__.py`

 * *Files identical despite different names*

### Comparing `prerun-1.1.1/src/prerun/client.py` & `prerun-1.1.2/src/prerun/client.py`

 * *Files identical despite different names*

### Comparing `prerun-1.1.1/src/prerun/server.py` & `prerun-1.1.2/src/prerun/server.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,32 +13,59 @@
 
 import psutil
 
 from .recv_bytes import recv_bytes
 from .sigint import sigint_defer, sigint_once
 
 
-def run_child(stdio, preloader, conn, files_to_close):
+def hide_stdout_stderr():
+    devnull_fd = os.open(os.devnull, os.O_WRONLY)
+
+    stdout_fd = sys.stdout.fileno()
+    stdout_fd2 = os.dup(stdout_fd)
+    os.dup2(devnull_fd, stdout_fd, inheritable=True)
+
+    stderr_fd = sys.stderr.fileno()
+    stderr_fd2 = os.dup(stderr_fd)
+    os.dup2(devnull_fd, stderr_fd, inheritable=True)
+
+    os.close(devnull_fd)
+    return stdout_fd2, stderr_fd2
+
+
+def restore_stdout_stderr(saved):
+    stdout_fd2, stderr_fd2 = saved
+    os.dup2(stdout_fd2, sys.stdout.fileno(), inheritable=True)
+    os.dup2(stderr_fd2, sys.stderr.fileno(), inheritable=True)
+    os.close(stdout_fd2)
+    os.close(stderr_fd2)
+
+
+def run_child(stdin, preloader, conn, files_to_close):
     for f in files_to_close:
         f.close()
     del files_to_close
 
     multiprocessing.set_start_method(None, force=True)
     os.dup2(sys.stdin.fileno(), 0, inheritable=True)
     signal.signal(signal.SIGINT, signal.default_int_handler)
 
+    saved = hide_stdout_stderr()
     sys.argv = [preloader]
-    runpy.run_path(preloader)
+    try:
+        runpy.run_path(preloader)
+    finally:
+        restore_stdout_stderr(saved)
 
     data = conn.recv()
     conn.close()
 
-    os.dup2(stdio[0], 0, inheritable=True)
-    os.close(stdio[0])
     sys.stdin.close()
+    os.dup2(stdin, 0, inheritable=True)
+    os.close(stdin)
     sys.stdin = open(0, closefd=False)
 
     os.environ.clear()
     for k, v in data["environ"].items():
         os.environ[k] = v
     os.chdir(data["cwd"])
 
@@ -53,23 +80,23 @@
         code.interact(local=code_locals, exitmsg="")
     else:
         sys.path = [os.path.dirname(os.path.realpath(data["args"][0]))] + sys.path
         sys.argv = list(data["args"])
         runpy.run_path(data["args"][0], run_name="__main__")
 
 
-def run(stdio, preloader, conn, socks_to_close):
+def run(stdin, preloader, conn, socks_to_close):
     sigint_defer()
 
     for s in socks_to_close:
         s.close()
     del socks_to_close
 
     c1, c2 = Pipe()
-    p = Process(target=run_child, args=(stdio, preloader, c2, [conn, c1]))
+    p = Process(target=run_child, args=(stdin, preloader, c2, [conn, c1]))
     p.start()
     c2.close()
 
     proc = psutil.Process(p.pid)
     if p.exitcode is not None:
         return
 
@@ -115,28 +142,28 @@
         proc.kill()
 
     data = json.dumps({"exit_code": p.exitcode if p.exitcode is not None else -signal.SIGKILL}).encode("utf-8")
     conn.sendall(struct.pack(">Q", len(data)) + data)
     conn.close()
 
 
-def launch_process(stdio, preloader, socks_to_close):
+def launch_process(stdin, preloader, socks_to_close):
     c1, c2 = socket.socketpair(socket.AF_UNIX, socket.SOCK_STREAM)
-    p = Process(target=run, args=(stdio, preloader, c2, socks_to_close + [c1]))
+    p = Process(target=run, args=(stdin, preloader, c2, socks_to_close + [c1]))
     p.start()
     c2.close()
     return p, c1
 
 
-def handler(stdio, preloader, num_proc, sock):
+def handler(stdin, preloader, num_proc, sock):
     sigint_defer()
 
     processes = []
     for _ in range(num_proc):
-        processes.append(launch_process(stdio, preloader, [sock] + [x[1] for x in processes]))
+        processes.append(launch_process(stdin, preloader, [sock] + [x[1] for x in processes]))
 
     while True:
         c = None
         conn = None
         proc = None
         try:
             c = sock.accept()[0]
@@ -160,23 +187,22 @@
         if c is not None:
             try:
                 c.close()
             except:
                 pass
 
         processes = processes[1:]
-        processes.append(launch_process(stdio, preloader, [sock] + [x[1] for x in processes]))
+        processes.append(launch_process(stdin, preloader, [sock] + [x[1] for x in processes]))
 
 
 def server(args):
     multiprocessing.set_start_method("fork")
 
     sigint_defer()
-    stdio = [os.dup(0)]
-    os.set_inheritable(stdio[0], True)
+    stdin = os.dup(0)
 
     if len(args) < 1:
         sys.stderr.write("Expected server argument.\n\nSee --help for more information.\n\n")
         return 1
     preloader = args[0]
     num_proc = 4
     if len(args) > 1:
@@ -189,15 +215,15 @@
     sock = socket.socket(socket.AF_UNIX, socket.SOCK_STREAM)
     sock_path = secrets.token_hex(16)
     sock_path = f"/tmp/prerun_{sock_path}"
     sock.bind(sock_path)
     sock.listen()
 
     try:
-        p = Process(target=handler, args=(stdio, preloader, num_proc, sock))
+        p = Process(target=handler, args=(stdin, preloader, num_proc, sock))
         p.start()
         sock.close()
 
         os.environ["PRERUN_SERVER"] = sock_path
         shell = os.environ.get("SHELL", "/bin/sh")
         proc = subprocess.Popen([shell])
         result = proc.wait()
```

### Comparing `prerun-1.1.1/src/prerun/sigint.py` & `prerun-1.1.2/src/prerun/sigint.py`

 * *Files identical despite different names*

### Comparing `prerun-1.1.1/src/prerun.egg-info/PKG-INFO` & `prerun-1.1.2/src/prerun.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: prerun
-Version: 1.1.1
+Version: 1.1.2
 Summary: Prerun
 License: Copyright (c) <year> <copyright holders>
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of
         this software and associated documentation files (the "Software"), to deal in
         the Software without restriction, including without limitation the rights to
         use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies
```

