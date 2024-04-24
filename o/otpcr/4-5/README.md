# Comparing `tmp/otpcr-4.tar.gz` & `tmp/otpcr-5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "otpcr-4.tar", last modified: Mon Apr  1 12:02:52 2024, max compression
+gzip compressed data, was "otpcr-5.tar", last modified: Tue Apr 23 12:58:29 2024, max compression
```

## Comparing `otpcr-4.tar` & `otpcr-5.tar`

### file list

```diff
@@ -1,41 +1,54 @@
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/
--rw-r--r--   0 bart      (1000) bart      (1000)     2374 2024-04-01 12:02:52.250407 otpcr-4/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)     1848 2024-03-27 18:21:46.000000 otpcr-4/README.rst
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.246407 otpcr-4/files/
--rw-r--r--   0 bart      (1000) bart      (1000)   234877 2024-03-27 18:21:46.000000 otpcr-4/files/verbatim2.png
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/otpcr/
--rw-r--r--   0 bart      (1000) bart      (1000)       66 2024-03-27 18:21:46.000000 otpcr-4/otpcr/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3952 2024-04-01 12:02:08.000000 otpcr-4/otpcr/__main__.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1401 2024-03-27 18:21:46.000000 otpcr-4/otpcr/broker.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1829 2024-03-27 18:21:46.000000 otpcr-4/otpcr/errors.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5051 2024-03-27 18:21:46.000000 otpcr-4/otpcr/handler.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/otpcr/modules/
--rw-r--r--   0 bart      (1000) bart      (1000)      411 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/__init__.py
--rw-r--r--   0 bart      (1000) bart      (1000)      208 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/cmd.py
--rw-r--r--   0 bart      (1000) bart      (1000)      553 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/err.py
--rw-r--r--   0 bart      (1000) bart      (1000)      379 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/flt.py
--rw-r--r--   0 bart      (1000) bart      (1000)      741 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/fnd.py
--rw-r--r--   0 bart      (1000) bart      (1000)    17673 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/irc.py
--rw-r--r--   0 bart      (1000) bart      (1000)      710 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/log.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3485 2024-04-01 10:39:35.000000 otpcr-4/otpcr/modules/mbx.py
--rw-r--r--   0 bart      (1000) bart      (1000)      238 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/mod.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2398 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/req.py
--rw-r--r--   0 bart      (1000) bart      (1000)     9689 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/rss.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2737 2024-04-01 10:39:57.000000 otpcr-4/otpcr/modules/rst.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1118 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/tdo.py
--rw-r--r--   0 bart      (1000) bart      (1000)     1059 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/thr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     5020 2024-03-27 18:21:46.000000 otpcr-4/otpcr/modules/tmr.py
--rw-r--r--   0 bart      (1000) bart      (1000)     2913 2024-04-01 10:40:14.000000 otpcr-4/otpcr/modules/udp.py
--rw-r--r--   0 bart      (1000) bart      (1000)     6954 2024-03-27 18:21:46.000000 otpcr-4/otpcr/object.py
--rw-r--r--   0 bart      (1000) bart      (1000)     4919 2024-03-27 18:21:46.000000 otpcr-4/otpcr/persist.py
--rw-r--r--   0 bart      (1000) bart      (1000)     3198 2024-03-27 18:21:46.000000 otpcr-4/otpcr/thread.py
-drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-01 12:02:52.250407 otpcr-4/otpcr.egg-info/
--rw-r--r--   0 bart      (1000) bart      (1000)     2374 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/PKG-INFO
--rw-r--r--   0 bart      (1000) bart      (1000)      701 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/SOURCES.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/dependency_links.txt
--rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/entry_points.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/top_level.txt
--rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-01 12:02:52.000000 otpcr-4/otpcr.egg-info/zip-safe
--rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-01 12:01:55.000000 otpcr-4/pyproject.toml
--rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-01 12:02:52.250407 otpcr-4/setup.cfg
--rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-03-27 18:21:46.000000 otpcr-4/setup.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.954451 otpcr-5/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-23 12:58:29.954451 otpcr-5/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)     1869 2024-04-23 12:52:59.000000 otpcr-5/README.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.946451 otpcr-5/docs/
+-rw-r--r--   0 bart      (1000) bart      (1000)     3451 2024-04-23 12:56:25.000000 otpcr-5/docs/MANUAL.rst
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.950451 otpcr-5/files/
+-rw-r--r--   0 bart      (1000) bart      (1000)   225470 2024-04-23 12:16:02.000000 otpcr-5/files/EM_Ack_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   238330 2024-04-23 12:16:02.000000 otpcr-5/files/EM_T04_OTP-CR-117_19.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   236671 2024-04-23 12:16:02.000000 otpcr-5/files/EM_T07_OTP-CR-117_19_001.pdf
+-rw-r--r--   0 bart      (1000) bart      (1000)   244503 2024-04-23 12:14:34.000000 otpcr-5/files/verbatim4.png
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.950451 otpcr-5/otpcr/
+-rw-r--r--   0 bart      (1000) bart      (1000)      876 2024-04-23 12:01:06.000000 otpcr-5/otpcr/__init__.py
+-rwxr-xr-x   0 bart      (1000) bart      (1000)     4636 2024-04-23 12:27:34.000000 otpcr-5/otpcr/__main__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1364 2024-04-23 12:01:06.000000 otpcr-5/otpcr/broker.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     3873 2024-04-23 12:01:06.000000 otpcr-5/otpcr/client.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1922 2024-04-23 12:01:06.000000 otpcr-5/otpcr/command.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      230 2024-04-23 12:01:06.000000 otpcr-5/otpcr/default.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1089 2024-04-23 12:01:06.000000 otpcr-5/otpcr/errors.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      766 2024-04-23 12:01:06.000000 otpcr-5/otpcr/event.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1930 2024-04-23 12:01:06.000000 otpcr-5/otpcr/find.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1362 2024-04-23 12:01:06.000000 otpcr-5/otpcr/handler.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.954451 otpcr-5/otpcr/modules/
+-rw-r--r--   0 bart      (1000) bart      (1000)      423 2024-04-23 12:39:26.000000 otpcr-5/otpcr/modules/__init__.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      211 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/cmd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      403 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/err.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      425 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/flt.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      819 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/fnd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17621 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/irc.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      776 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/log.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    17081 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/mdl.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      240 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/mod.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     2400 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/req.py
+-rw-r--r--   0 bart      (1000) bart      (1000)    11001 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/rss.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1184 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/tdo.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1038 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/thr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5130 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/tmr.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     5799 2024-04-23 12:01:18.000000 otpcr-5/otpcr/modules/wsd.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     6155 2024-04-23 12:01:06.000000 otpcr-5/otpcr/object.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      752 2024-04-23 12:01:06.000000 otpcr-5/otpcr/persist.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      275 2024-04-23 12:01:06.000000 otpcr-5/otpcr/repeater.py
+-rw-r--r--   0 bart      (1000) bart      (1000)      109 2024-04-23 12:01:06.000000 otpcr-5/otpcr/runtime.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1900 2024-04-23 12:01:06.000000 otpcr-5/otpcr/thread.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1091 2024-04-23 12:01:06.000000 otpcr-5/otpcr/timer.py
+-rw-r--r--   0 bart      (1000) bart      (1000)     1101 2024-04-23 12:01:06.000000 otpcr-5/otpcr/workdir.py
+drwxr-xr-x   0 bart      (1000) bart      (1000)        0 2024-04-23 12:58:29.950451 otpcr-5/otpcr.egg-info/
+-rw-r--r--   0 bart      (1000) bart      (1000)     2395 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/PKG-INFO
+-rw-r--r--   0 bart      (1000) bart      (1000)      939 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/SOURCES.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/dependency_links.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)       49 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/entry_points.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        6 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/top_level.txt
+-rw-r--r--   0 bart      (1000) bart      (1000)        1 2024-04-23 12:58:29.000000 otpcr-5/otpcr.egg-info/zip-safe
+-rw-r--r--   0 bart      (1000) bart      (1000)     1016 2024-04-23 12:50:22.000000 otpcr-5/pyproject.toml
+-rw-r--r--   0 bart      (1000) bart      (1000)       38 2024-04-23 12:58:29.954451 otpcr-5/setup.cfg
+-rw-r--r--   0 bart      (1000) bart      (1000)      148 2024-04-23 11:57:54.000000 otpcr-5/setup.py
```

### Comparing `otpcr-4/PKG-INFO` & `otpcr-5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 4
+Version: 5
 Summary: OTP-CR-117/19
 Author-email: xobjectz <objx@proton.me>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
@@ -16,16 +16,18 @@
 
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
+|
+
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
```

### Comparing `otpcr-4/README.rst` & `otpcr-5/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
+|
+
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
```

### Comparing `otpcr-4/otpcr/__main__.py` & `otpcr-5/otpcr/__main__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,60 +1,90 @@
-#!/usr/bin/env python3
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,E0611
+# pylint: disable=C,R,W0105,W0201,W0212,W0613,E0401,E0402,W0611
 # ruff: noqa: E402
 
 
+"""NAME
+
+    OTPCR - 117/19
+
+SYNOPSIS
+
+    otpcr <cmd> [key=val] [key==val]
+
+OPTIONS
+
+    -a     load all modules
+    -c     start console
+    -d     start daemon
+    -h     display help
+    -v     use verbose
+
+EXAMPLE
+
+    otpcr -cav
+
+COPYRIGHT
+
+    OTPCR is Public Domain."""
+
+
 "main"
 
 
 import getpass
 import os
 import pwd
-import readline # pylint: disable=W0611
+import readline
 import sys
 import termios
 import time
 
 
-from .broker  import Broker
-from .errors  import debug
-from .handler import Client, Event, cmnd, parse_cmd
-from .object  import Default, cdir, spl
-from .errors  import Errors
-from .persist import Workdir
-
-
-Cfg         = Default()
-Cfg.mod     = "cmd,mod"
-Cfg.name    = "otpcr"
-Cfg.version = "4"
-Cfg.wd      = os.path.expanduser(f"~/.{Cfg.name}")
-Cfg.pidfile = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
-Workdir.wd = Cfg.wd
+sys.path.insert(0, os.getcwd())
 
 
-from . import modules
+from otpcr.client  import Client, cmnd, parse_cmd, spl
+from otpcr.command import Command
+from otpcr.default import Default
+from otpcr.errors  import debug, enable, errors
+from otpcr.event   import Event
+from otpcr.object  import cdir
+from otpcr.runtime import broker
+from otpcr.workdir import Workdir, skel
+
+
+from otpcr import modules
 
 
 if os.path.exists("mods"):
     import mods
 else:
     mods = None
 
 
+Cfg             = Default()
+Cfg.mod         = "cmd,mod"
+Cfg.opts        = ""
+Cfg.name        = "otpcr"
+Cfg.version     = "5"
+Cfg.wd          = os.path.expanduser(f"~/.{Cfg.name}")
+Cfg.pidfile     = os.path.join(Cfg.wd, f"{Cfg.name}.pid")
+Workdir.workdir = Cfg.wd
+
+
 dte = time.ctime(time.time()).replace("  ", " ")
 
 
 class Console(Client):
 
     def __init__(self):
         Client.__init__(self)
-        Broker.add(self)
+        broker.add(self)
 
     def announce(self, txt):
         pass
 
     def callback(self, evt):
         Client.callback(self, evt)
         evt.wait()
@@ -94,15 +124,15 @@
     with open(pidfile, "w", encoding="utf-8") as fds:
         fds.write(str(os.getpid()))
 
 
 def init(pkg, modstr, disable=""):
     mds = []
     for modname in spl(modstr):
-        if modname in spl(disable):
+        if skip(modname, disable):
             continue
         module = getattr(pkg, modname, None)
         if not module:
             continue
         if "init" in dir(module):
             module.init()
             mds.append(module)
@@ -111,14 +141,21 @@
 
 def privileges(username):
     pwnam = pwd.getpwnam(username)
     os.setgid(pwnam.pw_gid)
     os.setuid(pwnam.pw_uid)
 
 
+def skip(name, skipped):
+    for skp in spl(skipped):
+        if skp in name:
+            return True
+    return False
+
+
 def wrap(func):
     old2 = None
     try:
         old2 = termios.tcgetattr(sys.stdin.fileno())
     except termios.error:
         pass
     try:
@@ -131,21 +168,22 @@
 
 
 def ver(event):
     event.reply(f"{Cfg.name.upper()} {Cfg.version}")
 
 
 def main():
-    Workdir.skel()
-    Errors.enable(print)
-    Client.add(ver)
+    Command.add(ver)
+    enable(print)
+    skel()
     parse_cmd(Cfg, " ".join(sys.argv[1:]))
     if 'a' in Cfg.opts:
-        Cfg.mod = ",".join(mods.__dir__())
-        Cfg.mod += "," + ",".join(modules.__dir__())
+        Cfg.mod = ",".join(modules.__dir__())
+        if mods:
+            Cfg.mod += "," + ",".join(mods.__dir__())
     if "v" in Cfg.opts:
         debug(f"{Cfg.name.upper()} {Cfg.opts.upper()} started {dte}")
     if "h" in Cfg.opts:
         print(__doc__)
         return
     if "d" in Cfg.opts:
         Cfg.mod = ",".join(modules.__dir__())
@@ -153,25 +191,32 @@
         daemon(Cfg.pidfile, "v" in Cfg.opts)
         privileges(Cfg.user)
         init(modules, Cfg.mod)
         while 1:
             time.sleep(1.0)
         return
     if "c" in Cfg.opts:
-        init(modules, Cfg.mod)
-        init(mods, Cfg.mod)
+        init(modules, Cfg.mod, Cfg.sets.dis)
+        if mods:
+            Cfg.mod += "," + ",".join(mods.__dir__())
+            init(mods, Cfg.mod)
         csl = Console()
         csl.start()
         while 1:
             time.sleep(1.0)
         return
     if Cfg.otxt:
         return cmnd(Cfg.otxt, print)
 
 
+def daemoned():
+    Cfg.opts += "d"
+    main()
+
+
 def wrapped():
     wrap(main)
-    Errors.show()
+    errors()
 
 
 if __name__ == "__main__":
     wrapped()
```

### Comparing `otpcr-4/otpcr/handler.py` & `otpcr-5/otpcr/client.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,140 +1,38 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0212,W0613,W0718,E0402,E1102
+# pylint: disable=C,R,W0105,W0718
 
 
-"event handler"
+"client"
 
 
-import queue
-import threading
-import _thread
-
-
-from .broker import Broker
-from .errors import Errors
-from .object import Default, Object
-from .thread import launch
-
-
-class Event(Default):
-
-    "Event"
-
-    def __init__(self):
-        Default.__init__(self)
-        self._thr    = None
-        self._ready  = threading.Event()
-        self.done    = False
-        self.orig    = None
-        self.result  = []
-        self.txt     = ""
-        self.type    = "event"
-
-    def ready(self):
-        "event is ready."
-        self._ready.set()
-
-    def reply(self, txt):
-        "add text to the result"
-        self.result.append(txt)
-
-    def wait(self):
-        "wait for event to be ready."
-        if self._thr:
-            self._thr.join()
-        self._ready.wait()
-        return self.result
-
-
-class Handler:
-
-    "Handler"
-
-    def __init__(self):
-        self.cbs = Object()
-        self.queue    = queue.Queue()
-        self.stopped  = threading.Event()
-        self.threaded = True
-
-    def callback(self, evt):
-        "call callback based on event type."
-        func = getattr(self.cbs, evt.type, None)
-        if not func:
-            evt.ready()
-            return
-        evt._thr = launch(func, evt)
-
-    def loop(self):
-        "proces events until interrupted."
-        while not self.stopped.is_set():
-            try:
-                evt = self.poll()
-                self.callback(evt)
-            except (KeyboardInterrupt, EOFError):
-                _thread.interrupt_main()
-
-    def poll(self):
-        "function to return event."
-        return self.queue.get()
-
-    def put(self, evt):
-        "put event into the queue."
-        self.queue.put_nowait(evt)
-
-    def register(self, typ, cbs):
-        "register callback for a type."
-        setattr(self.cbs, typ, cbs)
-
-    def start(self):
-        "start the event loop."
-        launch(self.loop)
-
-    def stop(self):
-        "stop the event loop."
-        self.stopped.set()
+from .command import Command
+from .default import Default
+from .errors  import later
+from .event   import Event
+from .handler import Handler
 
 
 class Client(Handler):
 
     "Client"
 
-    cmds = Object()
-
     def __init__(self):
         Handler.__init__(self)
-        self.register("command", self.command)
-        Broker.add(self)
-
-    @staticmethod
-    def add(func):
-        "add command to client."
-        setattr(Client.cmds, func.__name__, func)
+        self.register("command", command)
 
     def announce(self, txt):
         "announce text."
         self.raw(txt)
 
-    def command(self, evt):
-        "check for and run a command."
-        parse_cmd(evt)
-        func = getattr(Client.cmds, evt.cmd, None)
-        if func:
-            try:
-                func(evt)
-            except Exception as exc:
-                Errors.add(exc)
-        self.show(evt)
-        evt.ready()
-
     def raw(self, txt):
         "raw output."
 
-    def say(self, channel, txt):
+    def say(self, _channel, txt):
         "say text in a channel."
         self.raw(txt)
 
     def show(self, evt):
         "show results into a channel."
         for txt in evt.result:
             self.say(evt.channel, txt)
@@ -143,19 +41,72 @@
 def cmnd(txt, out):
     "do a command using the provided output function."
     clt = Client()
     clt.raw = out
     evn = Event()
     evn.orig = object.__repr__(clt)
     evn.txt = txt
-    clt.command(evn)
+    command(clt, evn)
     evn.wait()
     return evn
 
 
+def command(bot, evt):
+    "check for and run a command."
+    parse_cmd(evt)
+    func = getattr(Command.cmds, evt.cmd, None)
+    if func:
+        try:
+            func(evt)
+        except Exception as exc:
+            later(exc)
+    bot.show(evt)
+    evt.ready()
+
+
+def laps(seconds, short=True):
+    "show elapsed time."
+    txt = ""
+    nsec = float(seconds)
+    if nsec < 1:
+        return f"{nsec:.2f}s"
+    yea = 365*24*60*60
+    week = 7*24*60*60
+    nday = 24*60*60
+    hour = 60*60
+    minute = 60
+    yeas = int(nsec/yea)
+    nsec -= yeas*yea
+    weeks = int(nsec/week)
+    nsec -= weeks*week
+    nrdays = int(nsec/nday)
+    nsec -= nrdays*nday
+    hours = int(nsec/hour)
+    nsec -= hours*hour
+    minutes = int(nsec/minute)
+    nsec -= int(minute*minutes)
+    sec = int(nsec)
+    if yeas:
+        txt += f"{yeas}y"
+    if weeks:
+        nrdays += weeks * 7
+    if nrdays:
+        txt += f"{nrdays}d"
+    if short and txt:
+        return txt.strip()
+    if hours:
+        txt += f"{hours}h"
+    if minutes:
+        txt += f"{minutes}m"
+    if sec:
+        txt += f"{sec}s"
+    txt = txt.strip()
+    return txt
+
+
 def parse_cmd(obj, txt=None):
     "parse a string for a command."
     args = []
     obj.args    = obj.args or []
     obj.cmd     = obj.cmd or ""
     obj.gets    = obj.gets or Default()
     obj.hasmods = obj.hasmod or False
@@ -202,21 +153,14 @@
         obj.txt  = obj.cmd or ""
         obj.rest = " ".join(obj.args)
         obj.txt  = obj.cmd + " " + obj.rest
     else:
         obj.txt = obj.cmd or ""
 
 
-"interface"
-
-
-def __dir__():
-    return (
-        'Event',
-        'Handler',
-        'Client',
-        'cmnd',
-        'parse_cmd'
-    )
-
-
-__all__ = __dir__()
+def spl(txt):
+    "split comma separated string into a list."
+    try:
+        res = txt.split(',')
+    except (TypeError, ValueError):
+        res = txt
+    return [x for x in res if x]
```

### Comparing `otpcr-4/otpcr/modules/irc.py` & `otpcr-5/otpcr/modules/irc.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,50 +14,57 @@
 import ssl
 import textwrap
 import threading
 import time
 import _thread
 
 
-from ..broker  import Broker
-from ..handler import Client, Event
-from ..errors  import Errors, debug
-from ..object  import Default, Object, edit, fmt, keys
-from ..persist import Persist, last, sync
+from ..client  import Client, command
+from ..command import Command
+from ..default import Default
+from ..errors  import debug, later
+from ..event   import Event
+from ..find    import last
+from ..object  import Object, edit, fmt, keys
+from ..persist import whitelist
+from ..runtime import broker
 from ..thread  import launch
+from ..workdir import sync
 
 
-NAME    = __file__.split(os.sep)[-3]
-get     = Broker.get
-saylock = _thread.allocate_lock()
-
-
-Errors.filter = ["PING", "PONG", "PRIVMSG"]
+NAME       = __file__.split(os.sep)[-3]
+filterlist = ["PING", "PONG", "PRIVMSG"]
+saylock    = _thread.allocate_lock()
 
 
 myirc = None
 
 
+def dbg(txt):
+    for flt in filterlist:
+        if flt in txt:
+            return
+    debug(txt)
+
 def init():
     global myirc
     irc = IRC()
-    myirc = object.__repr__(irc)
     irc.start()
     irc.events.joined.wait()
+    myirc = irc
     return irc
 
 
 def shutdown():
-    debug(f"IRC stopping {myirc}")
-    irc = Broker.get(myirc)
-    if irc:
-        irc.state.pongcheck = True
-        irc.state.keeprunning = False
-        irc.events.connected.clear()
-        irc.stop()
+    dbg(f"IRC stopping {myirc}")
+    if myirc:
+        myirc.state.pongcheck = True
+        myirc.state.keeprunning = False
+        myirc.events.connected.clear()
+        myirc.stop()
 
 
 class Config(Default):
 
     channel = f'#{NAME}'
     commands = True
     control = '!'
@@ -80,15 +87,15 @@
         self.nick = self.nick or Config.nick
         self.port = self.port or Config.port
         self.realname = self.realname or Config.realname
         self.server = self.server or Config.server
         self.username = self.username or Config.username
 
 
-Persist.add(Config)
+whitelist(Config)
 
 
 class TextWrap(textwrap.TextWrapper):
 
     def __init__(self):
         super().__init__()
         self.break_long_words = False
@@ -192,15 +199,15 @@
         self.register('CAP', cb_cap)
         self.register('ERROR', cb_error)
         self.register('LOG', cb_log)
         self.register('NOTICE', cb_notice)
         self.register('PRIVMSG', cb_privmsg)
         self.register('QUIT', cb_quit)
         self.register("366", cb_ready)
-        Broker.add(self)
+        broker.add(self)
 
     def announce(self, txt):
         for channel in self.channels:
             self.oput(channel, txt)
 
     def docommand(self, cmd, *args):
         with saylock:
@@ -218,15 +225,15 @@
                 time.sleep(5.0)
             self.state.last = time.time()
 
     def connect(self, server, port=6667):
         self.state.nrconnect += 1
         self.events.connected.clear()
         if self.cfg.password:
-            debug("using SASL")
+            dbg("using SASL")
             self.cfg.sasl = True
             self.cfg.port = "6697"
             ctx = ssl.SSLContext(ssl.PROTOCOL_TLS)
             ctx.options |= ssl.OP_NO_TLSv1 | ssl.OP_NO_TLSv1_1
             ctx.minimum_version = ssl.TLSVersion.TLSv1_2
             sock = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
             self.sock = ctx.wrap_socket(sock)
@@ -255,29 +262,29 @@
         except (
                 ssl.SSLError,
                 OSError,
                 BrokenPipeError
                ) as ex:
             pass
         except Exception as ex:
-            Errors.add(ex)
+            later(ex)
 
     def doconnect(self, server, nck, port=6667):
         while 1:
             try:
                 if self.connect(server, port):
                     break
             except (
                     ssl.SSLError,
                     OSError,
                     ConnectionResetError
                    ) as ex:
                 self.state.error = str(ex)
-                debug(str(ex))
-            debug(f"sleeping {self.cfg.sleep} seconds")
+                dbg(str(ex))
+            dbg(f"sleeping {self.cfg.sleep} seconds")
             time.sleep(self.cfg.sleep)
         self.logon(server, nck)
 
     def event(self, txt):
         evt = self.parsing(txt)
         cmd = evt.command
         if cmd == 'PING':
@@ -315,15 +322,15 @@
             self.events.connected.wait()
             self.events.authed.wait()
             self.state.keeprunning = True
             time.sleep(self.cfg.sleep)
             self.state.pongcheck = True
             self.docommand('PING', self.cfg.server)
             if self.state.pongcheck:
-                debug("failed pongcheck, restarting")
+                dbg("failed pongcheck, restarting")
                 self.state.pongcheck = False
                 self.state.keeprunning = False
                 self.events.connected.clear()
                 self.stop()
                 init()
                 break
 
@@ -334,15 +341,15 @@
         self.direct(f'USER {nck} {server} {server} {nck}')
 
 
     def parsing(self, txt):
         rawstr = str(txt)
         rawstr = rawstr.replace('\u0001', '')
         rawstr = rawstr.replace('\001', '')
-        debug(txt)
+        dbg(txt)
         obj = Event()
         obj.args = []
         obj.rawstr = rawstr
         obj.command = ''
         obj.arguments = []
         arguments = rawstr.split()
         if arguments:
@@ -407,49 +414,49 @@
                     OSError,
                     socket.timeout,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Errors.add(ex)
+                later(ex)
                 self.stop()
-                debug("handler stopped")
+                dbg("handler stopped")
                 evt = self.event(str(ex))
                 return evt
         try:
             txt = self.buffer.pop(0)
         except IndexError:
             txt = ""
         return self.event(txt)
 
     def raw(self, txt):
         txt = txt.rstrip()
-        debug(txt)
+        dbg(txt)
         txt = txt[:500]
         txt += '\r\n'
         txt = bytes(txt, 'utf-8')
         if self.sock:
             try:
                 self.sock.send(txt)
             except (
                     OSError,
                     ssl.SSLError,
                     ssl.SSLZeroReturnError,
                     ConnectionResetError,
                     BrokenPipeError
                    ) as ex:
-                Errors.add(ex)
+                later(ex)
                 self.stop()
                 return
         self.state.last = time.time()
         self.state.nrsend += 1
 
     def reconnect(self):
-        debug(f"reconnecting to {self.cfg.server}")
+        dbg(f"reconnecting to {self.cfg.server}")
         try:
             self.disconnect()
         except (ssl.SSLError, OSError):
             pass
         self.events.connected.clear()
         self.events.joined.clear()
         self.doconnect(self.cfg.server, self.cfg.nick, int(self.cfg.port))
@@ -501,98 +508,90 @@
         self.oput(None, None)
         Client.stop(self)
 
     def wait(self):
         self.events.ready.wait()
 
 
-def cb_auth(evt):
-    bot = get(evt.orig)
+def cb_auth(bot, evt):
     bot.docommand(f'AUTHENTICATE {bot.cfg.password}')
 
 
-def cb_cap(evt):
-    bot = get(evt.orig)
+def cb_cap(bot, evt):
     if bot.cfg.password and 'ACK' in evt.arguments:
         bot.direct('AUTHENTICATE PLAIN')
     else:
         bot.direct('CAP REQ :sasl')
 
 
-def cb_error(evt):
-    bot = get(evt.orig)
+def cb_error(bot, evt):
     if not bot.state.nrerror:
         bot.state.nrerror = 0
     bot.state.nrerror += 1
     bot.state.error = evt.txt
-    debug(evt.txt)
+    dbg(evt.txt)
 
 
-def cb_h903(evt):
-    bot = get(evt.orig)
+def cb_h903(bot, evt):
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_h904(evt):
-    bot = get(evt.orig)
+def cb_h904(bot, evt):
     bot.direct('CAP END')
     bot.events.authed.set()
 
 
-def cb_kill(evt):
+def cb_kill(bot, evt):
     pass
 
 
-def cb_log(evt):
+def cb_log(bot, evt):
     pass
 
 
-def cb_ready(evt):
-    bot = get(evt.orig)
-    if bot:
-        bot.events.ready.set()
+def cb_ready(bot, evt):
+    bot.events.ready.set()
 
 
-def cb_001(evt):
-    bot = get(evt.orig)
+def cb_001(bot, evt):
     bot.logon()
 
 
-def cb_notice(evt):
-    bot = get(evt.orig)
+def cb_notice(bot, evt):
     if evt.txt.startswith('VERSION'):
         txt = f'\001VERSION {NAME.upper()} 140 - {bot.cfg.username}\001'
         bot.docommand('NOTICE', evt.channel, txt)
 
 
-def cb_privmsg(evt):
-    bot = get(evt.orig)
+def cb_privmsg(bot, evt):
     if not bot.cfg.commands:
         return
     if evt.txt:
         if evt.txt[0] in ['!',]:
             evt.txt = evt.txt[1:]
         elif evt.txt.startswith(f'{bot.cfg.nick}:'):
             evt.txt = evt.txt[len(bot.cfg.nick)+1:]
         else:
             return
         if evt.txt:
             evt.txt = evt.txt[0].lower() + evt.txt[1:]
-        debug(f"command from {evt.origin}: {evt.txt}")
-        bot.command(evt)
+        dbg(f"command from {evt.origin}: {evt.txt}")
+        command(bot, evt)
 
 
-def cb_quit(evt):
-    bot = get(evt.orig)
-    debug(f"quit from {bot.cfg.server}")
+def cb_quit(bot, evt):
+    dbg(f"quit from {bot.cfg.server}")
     if evt.orig and evt.orig in bot.zelf:
         bot.stop()
 
 
+"commands"
+
+
 def cfg(event):
     config = Config()
     path = last(config)
     if not event.sets:
         event.reply(
                     fmt(
                         config,
@@ -602,37 +601,37 @@
                    )
     else:
         edit(config, event.sets)
         sync(config, path)
         event.reply('ok')
 
 
-Client.add(cfg)
+Command.add(cfg)
 
 
 def mre(event):
     if not event.channel:
         event.reply('channel is not set.')
         return
-    bot = Broker.get(event.orig)
+    bot = broker.get(event.orig)
     if 'cache' not in dir(bot):
         event.reply('bot is missing cache')
         return
     if event.channel not in bot.cache:
         event.reply(f'no output in {event.channel} cache.')
         return
     for _x in range(3):
         txt = bot.gettxt(event.channel)
         if txt:
             bot.say(event.channel, txt)
     size = bot.size(event.channel)
     event.reply(f'{size} more in cache')
 
 
-Client.add(mre)
+Command.add(mre)
 
 
 def pwd(event):
     if len(event.args) != 2:
         event.reply('pwd <nick> <password>')
         return
     arg1 = event.args[0]
@@ -640,8 +639,8 @@
     txt = f'\x00{arg1}\x00{arg2}'
     enc = txt.encode('ascii')
     base = base64.b64encode(enc)
     dcd = base.decode('ascii')
     event.reply(dcd)
 
 
-Client.add(pwd)
+Command.add(pwd)
```

### Comparing `otpcr-4/otpcr/modules/log.py` & `otpcr-5/otpcr/modules/log.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,27 +5,30 @@
 
 "log text"
 
 
 import time
 
 
-from ..handler import Client
+from ..client  import laps
+from ..command import Command
 from ..object  import Object
-from ..persist import Persist, find, fntime, laps, sync
+from ..find    import find, fntime
+from ..workdir import  sync
+from ..persist import whitelist
 
 
 class Log(Object):
 
     def __init__(self):
         super().__init__()
         self.txt = ''
 
 
-Persist.add(Log)
+whitelist(Log)
 
 
 def log(event):
     if not event.rest:
         nmr = 0
         for fnm, obj in find('log'):
             lap = laps(time.time() - fntime(fnm))
@@ -36,8 +39,8 @@
         return
     obj = Log()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
 
 
-Client.add(log)
+Command.add(log)
```

### Comparing `otpcr-4/otpcr/modules/req.py` & `otpcr-5/otpcr/modules/req.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 
 
 (1) provided are the confirmation letters of both the chamber and the king.
 (2) your reference: OTP-CR-117/19
 """
 
 
-from ..handler import Client
+from ..command import Command
 
 
 def req(event):
     event.reply(__doc__)
 
 
-Client.add(req)
+Command.add(req)
```

### Comparing `otpcr-4/otpcr/modules/rss.py` & `otpcr-5/otpcr/modules/rss.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0201,W0612,E0402
+# pylint: disable=C,R,W0105
 
 
 "rich site syndicate"
 
 
 import html.parser
 import re
@@ -14,67 +14,83 @@
 import _thread
 
 
 from urllib.error import HTTPError, URLError
 from urllib.parse import quote_plus, urlencode
 
 
-from ..broker  import Broker
-from ..handler import Client
-from ..object  import Default, Object, fmt, spl, update
-from ..persist import Persist, find, fntime, laps, last, sync
-from ..thread  import Repeater, launch
+from ..client   import laps, spl
+from ..command  import Command
+from ..default  import Default
+from ..find     import find, fntime, last
+from ..object   import Object, fmt, update, values
+from ..persist  import whitelist
+from ..repeater import Repeater
+from ..runtime  import broker
+from ..thread   import launch
+from ..workdir  import sync
 
 
 def init():
+    "start fetcher."
     fetcher = Fetcher()
     fetcher.start()
     return fetcher
 
 
 DEBUG = False
 
 
 fetchlock = _thread.allocate_lock()
 
 
+TEMPLATE = """<opml version="1.0">
+    <head>
+        <title>rssbot opml</title>
+    </head>
+    <body>
+        <outline title="rssbot opml" text="24/7 feed fetcher">"""
+
+
 class Feed(Default):
 
-    pass
+    "Feed"
 
 
 class Rss(Default):
 
+    "Rss"
+
     def __init__(self):
         Default.__init__(self)
         self.display_list = 'title,link,author'
-
-
-Persist.add(Rss)
+        self.rss          = ''
 
 
 class Seen(Default):
 
+    "Seen"
+
     def __init__(self):
         Default.__init__(self)
         self.urls = []
 
 
-Persist.add(Seen)
-
-
 class Fetcher(Object):
 
+    "Fetcher"
+
     def __init__(self):
         self.dosave = False
         self.seen = Seen()
         self.seenfn = None
 
     @staticmethod
     def display(obj):
+        "display object."
         result = ''
         displaylist = []
         try:
             displaylist = obj.display_list or 'title,link'
         except AttributeError:
             displaylist = 'title,link,author'
         for key in displaylist.split(","):
@@ -87,14 +103,15 @@
             data = striphtml(data.rstrip())
             data = unescape(data)
             result += data.rstrip()
             result += ' - '
         return result[:-2].rstrip()
 
     def fetch(self, feed):
+        "fetch feed."
         with fetchlock:
             counter = 0
             result = []
             for obj in reversed(getfeed(feed.rss, feed.display_list)):
                 fed = Feed()
                 update(fed, obj)
                 update(fed, feed)
@@ -114,68 +131,75 @@
             sync(self.seen, self.seenfn)
         txt = ''
         feedname = getattr(feed, 'name', None)
         if feedname:
             txt = f'[{feedname}] '
         for obj in result:
             txt2 = txt + self.display(obj)
-            for bot in Broker.all():
+            for bot in values(broker.objs):
                 if "announce" in dir(bot):
                     bot.announce(txt2.rstrip())
         return counter
 
     def run(self):
+        "fetch all feeds."
         thrs = []
-        for fnm, feed in find('rss'):
+        for _fn, feed in find('rss'):
             thrs.append(launch(self.fetch, feed, name=f"{feed.rss}"))
         return thrs
 
     def start(self, repeat=True):
+        "start fetcher."
         self.seenfn = last(self.seen)
         if repeat:
             repeater = Repeater(300.0, self.run)
             repeater.start()
 
 
 class Parser:
 
+    "Parser"
+
     @staticmethod
     def getvalue(line, attr):
+        "retrieve attribute value."
         lne = ''
-        index1 = line.find(f' {attr}="')
+        index1 = line.find(f'{attr}="')
         if index1 == -1:
             return lne
-        index1 += len(attr) + 3
+        index1 += len(attr) + 2
         index2 = line.find('"', index1)
         if index2 == -1:
             index2 = line.find('"/>', index1)
         if index2 == -1:
             return lne
         lne = line[index1:index2]
         if 'CDATA' in lne:
             lne = lne.replace('![CDATA[', '')
             lne = lne.replace(']]', '')
             #lne = lne[1:-1]
         return lne
 
     @staticmethod
     def getattrs(line, token):
+        "split for attributes."
         result = ""
         index1 = line.find(f'<{token} ')
         if index1 == -1:
             return result
         index1 += len(token) + 2
         index2 = line.find('/>', index1)
         if index2 == -1:
             return result
         result = line[index1:index2]
         return result.strip()
-    
+
     @staticmethod
     def getitem(line, item):
+        "match items."
         lne = ''
         index1 = line.find(f'<{item}>')
         if index1 == -1:
             return lne
         index1 += len(item) + 2
         index2 = line.find(f'</{item}>', index1)
         if index2 == -1:
@@ -185,73 +209,79 @@
             lne = lne.replace('![CDATA[', '')
             lne = lne.replace(']]', '')
             lne = lne[1:-1]
         return lne.strip()
 
     @staticmethod
     def getitems(text, token):
+        "loop for items."
         index = 0
         result = []
         stop = False
         while not stop:
-            index1 = text.find(f'<{token}>', index)
+            index1 = text.find(f'<{token}', index)
             if index1 == -1:
                 break
             index1 += len(token) + 2
             index2 = text.find(f'</{token}>', index1)
             if index2 == -1:
                 break
             lne = text[index1:index2]
             result.append(lne)
-            index = index2             
+            index = index2
         return result
 
     @staticmethod
     def parse(txt, toke="item", items='title,link'):
+        "parse a text for tokens."
         result = []
         for line in Parser.getitems(txt, toke):
             line = line.strip()
             obj = Default()
             for itm in spl(items):
                 val = Parser.getitem(line, itm)
                 if val:
                     val = unescape(val.strip())
                     val = val.replace("\n", "")
                     val = striphtml(val)
                     setattr(obj, itm, val)
                 else:
-                    att = Parser.getattrs(line, itm)
-                    if att:
-                        if itm == "link":
-                            itm = "href"
-                        val = Parser.getvalue(att, itm)
-                        if val:
-                            if itm == "href":
-                                itm = "link"
-                            setattr(obj, itm, val.strip())
+                    att = Parser.getattrs(line, toke)
+                    if not att:
+                        continue
+                    if itm == "link":
+                        itm = "href"
+                    val = Parser.getvalue(att, itm)
+                    if not val:
+                        continue
+                    if itm == "href":
+                        itm = "link"
+                    setattr(obj, itm, val.strip())
             result.append(obj)
         return result
 
 
 def getfeed(url, items):
+    "fetch a feed."
+    result = [Object(), Object()]
     if DEBUG:
-        return [Object(), Object()]
+        return result
     try:
-        result = geturl(url)
+        rest = geturl(url)
     except (ValueError, HTTPError, URLError):
-        return [Object(), Object()]
-    if not result:
-        return [Object(), Object()]
-    if url.endswith('atom'):
-        return Parser.parse(str(result.data, 'utf-8'), 'entry', items) or []
-    else:
-        return Parser.parse(str(result.data, 'utf-8'), 'item', items) or []
-    
+        return result
+    if rest:
+        if url.endswith('atom'):
+            result = Parser.parse(str(rest.data, 'utf-8'), 'entry', items) or []
+        else:
+            result = Parser.parse(str(rest.data, 'utf-8'), 'item', items) or []
+    return result
 
 def gettinyurl(url):
+    "fetch a tinyurl."
     postarray = [
         ('submit', 'submit'),
         ('url', url),
     ]
     postdata = urlencode(postarray, quote_via=quote_plus)
     req = urllib.request.Request('http://tinyurl.com/create.php',
                   data=bytes(postdata, 'UTF-8'))
@@ -262,99 +292,113 @@
             i = re.search('data-clipboard-text="(.*?)"', line, re.M)
             if i:
                 return i.groups()
     return []
 
 
 def geturl(url):
+    "fetch a url."
     if not url.startswith("http://") and not url.startswith("https://"):
         return ""
     url = urllib.parse.urlunparse(urllib.parse.urlparse(url))
     req = urllib.request.Request(url)
     req.add_header('User-agent', useragent("rss fetcher"))
     with urllib.request.urlopen(req) as response: # nosec
         response.data = response.read()
         return response
 
 
 def striphtml(text):
+    "strip html."
     clean = re.compile('<.*?>')
     return re.sub(clean, '', text)
 
 
 def unescape(text):
+    "unescape text."
     txt = re.sub(r'\s+', ' ', text)
     return html.unescape(txt)
 
 
 def useragent(txt):
+    "return useragent."
     return 'Mozilla/5.0 (X11; Linux x86_64) ' + txt
 
 
+"commands"
+
+
 def dpl(event):
+    "set display items."
     if len(event.args) < 2:
         event.reply('dpl <stringinurl> <item1,item2>')
         return
     setter = {'display_list': event.args[1]}
-    for fnm, feed in find('rss', {'rss': event.args[0]}):
+    for _fn, feed in find('rss', {'rss': event.args[0]}):
         if feed:
             update(feed, setter)
             sync(feed)
     event.reply('ok')
 
 
-Client.add(dpl)
+def exp(event):
+    "export to opml."
+    event.reply(TEMPLATE)
+    nrs = 0
+    for _fn, obj in find("rss"):
+        nrs += 1
+        name = obj.name or f"url{nrs}"
+        txt = f'<outline name={name} display_list={obj.display_list} xmlUrl="{obj.rss}"/>'
+        event.reply(" "*12 + txt)
+    event.reply(" "*8 + "</outline>")
+    event.reply("    <body>")
+    event.reply("</opml>")
 
 
 def nme(event):
+    "set name of feed."
     if len(event.args) != 2:
         event.reply('nme <stringinurl> <name>')
         return
     selector = {'rss': event.args[0]}
-    for fnm, feed in find('rss', selector):
+    for _fn, feed in find('rss', selector):
         if feed:
             feed.name = event.args[1]
             sync(feed)
     event.reply('ok')
 
 
-Client.add(nme)
-
-
 def rem(event):
+    "remove a feed."
     if len(event.args) != 1:
         event.reply('rem <stringinurl>')
         return
     selector = {'rss': event.args[0]}
     for fnm, feed in find('rss', selector):
         if feed:
             feed.__deleted__ = True
             sync(feed, fnm)
     event.reply('ok')
 
 
-Client.add(rem)
-
-
 def res(event):
+    "restore a feed."
     if len(event.args) != 1:
         event.reply('res <stringinurl>')
         return
     selector = {'rss': event.args[0]}
     for fnm, feed in find('rss', selector, deleted=True):
         if feed:
             feed.__deleted__ = False
             sync(feed, fnm)
     event.reply('ok')
 
 
-Client.add(res)
-
-
 def rss(event):
+    "add a feed."
     if not event.rest:
         nrs = 0
         for fnm, feed in find('rss'):
             nrs += 1
             elp = laps(time.time()-fntime(fnm))
             txt = fmt(feed)
             event.reply(f'{nrs} {txt} {elp}')
@@ -371,8 +415,18 @@
             return
     feed = Rss()
     feed.rss = event.args[0]
     sync(feed)
     event.reply('ok')
 
 
-Client.add(rss)
+"register"
+
+
+Command.add(dpl)
+Command.add(exp)
+Command.add(nme)
+Command.add(rem)
+Command.add(res)
+Command.add(rss)
+whitelist(Rss)
+whitelist(Seen)
```

### Comparing `otpcr-4/otpcr/modules/tdo.py` & `otpcr-5/otpcr/modules/tdo.py`

 * *Files 25% similar despite different names*

```diff
@@ -5,32 +5,35 @@
 
 "todo list"
 
 
 import time
 
 
-from ..handler import Client
+from ..client  import laps
 from ..object  import Object
-from ..persist import Persist, fntime, find, laps, sync
+from ..command import Command
+from ..find    import fntime, find
+from ..persist import whitelist
+from ..workdir import sync
 
 
 class NoDate(Exception):
 
     pass
 
 
 class Todo(Object):
 
     def __init__(self):
         Object.__init__(self)
         self.txt = ''
 
 
-Persist.add(Todo)
+whitelist(Todo)
 
 
 def dne(event):
     if not event.args:
         event.reply("dne <txt>")
         return
     selector = {'txt': event.args[0]}
@@ -41,15 +44,15 @@
         sync(obj, fnm)
         event.reply('ok')
         break
     if not nmr:
         event.reply("nothing todo")
 
 
-Client.add(dne)
+Command.add(dne)
 
 
 def tdo(event):
     if not event.rest:
         nmr = 0
         for fnm, obj in find('todo'):
             lap = laps(time.time()-fntime(fnm))
@@ -60,8 +63,8 @@
         return
     obj = Todo()
     obj.txt = event.rest
     sync(obj)
     event.reply('ok')
 
 
-Client.add(tdo)
+Command.add(tdo)
```

### Comparing `otpcr-4/otpcr/modules/tmr.py` & `otpcr-5/otpcr/modules/tmr.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,28 +7,33 @@
 
 
 import datetime
 import re
 import time as ttime
 
 
-from ..broker import Broker
-from ..handler import Client, Event
-from ..object import update
-from ..persist import Persist, find, laps, sync
-from ..thread import Timer, launch
+from ..client  import laps
+from ..command import Command
+from ..event   import Event
+from ..find    import find
+from ..runtime import broker
+from ..timer   import Timer
+from ..thread  import launch
+from ..persist import whitelist
+from ..object  import update
+from ..workdir import sync
 
 
 def init():
     for fnm, obj in find("timer"):
         if "time" not in obj:
             continue
         diff = float(obj.time) - ttime.time()
         if diff > 0:
-            bot = Broker.first()
+            bot = broker.first()
             evt = Event()
             update(evt, obj)
             evt.orig = object.__repr__(bot)
             timer = Timer(diff, evt.show)
             launch(timer.start)
 
 
@@ -58,15 +63,15 @@
 
 
 class NoDate(Exception):
 
     pass
 
 
-Persist.add(Timer)
+whitelist(Timer)
 
 
 def extract_date(daystr):
     for fmt in FORMATS:
         try:
             res = ttime.mktime(ttime.strptime(daystr, fmt))
         except ValueError:
@@ -221,8 +226,8 @@
     event.result.append(event.rest)
     timer = Timer(diff, event.show, thrname=event.cmd)
     update(timer, event)
     sync(timer)
     launch(timer.start)
 
 
-Client.add(tmr)
+Command.add(tmr)
```

### Comparing `otpcr-4/otpcr/object.py` & `otpcr-5/otpcr/object.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,34 +1,27 @@
 # This file is placed in the Public Domain.
 #
-# pylint: disable=C,R,W0105,W0613,E0101
+# pylint: disable=C,R,W0105
 
 
-"""a clean namespace
-
-This module allows for easy json save//load to/from disk of objects. It
-provides an "clean namespace" Object class that only has dunder
-methods, so the namespace is not cluttered with method names. This makes
-storing and reading to/from json possible.
-
-"""
+"objects"
 
 
 import json
 import os
 import pathlib
 import _thread
 
 
 disklock = _thread.allocate_lock()
 
 
 class Object:
 
-    "Base class."
+    "Object"
 
     def __contains__(self, key):
         return key in dir(self)
 
     def __iter__(self):
         return iter(self.__dict__)
 
@@ -163,18 +156,18 @@
         cdir(os.path.dirname(pth))
         with open(pth, 'w', encoding='utf-8') as ofile:
             dump(obj, ofile, indent=4)
 
 
 class ObjectDecoder(json.JSONDecoder):
 
-    "Object decoded"
+    "ObjectDecoder"
 
     def __init__(self, *args, **kwargs):
-        return json.JSONDecoder.__init__(self, *args)
+        json.JSONDecoder.__init__(self, *args, **kwargs)
 
     def decode(self, s, _w=None):
         "decoding string to object."
         val = json.JSONDecoder.decode(self, s)
         if not val:
             val = {}
         return hook(val)
@@ -206,18 +199,18 @@
     kw["cls"] = ObjectDecoder
     kw["object_hook"] = hook
     return json.loads(string, *args, **kw)
 
 
 class ObjectEncoder(json.JSONEncoder):
 
-    "Object encoder."
+    "ObjectEncoder"
 
     def __init__(self, *args, **kwargs):
-        return json.JSONEncoder.__init__(self, *args, **kwargs)
+        json.JSONEncoder.__init__(self, *args, **kwargs)
 
     def default(self, o):
         "return stringable value."
         if isinstance(o, dict):
             return o.items()
         if isinstance(o, Object):
             return vars(o)
@@ -247,51 +240,27 @@
 
 def dumps(*args, **kw):
     "dump object to string."
     kw["cls"] = ObjectEncoder
     return json.dumps(*args, **kw)
 
 
-class Default(Object):
-
-    "Object that return a default value if key does not exist."
-
-    __slots__ = ("__default__",)
-
-    def __init__(self):
-        Object.__init__(self)
-        self.__default__ = ""
-
-    def __getattr__(self, key):
-        return self.__dict__.get(key, self.__default__)
-
-
 def cdir(pth):
     "create directory."
     if os.path.exists(pth):
         return
     pth = pathlib.Path(pth)
     os.makedirs(pth, exist_ok=True)
 
 
-def spl(txt):
-    "split comma separated string into a list."
-    try:
-        res = txt.split(',')
-    except (TypeError, ValueError):
-        res = txt
-    return [x for x in res if x]
-
-
 "interface"
 
 
 def __dir__():
     return (
-        'Default',
         'Object',
         'construct',
         'dump',
         'dumps',
         'edit',
         'fmt',
         'fqn',
```

### Comparing `otpcr-4/otpcr.egg-info/PKG-INFO` & `otpcr-5/otpcr.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: otpcr
-Version: 4
+Version: 5
 Summary: OTP-CR-117/19
 Author-email: xobjectz <objx@proton.me>
 License: Public Domain
 Project-URL: home, https://pypi.org/project/otpcr
 Project-URL: bugs, https://github.com/xobjectz/otpcr/issues
 Project-URL: source, https://github.com/xobjectz/otpcr
 Classifier: Development Status :: 3 - Alpha
@@ -16,16 +16,18 @@
 
 | **Information and Evidence Unit**
 | **Office of the Prosecutor**
 | **Post Office Box 19519**
 | **2500 CM The Hague**
 | **The Netherlands**
 |
+|
+
 
-Hello Office of the Prosecutor,
+Hello Office of the Prosecutor, ``OTP-CR-117/19``
 
 i write you in the context of communications and claims under art.15 of 
 the Rome Statute. i want to inform the prosecutor that the king of the 
 netherlands and his government are commiting 3 of the 5 crimes defined 
 in the Rome Statute.
 
 The dutch government has introduced three new forced care laws, the Wfz
```

### Comparing `otpcr-4/pyproject.toml` & `otpcr-5/pyproject.toml`

 * *Files 23% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     "wheel"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "otpcr"
 description = "OTP-CR-117/19"
-version = "4"
+version = "5"
 authors = [
     {name = "xobjectz", email = "objx@proton.me"},
 ]
 readme = "README.rst"
 license = {text="Public Domain"}
 classifiers = [ 
     'Development Status :: 3 - Alpha',
@@ -21,15 +21,14 @@
     'Programming Language :: Python',
     'Topic :: Utilities'
 ]
 
 [project.scripts]
 "otpcr" = "otpcr.__main__:wrapped"
 
-
 [project.urls]
 "home" = "https://pypi.org/project/otpcr"
 "bugs" = "https://github.com/xobjectz/otpcr/issues"
 "source" = "https://github.com/xobjectz/otpcr"
 
 [tool.setuptools]
 packages = [
@@ -38,9 +37,13 @@
 ]
 zip-safe=true
 
 
 [tool.setuptools.data-files]
 "share/doc/otpcr" = [
     "README.rst",
-    "files/verbatim2.png"
+    "docs/MANUAL.rst",
+    "files/verbatim4.png",
+    "files/EM_Ack_OTP-CR-117_19.pdf",
+    "files/EM_T07_OTP-CR-117_19_001.pdf",
+    "files/EM_T04_OTP-CR-117_19.pdf"
 ]
```

