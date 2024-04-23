# Comparing `tmp/pyorick-1.4.tar.gz` & `tmp/pyorick-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyorick-1.4.tar", last modified: Mon Feb 16 19:43:44 2015, max compression
+gzip compressed data, was "pyorick-1.5.tar", last modified: Tue Apr 23 23:22:02 2024, max compression
```

## Comparing `pyorick-1.4.tar` & `pyorick-1.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2015-02-16 19:43:44.000000 pyorick-1.4/
--rw-rw-r--   0 dave      (1000) dave      (1000)    13001 2015-02-16 19:40:32.000000 pyorick-1.4/DESCRIPTION.rst
--rw-rw-r--   0 dave      (1000) dave      (1000)       88 2015-02-16 19:43:44.000000 pyorick-1.4/setup.cfg
--rw-rw-r--   0 dave      (1000) dave      (1000)     1320 2014-11-16 00:53:45.000000 pyorick-1.4/LICENSE.txt
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2015-02-16 19:43:44.000000 pyorick-1.4/pyorick.egg-info/
--rw-rw-r--   0 dave      (1000) dave      (1000)      275 2015-02-16 19:43:43.000000 pyorick-1.4/pyorick.egg-info/SOURCES.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)     1774 2015-02-16 19:43:42.000000 pyorick-1.4/pyorick.egg-info/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)        1 2015-02-16 19:43:42.000000 pyorick-1.4/pyorick.egg-info/dependency_links.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)        8 2015-02-16 19:43:42.000000 pyorick-1.4/pyorick.egg-info/top_level.txt
--rw-rw-r--   0 dave      (1000) dave      (1000)      863 2015-02-16 19:11:45.000000 pyorick-1.4/README.rst
-drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2015-02-16 19:43:44.000000 pyorick-1.4/pyorick/
--rw-rw-r--   0 dave      (1000) dave      (1000)    16711 2015-02-16 19:11:45.000000 pyorick-1.4/pyorick/test_pyorick.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    62911 2015-02-16 19:11:45.000000 pyorick-1.4/pyorick/pyorick.py
--rw-rw-r--   0 dave      (1000) dave      (1000)    27262 2015-02-16 19:11:45.000000 pyorick-1.4/pyorick/pyorick.i0
--rw-rw-r--   0 dave      (1000) dave      (1000)    10130 2015-02-16 19:11:45.000000 pyorick-1.4/pyorick/__init__.py
--rw-rw-r--   0 dave      (1000) dave      (1000)       90 2014-11-16 00:55:23.000000 pyorick-1.4/MANIFEST.in
--rw-rw-r--   0 dave      (1000) dave      (1000)     1774 2015-02-16 19:43:44.000000 pyorick-1.4/PKG-INFO
--rw-rw-r--   0 dave      (1000) dave      (1000)     2401 2015-02-16 19:40:32.000000 pyorick-1.4/setup.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-23 23:22:02.557757 pyorick-1.5/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    13001 2023-02-08 17:25:06.000000 pyorick-1.5/DESCRIPTION.rst
+-rw-rw-r--   0 dave      (1000) dave      (1000)     1320 2023-02-08 17:25:06.000000 pyorick-1.5/LICENSE.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       90 2023-02-08 17:25:06.000000 pyorick-1.5/MANIFEST.in
+-rw-r--r--   0 dave      (1000) dave      (1000)     1603 2024-04-23 23:22:02.557757 pyorick-1.5/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      863 2023-02-08 17:25:06.000000 pyorick-1.5/README.rst
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-23 23:22:02.557757 pyorick-1.5/pyorick/
+-rw-rw-r--   0 dave      (1000) dave      (1000)    10130 2023-02-08 17:25:06.000000 pyorick-1.5/pyorick/__init__.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    27261 2023-02-08 17:25:06.000000 pyorick-1.5/pyorick/pyorick.i0
+-rw-rw-r--   0 dave      (1000) dave      (1000)    63191 2023-10-25 18:20:52.000000 pyorick-1.5/pyorick/pyorick.py
+-rw-rw-r--   0 dave      (1000) dave      (1000)    16711 2023-02-08 17:25:06.000000 pyorick-1.5/pyorick/test_pyorick.py
+drwxrwxr-x   0 dave      (1000) dave      (1000)        0 2024-04-23 23:22:02.557757 pyorick-1.5/pyorick.egg-info/
+-rw-r--r--   0 dave      (1000) dave      (1000)     1603 2024-04-23 23:22:02.000000 pyorick-1.5/pyorick.egg-info/PKG-INFO
+-rw-rw-r--   0 dave      (1000) dave      (1000)      265 2024-04-23 23:22:02.000000 pyorick-1.5/pyorick.egg-info/SOURCES.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        1 2024-04-23 23:22:02.000000 pyorick-1.5/pyorick.egg-info/dependency_links.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)        8 2024-04-23 23:22:02.000000 pyorick-1.5/pyorick.egg-info/top_level.txt
+-rw-rw-r--   0 dave      (1000) dave      (1000)       38 2024-04-23 23:22:02.557757 pyorick-1.5/setup.cfg
+-rw-rw-r--   0 dave      (1000) dave      (1000)     2231 2024-04-23 20:25:38.000000 pyorick-1.5/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `pyorick-1.4/DESCRIPTION.rst` & `pyorick-1.5/DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `pyorick-1.4/LICENSE.txt` & `pyorick-1.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyorick-1.4/pyorick.egg-info/PKG-INFO` & `pyorick-1.5/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyorick
-Version: 1.4
+Version: 1.5
 Summary: python connection to yorick
 Home-page: https://github.com/dhmunro/pyorick
 Author: David Munro and John Field
 Author-email: dhmunro@users.sourceforge.net
 License: http://opensource.org/licenses/BSD-2-Clause
-Description: Run Yorick from Python
-        ======================
-        
-        The pyorick package starts `yorick <http://yorick.github.com>`_ as a
-        subprocess and provides an interface between python and yorick
-        interpreted code.
-        
-        Features:
-        
-        - exec or eval arbitrary yorick code strings
-        - get or set yorick variables
-        - call yorick functions or subroutines with python arguments
-        - get or set slices of large yorick arrays
-        - terminal mode to interact with yorick by keyboard through python
-        
-        Most of the data is exchanged via binary pipes between the two
-        interpreters.  Yorick runs in a request-reply mode.  Python prints
-        anything yorick sends to stdout or stderr except prompts.
-        
-        See `DESCRIPTION.rst <https://github.com/dhmunro/pyorick/blob/master/DESCRIPTION.rst>`_
-        for a complete description of the interface.  You can clone or fork
-        https://github.com/dhmunro/pyorick to contribute to pyorick.
-        
-        
 Platform: Linux
 Platform: MacOS X
 Platform: Unix
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Interpreters
 Requires: numpy
+License-File: LICENSE.txt
+
+Run Yorick from Python
+======================
+
+The pyorick package starts `yorick <http://yorick.github.com>`_ as a
+subprocess and provides an interface between python and yorick
+interpreted code.
+
+Features:
+
+- exec or eval arbitrary yorick code strings
+- get or set yorick variables
+- call yorick functions or subroutines with python arguments
+- get or set slices of large yorick arrays
+- terminal mode to interact with yorick by keyboard through python
+
+Most of the data is exchanged via binary pipes between the two
+interpreters.  Yorick runs in a request-reply mode.  Python prints
+anything yorick sends to stdout or stderr except prompts.
+
+See `DESCRIPTION.rst <https://github.com/dhmunro/pyorick/blob/master/DESCRIPTION.rst>`_
+for a complete description of the interface.  You can clone or fork
+https://github.com/dhmunro/pyorick to contribute to pyorick.
+
```

### Comparing `pyorick-1.4/README.rst` & `pyorick-1.5/README.rst`

 * *Files identical despite different names*

### Comparing `pyorick-1.4/pyorick/test_pyorick.py` & `pyorick-1.5/pyorick/test_pyorick.py`

 * *Files identical despite different names*

### Comparing `pyorick-1.4/pyorick/pyorick.py` & `pyorick-1.5/pyorick/pyorick.py`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,18 @@
   import pickle
 else:
   import cPickle as pickle
 
 import numpy as np
 
 from numbers import Number
-from collections import Sequence, Mapping
+try:
+  from collections.abc import Sequence, Mapping
+except ImportError:  # fallback for python 2.7 or <3.3
+  from collections import Sequence, Mapping
 from ctypes import (c_byte, c_ubyte, c_short, c_ushort, c_int, c_uint,
                     c_long, c_ulong, c_longlong, c_ulonglong,
                     c_float, c_double, c_longdouble, sizeof)
 import os
 import shlex
 import fcntl
 import select
@@ -194,27 +197,30 @@
     hold = args[0]
     if hold and isinstance(hold, basestring) and hold[0]=='\05':
       hold = True
     else:
       hold = False
     reply = Message()
     self.proc.reqrep(Message(msgid, *args, **kwargs), reply)
-    while reply.packets and reply.packets[0][0] >= ID_EVAL:
+    while (reply.packets and reply.packets[0][0] >= ID_EVAL and
+           self.proc.pid is not None):
       if self.proc._debug:
         print("P>_reqrep: begin processing request (non-passive reply)")
       reply = reply.getreply(self.proc._debug, self._namespace)
       if not reply:
         raise PYorickError("yorick sent unknown active reply to request")
       if self.proc._debug:
         print("P>_reqrep: sending reply to request")
       self.proc.sendmsg(reply)
       reply = Message()  # get the next reply from yorick
       self.proc.recvmsg(reply)
     if self.proc._debug:
       print("P>_reqrep: got passive reply to original request")
+    if (self.proc.pid is None):
+      return None;
     reply = reply.decode()
     if not isinstance(reply, tuple):
       if not hold:
         return reply
       if (isinstance(reply, np.ndarray) and reply.dtype==np.dtype(c_long)
           and reply.shape==()):
         return YorickHold(self, reply)
@@ -1665,21 +1671,21 @@
       for packet in reply.reader():
         while True:  # do not block on rfd when pfd pending
           p = select.select([self.pfd, self.rfd], [], [self.pfd, self.rfd])
           if self.rfd in p[0]:
             break
           prompt = self.echo_pty()
           if prompt == 'PYORICK-QUIT> ':
-            return prompt
+            return  # yorick has quit, and process killed by echo_pty
         self.recv(packet)
     except:
       self.kill()
       raise PYorickError("failed to receive complete message, yorick killed")
     if prompt == 'PYORICK-QUIT> ':
-      return  # yorick has quit
+      return  # yorick has quit, and process killed by echo_pty
     if self._debug:
       print("P>reqrep: reply="+str(reply.packets[0]))
     if reply.packets[0][0]==ID_EOL and reply.packets[0][1]==-1:
       self.kill(True)
       reply.packets[0][0] = ID_NIL
     elif (not prompt) and reply.packets[0][0]<ID_EVAL:
       # not finished until yorick comes back to its prompt
```

### Comparing `pyorick-1.4/pyorick/pyorick.i0` & `pyorick-1.5/pyorick/pyorick.i0`

 * *Files 0% similar despite different names*

```diff
@@ -373,15 +373,15 @@
  */
 func _pyorick_get(ctx)
 {
   if (pydebug) write, "Y>_pyorick_get: blocking...";
   hdr = _pyorick_recv([0, 0]);
   if (pydebug) write, "Y>_pyorick_get: got message "+print(hdr)(1);
   ctx = ctx && allof(hdr == [_ID_GETVAR,0]);
-  if (!ctx) _pyorick_refs, 1, 3;  /* discard previous result, if any */ 
+  if (!ctx) _pyorick_refs, 1, 3;  /* discard previous result, if any */
   id = hdr(1);
   msg = save(_pyorick_id=id, hdr);
   if (id>=0 && id<_ID_STRING) {
     rank = hdr(2);
     dims = [rank];
     if (rank>0) grow, dims, _pyorick_recv(array(0, rank));
     if (rank<0 || (rank && anyof(dims(1:)<=0)))
@@ -626,15 +626,15 @@
     return [(noneof(names)? -2 : (allof(names)? -3 : -8))];
   } else if (is_range(a)) {
     return [-4];
   } else if (is_void(a)) {
     return [-5];
   } else if (is_stream(a)) {
     return [-6];
-  } else if (typeof(g) == "text_stream") {
+  } else if (typeof(a) == "text_stream") {
     return [-7];
   } else {
     return [-9];
   }
 }
 
 func _pyorick_encode(value, env)
```

### Comparing `pyorick-1.4/pyorick/__init__.py` & `pyorick-1.5/pyorick/__init__.py`

 * *Files identical despite different names*

### Comparing `pyorick-1.4/PKG-INFO` & `pyorick-1.5/pyorick.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,44 +1,45 @@
-Metadata-Version: 1.1
+Metadata-Version: 2.1
 Name: pyorick
-Version: 1.4
+Version: 1.5
 Summary: python connection to yorick
 Home-page: https://github.com/dhmunro/pyorick
 Author: David Munro and John Field
 Author-email: dhmunro@users.sourceforge.net
 License: http://opensource.org/licenses/BSD-2-Clause
-Description: Run Yorick from Python
-        ======================
-        
-        The pyorick package starts `yorick <http://yorick.github.com>`_ as a
-        subprocess and provides an interface between python and yorick
-        interpreted code.
-        
-        Features:
-        
-        - exec or eval arbitrary yorick code strings
-        - get or set yorick variables
-        - call yorick functions or subroutines with python arguments
-        - get or set slices of large yorick arrays
-        - terminal mode to interact with yorick by keyboard through python
-        
-        Most of the data is exchanged via binary pipes between the two
-        interpreters.  Yorick runs in a request-reply mode.  Python prints
-        anything yorick sends to stdout or stderr except prompts.
-        
-        See `DESCRIPTION.rst <https://github.com/dhmunro/pyorick/blob/master/DESCRIPTION.rst>`_
-        for a complete description of the interface.  You can clone or fork
-        https://github.com/dhmunro/pyorick to contribute to pyorick.
-        
-        
 Platform: Linux
 Platform: MacOS X
 Platform: Unix
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 2.7
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Unix
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Software Development :: Interpreters
 Requires: numpy
+License-File: LICENSE.txt
+
+Run Yorick from Python
+======================
+
+The pyorick package starts `yorick <http://yorick.github.com>`_ as a
+subprocess and provides an interface between python and yorick
+interpreted code.
+
+Features:
+
+- exec or eval arbitrary yorick code strings
+- get or set yorick variables
+- call yorick functions or subroutines with python arguments
+- get or set slices of large yorick arrays
+- terminal mode to interact with yorick by keyboard through python
+
+Most of the data is exchanged via binary pipes between the two
+interpreters.  Yorick runs in a request-reply mode.  Python prints
+anything yorick sends to stdout or stderr except prompts.
+
+See `DESCRIPTION.rst <https://github.com/dhmunro/pyorick/blob/master/DESCRIPTION.rst>`_
+for a complete description of the interface.  You can clone or fork
+https://github.com/dhmunro/pyorick to contribute to pyorick.
+
```

### Comparing `pyorick-1.4/setup.py` & `pyorick-1.5/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,11 @@
 #!/usr/bin/env python
 
-# to upload to pypi:
-# <switch to setuptools branch, merge with master>
-# git clean -fdx
-#   first time: python setup.py register
-# python setup.py sdist bdist_wheel upload
-
 from __future__ import print_function
-from setuptools import setup, Command
+from distutils.core import setup, Command
 
 class TestCommand(Command):
   description = "PYorick test/check command"
   user_options = []
   def get_command_name(self):
       return "test"
   def initialize_options(self):
@@ -36,15 +30,15 @@
 # make pyorick.py work by creating a directory, copying pyorick.py
 # and pyorick.i0 to that directory, and adding the directory to
 # your PYTHONPATH environment variable.  You can optionally copy
 # test_pyorick.py to the same directory, cd there, and run nosetests
 # or py.test or python -m unittest -v test_pyorick to test pyorick.
 
 setup(name='pyorick',
-      version='1.4',
+      version='1.5',
       description='python connection to yorick',
       long_description=open('README.rst').read(),
       author='David Munro and John Field',
       author_email='dhmunro@users.sourceforge.net',
       url='https://github.com/dhmunro/pyorick',
       packages=['pyorick'],
       package_data={'pyorick': ['pyorick.i0']},
```

