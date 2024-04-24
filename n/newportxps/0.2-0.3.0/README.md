# Comparing `tmp/newportxps-0.2.tar.gz` & `tmp/newportxps-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/newportxps-0.2.tar", last modified: Sun Nov  1 16:40:42 2020, max compression
+gzip compressed data, was "newportxps-0.3.0.tar", last modified: Wed Apr 24 18:15:49 2024, max compression
```

## Comparing `newportxps-0.2.tar` & `newportxps-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,20 @@
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2020-11-01 16:40:42.879908 newportxps-0.2/
--rw-r--r--   0 Newville   (501) staff       (20)      242 2020-11-01 16:40:42.879133 newportxps-0.2/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)     3718 2020-01-31 12:45:03.000000 newportxps-0.2/README.md
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2020-11-01 16:40:42.875171 newportxps-0.2/newportxps/
--rw-r--r--   0 Newville   (501) staff       (20)    94910 2018-11-10 20:11:51.000000 newportxps-0.2/newportxps/XPS_C8_drivers.py
--rw-r--r--   0 Newville   (501) staff       (20)       35 2018-11-10 20:11:51.000000 newportxps-0.2/newportxps/__init__.py
--rw-r--r--   0 Newville   (501) staff       (20)     1205 2018-11-10 20:11:51.000000 newportxps-0.2/newportxps/debugtime.py
--rw-r--r--   0 Newville   (501) staff       (20)     4480 2020-11-01 16:19:13.000000 newportxps-0.2/newportxps/ftp_wrapper.py
--rwxr-xr-x   0 Newville   (501) staff       (20)    40442 2020-11-01 16:29:51.000000 newportxps-0.2/newportxps/newportxps.py
--rw-r--r--   0 Newville   (501) staff       (20)      450 2018-11-10 20:11:51.000000 newportxps-0.2/newportxps/utils.py
-drwxr-xr-x   0 Newville   (501) staff       (20)        0 2020-11-01 16:40:42.878346 newportxps-0.2/newportxps.egg-info/
--rw-r--r--   0 Newville   (501) staff       (20)      242 2020-11-01 16:40:42.000000 newportxps-0.2/newportxps.egg-info/PKG-INFO
--rw-r--r--   0 Newville   (501) staff       (20)      334 2020-11-01 16:40:42.000000 newportxps-0.2/newportxps.egg-info/SOURCES.txt
--rw-r--r--   0 Newville   (501) staff       (20)        1 2020-11-01 16:40:42.000000 newportxps-0.2/newportxps.egg-info/dependency_links.txt
--rw-r--r--   0 Newville   (501) staff       (20)        7 2020-11-01 16:40:42.000000 newportxps-0.2/newportxps.egg-info/requires.txt
--rw-r--r--   0 Newville   (501) staff       (20)       11 2020-11-01 16:40:42.000000 newportxps-0.2/newportxps.egg-info/top_level.txt
--rw-r--r--   0 Newville   (501) staff       (20)       38 2020-11-01 16:40:42.880164 newportxps-0.2/setup.cfg
--rw-r--r--   0 Newville   (501) staff       (20)      356 2020-11-01 16:39:06.000000 newportxps-0.2/setup.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-24 18:15:49.888449 newportxps-0.3.0/
+-rw-r--r--   0 Newville   (501) staff       (20)     1348 2018-11-10 20:11:51.000000 newportxps-0.3.0/LICENSE
+-rw-r--r--   0 Newville   (501) staff       (20)     5216 2024-04-24 18:15:49.888080 newportxps-0.3.0/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)     3718 2020-01-31 12:45:03.000000 newportxps-0.3.0/README.md
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-24 18:15:49.886467 newportxps-0.3.0/newportxps/
+-rw-r--r--   0 Newville   (501) staff       (20)    96652 2024-04-24 02:15:23.000000 newportxps-0.3.0/newportxps/XPS_C8_drivers.py
+-rw-r--r--   0 Newville   (501) staff       (20)       35 2018-11-10 20:11:51.000000 newportxps-0.3.0/newportxps/__init__.py
+-rw-r--r--   0 Newville   (501) staff       (20)     1205 2018-11-10 20:11:51.000000 newportxps-0.3.0/newportxps/debugtime.py
+-rw-r--r--   0 Newville   (501) staff       (20)     4552 2024-04-24 17:16:24.000000 newportxps-0.3.0/newportxps/ftp_wrapper.py
+-rwxr-xr-x   0 Newville   (501) staff       (20)    44417 2024-04-24 18:15:26.000000 newportxps-0.3.0/newportxps/newportxps.py
+-rw-r--r--   0 Newville   (501) staff       (20)      800 2024-04-24 02:15:23.000000 newportxps-0.3.0/newportxps/utils.py
+drwxr-xr-x   0 Newville   (501) staff       (20)        0 2024-04-24 18:15:49.887629 newportxps-0.3.0/newportxps.egg-info/
+-rw-r--r--   0 Newville   (501) staff       (20)     5216 2024-04-24 18:15:49.000000 newportxps-0.3.0/newportxps.egg-info/PKG-INFO
+-rw-r--r--   0 Newville   (501) staff       (20)      357 2024-04-24 18:15:49.000000 newportxps-0.3.0/newportxps.egg-info/SOURCES.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        1 2024-04-24 18:15:49.000000 newportxps-0.3.0/newportxps.egg-info/dependency_links.txt
+-rw-r--r--   0 Newville   (501) staff       (20)        7 2024-04-24 18:15:49.000000 newportxps-0.3.0/newportxps.egg-info/requires.txt
+-rw-r--r--   0 Newville   (501) staff       (20)       11 2024-04-24 18:15:49.000000 newportxps-0.3.0/newportxps.egg-info/top_level.txt
+-rw-r--r--   0 Newville   (501) staff       (20)     1493 2024-04-24 17:33:12.000000 newportxps-0.3.0/pyproject.toml
+-rw-r--r--   0 Newville   (501) staff       (20)       38 2024-04-24 18:15:49.888513 newportxps-0.3.0/setup.cfg
+-rw-r--r--   0 Newville   (501) staff       (20)       92 2024-04-24 17:29:16.000000 newportxps-0.3.0/setup.py
```

### Comparing `newportxps-0.2/README.md` & `newportxps-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `newportxps-0.2/newportxps/XPS_C8_drivers.py` & `newportxps-0.3.0/newportxps/XPS_C8_drivers.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,19 +10,16 @@
 #          if (XPS.__usedSockets[socketId] == 0):   return
 #       with "withValidSocket" decorator, whch raises an exception
 #       if there is not a valid socket.
 # made many return values "consistent".
 
 import sys
 import socket
-import six
-from collections import OrderedDict
-
-from .utils import bytes2str
 
+from .utils import bytes2str, str2bytes
 
 class XPSException(Exception):
     """XPS Controller Exception"""
     def __init__(self, msg,*args):
         self.msg = msg
     def __str__(self):
         return str(self.msg)
@@ -37,15 +34,15 @@
     __nbSockets = 0
 
     # Initialization Function
     def __init__ (self):
         XPS.__nbSockets = 0
         for socketId in range(self.MAX_NB_SOCKETS):
             XPS.__usedSockets[socketId] = 0
-        self.errorcodes = OrderedDict()
+        self.errorcodes = {}
 
     def withValidSocket(fcn):
         """ decorator to ensure that a valid socket is passed as the
         first argument of the decorated function"""
         def wrapper(*args, **kw):
             try:
                 sid = args[1]
@@ -60,15 +57,15 @@
         return wrapper
 
     # Send command and get return
     @withValidSocket
     def __sendAndReceive (self, socketId, command):
         # print("SEND REC ", command, type(command))
         try:
-            XPS.__sockets[socketId].send(six.b(command))
+            XPS.__sockets[socketId].send(str2bytes(command))
             ret = bytes2str(XPS.__sockets[socketId].recv(1024))
             while (ret.find(',EndOfAPI') == -1):
                 ret += bytes2str(XPS.__sockets[socketId].recv(1024))
         except socket.timeout:
             return [-2, '']
         except socket.error as err: #  (errNb, errString):
             print( 'Socket error : ', err.errno, err)
@@ -110,15 +107,15 @@
             XPS.__sockets[socketId].connect((IP, port))
             XPS.__sockets[socketId].settimeout(timeOut)
             XPS.__sockets[socketId].setblocking(1)
         except socket.error:
             return -1
 
         err, ret = self.ErrorListGet(socketId)
-        self.errorcodes = OrderedDict()
+        self.errorcodes = {}
         for cline in ret.split(';'):
             if ':' in cline:
                 ecode, message = cline.split(':', 1)
                 ecode = ecode.replace('Error', '').strip()
                 message = message.strip()
                 self.errorcodes[ecode] = message
 
@@ -229,15 +226,15 @@
             j += 1
         retList.append(eval(returnedString[i:i+j]))
 
         return retList
 
     # TimerSet :  Set a timer
     def TimerSet (self, socketId, TimerName, FrequencyTicks):
-        return self.Send(socketId, 'TimerSet(%s, %s)' (TimerName, str(FrequencyTicks)))
+        return self.Send(socketId, 'TimerSet(%s, %s)' % (TimerName, str(FrequencyTicks)))
 
     # Reboot :  Reboot the controller
     def Reboot (self, socketId):
         return self.Send(socketId, 'Reboot()')
 
     # Login :  Log in
     def Login (self, socketId, Name, Password):
@@ -1341,14 +1338,27 @@
         return retList
 
     # PositionerPositionCompareAquadBWindowedSet :  Set position compare AquadB windowed parameters
     def PositionerPositionCompareAquadBWindowedSet (self, socketId, PositionerName, MinimumPosition, MaximumPosition):
         command = 'PositionerPositionCompareAquadBWindowedSet(' + PositionerName + ',' + str(MinimumPosition) + ',' + str(MaximumPosition) + ')'
         return self.Send(socketId, command)
 
+    # PositionerPositionCompareAquadBPrescalerSet: Sets PCO AquadB interpolation factor.
+    def PositionerPositionCompareAquadBPrescalerSet(self, socketId, PositionerName, PCOInterpolationFactor):
+        command = 'PositionerPositionCompareAquadBPrescalerSet(' + PositionerName + ',' + str(
+            PCOInterpolationFactor) + ')'
+        return self.Send(socketId, command)
+
+    # PositionerPositionCompareAquadBPrescalerGet : Gets PCO AquadB interpolation factor.
+    def PositionerPositionCompareAquadBPrescalerGet(self, socketId, PositionerName):
+        command = 'PositionerPositionCompareAquadBPrescalerGet(' + PositionerName + ',double *)'
+        error, returnedString = self.Send(socketId, command)
+        if (error != 0):
+            return [error, returnedString]
+
     # PositionerPositionCompareGet :  Read position compare parameters
     def PositionerPositionCompareGet (self, socketId, PositionerName):
         command = 'PositionerPositionCompareGet(' + PositionerName + ',double *,double *,double *,bool *)'
         error, returnedString = self.Send(socketId, command)
         if (error != 0):
             return [error, returnedString]
 
@@ -1597,14 +1607,19 @@
         retList.append(eval(returnedString[i:i+j]))
         return retList
 
     # MultipleAxesPVTVerification :  Multiple axes PVT trajectory verification
     def MultipleAxesPVTVerification (self, socketId, GroupName, TrajectoryFileName):
         command = 'MultipleAxesPVTVerification(' + GroupName + ',' + TrajectoryFileName + ')'
         return self.Send(socketId, command)
+    
+    # MultipleAxesPTVerification :  Multiple axes PT trajectory verification
+    def MultipleAxesPTVerification (self, socketId, GroupName, TrajectoryFileName):
+        command = 'MultipleAxesPTVerification(' + GroupName + ',' + TrajectoryFileName + ')'
+        return self.Send(socketId, command)
 
     # MultipleAxesPVTVerificationResultGet :  Multiple axes PVT trajectory verification result get
     def MultipleAxesPVTVerificationResultGet (self, socketId, PositionerName):
         command = 'MultipleAxesPVTVerificationResultGet(' + PositionerName + ',char *,double *,double *,double *,double *)'
         error, returnedString = self.Send(socketId, command)
         if (error != 0):
             return [error, returnedString]
@@ -1617,14 +1632,19 @@
             i, j = i+j+1, 0
         return retList
 
     # MultipleAxesPVTExecution :  Multiple axes PVT trajectory execution
     def MultipleAxesPVTExecution (self, socketId, GroupName, TrajectoryFileName, ExecutionNumber):
         command = 'MultipleAxesPVTExecution(' + GroupName + ',' + TrajectoryFileName + ',' + str(ExecutionNumber) + ')'
         return self.Send(socketId, command)
+    
+    # MultipleAxesPTExecution :  Multiple axes PT trajectory execution
+    def MultipleAxesPTExecution (self, socketId, GroupName, TrajectoryFileName, ExecutionNumber):
+        command = 'MultipleAxesPTExecution(' + GroupName + ',' + TrajectoryFileName + ',' + str(ExecutionNumber) + ')'
+        return self.Send(socketId, command)
 
     # MultipleAxesPVTParametersGet :  Multiple axes PVT trajectory get parameters
     def MultipleAxesPVTParametersGet (self, socketId, GroupName):
         command = 'MultipleAxesPVTParametersGet(' + GroupName + ',char *,int *)'
         error, returnedString = self.Send(socketId, command)
         if (error != 0):
             return [error, returnedString]
@@ -2032,7 +2052,17 @@
     # SocketsStatusGet :  Get sockets current status
     def SocketsStatusGet (self, socketId):
         return self.Send(socketId, 'SocketsStatusGet(char *)')
 
     # TestTCP :  Test TCP/IP transfert
     def TestTCP (self, socketId, InputString):
         return self.Send(socketId, 'TestTCP(%s, char *)' % InputString)
+
+    # ========== Only for XPS-D ==========
+
+    # CleanCoreDumpFolder :   Remove core file in /Admin/Public/CoreDump folder
+    def CleanCoreDumpFolder (self, socketId):
+        return self.Send(socketId, 'CleanCoreDumpFolder()')
+
+    # CleanTmpFolder :   Clean the tmp folder
+    def CleanTmpFolder(self, socketId):
+        return self.Send(socketId, 'CleanTmpFolder()')
```

### Comparing `newportxps-0.2/newportxps/debugtime.py` & `newportxps-0.3.0/newportxps/debugtime.py`

 * *Files identical despite different names*

### Comparing `newportxps-0.2/newportxps/ftp_wrapper.py` & `newportxps-0.3.0/newportxps/ftp_wrapper.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 #!/usr/bin/env python
 
-from __future__ import print_function
-import os
 import ftplib
-import six
-from .utils import six, bytes2str, bytesio, FTP_ENCODING
+from io import BytesIO
+from .utils import str2bytes, bytes2str, ENCODING
 
 import logging
 logger = logging.getLogger('paramiko')
 logger.setLevel(logging.ERROR)
 
 
 HAS_PYSFTP = False
@@ -33,27 +31,27 @@
             self._conn.close()
         self._conn = None
 
     def cwd(self, remotedir):
         self._conn.cwd(remotedir)
 
     def connect(self, host=None, username=None, password=None):
-        raise NotImplemented
+        raise NotImplementedError
 
     def save(self, remotefile, localfile):
         "save remote file to local file"
-        raise NotImplemented
+        raise NotImplementedError
 
     def getlines(self, remotefile):
         "read text of remote file"
-        raise NotImplemented
+        raise NotImplementedError
 
     def put(self, text, remotefile):
         "put text to remote file"
-        raise NotImplemented
+        raise NotImplementedError
 
 
 class SFTPWrapper(FTPBaseWrapper):
     """wrap ftp interactions for Newport XPS models D"""
     def __init__(self, host=None, username='Administrator',
                  password='Administrator'):
         FTPBaseWrapper.__init__(self, host=host,
@@ -68,36 +66,36 @@
             self.password = password
 
         if not HAS_PYSFTP:
             raise ValueError("pysftp not installed.")
         try:
             self._conn = pysftp.Connection(self.host,
                                            username=self.username,
-                                           password=self.username)
+                                           password=self.password)
         except:
             print("ERROR: sftp connection to %s failed" % self.host)
             print("You may need to add the host keys for your XPS to your")
             print("ssh known_hosts file, using a command like this:")
             print("  ssh-keyscan %s >> ~/.ssh/known_hosts" % self.host)
 
 
     def save(self, remotefile, localfile):
         "save remote file to local file"
-        self._conn.get(remotefile, remotefile)
+        self._conn.get(remotefile, localfile)
 
     def getlines(self, remotefile):
         "read text of remote file"
-        tmp = bytesio()
+        tmp = BytesIO()
         self._conn.getfo(remotefile, tmp)
         tmp.seek(0)
         text = bytes2str(tmp.read())
         return text.split('\n')
 
     def put(self, text, remotefile):
-        txtfile = bytesio(six.b(text))
+        txtfile = BytesIO(str2bytes(text))
         self._conn.putfo(txtfile, remotefile)
 
 
 class FTPWrapper(FTPBaseWrapper):
     """wrap ftp interactions for Newport XPS models C and Q"""
     def __init__(self, host=None, username='Administrator',
                  password='Administrator'):
@@ -112,28 +110,32 @@
         if password is not None:
             self.password = password
 
         self._conn = ftplib.FTP()
         self._conn.connect(self.host)
         self._conn.login(self.username, self.password)
 
+    def list(self):
+        "list files in a given directory (default the current)"
+        return self._conn.nlst()
+
     def save(self, remotefile, localfile):
         "save remote file to local file"
         output = []
-        x = self._conn.retrbinary('RETR %s' % remotefile, output.append)
-        open_opts = {}
-        if six.PY3:
-            open_opts['encoding'] = FTP_ENCODING
-        with open(localfile, 'w', **open_opts) as fout:
+        self._conn.retrbinary(f'RETR {remotefile}', output.append)
+        with open(localfile, 'w', encoding=ENCODING) as fout:
             fout.write(''.join([bytes2str(s) for s in output]))
 
     def getlines(self, remotefile):
         "read text of remote file"
         output = []
         self._conn.retrbinary('RETR %s' % remotefile, output.append)
         text = ''.join([bytes2str(line) for line in output])
         return text.split('\n')
 
     def put(self, text, remotefile):
-        txtfile = bytesio(six.b(text))
-        # print(" Put ", text, txtfile)
+        txtfile = BytesIO(str2bytes(text))
         self._conn.storbinary('STOR %s' % remotefile, txtfile)
+
+    def delete(self, remotefile):
+        "delete remote file"
+        self._conn.delete(remotefile)
```

### Comparing `newportxps-0.2/newportxps/newportxps.py` & `newportxps-0.3.0/newportxps/newportxps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,21 @@
-#!/usr/bin/env python
+ #!/usr/bin/env python
 
-from __future__ import print_function
 import os
 import posixpath
 import sys
 import time
 import socket
-from collections import OrderedDict
-
-from six.moves import StringIO
-from six.moves.configparser import  ConfigParser
+from io import StringIO
+from configparser import  ConfigParser
 import numpy as np
 
+from .debugtime import debugtime
+from .utils import clean_text
 from .XPS_C8_drivers import XPS, XPSException
-
 from .ftp_wrapper import SFTPWrapper, FTPWrapper
 
 IDLE, ARMING, ARMED, RUNNING, COMPLETE, WRITING, READING = \
       'IDLE', 'ARMING', 'ARMED', 'RUNNING', 'COMPLETE', 'WRITING', 'READING'
 
 def withConnectedXPS(fcn):
     """decorator to ensure a NewportXPS is connected before a method is called"""
@@ -27,54 +25,54 @@
         return fcn(self, *args, **kwargs)
     wrapper.__doc__ = fcn.__doc__
     wrapper.__name__ = fcn.__name__
     wrapper.__dict__.update(fcn.__dict__)
 
     return wrapper
 
+
 class NewportXPS:
     gather_header = '# XPS Gathering Data\n#--------------'
     def __init__(self, host, group=None,
                  username='Administrator', password='Administrator',
                  port=5001, timeout=10, extra_triggers=0,
                  outputs=('CurrentPosition', 'SetpointPosition')):
 
-        socket.setdefaulttimeout(5.0)
-        try:
-            host = socket.gethostbyname(host)
-        except:
-            raise ValueError('Could not resolve XPS name %s' % host)
         self.host = host
         self.port = port
         self.username = username
         self.password = password
         self.timeout = timeout
         self.extra_triggers = extra_triggers
 
         self.gather_outputs = tuple(outputs)
         self.trajectories = {}
         self.traj_state = IDLE
         self.traj_group = None
         self.traj_file = None
         self.traj_positioners = None
 
-        self.stages = OrderedDict()
-        self.groups = OrderedDict()
+        self.nsegments = -1
+        self.stages = {}
+        self.groups = {}
         self.firmware_version = None
 
         self.ftpconn = None
         self.ftpargs = dict(host=self.host,
                             username=self.username,
                             password=self.password)
         self._sid = None
         self._xps = XPS()
         self.connect()
         if group is not None:
             self.set_trajectory_group(group)
 
+    def __repr__(self):
+        return f"NewportXPS(host='{self.host}', port={self.port})"
+
     @withConnectedXPS
     def status_report(self):
         """return printable status report"""
         err, uptime = self._xps.ElapsedTimeGet(self._sid)
         self.check_error(err, msg="Elapsed Time")
         boottime = time.time() - uptime
         out = ["# XPS host:         %s (%s)" % (self.host, socket.getfqdn(self.host)),
@@ -109,30 +107,30 @@
         except:
             raise XPSException('Login failed for %s' % self.host)
 
         err, val = self._xps.FirmwareVersionGet(self._sid)
         self.firmware_version = val
         self.ftphome = ''
 
-        if 'XPS-D' in self.firmware_version:
+        if any([m in self.firmware_version for m in ['XPS-D', 'HXP-D']]):
             err, val = self._xps.Send(self._sid, 'InstallerVersionGet(char *)')
             self.firmware_version = val
             self.ftpconn = SFTPWrapper(**self.ftpargs)
         else:
             self.ftpconn = FTPWrapper(**self.ftpargs)
             if 'XPS-C' in self.firmware_version:
                 self.ftphome = '/Admin'
         try:
             self.read_systemini()
         except:
             print("Could not read system.ini!!!")
 
 
     def check_error(self, err, msg='', with_raise=True):
-        if err is not 0:
+        if err != 0:
             err = "%d" % err
             desc = self._xps.errorcodes.get(err, 'unknown error')
             print("XPSError: message= %s, error=%s, description=%s" % (msg, err, desc))
             if with_raise:
                 raise XPSException("%s %s [Error %s]" % (msg, desc, err))
 
     def save_systemini(self, fname='system.ini'):
@@ -161,27 +159,28 @@
         """read group info from system.ini
         this is part of the connection process
         """
         self.ftpconn.connect(**self.ftpargs)
         self.ftpconn.cwd(posixpath.join(self.ftphome, 'Config'))
         lines = self.ftpconn.getlines('system.ini')
         self.ftpconn.close()
+        initext = '\n'.join([line.strip() for line in lines])
 
         pvtgroups = []
-        self.stages= OrderedDict()
-        self.groups = OrderedDict()
+        self.stages= {}
+        self.groups = {}
         sconf = ConfigParser()
-        sconf.readfp(StringIO('\n'.join(lines)))
+        sconf.readfp(StringIO(initext))
 
         # read and populate lists of groups first
         for gtype, glist in sconf.items('GROUPS'): # ].items():
             if len(glist) > 0:
                 for gname in glist.split(','):
                     gname = gname.strip()
-                    self.groups[gname] = OrderedDict()
+                    self.groups[gname] = {}
                     self.groups[gname]['category'] = gtype.strip()
                     self.groups[gname]['positioners'] = []
                     if gtype.lower().startswith('multiple'):
                         pvtgroups.append(gname)
 
         for section in sconf.sections():
             if section in ('DEFAULT', 'GENERAL', 'GROUPS'):
@@ -232,28 +231,90 @@
         Arguments:
         ----------
            filename (str):  name of trajectory file
            text  (str):   full text of trajectory file
         """
         self.ftpconn.connect(**self.ftpargs)
         self.ftpconn.cwd(posixpath.join(self.ftphome, 'Public', 'Trajectories'))
-        self.ftpconn.put(text, filename)
+        self.ftpconn.put(clean_text(text), filename)
+        self.ftpconn.close()
+
+    def list_scripts(self):
+        """list all existent scripts files
+        """
+        remotefiles = ""
+        self.ftpconn.connect(**self.ftpargs)
+        self.ftpconn.cwd(posixpath.join(self.ftphome, 'Public', 'Scripts'))
+        remotefiles = self.ftpconn.list()
+        self.ftpconn.close()
+
+        return remotefiles
+
+    def read_script(self, filename):
+        """read script content
+
+        Arguments:
+        ----------
+           filename (str):  name of script file
+        """
+        filecontent = ""
+        self.ftpconn.connect(**self.ftpargs)
+        self.ftpconn.cwd(posixpath.join(self.ftphome, 'Public', 'Scripts'))
+        filecontent = self.ftpconn.getlines(filename)
+        self.ftpconn.close()
+
+        return filecontent
+
+    def download_script(self, filename):
+        """download script file
+
+        Arguments:
+        ----------
+           filename (str):  name of script file
+        """
+        self.ftpconn.connect(**self.ftpargs)
+        self.ftpconn.cwd(posixpath.join(self.ftphome, 'Public', 'Scripts'))
+        self.ftpconn.save(filename, filename)
+        self.ftpconn.close()
+
+    def upload_script(self, filename, text):
+        """upload script file
+
+        Arguments:
+        ----------
+           filename (str):  name of script file
+           text  (str):   full text of script file
+        """
+        self.ftpconn.connect(**self.ftpargs)
+        self.ftpconn.cwd(posixpath.join(self.ftphome, 'Public', 'Scripts'))
+        self.ftpconn.put(clean_text(text), filename)
         self.ftpconn.close()
 
+    def delete_script(self, filename):
+        """delete script file
+
+        Arguments:
+        ----------
+           filename (str):  name of script file
+        """
+        self.ftpconn.connect(**self.ftpargs)
+        self.ftpconn.cwd(posixpath.join(self.ftphome, 'Public', 'Scripts'))
+        self.ftpconn.delete(filename)
+        self.ftpconn.close()
 
     def upload_systemini(self, text):
         """upload text of system.ini
 
         Arguments:
         ----------
            text  (str):   full text of system.ini
         """
         self.ftpconn.connect(**self.ftpargs)
         self.ftpconn.cwd(posixpath.join(self.ftphome, 'Config'))
-        self.ftpconn.put(text, 'system.ini')
+        self.ftpconn.put(clean_text(text), 'system.ini')
         self.ftpconn.close()
 
     def upload_stagesini(self, text):
         """upload text of stages.ini
 
         Arguments:
         ----------
@@ -265,15 +326,15 @@
           >>> fh = open('mystages.ini', 'r', encoding='ISO8859')
           >>> text = fh.read()
           >>> xps.upload_stageini(text)
 
         """
         self.ftpconn.connect(**self.ftpargs)
         self.ftpconn.cwd(posixpath.join(self.ftphome, 'Config'))
-        self.ftpconn.put(text, 'system.ini')
+        self.ftpconn.put(clean_text(text), 'stages.ini')
         self.ftpconn.close()
 
     @withConnectedXPS
     def set_tuning(self, stage, kp=None, ki=None, kd=None, ks=None,
                    inttime=None, dfilter=None, closedloopstatus=1,
                    gkp=None, gki=None, gkd=None, kform=None, ffgain=None):
         """set tuning parameters for a stage:
@@ -409,16 +470,20 @@
         self._group_act(method, group=group, action='killing')
 
     def initialize_allgroups(self, with_encoder=True, home=False):
         """
         initialize all groups, no homing
         """
         for g in self.groups:
-            self.initialize_group(group=g)
-
+            try:
+                self.initialize_group(group=g)
+            except XPSException:
+                print(f"Warning: could not initialize '{g}' (already initialized?)")
+                
+                
     def home_allgroups(self, with_encoder=True, home=False):
         """
         home all groups
         """
         for g in self.groups:
             self.home_group(group=g)
 
@@ -477,15 +542,15 @@
         self._group_act('GroupMotionDisable', group=group, action='disabling')
 
     @withConnectedXPS
     def get_group_status(self):
         """
         get dictionary of status for each group
         """
-        out = OrderedDict()
+        out = {}
         for group in self.groups:
             err, stat = self._xps.GroupStatusGet(self._sid, group)
             self.check_error(err, msg="GroupStatus '%s'" % (group))
 
             err, val = self._xps.GroupStatusStringGet(self._sid, stat)
             self.check_error(err, msg="GroupStatusString '%s'" % (stat))
 
@@ -493,15 +558,15 @@
         return out
 
     @withConnectedXPS
     def get_hardware_status(self):
         """
         get dictionary of hardware status for each stage
         """
-        out = OrderedDict()
+        out = {}
         for stage in self.stages:
             if stage in ('', None): continue
             err, stat = self._xps.PositionerHardwareStatusGet(self._sid, stage)
             self.check_error(err, msg="Pos HardwareStatus '%s'" % (stage))
 
             err, val = self._xps.PositionerHardwareStatusStringGet(self._sid, stat)
             self.check_error(err, msg="Pos HardwareStatusString '%s'" % (stat))
@@ -509,15 +574,15 @@
         return out
 
     @withConnectedXPS
     def get_positioner_errors(self):
         """
         get dictionary of positioner errors for each stage
         """
-        out = OrderedDict()
+        out = {}
         for stage in self.stages:
             if stage in ('', None): continue
             err, stat = self._xps.PositionerErrorGet(self._sid, stage)
             self.check_error(err, msg="Pos Error '%s'" % (stage))
 
             err, val = self._xps.PositionerErrorStringGet(self._sid, stat)
             self.check_error(err, msg="Pos ErrorString '%s'" % (stat))
@@ -580,14 +645,26 @@
             if p in kwargs:
                 vals.append(kwargs[p])
             else:
                 vals.append(ret[i+1])
         self._xps.GroupMoveAbsolute(self._sid, group, vals)
 
     @withConnectedXPS
+    def execute_script(self, script, task, arguments):
+        """
+        Execute a TCL script
+
+        Parameters:
+           script (string): name of script file
+           task (string): task name to be identified
+           arguments (string): script arguments
+        """
+        self._xps.TCLScriptExecute(self._sid, script, task, arguments)
+
+    @withConnectedXPS
     def move_stage(self, stage, value, relative=False):
         """
         move stage to position, optionally relative
 
         Parameters:
            stage (string): name of stage -- must be in self.stages
            value (float): target position
@@ -763,33 +840,31 @@
         self.traj_file = '%s.trj'  % name
 
         # move_kws = {}
         outputs = []
         for out in self.gather_outputs:
             for i, ax in enumerate(traj['axes']):
                 outputs.append('%s.%s.%s' % (self.traj_group, ax, out))
-                # move_kws[ax] = float(traj['start'][i])
 
+        end_segment = traj['nsegments'] # - 1 + self.extra_triggers
+        self.nsegments = end_segment
 
-        end_segment = traj['nsegments'] - 1 + self.extra_triggers
-        # self.move_group(self.traj_group, **move_kws)
         self.gather_titles = "%s\n#%s\n" % (self.gather_header, " ".join(outputs))
-
         err, ret = self._xps.GatheringReset(self._sid)
         self.check_error(err, msg="GatheringReset")
         if verbose:
             print(" GatheringReset returned ", ret)
 
         err, ret = self._xps.GatheringConfigurationSet(self._sid, outputs)
         self.check_error(err, msg="GatheringConfigSet")
 
         if verbose:
             print(" GatheringConfigurationSet outputs ", outputs)
             print(" GatheringConfigurationSet returned ", ret)
-            print( end_segment, traj['pixeltime'])
+            print(" segments, pixeltime" , end_segment, traj['pixeltime'])
 
         err, ret = self._xps.MultipleAxesPVTPulseOutputSet(self._sid, self.traj_group,
                                                            2, end_segment,
                                                            traj['pixeltime'])
         self.check_error(err, msg="PVTPulseOutputSet", with_raise=False)
         if verbose:
             print(" PVTPulse  ", ret)
@@ -799,24 +874,30 @@
 
         self.check_error(err, msg="PVTVerification", with_raise=False)
         if verbose:
             print(" PVTVerify  ", ret)
         self.traj_state = ARMED
 
     @withConnectedXPS
-    def run_trajectory(self, name=None, save=True,
+    def run_trajectory(self, name=None, save=True, clean=False,
                        output_file='Gather.dat', verbose=False):
 
         """run a trajectory in PVT mode
 
         The trajectory *must be in the ARMED state
         """
 
-        if name in self.trajectories:
-            self.arm_trajectory(name)
+        if 'xps-d' in self.firmware_version.lower():
+            self._xps.CleanTmpFolder(self._sid)
+
+            if clean:
+                self._xps.CleanCoreDumpFolder(self._sid)
+
+        if name in self.trajectories and self.traj_state != ARMED:
+            self.arm_trajectory(name, verbose=verbose)
 
         if self.traj_state != ARMED:
             raise XPSException("Must arm trajectory before running!")
 
         buffer = ('Always', '%s.PVT.TrajectoryPulse' % self.traj_group,)
         err, ret = self._xps.EventExtendedConfigurationTriggerSet(self._sid, buffer,
                                                                   ('0','0'), ('0','0'),
@@ -847,49 +928,78 @@
 
         ret = self._xps.EventExtendedRemove(self._sid, eventID)
         ret = self._xps.GatheringStop(self._sid)
 
         self.traj_state = COMPLETE
         npulses = 0
         if save:
-            self.read_and_save(output_file)
+            self.read_and_save(output_file, verbose=verbose)
         self.traj_state = IDLE
         return npulses
 
     @withConnectedXPS
-    def read_and_save(self, output_file):
+    def read_and_save(self, output_file, verbose=False):
         "read and save gathering file"
         self.ngathered = 0
-        npulses, buff = self.read_gathering(set_idle_when_done=False)
+        npulses, buff = self.read_gathering(set_idle_when_done=False,
+                                            verbose=verbose)
+        if npulses < 1:
+            return
         self.save_gathering_file(output_file, buff,
-                                 verbose=False,
+                                 verbose=verbose,
                                  set_idle_when_done=False)
         self.ngathered = npulses
 
     @withConnectedXPS
-    def read_gathering(self, set_idle_when_done=True, debug_time=False):
+    def read_gathering(self, set_idle_when_done=True, verbose=False,
+                       debug_time=False):
         """
         read gathering data from XPS
         """
+        verbose = verbose or debug_time
+        if verbose:
+            print("READ Gathering XPS ", self.host, self._sid,
+                  self.nsegments, time.ctime())
+        dt = debugtime()
         self.traj_state = READING
-        ret, npulses, nx = self._xps.GatheringCurrentNumberGet(self._sid)
+        npulses = -1
+        t0 = time.time()
+        while npulses < 1:
+            try:
+                ret, npulses, nx = self._xps.GatheringCurrentNumberGet(self._sid)
+            except SyntaxError:
+                print("#XPS Gathering Read failed, will try again")
+                pass
+            if time.time()-t0 > 5:
+                print("Failed to get gathering size after 5 seconds: return 0 points")
+                print("Gather Returned: ", ret, npulses, nx, self._xps, time.ctime())
+                return (0, ' \n')
+            if npulses < 1 or ret != 0:
+                time.sleep(0.05)
+        dt.add("gather num %d npulses=%d (%d)" % (ret, npulses, self.nsegments))
         counter = 0
         while npulses < 1 and counter < 5:
             counter += 1
-            time.sleep(0.5)
+            time.sleep(0.25)
             ret, npulses, nx = self._xps.GatheringCurrentNumberGet(self._sid)
             print( 'Had to do repeat XPS Gathering: ', ret, npulses, nx)
-        ret, buff = self._xps.GatheringDataMultipleLinesGet(self._sid, 0, npulses)
+        dt.add("gather before multilinesget, npulses=%d" % (npulses))
+        try:
+            ret, buff = self._xps.GatheringDataMultipleLinesGet(self._sid, 0, npulses)
+        except ValueError:
+            print("Failed to read gathering: ", ret, buff)
+            return (0, ' \n')
+        dt.add("gather after multilinesget  %d" % ret)
         nchunks = -1
         if ret < 0:  # gathering too long: need to read in chunks
             nchunks = 3
             nx  = int((npulses-2) / nchunks)
             ret = 1
             while True:
-                time.sleep(0.1)
+                time.sleep(0.05)
                 ret, xbuff = self._xps.GatheringDataMultipleLinesGet(self._sid, 0, nx)
                 if ret == 0:
                     break
                 nchunks = nchunks + 2
                 nx      = int((npulses-2) / nchunks)
                 if nchunks > 10:
                     print('looks like something is wrong with the XPS!')
@@ -898,31 +1008,33 @@
             for i in range(1, nchunks):
                 ret, xbuff = self._xps.GatheringDataMultipleLinesGet(self._sid, i*nx, nx)
                 buff.append(xbuff)
             ret, xbuff = self._xps.GatheringDataMultipleLinesGet(self._sid, nchunks*nx,
                                                                 npulses-nchunks*nx)
             buff.append(xbuff)
             buff = ''.join(buff)
-
+        dt.add("gather after got buffer  %d" % len(buff))
         obuff = buff[:]
         for x in ';\r\t':
             obuff = obuff.replace(x,' ')
-
+        dt.add("gather cleaned buffer  %d" % len(obuff))
         if set_idle_when_done:
             self.traj_state = IDLE
+        if verbose:
+            dt.show()
         return npulses, obuff
 
-    def save_gathering_file(self, fname, buffer, verbose=False, set_idle_when_done=True):
+    def save_gathering_file(self, fname, buff, verbose=False, set_idle_when_done=True):
         """save gathering buffer read from read_gathering() to text file"""
         self.traj_state = WRITING
         f = open(fname, 'w')
         f.write(self.gather_titles)
-        f.write(buffer)
+        f.write(buff)
         f.close()
-        nlines = len(buffer.split('\n')) - 1
+        nlines = len(buff.split('\n')) - 1
         if verbose:
             print('Wrote %i lines, %i bytes to %s' % (nlines, len(buff), fname))
         if set_idle_when_done:
             self.traj_state = IDLE
 
     def define_line_trajectories_general(self, name='default',
                                          start_values=None,
@@ -1048,24 +1160,22 @@
 
         outputs = []
         for out in self.gather_outputs:
             for i, ax in enumerate(traj['axes']):
                 outputs.append('%s.%s.%s' % (self.traj_group, ax, out))
                 # move_kws[ax] = float(traj['start'][i])
 
-
         end_segment = traj['nsegments'] - 1 + self.extra_triggers
         # self.move_group(self.traj_group, **move_kws)
         self.gather_titles = "%s\n#%s\n" % (self.gather_header, " ".join(outputs))
 
-
         self._xps.GatheringReset(self._sid)
         self._xps.GatheringConfigurationSet(self._sid, self.gather_outputs)
 
-        print("step_number", step_number)
+        # print("step_number", step_number)
         ret = self._xps.MultipleAxesPVTPulseOutputSet(self._sid, self.traj_group,
                                                       2, step_number + 1, dtime)
         ret = self._xps.MultipleAxesPVTVerification(self._sid, self.traj_group, traj_file)
 
         buffer = ('Always', self.traj_group + '.PVT.TrajectoryPulse')
         o = self._xps.EventExtendedConfigurationTriggerSet(self._sid, buffer,
                                                           ('0', '0'), ('0', '0'),
```

